# Comparing `tmp/petkitaio-0.1.6.1.tar.gz` & `tmp/petkitaio-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petkitaio-0.1.6.1.tar", last modified: Sun Jul  9 20:04:05 2023, max compression
+gzip compressed data, was "petkitaio-0.1.7.tar", last modified: Tue Jul 18 18:46:41 2023, max compression
```

## Comparing `petkitaio-0.1.6.1.tar` & `petkitaio-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.159901 petkitaio-0.1.6.1/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6155 2023-07-09 20:04:05.160115 petkitaio-0.1.6.1/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     4546 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.157588 petkitaio-0.1.6.1/petkitaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1904 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    10807 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      835 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    43340 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/petkit_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/petkitaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-09 20:04:05.159570 petkitaio-0.1.6.1/petkitaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)     6155 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-09 20:04:05.000000 petkitaio-0.1.6.1/petkitaio.egg-info/top_level.txt
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-09 20:04:05.160680 petkitaio-0.1.6.1/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1052 2023-07-09 19:59:24.000000 petkitaio-0.1.6.1/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.846050 petkitaio-0.1.7/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1067 2023-07-18 18:42:51.000000 petkitaio-0.1.7/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6428 2023-07-18 18:46:41.846290 petkitaio-0.1.7/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     4813 2023-07-18 18:42:51.000000 petkitaio-0.1.7/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.843588 petkitaio-0.1.7/petkitaio/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1942 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/__init__.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    10841 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/constants.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1059 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/exceptions.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1392 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/model.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)    43642 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/petkit_client.py
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      680 2023-07-18 18:42:51.000000 petkitaio-0.1.7/petkitaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-07-18 18:46:41.845649 petkitaio-0.1.7/petkitaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     6428 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      337 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       28 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       10 2023-07-18 18:46:41.000000 petkitaio-0.1.7/petkitaio.egg-info/top_level.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-07-18 18:46:41.846837 petkitaio-0.1.7/setup.cfg
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)     1050 2023-07-18 18:42:51.000000 petkitaio-0.1.7/setup.py
```

### Comparing `petkitaio-0.1.6.1/LICENSE` & `petkitaio-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6.1/PKG-INFO` & `petkitaio-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`. In order to use this library with PetKit China accounts, be sure to set the china_account parameter to `True`.
         
         ## **Currently Supported Devices**:
         
         `Feeders`
         - [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
         - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
@@ -53,14 +53,15 @@
         from aiohttp import ClientSession
         
         async def main():
             async with ClientSession() as session:
         
                 # Create a client using PetKit account email and password
                 # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
+                # For PetKit China accounts, the client would be in the form of client = PetKitClient('account number as string', 'password', session, False, True)
                 client = PetKitClient('email', 'password', session)
         
         
                 ###################################################################################
                 Examples within the examples section utilize the PetKitClient instance created above
                 ###################################################################################
```

### Comparing `petkitaio-0.1.6.1/README.md` & `petkitaio-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PetKitAIO
 
 Asynchronous Python library for PetKit's API.
 
-This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
+This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`. In order to use this library with PetKit China accounts, be sure to set the china_account parameter to `True`.
 
 ## **Currently Supported Devices**:
 
 `Feeders`
 - [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
 - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
 - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
@@ -43,14 +43,15 @@
 from aiohttp import ClientSession
 
 async def main():
     async with ClientSession() as session:
 
         # Create a client using PetKit account email and password
         # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
+        # For PetKit China accounts, the client would be in the form of client = PetKitClient('account number as string', 'password', session, False, True)
         client = PetKitClient('email', 'password', session)
 
 
         ###################################################################################
         Examples within the examples section utilize the PetKitClient instance created above
         ###################################################################################
```

### Comparing `petkitaio-0.1.6.1/petkitaio/__init__.py` & `petkitaio-0.1.7/petkitaio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_MODE,
     W5_SETTINGS_COMMANDS,
 )
 from .petkit_client import (PetKitClient, LOGGER,)
-from .exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
+from .exceptions import (AccountTypeError, AuthError, BluetoothError, PetKitError, ServerError)
 from .model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain, )
 from .str_enum import StrEnum
 
