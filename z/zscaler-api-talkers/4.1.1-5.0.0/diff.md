# Comparing `tmp/zscaler_api_talkers-4.1.1.tar.gz` & `tmp/zscaler_api_talkers-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_api_talkers-4.1.1.tar", max compression
+gzip compressed data, was "zscaler_api_talkers-5.0.0.tar", max compression
```

## Comparing `zscaler_api_talkers-4.1.1.tar` & `zscaler_api_talkers-5.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-4.1.1/LICENSE.txt
--rw-r--r--   0        0        0     4541 2023-07-05 00:56:15.951278 zscaler_api_talkers-4.1.1/README.md
--rw-r--r--   0        0        0      434 2023-07-05 03:00:17.891927 zscaler_api_talkers-4.1.1/pyproject.toml
--rw-r--r--   0        0        0      441 2023-07-05 01:15:40.406964 zscaler_api_talkers-4.1.1/zscaler_api_talkers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.707836 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zcc_talker/__init__.py
--rw-r--r--   0        0        0     7195 2023-07-05 01:15:40.407601 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zcc_talker/zcc_talker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.708427 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/__init__.py
--rw-r--r--   0        0        0    14324 2023-07-05 01:15:40.408211 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.709020 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/__init__.py
--rw-r--r--   0        0        0     1144 2023-07-05 01:15:40.408775 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/helpers.py
--rw-r--r--   0        0        0    13788 2023-06-29 23:34:03.620027 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/models.py
--rw-r--r--   0        0        0    15558 2023-07-05 01:15:40.409383 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_portaltalker.py
--rw-r--r--   0        0        0    75250 2023-07-05 01:15:40.410190 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_talker.py
--rw-r--r--   0        0        0        0 2023-06-27 20:53:48.710832 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/__init__.py
--rw-r--r--   0        0        0     3627 2023-07-05 01:15:40.410779 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/zpa_portaltalker.py
--rw-r--r--   0        0        0    26074 2023-07-05 01:15:40.411442 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/zpa_talker.py
--rw-r--r--   0        0        0      205 2023-07-05 00:56:15.958091 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/__init__.py
--rw-r--r--   0        0        0     8820 2023-07-05 00:56:15.958333 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/http_calls.py
--rw-r--r--   0        0        0     1724 2023-07-05 00:56:15.958655 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/logger.py
--rw-r--r--   0        0        0     6482 2023-07-05 00:56:15.958902 zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/utilities.py
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 zscaler_api_talkers-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-21 16:27:44.526756 zscaler_api_talkers-5.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4641 2023-07-11 14:25:40.148396 zscaler_api_talkers-5.0.0/README.md
+-rw-r--r--   0        0        0      455 2023-07-18 01:31:52.736800 zscaler_api_talkers-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      470 2023-07-11 14:25:40.155870 zscaler_api_talkers-5.0.0/zscaler_api_talkers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.156073 zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/__init__.py
+-rw-r--r--   0        0        0     7610 2023-07-18 01:05:14.039703 zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/talker.py
+-rw-r--r--   0        0        0      205 2023-07-17 12:24:00.512588 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/__init__.py
+-rw-r--r--   0        0        0     8821 2023-07-17 16:09:13.247599 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/http_calls.py
+-rw-r--r--   0        0        0     1724 2023-07-11 14:25:40.157783 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/logger.py
+-rw-r--r--   0        0        0     6482 2023-07-11 14:25:40.157979 zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158067 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/__init__.py
+-rw-r--r--   0        0        0    14350 2023-07-17 12:24:00.513688 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/portal_talker.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.158774 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-11 14:25:40.159069 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/helpers.py
+-rw-r--r--   0        0        0    13788 2023-07-11 14:25:40.159489 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/models.py
+-rw-r--r--   0        0        0    43204 2023-07-17 12:24:00.514405 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/portal_talker.py
+-rw-r--r--   0        0        0    80884 2023-07-17 12:24:00.515262 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/talker.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:25:40.161421 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/__init__.py
+-rw-r--r--   0        0        0    14603 2023-07-17 12:24:00.515998 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/portal_talker.py
+-rw-r--r--   0        0        0    31531 2023-07-17 12:27:01.950284 zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/talker.py
+-rw-r--r--   0        0        0     5306 1970-01-01 00:00:00.000000 zscaler_api_talkers-5.0.0/PKG-INFO
```

### Comparing `zscaler_api_talkers-4.1.1/LICENSE.txt` & `zscaler_api_talkers-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.1/README.md` & `zscaler_api_talkers-5.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 # Unofficial Zscaler API talkers
 
 ## API Talkers
 
 ### ZIA API Talker
 Python classes to leverage [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
-The ZIA API talker is divided into two Class objects: ZiaTalker and ZiaPortalTalker.  ZiaTalker interacts with ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
+The ZIA API talker is divided into two Class objects: **ZiaTalker** and **ZiaPortalTalker**.  ZiaTalker interacts with 
+ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
 
 ### ZPA API Talker
 Python classes to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
 
-The ZPA API talker is divided into two Class objects: ZpaTalker and ZpaPortalTalker.  ZpaTalker interacts with ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
+The ZPA API talker is divided into two Class objects: **ZpaTalker** and **ZpaPortalTalker**.  ZpaTalker interacts with 
+ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
 
-### ZCC API Talker
+### Client Connector API Talker
 A Python class to leverage Zscaler Client Connector API. (Currently in Beta status.)
 
-The ZCC API talker is accessed via the Class object named: ZccTalker
+The Client Connector API talker is accessed via the Class object named: **ClientConnectorTalker**
 
 ### ZDX API Talker
 A Python class to leverage Zscaler Digital Experience API. (Currently in development.)
 
-This class is interacts with ZDX via the URLs presented in the Portal (aka, the ZDX configuration website).  It is named: ZdxPortalTalker
+This class is interacts with ZDX via the URLs presented in the Portal (aka, the ZDX configuration website).  It is 
+named: **ZdxPortalTalker**
 
 ## Installation
 
-### Option 1: Run within a Docker Container
+### Option 1: Run in a Python Virtual Environment
+1. Create a virtual Environment: `python3 -m venv .zs_api_talkers`
+1. Activate virtual environment:
+   - Linux: `source .zs_api_talkers/bin/activate`
+   - Windows: `.\.zs_api_talkers\Scripts\activate`
+1. Install Zscaler API talkers: `pip install zscaler-api-talkers`
+
+### Option 2: Run within a Docker Container
 We provide two methods to build a Docker container.  Either using the code hosted on GitHub or the code published to PyPi.
 
-#### GitHub Method
+#### PyPi Method
 1. Download Dockerfile
-   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile`
-   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile` 
+   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile`
+   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile` 
 1. Build Image and Run Container
-   1. `docker build -f git_version.Dockerfile -t zscaler_api_talkers .`
+   1. `docker build -t zscaler_api_talkers .`
    1. `docker run -it zscaler_api_talkers bash`
 1. Usage (program is in /zscaler_api_talkers/)
    - `cd zscaler_api_talkers`
 
-#### PyPi Method
+#### GitHub Method
 1. Download Dockerfile
-   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile`
-   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile` 
+   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile`
+   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile` 
 1. Build Image and Run Container
-   1. `docker build -t zscaler_api_talkers .`
+   1. `docker build -f git_version.Dockerfile -t zscaler_api_talkers .`
    1. `docker run -it zscaler_api_talkers bash`
 1. Usage (program is in /zscaler_api_talkers/)
    - `cd zscaler_api_talkers`
 
-### Option 2: Run in a Python Virtual Environment
-1. Create a virtual Environment: `python3 -m venv .zs_api_talkers`
-1. Activate virtual environment:
-   - Linux: `source .zs_api_talkers/bin/activate`
-   - Windows: `.\.zs_api_talkers\Scripts\activate`
-1. Install Zscaler API talkers: `pip install zscaler-api-talkers`
-
-
 ## Zscaler Secure Internet and SaaS Access SDK
 
 ### Usage ZiaTalker
 ``` python
 from zscaler_api_talkers import ZiaTalker
 zia=ZiaTalker('<Zscaler Cloud Name>')
 zia.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
@@ -88,18 +90,18 @@
 a.authenticate(client_id='clientID',client_secret='clientSecret')
 # To view all methods available
 print(dir(a))
 ```
 
 ## Zscaler Client Connector SDK
 
-### Usage ZccTalker
+### Usage ClientConnectorTalker
 ``` python
-from zscaler_api_talkers import ZccTalker
-a=ZccTalker('<Zscaler Cloud Name>')    
+from zscaler_api_talkers import ClientConnectorTalker
+a=ClientConnectorTalker('<Zscaler Cloud Name>')    
 a.authenticate(clientid='clientID',secretkey='clientSecret')
 a.list_devices('companyID')
 a.list_OTP('companyID','user device id')
 # To view all methods available
 print(dir(a))
 ```
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zcc_talker/zcc_talker.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/client_connector/talker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
+import pdb
 import time
-
-from zscaler_api_talkers.zscaler_helpers.http_calls import HttpCalls
-from zscaler_api_talkers.zscaler_helpers.logger import setup_logger
+import requests
+from zscaler_api_talkers.helpers.http_calls import HttpCalls
+from zscaler_api_talkers.helpers.logger import setup_logger
 
 logger = setup_logger(name=__name__)
 
 
-class ZccTalker(object):
+class ClientConnectorTalker(object):
     """
     Client Connector API talker
     Documentation: under development
     Currently in beta status
     """
 
     def __init__(
-        self,
-        cloud: str,
-        client_id: str = "",
-        secret_key: str = "",
+            self,
+            cloud: str,
+            client_id: str = "",
+            secret_key: str = "",
     ):
         """
         :param cloud: (str) Top Level Domain (TLD) of the Zscaler cloud where tenant resides.
         :param client_id: (str) Client ID
         :param secret_key: (str) Secret Key
         """
         self.base_uri = f"https://api-mobile.{cloud}/papi"
@@ -36,17 +37,17 @@
         if client_id and secret_key:
             self.authenticate(
                 client_id=client_id,
                 secret_key=secret_key,
             )
 
     def authenticate(
-        self,
-        client_id: str,
-        secret_key: str,
+            self,
+            client_id: str,
+            secret_key: str,
     ):
         """
         Method to authenticate.
 
         :param client_id: (str) Client id
         :param secret_key: (str) Client secret, obtained from portal.
         """
@@ -59,19 +60,19 @@
             url=url,
             headers={"Accept": "*/*"},
             payload=payload,
         )
         self.header = {"auth-token": response.json()["jwtToken"]}
 
     def _obtain_all(
-        self,
-        url: str,
-        cookies: dict = None,
-        params: dict = None,
-        headers: dict = None,
+            self,
+            url: str,
+            cookies: dict = None,
+            params: dict = None,
+            headers: dict = None,
     ) -> json:
         """
         Internal method that queries all pages
 
         :param url: (str) URL
         :param cookies: (dict?) Cookies
         :param params: (dict) Parameters to pass in request
@@ -95,177 +96,173 @@
                 time.sleep(0.5)
             else:
                 break
 
         return result
 
     def list_devices(
-        self,
-        company_id: int,
-        username: str = None,
-        os_type: str = None,
+            self,
+            username: str = None,
+            os_type: str = None,
     ) -> json:
         """
