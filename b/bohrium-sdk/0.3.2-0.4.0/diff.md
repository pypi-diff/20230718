# Comparing `tmp/bohrium-sdk-0.3.2.tar.gz` & `tmp/bohrium-sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.3.2.tar", last modified: Tue Jul  4 09:48:54 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.4.0.tar", last modified: Tue Jul 18 08:12:16 2023, max compression
```

## Comparing `bohrium-sdk-0.3.2.tar` & `bohrium-sdk-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:48:54.251503 bohrium-sdk-0.3.2/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 09:48:54.251203 bohrium-sdk-0.3.2/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:48:54.242694 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-07-04 09:48:54.000000 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      478 2023-07-04 09:48:54.000000 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-07-04 09:48:54.000000 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       20 2023-07-04 09:48:54.000000 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/requires.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-07-04 09:48:54.000000 bohrium-sdk-0.3.2/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:48:54.248356 bohrium-sdk-0.3.2/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7031 2023-07-04 03:12:10.000000 bohrium-sdk-0.3.2/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     8428 2023-07-04 03:26:27.000000 bohrium-sdk-0.3.2/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-04 09:48:54.249093 bohrium-sdk-0.3.2/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-15 02:43:18.000000 bohrium-sdk-0.3.2/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-07-04 09:48:54.251565 bohrium-sdk-0.3.2/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      412 2023-07-04 09:48:43.000000 bohrium-sdk-0.3.2/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-18 08:12:16.215747 bohrium-sdk-0.4.0/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      232 2023-07-18 08:12:16.215495 bohrium-sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-18 08:12:16.210245 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      232 2023-07-18 08:12:16.000000 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      478 2023-07-18 08:12:16.000000 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-07-18 08:12:16.000000 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       13 2023-07-18 08:12:16.000000 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/requires.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-07-18 08:12:16.000000 bohrium-sdk-0.4.0/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-18 08:12:16.214547 bohrium-sdk-0.4.0/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     5758 2023-07-10 07:56:17.000000 bohrium-sdk-0.4.0/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4121 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     8436 2023-07-14 02:58:31.000000 bohrium-sdk-0.4.0/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-07-18 08:12:16.215148 bohrium-sdk-0.4.0/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4649 2023-07-07 11:26:30.000000 bohrium-sdk-0.4.0/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-15 02:43:18.000000 bohrium-sdk-0.4.0/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-07-18 08:12:16.215813 bohrium-sdk-0.4.0/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      432 2023-07-18 08:12:01.000000 bohrium-sdk-0.4.0/setup.py
```

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/client.py` & `bohrium-sdk-0.4.0/bohriumsdk/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,64 +10,34 @@
 
 class RequestInfoException(Exception):
     pass
 
 class Client:
     def __init__(
             self, 
-            api_version: str = 'v2',
-            email: str = "",
-            password: str = "",
-            base_url_v1: str = 'https://bohrium.dp.tech',
-            token: str = "",
-            debug: bool = False,
-            use_config_file: bool = False,
-            config_file_location_v1: str = '~/.lebesgue_config.json',
             config_file_location_v2: str ='~/.brmconfig'
         ) -> None:
-        if api_version == "v1":
-            self.debug = debug
-            self.debug = os.getenv('LBG_CLI_DEBUG_PRINT', debug)
-            self.config = {}
-            config_file_location_expand = os.path.expanduser(config_file_location_v1)
-            file_data = {}
-            self.token = ''
-            self.user_id = None
-            if use_config_file:
-                if os.path.exists(config_file_location_expand):
-                    with open(config_file_location_expand, 'r') as f:
-                        file_data = json.loads(f.read())
-                self.config['email'] = file_data.get('email', email)
-                self.config['password'] = file_data.get('password', password)
-                self.base_url = file_data.get('base_url', base_url_v1)
-            else:
-                self.config['email'] = email
-                self.config['password'] = password
-                self.base_url = base_url_v1
-            if token is not None:
-                self.token = token
-            else:
-                self._login()
-        elif api_version == "v2":
-            self.openapi_host = os.getenv("OPENAPI_HOST", "https://openapi.dp.tech")
-            self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
-            if not os.path.exists(self.config_file_location_expand):
-                weburl = self.openapi_host.replace("openapi", "bohrium")
-                print(f"Config File ~/.brmconfig not found! Please visit {weburl}/personal/setting and click AccessKey create button to generate it !")
-                self.access_key = input("Please enter AccessKey: ")
-                data = f"[Credentials]\naccessKey={self.access_key}"
-                with open(self.config_file_location_expand, 'w') as f:
-                    f.write(data)
-            config = configparser.ConfigParser()
-            config.read(self.config_file_location_expand)
-            self.base_url = self.openapi_host
-            self.access_key = config.get('Credentials', 'accessKey')
-            self.params = {"accessKey": self.access_key}
-            self.token = ""
-            self.check_ak()
+
+        self.openapi_host = os.getenv("OPENAPI_HOST", "https://openapi.dp.tech")
+        self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
+        self.ticket = os.environ.get("BHOR_TICKET", "")
+        if not os.path.exists(self.config_file_location_expand) and self.ticket == "":
+            weburl = self.openapi_host.replace("openapi", "bohrium")
+            print(f"Config File ~/.brmconfig not found! Please visit {weburl}/personal/setting and click AccessKey create button to generate it !")
+            self.access_key = input("Please enter AccessKey: ")
+            data = f"[Credentials]\naccessKey={self.access_key}"
+            with open(self.config_file_location_expand, 'w') as f:
+                f.write(data)
+        config = configparser.ConfigParser()
+        config.read(self.config_file_location_expand)
+        self.base_url = self.openapi_host
+        self.access_key = config.get('Credentials', 'accessKey')
+        self.params = {"accessKey": self.access_key}
+        self.token = ""
+        self.check_ak()
             
 
     def post(self, url, host="", json=None, data=None, headers=None, params=None, stream=False, retry=5):
         return self._req('POST', url, host=host, json=json, data=data, headers=headers, params=params, stream=stream, retry=retry)
 
     def get(self, url, host="", json=None, headers=None, params=None, stream=False, retry=5):
         return self._req('GET', url, host=host, json=json, headers=headers, params=params, stream=stream, retry=retry)
@@ -78,29 +48,30 @@
         else:
             url = urllib.parse.urljoin(self.base_url, url)
         
         # Set Headers
         if headers is None: headers = {}
        
         if self.token: headers['Authorization'] = f'Bearer {self.token}'
-     
-
+        if self.ticket: headers['Brm-Ticket'] = self.ticket
+        
         # headers['bohr-client'] = f'utility:0.0.2'
         resp_code = None
         for i in range(retry):
             resp = None
             err = ""
             if method == 'GET':
                 resp = requests.get(url=url, params=params, headers=headers, stream=stream)
             if method == 'POST':
                 resp = requests.post(url=url, json=json, data=data, params=params, headers=headers, stream=stream)
             resp_code = resp.status_code
             if resp_code == 401:
-                os.remove(self.config_file_location_expand)
-                print("Config file(~/.brmconfig) AccessKey invalid! Visit https://bohrium.dp.tech/personal/setting to generate it! ")
+                # os.remove(self.config_file_location_expand)
+                weburl = self.openapi_host.replace("openapi", "bohrium")
+                print(f"Config file(~/.brmconfig) AccessKey invalid! Visit {weburl}/personal/setting to generate it! ")
                 sys.exit()
             if not resp.ok:
                 try:
                     result = resp.json()
                     err = result.get("error")
                 except:
                     pass
```

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/database.py` & `bohrium-sdk-0.4.0/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/image.py` & `bohrium-sdk-0.4.0/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/job.py` & `bohrium-sdk-0.4.0/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/node.py` & `bohrium-sdk-0.4.0/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/project.py` & `bohrium-sdk-0.4.0/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/storage.py` & `bohrium-sdk-0.4.0/bohriumsdk/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
         if parameter:
             param["option"] = parameter.__dict__
         # print(param)
         headers = {}
         headers[self.TIEFBLUE_HEADER_KEY] = self.encode_base64(param)
         headers['Authorization'] = "Bearer " + token
-
+        
         # req = self.client.post(f"/api/upload/binary", data=body)
         url = f"/api/upload/binary"
         
         req = self.client.post(url=url, host=self.host, headers=headers, data=data)
         # req = requests.post("https://tiefblue.dp.tech/api/upload/binary", headers=headers, data=data)
         # self._raise_error(req)
         return req
```

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/test.py` & `bohrium-sdk-0.4.0/bohriumsdk/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,11 +154,11 @@
     c = Client()
     prompt = "你好"
     res = c.chat(prompt)
     print(res)
 
 
 if __name__ == "__main__":
-    # test_chat()
-    test_job_detail()
+    test_chat()
+    # test_job_detail()
     # test_base64()
     # test_db()
```

### Comparing `bohrium-sdk-0.3.2/bohriumsdk/util.py` & `bohrium-sdk-0.4.0/bohriumsdk/util.py`

 * *Files identical despite different names*

