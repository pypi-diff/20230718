# Comparing `tmp/tmsproviderapisdk-0.1.2.tar.gz` & `tmp/tmsproviderapisdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmsproviderapisdk-0.1.2.tar", last modified: Mon Jul 17 13:59:50 2023, max compression
+gzip compressed data, was "tmsproviderapisdk-0.1.3.tar", last modified: Tue Jul 18 07:09:47 2023, max compression
```

## Comparing `tmsproviderapisdk-0.1.2.tar` & `tmsproviderapisdk-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-17 13:59:49.000000 tmsproviderapisdk-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/tmsproviderapisdk/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_extended_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-17 13:59:37.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:59:50.428524 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 13:59:50.000000 tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:09:47.962818 tmsproviderapisdk-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-18 07:09:47.962818 tmsproviderapisdk-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:09:47.962818 tmsproviderapisdk-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 07:09:47.000000 tmsproviderapisdk-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:09:47.962818 tmsproviderapisdk-0.1.3/tmsproviderapisdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_device_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_devices_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_extended_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-18 07:09:37.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_tarif_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:09:47.962818 tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-18 07:09:47.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 07:09:47.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:09:47.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:09:47.000000 tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/top_level.txt
```

### Comparing `tmsproviderapisdk-0.1.2/LICENSE` & `tmsproviderapisdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/PKG-INFO` & `tmsproviderapisdk-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmsproviderapisdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: TVIP TMS provider api sdk
 Home-page: https://github.com/tvip/tmsproviderapisdk
 Author: Tvip
 Author-email: td@tvip.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tmsproviderapisdk-0.1.2/setup.py` & `tmsproviderapisdk-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmsproviderapisdk",
-    version="0.1.2",
+    version="0.1.3",
     author="Tvip",
     author_email="td@tvip.ru",
     description="TVIP TMS provider api sdk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tvip/tmsproviderapisdk",
     packages=setuptools.find_packages(),
```

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/__init__.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+from pkg_resources import get_distribution, DistributionNotFound
+
+try:
+    __version__ = get_distribution('tmsproviderapisdk').version
+except DistributionNotFound:
+    __version__ = 'unknown'
+
 from tmsproviderapisdk.tms_config import TmsConfig, TmsConfigHolder
 from tmsproviderapisdk.tms_account import TmsAccount
 from tmsproviderapisdk.tms_account_subscription import TmsAccountSubscription
 from tmsproviderapisdk.tms_channel import TmsChannel
 from tmsproviderapisdk.tms_device import TmsDevice
 from tmsproviderapisdk.tms_device_subscription import TmsDeviceSubscription
 from tmsproviderapisdk.tms_tarif import TmsTarif
 from tmsproviderapisdk.tms_tarif_tag import TmsTarifTag
 from tmsproviderapisdk.tms_region import TmsRegion
 from tmsproviderapisdk.tms_account_network import TmsAccountNetwork
+from tmsproviderapisdk.tms_devices_types import TmsDeviceTypes
```

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_network.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account_network.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_account_subscription.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_account_subscription.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_base_model.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_base_model.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_channel.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_channel.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_config.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import base64
-
-
+from tmsproviderapisdk import __version__
 class TmsConfig:
 
     def __init__(self, base_url: str, username: str = None, password: str = None, token: str = None):
 
         self.base_url = base_url
         self.username = username
         self.password = password
@@ -12,14 +11,17 @@
         self.headers = None
         self._configure()
 
     def _configure(self):
         self.base_url = self.base_url + '/api/provider'
 
         headers = {
+            'User-Agent': 'Tmsproviderapisdk v:{}'.format(
+                __version__
+            ),
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         if self.username and (self.password or self.token):
             if self.password:
                 login_password = "{}:{}".format(
```

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_device.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_device_subscription.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_device_subscription.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_exceptions.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_extended_model.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_extended_model.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_provider.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_provider.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_region.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_region.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_tarif.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk/tms_tarif_tag.py` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk/tms_tarif_tag.py`

 * *Files identical despite different names*

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/PKG-INFO` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmsproviderapisdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: TVIP TMS provider api sdk
 Home-page: https://github.com/tvip/tmsproviderapisdk
 Author: Tvip
 Author-email: td@tvip.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tmsproviderapisdk-0.1.2/tmsproviderapisdk.egg-info/SOURCES.txt` & `tmsproviderapisdk-0.1.3/tmsproviderapisdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 tmsproviderapisdk/tms_account_network.py
 tmsproviderapisdk/tms_account_subscription.py
 tmsproviderapisdk/tms_base_model.py
 tmsproviderapisdk/tms_channel.py
 tmsproviderapisdk/tms_config.py
 tmsproviderapisdk/tms_device.py
 tmsproviderapisdk/tms_device_subscription.py
+tmsproviderapisdk/tms_devices_types.py
 tmsproviderapisdk/tms_exceptions.py
 tmsproviderapisdk/tms_extended_model.py
 tmsproviderapisdk/tms_provider.py
 tmsproviderapisdk/tms_region.py
 tmsproviderapisdk/tms_tarif.py
 tmsproviderapisdk/tms_tarif_tag.py
 tmsproviderapisdk.egg-info/PKG-INFO
```