-        Method to authenticate.
-
-        :param company_id: (int) ORG ID
+        Gets the list of all enrolled devices of your organization and their basic details.
         :param username: (str) Username in email format
-        :param os_type: (str)
-
+        :param os_type: (str)  1 - iOS, 2 - Android, 3 - Windows, 4 - macOS, 5 - Linux
         :return: (json) JSON of results
         """
-        url = "/public/v1/getDevices"
-        parameters = {
-            "companyId": company_id,
-        }
+        url = "/public/v1/getDevices?pageSize=500"
         if username:
-            parameters.update({"username": username})
-        elif os_type:
-            parameters.update({"osType": os_type})
-        else:
-            parameters.update({"pagesize": 100})
+            url += f'&username={username}'
+        if os_type:
+            url += f'&osType={os_type}'
+
         response = self._obtain_all(
             url=url,
-            params=parameters,
             headers=self.header,
         )
 
         return response
 
     def list_otp(
-        self,
-        company_id: int,
-        ud_id: int,
+            self,
+            ud_id: int,
     ) -> json:
         """
         Method to fetch the One Time Password for a specific device. These passwords are unique and tied to a device
         UDID.
-
-        :param company_id: (int) ORG ID
         :param ud_id: (int) User device ID
-
         :return: (json) JSON of results
         """
         url = f"/public/v1/getOtp"
         parameters = {
-            "companyId": company_id,
             "udid": ud_id,
         }
         response = self.hp_http.get_call(
             url=url,
             params=parameters,
             headers=self.header,
         )
 
         return response.json()
 
     def list_passwords(
-        self,
-        company_id: int,
-        ud_id: int,
+            self,
+            ud_id: int,
     ):
         """
         Method to fetch the One Time Password for a specific device. These passwords are unique and tied to a device UDID
 
