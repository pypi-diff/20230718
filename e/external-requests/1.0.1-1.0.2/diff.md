# Comparing `tmp/external_requests-1.0.1.tar.gz` & `tmp/external_requests-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "external_requests-1.0.1.tar", last modified: Tue Apr 11 14:27:12 2023, max compression
+gzip compressed data, was "external_requests-1.0.2.tar", last modified: Tue Jul 18 16:42:00 2023, max compression
```

## Comparing `external_requests-1.0.1.tar` & `external_requests-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.955052 external_requests-1.0.1/
--rw-rw-rw-   0        0        0     3549 2023-04-11 14:27:12.955052 external_requests-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2023-04-11 14:24:01.000000 external_requests-1.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-11 14:27:12.957054 external_requests-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-04-11 14:27:05.000000 external_requests-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.873053 external_requests-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.924053 external_requests-1.0.1/src/external_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:28:27.000000 external_requests-1.0.1/src/external_requests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.939052 external_requests-1.0.1/src/external_requests/base_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 10:37:43.000000 external_requests-1.0.1/src/external_requests/base_requests/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-04-11 11:01:40.000000 external_requests-1.0.1/src/external_requests/base_requests/external_request.py
--rw-rw-rw-   0        0        0      623 2023-04-11 11:01:40.000000 external_requests-1.0.1/src/external_requests/base_requests/external_request_with_body.py
--rw-rw-rw-   0        0        0       54 2023-04-11 10:51:07.000000 external_requests-1.0.1/src/external_requests/exceptions.py
--rw-rw-rw-   0        0        0      158 2023-04-11 10:48:26.000000 external_requests-1.0.1/src/external_requests/external_response.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.954052 external_requests-1.0.1/src/external_requests/method_requests/
--rw-rw-rw-   0        0        0        0 2023-04-11 11:02:21.000000 external_requests-1.0.1/src/external_requests/method_requests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/delete_request.py
--rw-rw-rw-   0        0        0      424 2023-04-11 11:55:31.000000 external_requests-1.0.1/src/external_requests/method_requests/get_request.py
--rw-rw-rw-   0        0        0      310 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/head_request.py
--rw-rw-rw-   0        0        0      316 2023-04-11 11:09:45.000000 external_requests-1.0.1/src/external_requests/method_requests/options_request.py
--rw-rw-rw-   0        0        0      454 2023-04-11 11:08:43.000000 external_requests-1.0.1/src/external_requests/method_requests/patch_request.py
--rw-rw-rw-   0        0        0      457 2023-04-11 11:07:14.000000 external_requests-1.0.1/src/external_requests/method_requests/post_request.py
--rw-rw-rw-   0        0        0      450 2023-04-11 11:10:11.000000 external_requests-1.0.1/src/external_requests/method_requests/put_request.py
--rw-rw-rw-   0        0        0      197 2023-04-11 10:41:11.000000 external_requests-1.0.1/src/external_requests/request_methods.py
--rw-rw-rw-   0        0        0      354 2023-04-11 11:33:25.000000 external_requests-1.0.1/src/external_requests/serialization_schema.py
-drwxrwxrwx   0        0        0        0 2023-04-11 14:27:12.936053 external_requests-1.0.1/src/external_requests.egg-info/
--rw-rw-rw-   0        0        0     3549 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-11 14:27:12.000000 external_requests-1.0.1/src/external_requests.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 16:42:00.083851 external_requests-1.0.2/
+-rw-rw-rw-   0        0        0     3549 2023-07-18 16:42:00.083851 external_requests-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2023-04-11 14:24:01.000000 external_requests-1.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-18 16:42:00.103846 external_requests-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-18 16:38:21.000000 external_requests-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:41:59.964845 external_requests-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 16:41:59.998845 external_requests-1.0.2/src/external_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:28:27.000000 external_requests-1.0.2/src/external_requests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:42:00.023845 external_requests-1.0.2/src/external_requests/base_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 10:37:43.000000 external_requests-1.0.2/src/external_requests/base_requests/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-07-18 16:38:04.000000 external_requests-1.0.2/src/external_requests/base_requests/external_request.py
+-rw-rw-rw-   0        0        0      645 2023-07-18 16:38:04.000000 external_requests-1.0.2/src/external_requests/base_requests/external_request_with_body.py
+-rw-rw-rw-   0        0        0       54 2023-04-11 10:51:07.000000 external_requests-1.0.2/src/external_requests/exceptions.py
+-rw-rw-rw-   0        0        0      158 2023-04-11 10:48:26.000000 external_requests-1.0.2/src/external_requests/external_response.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:42:00.065845 external_requests-1.0.2/src/external_requests/method_requests/
+-rw-rw-rw-   0        0        0        0 2023-04-11 11:02:21.000000 external_requests-1.0.2/src/external_requests/method_requests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-11 11:08:43.000000 external_requests-1.0.2/src/external_requests/method_requests/delete_request.py
+-rw-rw-rw-   0        0        0      424 2023-04-11 11:55:31.000000 external_requests-1.0.2/src/external_requests/method_requests/get_request.py
+-rw-rw-rw-   0        0        0      310 2023-04-11 11:08:43.000000 external_requests-1.0.2/src/external_requests/method_requests/head_request.py
+-rw-rw-rw-   0        0        0      316 2023-04-11 11:09:45.000000 external_requests-1.0.2/src/external_requests/method_requests/options_request.py
+-rw-rw-rw-   0        0        0      454 2023-04-11 11:08:43.000000 external_requests-1.0.2/src/external_requests/method_requests/patch_request.py
+-rw-rw-rw-   0        0        0      457 2023-04-11 11:07:14.000000 external_requests-1.0.2/src/external_requests/method_requests/post_request.py
+-rw-rw-rw-   0        0        0      450 2023-04-11 11:10:11.000000 external_requests-1.0.2/src/external_requests/method_requests/put_request.py
+-rw-rw-rw-   0        0        0      197 2023-04-11 10:41:11.000000 external_requests-1.0.2/src/external_requests/request_methods.py
+-rw-rw-rw-   0        0        0      354 2023-04-11 11:33:25.000000 external_requests-1.0.2/src/external_requests/serialization_schema.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:42:00.019844 external_requests-1.0.2/src/external_requests.egg-info/
+-rw-rw-rw-   0        0        0     3549 2023-07-18 16:41:59.000000 external_requests-1.0.2/src/external_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-07-18 16:41:59.000000 external_requests-1.0.2/src/external_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:41:59.000000 external_requests-1.0.2/src/external_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-18 16:41:59.000000 external_requests-1.0.2/src/external_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-18 16:41:59.000000 external_requests-1.0.2/src/external_requests.egg-info/top_level.txt
```

### Comparing `external_requests-1.0.1/PKG-INFO` & `external_requests-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: external_requests
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/VenfiOranai/external-requests
 Author: Venfi Oranai
 Author-email: venfioranai@gmail.com
 Description-Content-Type: text/markdown
 
 # External Requests
 A class based alternative to making HTTP requests in Python.
