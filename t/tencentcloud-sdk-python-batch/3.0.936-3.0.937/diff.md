# Comparing `tmp/tencentcloud-sdk-python-batch-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-batch-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.936.tar", last modified: Mon Jul 17 00:17:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-batch-3.0.937.tar", last modified: Tue Jul 18 00:17:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-batch-3.0.936.tar` & `tencentcloud-sdk-python-batch-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)    31537 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   299592 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-07-17 00:17:46.000000 tencentcloud-sdk-python-batch-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    31537 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   299742 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-07-18 00:17:33.000000 tencentcloud-sdk-python-batch-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-batch-3.0.936/setup.py` & `tencentcloud-sdk-python-batch-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-batch-3.0.936/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-batch-3.0.937/tencentcloud/batch/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5674,15 +5674,15 @@
 class InternetAccessible(AbstractModel):
     """描述了实例的公网可访问性，声明了实例的公网使用计费模式，最大带宽等
 
     """
 
     def __init__(self):
         r"""
-        :param _InternetChargeType: 网络计费类型。取值范围：<br><li>BANDWIDTH_PREPAID：预付费按带宽结算<br><li>TRAFFIC_POSTPAID_BY_HOUR：流量按小时后付费<br><li>BANDWIDTH_POSTPAID_BY_HOUR：带宽按小时后付费<br><li>BANDWIDTH_PACKAGE：带宽包用户<br>默认取值：非带宽包用户默认与子机付费类型保持一致。
+        :param _InternetChargeType: 网络计费类型。取值范围：<br><li>BANDWIDTH_PREPAID：预付费按带宽结算<br><li>TRAFFIC_POSTPAID_BY_HOUR：流量按小时后付费<br><li>BANDWIDTH_POSTPAID_BY_HOUR：带宽按小时后付费<br><li>BANDWIDTH_PACKAGE：带宽包用户<br>默认取值：非带宽包用户默认与子机付费类型保持一致，比如子机付费类型为预付费，网络计费类型默认为预付费；子机付费类型为后付费，网络计费类型默认为后付费。
         :type InternetChargeType: str
         :param _InternetMaxBandwidthOut: 公网出带宽上限，单位：Mbps。默认值：0Mbps。不同机型带宽上限范围不一致，具体限制详见[购买网络带宽](https://cloud.tencent.com/document/product/213/12523)。
         :type InternetMaxBandwidthOut: int
         :param _PublicIpAssigned: 是否分配公网IP。取值范围：<br><li>TRUE：表示分配公网IP<br><li>FALSE：表示不分配公网IP<br><br>当公网带宽大于0Mbps时，可自由选择开通与否，默认开通公网IP；当公网带宽为0，则不允许分配公网IP。该参数仅在RunInstances接口中作为入参使用。
         :type PublicIpAssigned: bool
         :param _BandwidthPackageId: 带宽包ID。可通过[`DescribeBandwidthPackages`](https://cloud.tencent.com/document/api/215/19209)接口返回值中的`BandwidthPackageId`获取。该参数仅在RunInstances接口中作为入参使用。
         :type BandwidthPackageId: str
```

### Comparing `tencentcloud-sdk-python-batch-3.0.936/tencentcloud_sdk_python_batch.egg-info/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.937/tencentcloud_sdk_python_batch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-batch-3.0.937/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-batch
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Batch SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-batch-3.0.936/README.rst` & `tencentcloud-sdk-python-batch-3.0.937/README.rst`

 * *Files identical despite different names*