-        :param company_id: (int) ORG ID
         :param ud_id: (int) User device ID
-
         :return: (json) JSON of results
         """
         url = f"/public/v1/getOtp"
         parameters = {
-            "companyId": company_id,
             "udid": ud_id,
         }
         response = self.hp_http.get_call(
             url=url,
             params=parameters,
             headers=self.header,
         )
 
         return response.json()
 
     def remove_devices(
-        self,
-        company_id: int,
-        ud_ids: list,
-        os_type: int = 0,
+            self,
+            username: str = None,
+            client_connector_version: str = None,
+            ud_ids: list = None,
+            os_type: int = 0,
     ) -> json:
         """
         Method to  mark the device for removal (Device Removal Pending).
         API currently can remove up to 30 devices per call
-
-        :param company_id: type int. ORG ID
+        :param username: type str. Userna,e
         :param ud_ids: type list. List of user devices ids
         :param os_type: 0 ALL OS types, 1 IOS, 2 Android, 3 Windows, 4 macOS, 5 Linux
-
+        :param client_connector_version: Client connector version
         :return: (json) JSON of results
         """
         url = f"/public/v1/removeDevices"
         payload = {
-            "companyId": company_id,
+            "userName": username,
+            "clientConnectorVersion": client_connector_version,
             "udids": ud_ids,
             "osType": os_type,
         }
         response = self.hp_http.post_call(
             url=url,
             headers=self.header,
             payload=payload,
         )
 
         return response.json()
 
     def force_remove_devices(
-        self,
-        company_id: int,
-        ud_ids: list = None,
-        os_type: int = 0,
+            self,
+            username: str = None,
+            client_connector_version: str = None,
+            ud_ids: list = None,
+            os_type: int = 0,
     ) -> json:
         """
         Force Remove, has the same effect as Remove, though it additionally moves the device straight to Removed and also
         signals the cloud to invalidate the user’s session.
         API currently can remove up to 30 devices per call
 
-        :param company_id: (int) ORG ID
+        :param client_connector_version: (str) ZCC version
         :param ud_ids: (list) List of user devices ids
         :param os_type: (int) 0 ALL OS types, 1 IOS, 2 Android, 3 Windows, 4 macOS, 5 Linux
+        :param username:(str) Username
 
         :return: (json) JSON of results
         """
         if ud_ids is None:
             ud_ids = []
         url = f"/public/v1/forceRemoveDevices"
         payload = {
-            "companyId": company_id,
+            "clientConnectorVersion": client_connector_version,
             "udids": ud_ids,
             "osType": os_type,
+            "userName": username
         }
         response = self.hp_http.post_call(
             url=url,
             headers=self.header,
             payload=payload,
         )
 
         return response.json()
 
-    def download_service_status(
-        self,
-        company_id: int,
-    ) -> json:
+    def list_download_service_status(
+            self,
+    ) -> requests.Response.content:
         """
         Method to download Service Status
