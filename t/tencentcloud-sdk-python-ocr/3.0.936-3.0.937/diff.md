# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.936.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.937.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.936.tar", last modified: Mon Jul 17 00:32:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.937.tar", last modified: Tue Jul 18 00:28:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.936.tar` & `tencentcloud-sdk-python-ocr-3.0.937.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   115238 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)   816287 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-17 00:32:13.000000 tencentcloud-sdk-python-ocr-3.0.936/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   115253 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)   816315 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-18 00:28:23.000000 tencentcloud-sdk-python-ocr-3.0.937/README.rst
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/setup.py` & `tencentcloud-sdk-python-ocr-3.0.937/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,16 +948,16 @@
                 </tr>
                   <tr>
                   <td>身份证框内遮挡告警</td>
                 </tr>
                  <tr>
                   <td>临时身份证告警</td>
                 </tr>
-                  <tr>
-                  <td>身份证 PS 告警</td>
+                 <tr>
+                  <td>身份证疑似存在PS痕迹告警</td>
                 </tr>
                   <tr>
                   <td>图片模糊告警（可根据图片质量分数判断）</td>
                 </tr>
               </tbody>
             </table>
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.937/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6224,15 +6224,15 @@
         :type CardSide: str
         :param _Config: 以下可选字段均为bool 类型，默认false：
 CropIdCard，身份证照片裁剪（去掉证件外多余的边缘、自动矫正拍摄角度）
 CropPortrait，人像照片裁剪（自动抠取身份证头像区域）
 CopyWarn，复印件告警
 BorderCheckWarn，边框和框内遮挡告警
 ReshootWarn，翻拍告警
-DetectPsWarn，PS检测告警
+DetectPsWarn，疑似存在PS痕迹告警
 TempIdWarn，临时身份证告警
 InvalidDateWarn，身份证有效日期不合法告警
 Quality，图片质量分数（评价图片的模糊程度）
 MultiCardDetect，是否开启多卡证检测
 ReflectWarn，是否开启反光检测
 
 SDK 设置方式参考：
@@ -6327,15 +6327,15 @@
 WarnInfos，告警信息，Code 告警码列表和释义：
 -9100	身份证有效日期不合法告警，
 -9101	身份证边框不完整告警，
 -9102	身份证复印件告警，
 -9103	身份证翻拍告警，
 -9105	身份证框内遮挡告警，
 -9104	临时身份证告警，
--9106	身份证 PS 告警，
+-9106	身份证疑似存在PS痕迹告警，
 -9107       身份证反光告警。
         :type AdvancedInfo: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Name = None
         self._Sex = None
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.937/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.937/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.936
+Version: 3.0.937
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.936/README.rst` & `tencentcloud-sdk-python-ocr-3.0.937/README.rst`

 * *Files identical despite different names*