```

### Comparing `external_requests-1.0.1/README.md` & `external_requests-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `external_requests-1.0.1/setup.py` & `external_requests-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open(file_name) as file:
         content = file.read()
     return content
 
 
 setup(
     name='external_requests',
-    version='1.0.1',
+    version='1.0.2',
     author='Venfi Oranai',
     author_email='venfioranai@gmail.com',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://gitlab.com/VenfiOranai/external-requests',
```

### Comparing `external_requests-1.0.1/src/external_requests/base_requests/external_request.py` & `external_requests-1.0.2/src/external_requests/base_requests/external_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     def _expected_status_codes(self) -> List[int]:
         pass
 
     @property
     def _headers(self) -> dict:
         return {'Content-Type': 'application/json'}
 
-    def _send_request(self) -> Response:
-        return request(self._request_method.value, self._base_url + self._route, headers=self._headers)
+    def _send_request(self, **kwargs) -> Response:
+        return request(self._request_method.value, self._base_url + self._route, headers=self._headers, **kwargs)
 
-    def request(self) -> ExternalResponse:
+    def request(self, **kwargs) -> ExternalResponse:
         try:
-            response: Response = self._send_request()
+            response: Response = self._send_request(**kwargs)
         except Exception as e:
             raise ExternalRequestException(f'Failed to send a request to {self._base_url + self._route}. '
                                            f'Error - {str(e)}')
         else:
             if response.status_code not in self._expected_status_codes:
                 raise ExternalRequestException(f'Received unexpected status code {response.status_code}. '
                                                f'Reason - {response.text}')
```

### Comparing `external_requests-1.0.1/src/external_requests/base_requests/external_request_with_body.py` & `external_requests-1.0.2/src/external_requests/base_requests/external_request_with_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 
 class ExternalRequestWithBody(ExternalRequest, ABC):
     @property
     @abstractmethod
     def _body_schema(self) -> SerializationSchema:
         pass
 
-    def _send_request(self) -> Response:
+    def _send_request(self, **kwargs) -> Response:
         return request(self._request_method.value, self._base_url + self._route, headers=self._headers,
-                       data=json.dumps(self._body_schema.serialize()))
+                       data=json.dumps(self._body_schema.serialize()), **kwargs)
```

### Comparing `external_requests-1.0.1/src/external_requests.egg-info/PKG-INFO` & `external_requests-1.0.2/src/external_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: external-requests
-Version: 1.0.1
+Version: 1.0.2
 Home-page: https://gitlab.com/VenfiOranai/external-requests
 Author: Venfi Oranai
 Author-email: venfioranai@gmail.com
 Description-Content-Type: text/markdown
 
 # External Requests
 A class based alternative to making HTTP requests in Python.
```

### Comparing `external_requests-1.0.1/src/external_requests.egg-info/SOURCES.txt` & `external_requests-1.0.2/src/external_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