-
-        :param company_id: (int) ORG ID
-
         :return: (str) String of results
         """
         url = "/public/v1/downloadServiceStatus"
-        parameters = {
-            "companyId": company_id,
-        }
+
         response = self.hp_http.get_call(
             url=url,
-            params=parameters,
             headers=self.header,
         )
 
-        return response.json()
+        return response.content
+
+
+class ZccTalker(ClientConnectorTalker):
+    def __init__(
+            self,
+            cloud: str,
+            client_id: str = "",
+            secret_key: str = "",
+    ):
+        logger.warning(
+            "Deprecating ZccTalker. Start using ClientConnectorTalker instead."
+        )
+        super().__init__(
+            cloud,
+            client_id,
+            secret_key,
+        )
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zdx_talker/zdx_portaltalker.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zdx/portal_talker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
 import urllib
 
-import json
 import requests
-from zscaler_api_talkers.zscaler_helpers import request_, get_user_agent, setup_logger
+
+from zscaler_api_talkers.helpers import get_user_agent, request_, setup_logger
 
 logger = setup_logger(name=__name__)
 
 
 class ZdxPortalTalker:
     def __init__(
         self,
@@ -16,15 +17,17 @@
     ):
         """Class object to provide access to ZDX via web portal backend APIs.
 
         :param username: (str) Admin username
         :param password: (str) Admin password
         :param zia_cloud: (str) ZIA Portal associated with this ZDX tenant. Example: "zscalerthree.net"
         """
-        logger.warning("These API endpoints are unsupported and Zscaler can change at will and without notice.")
+        logger.warning(
+            "These API endpoints are unsupported and Zscaler can change at will and without notice."
+        )
         self.username = username
         self.password = password
         self.base_url = "https://admin.zdxcloud.net"
         self.api_base_url = f"{self.base_url}/zdx/api/v1"
         self.headers = {
             "User-Agent": get_user_agent(),
             "X-CSRF-Token": "Fetch",
@@ -270,16 +273,18 @@
         return result.json()
 
     def zia_authenticate(
         self,
         **kwargs,
     ):
         """Cross authentication into ZIA to work on user and roles."""
-        logger.warning("Regular ZDX methods will no longer work after ZIA auth.  Create a new ZdxPortalTalker object "
-                       "if further access is needed.")
+        logger.warning(
+            "Regular ZDX methods will no longer work after ZIA auth.  Create a new ZdxPortalTalker object "
+            "if further access is needed."
+        )
         result = request_(
             method="post",
             url=f"{self.api_base_url}/auth/token",
             headers=self.headers,
             data=f'["{self.zia_cloud}"]',
             cookies=self.cookie_jar,
             **kwargs,
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/helpers.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 
-from zscaler_api_talkers.zscaler_helpers import request_
+from zscaler_api_talkers.helpers import request_
 
 
 def _obfuscate_api_key(
     seed: str,
 ) -> (time, str):
     """
     Internal method to Obfuscate the API key
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/models.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/models.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zia_talker/zia_talker.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zia/talker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import json
 import pdb  # noqa
 import time
 
 import requests
-from zscaler_api_talkers.zia_talker.models import (super_categories, valid_category_ids, valid_countries)
-from zscaler_api_talkers.zscaler_helpers import HttpCalls, setup_logger
 
-from .helpers import _obfuscate_api_key
+from zscaler_api_talkers.helpers import HttpCalls, setup_logger
+from zscaler_api_talkers.zia.models import (
+    super_categories,
+    valid_category_ids,
+    valid_countries,
+)
+
+from zscaler_api_talkers.zia.helpers import _obfuscate_api_key
 
 logger = setup_logger(name=__name__)
 
 
 class ZiaTalker(object):
     """
     ZIA API talker
@@ -281,14 +286,81 @@
             if query:
                 url = f"/adminUsers?{query}?pageSize=1000"
             else:
                 url = "/adminUsers?pageSize=1000"
 
         return self._obtain_all(url)
 
+    def add_admin_users(self, loginName: str, userName: str, email: str, password: str, role: dict, comments: str = '',
+                       adminScopeType: str ='ORGANIZATION',
+                       adminScopeScopeEntities: list =[],
+                       adminScopescopeGroupMemberEntities: list =[],
+                       isNonEditable: bool = False,
+                       disabled: bool = False,
+                       isAuditor: bool = False,
+                       isPasswordLoginAllowed: object = False,
+                       isSecurityReportCommEnabled: object = False,
+                       isServiceUpdateCommEnabled: object = False,
+                       isProductUpdateCommEnabled: object = False,
+                       isPasswordExpired: object = False,
+                       isExecMobileAppEnabled: object = False,
+                       execMobileAppTokens: object = []) -> json:
+        """
+        Adds a new Admininstrator.
+               :param loginName: string. Admin or auditor's login name. loginName is in email format
+               and uses the domain name associated to the Zscaler account.
+               :param userName: string. UserName.
+               :param email: string. Email Address.
+               :param password: string. Password for administrator. If admin single sign-on (SSO) is disabled, then this field is mandatory
+               :param role : Role of the Admin
+               :param comments: string. Comments.
+               :param adminScopeType: string. Scope of the admin.
+               :param adminScopeScopeEntities: list: Department or Location when adminScopeType is set to Deportment or Location.
+               :param adminScopescopeGroupMemberEntities: list. Location Groups when adminScopeType is set to Location Group.
+               :param isNonEditable: boolean. Indicates whether or not the admin can be edited or deleted. default: False.
+               :param disabled: boolean. If admin accounts is disabled. default: False.
+               :param isAuditor:boolean. Indicates if user is auditor. default: False.
+               :param isPasswordLoginAllowed: boolean. If password login is allowed. default: False.
+               :param isSecurityReportCommEnabled: boolean. Communication for Security Report is enabled. default: False.
+               :param isServiceUpdateCommEnabled: boolean. Communication setting for Service Update. default: False.
+               :param isProductUpdateCommEnabled: boolean. Communication setting for Product Update. default: False.
+               :param isPasswordExpired: boolean. Expire password to force user to change password on logon. default: False.
+               :param isExecMobileAppEnabled: boolean. Indicates whether or not Executive Insights App access is enabled for the admin. default: False.
+               :return:json()
+               """
+        url = "/adminUsers"
+        payload = {
+            "loginName": loginName,
+            "userName": userName,
+            "email": email,
+            "password": password,
+            "role": role,
+            "comments": comments,
+            "adminScopeType": adminScopeType,
+            "adminScopeScopeEntities": adminScopeScopeEntities,
+            "adminScopescopeGroupMemberEntities": adminScopescopeGroupMemberEntities,
+            "isNonEditable": isNonEditable,
+            "disabled": disabled,
+            "isAuditor": isAuditor,
+            "isPasswordLoginAllowed": isPasswordLoginAllowed,
+            "isSecurityReportCommEnabled": isSecurityReportCommEnabled,
+            "isServiceUpdateCommEnabled": isServiceUpdateCommEnabled,
+            "isProductUpdateCommEnabled": isProductUpdateCommEnabled,
+            "isPasswordExpired": isPasswordExpired,
+            "isExecMobileAppEnabled": isExecMobileAppEnabled,
+            "execMobileAppTokens": execMobileAppTokens
+        }
+        response = self.hp_http.post_call(
+            url,
+            payload=payload,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
+        )
+        return response.json()
     def list_admin_roles(
         self,
         query: str = None,
     ) -> json:
         """
         Gets a name and ID dictionary of al admin roles
 
