# Comparing `tmp/nc_py_api-0.0.23.tar.gz` & `tmp/nc_py_api-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.23.tar", last modified: Fri Jul  7 18:45:52 2023, max compression
+gzip compressed data, was "nc_py_api-0.0.24.tar", last modified: Tue Jul 18 20:10:33 2023, max compression
```

## Comparing `nc_py_api-0.0.23.tar` & `nc_py_api-0.0.24.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12338 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    15409 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3796 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      731 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-07 18:45:52.000000 nc_py_api-0.0.23/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 18:45:45.000000 nc_py_api-0.0.23/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-07-07 18:45:52.886484 nc_py_api-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-07 18:45:37.000000 nc_py_api-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2640 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.022885 nc_py_api-0.0.24/nc_py_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13514 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/appconfig_preferences_ex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23440 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/integration_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4111 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/nextcloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/theming.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/ui_files_actions_menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4232 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/users_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/nc_py_api/weather_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/nc_py_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-18 20:10:33.000000 nc_py_api-0.0.24/nc_py_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 20:10:24.000000 nc_py_api-0.0.24/nc_py_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1782 2023-07-18 20:10:33.026886 nc_py_api-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-18 20:10:13.000000 nc_py_api-0.0.24/setup.py
```

### Comparing `nc_py_api-0.0.23/PKG-INFO` & `nc_py_api-0.0.24/nc_py_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: nc_py_api
-Version: 0.0.23
+Name: nc-py-api
+Version: 0.0.24
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
-License: Apache License 3.0
+License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
@@ -18,29 +18,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: bench
 Provides-Extra: dev
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Official Nextcloud Python Framework
 
 [![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
+[![Docs](https://github.com/cloud-py-api/nc_py_api/actions/workflows/docs.yml/badge.svg)](https://cloud-py-api.github.io/nc_py_api/)
+[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
+
+![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
-[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ### Remark
 
 Project cloud-py-api was **abandoned** and divided into two parts:
  * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
  * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
```

### Comparing `nc_py_api-0.0.23/README.md` & `nc_py_api-0.0.24/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Official Nextcloud Python Framework
 
 [![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
+[![Docs](https://github.com/cloud-py-api/nc_py_api/actions/workflows/docs.yml/badge.svg)](https://cloud-py-api.github.io/nc_py_api/)
+[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
+
+![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
-[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ### Remark
 
 Project cloud-py-api was **abandoned** and divided into two parts:
  * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
  * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
```

### Comparing `nc_py_api-0.0.23/nc_py_api/_session.py` & `nc_py_api-0.0.24/nc_py_api/_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Session represents one connection to Nextcloud. All related stuff for these live here.
 """
 
 import asyncio
 import hmac
 from abc import ABC, abstractmethod
+from collections.abc import Iterator
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from hashlib import sha256
 from json import dumps, loads
 from os import environ
 from typing import Optional, TypedDict, Union
 from urllib.parse import quote, urlencode
@@ -27,22 +28,21 @@
     micro: int
     string: str
     extended_support: bool
 
 
 @dataclass
 class BasicConfig:
-    full_nc_url: str
     endpoint: str
     dav_endpoint: str
     dav_url_suffix: str
 
     def __init__(self, **kwargs):
-        self.full_nc_url = self._get_value("nextcloud_url", **kwargs)
-        self.endpoint = self.full_nc_url.removesuffix("/index.php").removesuffix("/")
+        full_nc_url = self._get_value("nextcloud_url", **kwargs)
+        self.endpoint = full_nc_url.removesuffix("/index.php").removesuffix("/")
         self.dav_url_suffix = self._get_value("dav_url_suffix", raise_not_found=False, **kwargs)
         if not self.dav_url_suffix:
             self.dav_url_suffix = options.DAV_URL_SUFFIX
         self.dav_endpoint = self.endpoint + self.dav_url_suffix
 
     @staticmethod
     def _get_value(value_name: str, raise_not_found=True, **kwargs):
@@ -148,43 +148,59 @@
                     if str(ocs_meta["message"]).lower().find("password confirmation is required") != -1:
                         self.adapter.close()
                         self.init_adapter(restart=True)
                         return self._ocs(method, path_params, headers, data, **kwargs, nested_req=True)
             raise NextcloudException(status_code=ocs_meta["statuscode"], reason=ocs_meta["message"], info=info)
         return response_data["ocs"]["data"]
 
-    def dav(self, method: str, path: str, data: Optional[Union[str, bytes]] = None, **kwargs):
+    def dav(self, method: str, path: str, data: Optional[Union[str, bytes]] = None, **kwargs) -> Response:
         headers = kwargs.pop("headers", {})
         data_bytes = None
         if data is not None:
             data_bytes = data.encode("UTF-8") if isinstance(data, str) else data
         return self._dav(method, quote(self.cfg.dav_url_suffix + path), headers, data_bytes, **kwargs)
 
+    def dav_stream(
+        self, method: str, path: str, data: Optional[Union[str, bytes]] = None, **kwargs
+    ) -> Iterator[Response]:
+        headers = kwargs.pop("headers", {})
+        data_bytes = None
+        if data is not None:
+            data_bytes = data.encode("UTF-8") if isinstance(data, str) else data
+        return self._dav_stream(method, quote(self.cfg.dav_url_suffix + path), headers, data_bytes, **kwargs)
+
     def _dav(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Response:
         self.init_adapter()
         timeout = kwargs.pop("timeout", options.TIMEOUT_DAV)
         return self.adapter.request(
             method, self.cfg.endpoint + path, headers=headers, content=data, timeout=timeout, **kwargs
         )
 
+    def _dav_stream(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Iterator[Response]:
+        self.init_adapter()
+        timeout = kwargs.pop("timeout", options.TIMEOUT_DAV)
+        return self.adapter.stream(
+            method, self.cfg.endpoint + path, headers=headers, content=data, timeout=timeout, **kwargs
+        )
+
     def init_adapter(self, restart=False) -> None:
         if getattr(self, "adapter", None) is None or restart:
             if restart and hasattr(self, "adapter"):
                 self.adapter.close()
             self.adapter = self._create_adapter()
             self.adapter.headers.update({"OCS-APIRequest": "true"})
             if self.custom_headers:
                 self.adapter.headers.update(self.custom_headers)
             if options.XDEBUG_SESSION:
                 self.adapter.cookies.set("XDEBUG_SESSION", options.XDEBUG_SESSION)
             self._capabilities = {}
 
     @abstractmethod
     def _create_adapter(self) -> Client:
-        pass
+        pass  # pragma: no cover
 
     def update_server_info(self) -> None:
         self._capabilities = self.ocs(method="GET", path="/ocs/v1.php/cloud/capabilities")
 
     @property
     def capabilities(self) -> dict:
         if not self._capabilities:
@@ -209,15 +225,17 @@
     cfg: Config
 
     def __init__(self, **kwargs):
         self.cfg = Config(**kwargs)
         super().__init__(user=self.cfg.auth[0])
 
     def _create_adapter(self) -> Client:
-        return Client(auth=self.cfg.auth, follow_redirects=True, limits=self.limits)
+        return Client(
+            auth=self.cfg.auth, follow_redirects=True, limits=self.limits, verify=options.VERIFY_NC_CERTIFICATE
+        )
 
 
 class NcSessionApp(NcSessionBasic):
     cfg: AppConfig
 
     def __init__(self, **kwargs):
         self.cfg = AppConfig(**kwargs)
@@ -227,16 +245,20 @@
         self.sign_request(method, path_params, headers, data)
         return super()._ocs(method, path_params, headers, data, **kwargs)
 
     def _dav(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Response:
         self.sign_request(method, path, headers, data)
         return super()._dav(method, path, headers, data, **kwargs)
 
+    def _dav_stream(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Iterator[Response]:
+        self.sign_request(method, path, headers, data)
+        return super()._dav_stream(method, path, headers, data, **kwargs)
+
     def _create_adapter(self) -> Client:
-        adapter = Client(follow_redirects=True, limits=self.limits)
+        adapter = Client(follow_redirects=True, limits=self.limits, verify=options.VERIFY_NC_CERTIFICATE)
         adapter.headers.update(
             {
                 "AE-VERSION": self.cfg.ae_version,
                 "EX-APP-ID": self.cfg.app_name,
                 "EX-APP-VERSION": self.cfg.app_version,
             }
         )
```

### Comparing `nc_py_api-0.0.23/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.24/nc_py_api/appconfig_preferences_ex.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/constants.py` & `nc_py_api-0.0.24/nc_py_api/constants.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/exceptions.py` & `nc_py_api-0.0.24/nc_py_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.24/nc_py_api/integration_fastapi.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/misc.py` & `nc_py_api-0.0.24/nc_py_api/misc.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/nextcloud.py` & `nc_py_api-0.0.24/nc_py_api/nextcloud.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/preferences.py` & `nc_py_api-0.0.24/nc_py_api/preferences.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/theming.py` & `nc_py_api-0.0.24/nc_py_api/theming.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.24/nc_py_api/ui_files_actions_menu.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/users.py` & `nc_py_api-0.0.24/nc_py_api/users.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/users_groups.py` & `nc_py_api-0.0.24/nc_py_api/users_groups.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/users_status.py` & `nc_py_api-0.0.24/nc_py_api/users_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api/weather_status.py` & `nc_py_api-0.0.24/nc_py_api/weather_status.py`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.23/nc_py_api.egg-info/PKG-INFO` & `nc_py_api-0.0.24/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: nc-py-api
-Version: 0.0.23
+Name: nc_py_api
+Version: 0.0.24
 Summary: Nextcloud Python Framework
 Home-page: https://github.com/cloud-py-api/nc_py_api
 Author: Alexander Piskun
-License: Apache License 3.0
+License: BSD-3-Clause
 Project-URL: Source, https://github.com/cloud-py-api/nc_py_api
 Keywords: nextcloud,api,framework
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
@@ -18,29 +18,35 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: bench
 Provides-Extra: dev
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # Official Nextcloud Python Framework
 
 [![Analysis & Coverage](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml/badge.svg)](https://github.com/cloud-py-api/nc_py_api/actions/workflows/analysis-coverage.yml)
+[![Docs](https://github.com/cloud-py-api/nc_py_api/actions/workflows/docs.yml/badge.svg)](https://cloud-py-api.github.io/nc_py_api/)
+[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
+
+![NextcloudVersion](https://img.shields.io/badge/Nextcloud-26%20%7C%2027%20%7C%2028-blue)
 ![PythonVersion](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
 ![impl](https://img.shields.io/pypi/implementation/nc_py_api)
 ![pypi](https://img.shields.io/pypi/v/nc_py_api.svg)
-[![codecov](https://codecov.io/github/cloud-py-api/nc_py_api/branch/main/graph/badge.svg?token=C91PL3FYDQ)](https://codecov.io/github/cloud-py-api/nc_py_api)
 
 ### Remark
 
 Project cloud-py-api was **abandoned** and divided into two parts:
  * `nc_py_api` - this repository, which contains Python Framework to work with Nextcloud and `app_ecosystem_v2`
  * `app_ecosystem_v2` - New [Nextcloud Application Ecosystem](https://github.com/cloud-py-api/app_ecosystem_v2) that allows writing applications for Nextcloud in any language
```

### Comparing `nc_py_api-0.0.23/nc_py_api.egg-info/SOURCES.txt` & `nc_py_api-0.0.24/nc_py_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 CHANGELOG.md
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 nc_py_api/__init__.py
 nc_py_api/_session.py
```

### Comparing `nc_py_api-0.0.23/pyproject.toml` & `nc_py_api-0.0.24/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 ]
 
 [tool.black]
 line-length = 120
 target-versions = ["py39"]
 preview = true
 
+[tool.ruff]
+line-length = 120
+target-version = "py39"
+
+[tool.ruff.per-file-ignores]
+"nc_py_api/__init__.py" = ["F401"]
+
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = [
     "tests",
```

### Comparing `nc_py_api-0.0.23/setup.cfg` & `nc_py_api-0.0.24/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -18,37 +18,45 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
-	License :: OSI Approved :: GNU Affero General Public License v3
+	License :: OSI Approved :: BSD License
+	Operating System :: MacOS :: MacOS X
 	Operating System :: POSIX :: Linux
-license = Apache License 3.0
+	Operating System :: Microsoft :: Windows
+license = BSD-3-Clause
 project_urls = 
 	Source=https://github.com/cloud-py-api/nc_py_api
 
 [options]
 python_requires = >=3.9
 zip_safe = True
 packages = find:
 install_requires = 
-	requests
-	httpx
-	xmltodict
-	pydantic
-	xxhash
-	fastapi
+	requests==2.31.0
+	httpx==0.24.1
+	xmltodict==0.13.0
+	pydantic==2.0.3
+	xxhash==3.2.0
+	fastapi==0.100.0
 
 [options.extras_require]
 docs = 
 	sphinx>=4.4
 	sphinx-issues>=3.0.1
 	sphinx-rtd-theme>=1.0
+	sphinx-copybutton
+	sphinx-inline-tabs
+bench = 
+	matplotlib
+	py-cpuinfo
+	numpy
 dev = 
 	pytest
 	pre-commit
 	pylint
 	coverage
 	pillow
 	uvicorn
```