-__all__ = ['AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint', 'FeederCommand',
+__all__ = ['AccountTypeError', 'AuthError', 'AUTH_ERROR_CODES', 'BLE_HEADER', 'BluetoothError', 'BLUETOOTH_ERRORS', 'CLIENT_DICT', 'Feeder', 'Endpoint', 'FeederCommand',
            'FEEDER_LIST', 'FeederSetting', 'Header', 'LB_CMD_TO_KEY', 'LB_CMD_TO_TYPE', 'LB_CMD_TO_VALUE', 'LitterBox', 'LitterBoxCommand', 'LitterBoxCommandKey',
            'LitterBoxCommandType', 'LitterBoxSetting', 'LITTER_LIST', 'LOGGER', 'Pet', 'PetKitClient', 'PetKitData', 'PetKitError', 'PetSetting', 'Purifier',
            'PurifierCommand', 'PurifierCommandKey', 'PurifierCommandType', 'PUR_CMD_TO_KEY', 'PUR_CMD_TO_TYPE', 'PUR_CMD_TO_VALUE', 'PURIFIER_LIST', 'PurifierSetting', 'Region',
            'ServerError', 'SERVER_ERROR_CODES', 'StrEnum', 'TIMEOUT', 'WATER_FOUNTAIN_LIST', 'W5Command', 'W5_COMMAND_TO_CODE', 'W5_DND_COMMANDS', 'W5Fountain', 'W5_LIGHT_BRIGHTNESS',
            'W5_LIGHT_POWER', 'W5_MODE', 'W5_SETTINGS_COMMANDS',  ]
```

### Comparing `petkitaio-0.1.6.1/petkitaio/constants.py` & `petkitaio-0.1.7/petkitaio/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .str_enum import StrEnum
 
 class Region(StrEnum):
 
     US = 'http://api.petkt.com/latest'
     ASIA = 'http://api.petktasia.com/latest'
+    CN = 'http://api.petkit.cn/6'
 
 
 class Endpoint(StrEnum):
 
     BLE_CANCEL = '/ble/cancel'
     BLE_CONNECT = '/ble/connect'
     BLE_DEVICES = '/ble/ownSupportBleDevices'
```

### Comparing `petkitaio-0.1.6.1/petkitaio/exceptions.py` & `petkitaio-0.1.7/petkitaio/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,21 @@
     """Error from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
 
 
+class AccountTypeError(Exception):
+    """User has set account region to more than one region."""
+
+    def __init__(self, *args: Any) -> None:
+        """Initialize the exception."""
+        Exception.__init__(self, *args)
+
 class AuthError(Exception):
     """Authentication issue from PetKit api."""
 
     def __init__(self, *args: Any) -> None:
         """Initialize the exception."""
         Exception.__init__(self, *args)
```

### Comparing `petkitaio-0.1.6.1/petkitaio/model.py` & `petkitaio-0.1.7/petkitaio/model.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6.1/petkitaio/petkit_client.py` & `petkitaio-0.1.7/petkitaio/petkit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,36 +44,40 @@
     W5Command,
     W5_COMMAND_TO_CODE,
     W5_DND_COMMANDS,
     W5_LIGHT_BRIGHTNESS,
     W5_LIGHT_POWER,
     W5_SETTINGS_COMMANDS,
 )
-from petkitaio.exceptions import (AuthError, BluetoothError, PetKitError, ServerError)
+from petkitaio.exceptions import (AccountTypeError, AuthError, BluetoothError, PetKitError, ServerError)
 from petkitaio.model import (Feeder, LitterBox, Pet, PetKitData, Purifier, W5Fountain)
 
 LOGGER = logging.getLogger(__name__)
 
 
 class PetKitClient:
     """PetKit client."""
 
     def __init__(
-        self, username: str, password: str, session: ClientSession | None = None, asia_account: bool = False, timeout: int = TIMEOUT
+        self, username: str, password: str, session: ClientSession | None = None, asia_account: bool = False, china_account: bool = False, timeout: int = TIMEOUT
     ) -> None:
         """Initialize PetKit Client.
 
         username: PetKit username/email
         password: PetKit account password
         session: aiohttp.ClientSession or None to create a new session
         """
 
+        # Catch if a user is trying to set both asia and china account to true
+        if asia_account and china_account:
+            raise AccountTypeError('Only one region (Asia or China) may be set to True. Not both.')
+
         self.username: str = username
         self.password: str = password
-        self.base_url: Region = Region.ASIA if asia_account else Region.US
+        self.base_url: Region = Region.ASIA if asia_account else Region.CN if china_account else Region.US
         self.server_list: list | None = None
         self._session: ClientSession = session if session else ClientSession()
         self.tz: str = get_localzone_name()
         self.timeout: int = timeout
         self.token: str | None = None
         self.token_expiration: datetime | None = None
         self.user_id: str | None = None
```

### Comparing `petkitaio-0.1.6.1/petkitaio/str_enum.py` & `petkitaio-0.1.7/petkitaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `petkitaio-0.1.6.1/petkitaio.egg-info/PKG-INFO` & `petkitaio-0.1.7/petkitaio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: petkitaio
-Version: 0.1.6.1
+Version: 0.1.7
 Summary: Asynchronous Python library for PetKit's API
 Home-page: https://github.com/RobertD502/petkitaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/petkitaio/issues
 Project-URL: Source, https://github.com/RobertD502/petkitaio/
 Description: # PetKitAIO
         
         Asynchronous Python library for PetKit's API.
         
-        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`.
+        This is PetKit's undocumented API. With that said, future changes made by PetKit may break this library. The API endpoint used is determined based on the region your account is locked to. In order to use this library with PetKit Asia accounts, be sure to set the asia_account parameter to `True`. In order to use this library with PetKit China accounts, be sure to set the china_account parameter to `True`.
         
         ## **Currently Supported Devices**:
         
         `Feeders`
         - [Fresh Element](https://petkit.us/products/petkit-element-wi-fi-enabled-smart-pet-food-container-feeder)
         - [D3 (Fresh Element Infinity)](https://www.amazon.com/PETKIT-Automatic-Stainless-Programmable-Dispenser/dp/B09JFK8BCQ)
         - [D4 (Fresh Element Solo)](https://www.amazon.com/PETKIT-Automatic-Dispenser-Compatible-Freeze-Dried/dp/B09158J9PF/)
@@ -53,14 +53,15 @@
         from aiohttp import ClientSession
         
         async def main():
             async with ClientSession() as session:
         
                 # Create a client using PetKit account email and password
                 # For PetKit Asia accounts, the client would be in the form of client = PetKitClient('email', 'password', session, True)
+                # For PetKit China accounts, the client would be in the form of client = PetKitClient('account number as string', 'password', session, False, True)
                 client = PetKitClient('email', 'password', session)
         
         
                 ###################################################################################
                 Examples within the examples section utilize the PetKitClient instance created above
                 ###################################################################################
```

### Comparing `petkitaio-0.1.6.1/setup.py` & `petkitaio-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="petkitaio",
-    version="0.1.6.1",
+    version="0.1.7",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="Asynchronous Python library for PetKit's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/petkitaio',
     keywords='petkit, eversweet 3 pro, feeder mini, d4, petkit feeder, petkit water fountain, freshelement solo, pura x, pura max, pura air',
```