@@ -351,22 +423,23 @@
 
         return response.json()
 
     def add_url_categories(
         self,
         name: str,
         super_category: str,
-        type_list: list = None,
+        type_list: str = None,
         urls: list = None,
         db_categorized_urls: list = None,
         keywords_retaining_parent_category: list = None,
         keywords: list = None,
         custom_category: bool = False,
         ip_ranges: list = None,
         ip_ranges_retaining_parent_category: list = None,
+        description: str = None,
     ) -> json:
         """
          Adds a new custom URL category.
 
         :param name: (str) Name of the custom category. Possible values URL_CATEGORY, TLD_CATEGORY, ALL
         :param super_category: (str) super category
         :param type_list: (list)
@@ -375,39 +448,47 @@
         :param keywords_retaining_parent_category: (list) Retained custom keywords from the parent URL category that is
         associated to a URL category.
         :param keywords: (list) Custom keywords associated to a URL category.
         :param custom_category: (bool) Default False. Set to True for custom category
         :param ip_ranges: (list) Custom IP address ranges associated to a URL category
         :param ip_ranges_retaining_parent_category: (list) The retaining parent custom IP address ranges associated to a
         URL category.
+        :param description: (str) Description or notes
 
         :return:  json
         """
         if not type_list:
-            type_list = ["URL_CATEGORY"]
+            type_list = "URL_CATEGORY"
 
         if keywords_retaining_parent_category is None:
             keywords_retaining_parent_category = []
 
         if super_category not in super_categories:
             logger.error(f"Invalid Super Category: {super_categories}")
             raise ValueError("Invalid super category")
 
+        if keywords is None:
+            keywords = []
+
+        if ip_ranges is None:
+            ip_ranges = []
+
         url = "/urlCategories"
         payload = {
             "configuredName": name,
             "customCategory": custom_category,
             "superCategory": super_category,
             "keywordsRetainingParentCategory": keywords_retaining_parent_category,
             "keywords": keywords,
             "urls": urls,
             "dbCategorizedUrls": db_categorized_urls,
             "ipRanges": ip_ranges,
             "ipRangesRetainingParentCategory": ip_ranges_retaining_parent_category,
             "type": type_list,
+            "description": description,
         }
         response = self.hp_http.post_call(
             url,
             payload=payload,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
@@ -503,15 +584,15 @@
             headers=self.headers,
         )
 
         return response.json()
 
     def delete_url_categories(
         self,
-        category_id: int,
+        category_id: str,
     ) -> requests.Response:
         """
         Deletes the custom URL category for the specified ID. You cannot delete a custom category while it is being
         used by a URL policy or NSS feed. Also, predefined categories cannot be deleted.
 
         :param category_id: (inst) Category ID
 
@@ -594,14 +675,15 @@
         self,
         url_list: list,
     ) -> list:
         """
         Method to look up the categorization of the given list of URLs, ["abc.com","zyz.com"]
 
         :param url_list: (list) List of urls
+
         :return: (list)
         """
         result = []
         url = "/urlLookup"
         # Verify urls format
         list(set(url_list))
         # Rate limit 1/sec  and 400 hr and 100 URLs per call
@@ -658,14 +740,15 @@
         location_groups=None,
         enforce_time_validity: bool = False,
         validity_end_time=None,
         validity_start_time=None,
         validity_time_zone_id=None,
         cbi_profile_id: int = 0,
         block_override: bool = False,
+        **kwargs,
     ) -> json:
         """
          Adds a URL Filtering Policy rule. If you are using the Rank feature, refer to About Admin Rank to
          determine which value to provide for rank when adding a policy rule. If you are not using Admin Rank,
          the rank value must be 7.
 
         :param name: (str)  Name of the rule
@@ -715,14 +798,15 @@
             "order": order,
             "protocols": protocols,
             "urlCategories": url_categories,
             "state": state,
             "rank": rank,
             "action": action,
         }
+        payload.update(kwargs)
         if locations:
             payload.update(locations=locations)
         if location_groups:
             payload.update(locationGroups=location_groups)
         if groups:
             payload.update(groups=groups)
         if departments:
@@ -742,14 +826,31 @@
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
 
         return response.json()
 
+    def update_url_filtering_rules(
+        self,
+        rule_id: int,
+        **kwargs,
+    ) -> json:
+        url = f"/urlFilteringRules/{rule_id}"
+        payload = kwargs
+        response = self.hp_http.put_call(
+            url,
+            payload=payload,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
+        )
+
+        return response.json()
+
     # User Management
 
     def list_departments(
         self,
         department_id: int = None,
     ) -> json or list:
         """
@@ -1500,15 +1601,15 @@
         Removes a URL from the black list.
 
         :param urls: (list) List of urls
 
         :return: (json)
         """
         url = "/security/advanced/blacklistUrls"
-        parameters = {"action" "REMOVE_FROM_LIST"}
+        parameters = {"action": "REMOVE_FROM_LIST"}
         payload = {"blacklistUrls": urls}
         response = self.hp_http.post_call(
             url,
             payload=payload,
             params=parameters,
             cookies=self.cookies,
             error_handling=True,
@@ -1894,14 +1995,31 @@
             headers=self.headers,
         )
 
         return response.json()
 
     # Firewall Policies
 
+    def list_network_services_lite(
+        self,
+    ) -> json:
+        """
+        Gets a summary list of all network service groups.
+
+        :return: (json)
+        """
+        response = self.hp_http.get_call(
+            "/networkServices/lite",
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
+        )
+
+        return response.json()
+
     def list_network_services(
         self,
         service_id: int = None,
     ) -> json:
         """
         Gets a list of all network service groups. The search parameters find matching values within the "name" or
         "description" attributes.
@@ -2029,15 +2147,14 @@
         dest_addresses: list = None,
         dest_ip_groups: list = None,
         src_ip_groups: list = None,
         dest_ip_categories: list = None,
         labels=None,
         nw_services: list = None,
         rank: int = 0,
-        **kwargs,
     ) -> requests.Response:
         """
         :param name: (str) Name of the Firewall Filtering policy rule ["String"]
         :param order: (int), Rule order number of the Firewall Filtering policy rule
         :param state: (str) Possible values : DISABLED or  ENABLED
         :param action: (str) Possible values: ALLOW, BLOCK_DROP, BLOCK_RESET, BLOCK_ICMP, EVAL_NWAPP
         :param description: (str) Additional information about the rule
@@ -2087,15 +2204,15 @@
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
         )
 
         return response
 
-    def delete_firewall_f_iltering_rules(
+    def delete_firewall_filtering_rules(
         self,
         rule_id: int,
     ) -> requests.Response:
         """
         Deletes a Firewall Filtering policy rule for the specified ID.
 
         :param rule_id: (int) The unique identifier for the policy rule
@@ -2400,33 +2517,47 @@
             headers=self.headers,
         )
 
         return response.json()
 
     def add_rule_label(
         self,
-        payload: dict,
+        name: str,
+        description: str = "",
+        payload: dict = None,
     ) -> json:
         """
         Adds new rule labels with the given name
         :param name: (str) name  # FIXME: Not in passed attributes.
         :param description: (str) description  # FIXME: Not in passed attributes.
         :param payload: (dict)
         """
         url = "/ruleLabels"
+        if not payload:
+            payload = {"name": name, "description": description}
         response = self.hp_http.post_call(
             url,
             cookies=self.cookies,
             error_handling=True,
             headers=self.headers,
             payload=payload,
         )
 
         return response.json()
 
+    def delete_rule_label(self, rule_id: str):
+        url = f"/ruleLabels/{rule_id}"
+        response = self.hp_http.delete_call(
+            url,
+            cookies=self.cookies,
+            error_handling=True,
+            headers=self.headers,
+        )
+        return response
+
     def update_call(
         self,
         url: str,
         payload: json,
     ) -> json:
         """
         Generic PUT call. This call will overwrite all the configuration with the new payload
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zpa_talker/zpa_talker.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/zpa/talker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 import requests
-from zscaler_api_talkers.zscaler_helpers import HttpCalls, setup_logger
+
+from zscaler_api_talkers.helpers import HttpCalls, setup_logger
 
 logger = setup_logger(name=__name__)
 
 
 class ZpaTalker(object):
     """
     ZPA API talker
@@ -78,15 +79,15 @@
 
         return result
 
     def authenticate(
         self,
         client_id: str,
         client_secret: str,
-    ) -> json:
+    ) -> None:
         """
         Method to obtain the Bearer Token. Refer to https://help.zscaler.com/zpa/adding-api-keys
         :param client_id: (str) client id
         :param client_secret. (str) client secret
 
         return (json))
         """
@@ -103,15 +104,15 @@
             payload=payload,
             urlencoded=True,
         )
         self.header = {
             "Authorization": f"{response.json()['token_type']} {response.json()['access_token']}"
         }
 
-        return response.json()
+        return
 
     # app-server-controller
 
     def list_servers(
         self,
         query: str = False,
         server_id: int = None,
@@ -359,14 +360,35 @@
             headers=self.header,
             error_handling=True,
             payload=payload,
         )
 
         return response.json()
 
+    def delete_segment_group(self, segmentGroupId: int) -> json:
+        """
+        Deletes specified Segment Group.
+        :param segmentGroupId: The unique identifier of the Segment Group.
+        return: response
+        """
+        url: str = f'/mgmtconfig/v1/admin/customers/{self.customerId}/segmentGroup/{segmentGroupId}'
+        response = self.hp_http.delete_call(url=url, error_handling=True)
+        return response
+
+    def update_segment_group(self, segmentGroupId: int, payload: object) -> json:
+        """
+        Update Segment Group
+        :param segmentGroupId: type int. The unique identifier of the Segment Group.
+        :param payload: type dict. Segment Group details to be updated.
+        :return: Json
+        """
+        url: str = f'/mgmtconfig/v1/admin/customers/{self.customerId}/segmentGroup/{segmentGroupId}'
+        response = self.hp_http.put_call(url, headers=self.header, error_handling=True, payload=payload)
+        return response
+
     # connector-controller
     def list_connector(
         self,
         connector_id: int = None,
     ) -> json or list:
         """
         Get all the configured Segment Groups. If segmentGroupId obtains the segment group details
@@ -431,14 +453,82 @@
             ).json()
         else:
             url = f"/mgmtconfig/v1/admin/customers/{self.customer_id}/appConnectorGroup"
             response = self._obtain_all_results(url)
 
         return response
 
+    def add_connector_group(self, name: str, description: str, latitude: str, longitude: str, location: str, upgradeDay: str = 'SUNDAY',
+                            enabled: bool = True,
+                            dnsQueryType: str = 'IPV4_IPV6', upgradeTimeInSecs: int = 66600,
+                            overrideVersionProfile: bool = False, versionProfileId: int = None, tcpQuickAckApp: bool = False,
+                            tcpQuickAckAssistant: bool = False, tcpQuickAckReadAssistant: bool = False, cityCountry: str = "",
+                            countryCode: str = "", connectors: list = [], serverGroups: list = [], lssAppConnectorGroup: bool = False) -> json:
+        """
+        :param name: type string. Name of App Connector Group
+        :param description: type string. Description
+        :param latitude: type string. Latitude of App Connector Group
+        :param longitude: type string. Longitude of App Connector Group
+        :param location: type string. Location of the App Connector Group
+        :param upgradeDay: type string. App Connectors in this group attempt to update to a newer version of the software during this specified day
+        :param upgradeTimeInSecs: type int. App Connectors in this group attempt to update to a newer version of the software during this specified time
+        :param overrideVersionProfile: type boolean. Whether the default version profile of the App Connector Group is applied or overridden
+        :param versionProfileId: type int. ID of the version profile
+        :param tcpQuickAckApp: type boolean. Whether TCP Quick Acknowledgement is enabled or disabled for the application. The tcpQuickAckApp, tcpQuickAckAssistant, and tcpQuickAckReadAssistant fields must all share the same value.
+        :param tcpQuickAckAssistant: type boolean. Whether TCP Quick Acknowledgement is enabled or disabled for the application
+        :param tcpQuickAckReadAssistant: type boolean. Whether TCP Quick Acknowledgement is enabled or disabled for the application
+        :param connectors: type dict. App Connector Id's part of the App Connector Group.
+        :param serverGroups: type dict. Server Groups part of App Connector Group
+        :param lssAppConnectorGroup: type boolean. Is App Connector Group reserved for LSS
+        """
+        url: str = f'/mgmtconfig/v1/admin/customers/{self.customerId}/appConnectorGroup'
+        payload: dict[str | Any, object | Any] = {
+            "name": name,
+            "description": description,
+            "latitude": latitude,
+            "longitude": longitude,
+            "location": location,
+            "upgradeDay": upgradeDay,
+            "enabled": enabled,
+            "dnsQueryType": dnsQueryType,
+            "upgradeTimeInSecs": upgradeTimeInSecs,
+            "overrideVersionProfile": overrideVersionProfile,
+            "versionProfileId": versionProfileId,
+            "tcpQuickAckApp": tcpQuickAckApp,
+            "tcpQuickAckAssistant": tcpQuickAckAssistant,
+            "tcpQuickAckReadAssistant": tcpQuickAckReadAssistant,
+            "cityCountry": cityCountry,
+            "countryCode": countryCode,
+            "connectors": connectors,
+            "serverGroups": serverGroups,
+            "lssAppConnectorGroup": lssAppConnectorGroup
+        }
+        response = self.hp_http.post_call(url, headers=self.header, error_handling=True, payload=payload)
+        return response.json()
+
+    def update_connector_group(self, appConnectorGroupId: int, payload: dict) -> json:
+        """
+        Update configured App Connector Groups for a ZPA tenant.
+        :param appConnectorGroupId: type int. The unique identifier of the Connector Group
+        :param payload: type dict. Details of App Connector group to be updated
+        return response
+        """
+        url: str = f'/mgmtconfig/v1/admin/customers/{self.customerId}/appConnectorGroup/{appConnectorGroupId}'
+        response = self.hp_http.put_call(url, headers=self.header, error_handling=True, payload=payload)
+        return response
+
+    def delete_connector_group(self, appConnectorGroupId: int) -> json:
+        """
+            Delete specified App Connector Group
+            :param appConnectorGroupId: type int. The unique identifier of the Connector Group
+            return response
+        """
+        url: str = f'/mgmtconfig/v1/admin/customers/{self.customerId}/appConnectorGroup/{appConnectorGroupId}'
+        response = self.hp_http.delete_call(url, error_handling=True)
+        return response
     # ba-certificate-controller-v-2
 
     def list_browser_access_certificates(
         self,
     ) -> list:  # FIXME: duplicate but URL is slightly different.
         """
         Get all Browser issued certificates
@@ -802,15 +892,15 @@
         return response
 
     def list_privileged_consoles(
         self,
         query: str = False,
     ) -> list:
         """
-        Method to Get all the privleged_remote_consoles for a ZPA tenant
+        Method to Get all the privileged_remote_consoles for a ZPA tenant
 
         :param query: (str) HTTP query
 
         :return: (list)
         """
         if not query:
             query = "?pagesize=500"
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/http_calls.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/http_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+
 from .logger import setup_logger
 
 logger = setup_logger(name=__name__)
 
 
 def _zia_http_codes(response: requests.Response):
     """
```

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/logger.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.1/zscaler_api_talkers/zscaler_helpers/utilities.py` & `zscaler_api_talkers-5.0.0/zscaler_api_talkers/helpers/utilities.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.1.1/PKG-INFO` & `zscaler_api_talkers-5.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: zscaler-api-talkers
-Version: 4.1.1
-Summary: Unofficial Zscaler API python SDK for ZIA, ZPA, ZDX, and ZCC
+Version: 5.0.0
+Summary: Unofficial Zscaler API python SDK for ZIA, ZPA, ZDX, and Zscaler Client Connector
 Author: Sergio Pereira
 Author-email: sergitopereira@hotmail.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,64 +18,66 @@
 # Unofficial Zscaler API talkers
 
 ## API Talkers
 
 ### ZIA API Talker
 Python classes to leverage [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
-The ZIA API talker is divided into two Class objects: ZiaTalker and ZiaPortalTalker.  ZiaTalker interacts with ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
+The ZIA API talker is divided into two Class objects: **ZiaTalker** and **ZiaPortalTalker**.  ZiaTalker interacts with 
+ZIA via the published APIs; whereas ZiaPortalTalker interacts with ZIA via the URLs presented in the Portal (aka, the ZIA configuration website).
 
 ### ZPA API Talker
 Python classes to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
 
-The ZPA API talker is divided into two Class objects: ZpaTalker and ZpaPortalTalker.  ZpaTalker interacts with ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
+The ZPA API talker is divided into two Class objects: **ZpaTalker** and **ZpaPortalTalker**.  ZpaTalker interacts with 
+ZPA via the published APIs; whereas ZpaPortalTalker interacts with ZPA via the URLs presented in the Portal (aka, the ZPA configuration website).
 
-### ZCC API Talker
+### Client Connector API Talker
 A Python class to leverage Zscaler Client Connector API. (Currently in Beta status.)
 
-The ZCC API talker is accessed via the Class object named: ZccTalker
+The Client Connector API talker is accessed via the Class object named: **ClientConnectorTalker**
 
 ### ZDX API Talker
 A Python class to leverage Zscaler Digital Experience API. (Currently in development.)
 
-This class is interacts with ZDX via the URLs presented in the Portal (aka, the ZDX configuration website).  It is named: ZdxPortalTalker
+This class is interacts with ZDX via the URLs presented in the Portal (aka, the ZDX configuration website).  It is 
+named: **ZdxPortalTalker**
 
 ## Installation
 
-### Option 1: Run within a Docker Container
+### Option 1: Run in a Python Virtual Environment
+1. Create a virtual Environment: `python3 -m venv .zs_api_talkers`
+1. Activate virtual environment:
+   - Linux: `source .zs_api_talkers/bin/activate`
+   - Windows: `.\.zs_api_talkers\Scripts\activate`
+1. Install Zscaler API talkers: `pip install zscaler-api-talkers`
+
+### Option 2: Run within a Docker Container
 We provide two methods to build a Docker container.  Either using the code hosted on GitHub or the code published to PyPi.
 
-#### GitHub Method
+#### PyPi Method
 1. Download Dockerfile
-   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile`
-   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile` 
+   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile`
+   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile` 
 1. Build Image and Run Container
-   1. `docker build -f git_version.Dockerfile -t zscaler_api_talkers .`
+   1. `docker build -t zscaler_api_talkers .`
    1. `docker run -it zscaler_api_talkers bash`
 1. Usage (program is in /zscaler_api_talkers/)
    - `cd zscaler_api_talkers`
 
-#### PyPi Method
+#### GitHub Method
 1. Download Dockerfile
-   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile`
-   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/Dockerfile` 
+   - Linux: `curl -O https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile`
+   - Windows: `wget -O Dockerfile https://raw.githubusercontent.com/sergitopereira/zscaler_api_talkers/sergiodevelop/git_version.Dockerfile` 
 1. Build Image and Run Container
-   1. `docker build -t zscaler_api_talkers .`
+   1. `docker build -f git_version.Dockerfile -t zscaler_api_talkers .`
    1. `docker run -it zscaler_api_talkers bash`
 1. Usage (program is in /zscaler_api_talkers/)
    - `cd zscaler_api_talkers`
 
-### Option 2: Run in a Python Virtual Environment
-1. Create a virtual Environment: `python3 -m venv .zs_api_talkers`
-1. Activate virtual environment:
-   - Linux: `source .zs_api_talkers/bin/activate`
-   - Windows: `.\.zs_api_talkers\Scripts\activate`
-1. Install Zscaler API talkers: `pip install zscaler-api-talkers`
-
-
 ## Zscaler Secure Internet and SaaS Access SDK
 
 ### Usage ZiaTalker
 ``` python
 from zscaler_api_talkers import ZiaTalker
 zia=ZiaTalker('<Zscaler Cloud Name>')
 zia.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
@@ -105,18 +107,18 @@
 a.authenticate(client_id='clientID',client_secret='clientSecret')
 # To view all methods available
 print(dir(a))
 ```
 
 ## Zscaler Client Connector SDK
 
-### Usage ZccTalker
+### Usage ClientConnectorTalker
 ``` python
-from zscaler_api_talkers import ZccTalker
-a=ZccTalker('<Zscaler Cloud Name>')    
+from zscaler_api_talkers import ClientConnectorTalker
+a=ClientConnectorTalker('<Zscaler Cloud Name>')    
 a.authenticate(clientid='clientID',secretkey='clientSecret')
 a.list_devices('companyID')
 a.list_OTP('companyID','user device id')
 # To view all methods available
 print(dir(a))
 ```
```

