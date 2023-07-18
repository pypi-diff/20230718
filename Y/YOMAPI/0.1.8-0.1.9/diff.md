# Comparing `tmp/YOMAPI-0.1.8.tar.gz` & `tmp/YOMAPI-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/YOMAPI-0.1.8.tar", last modified: Tue Jun  6 20:37:26 2023, max compression
+gzip compressed data, was "dist/YOMAPI-0.1.9.tar", last modified: Mon Jul  3 20:18:27 2023, max compression
```

## Comparing `YOMAPI-0.1.8.tar` & `YOMAPI-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/YOMAPI/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    41142 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/YOMAPI/YOMAPI.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/YOMAPI/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-06-06 20:37:17.000000 YOMAPI-0.1.8/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-06-06 20:37:26.000000 YOMAPI-0.1.8/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 20:18:27.000000 YOMAPI-0.1.9/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-03 20:18:27.000000 YOMAPI-0.1.9/YOMAPI/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    41804 2023-07-03 20:18:17.000000 YOMAPI-0.1.9/YOMAPI/YOMAPI.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-07-03 20:18:17.000000 YOMAPI-0.1.9/YOMAPI/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-07-03 20:18:17.000000 YOMAPI-0.1.9/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-07-03 20:18:17.000000 YOMAPI-0.1.9/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-07-03 20:18:27.000000 YOMAPI-0.1.9/PKG-INFO
```

### Comparing `YOMAPI-0.1.8/YOMAPI/YOMAPI.py` & `YOMAPI-0.1.9/YOMAPI/YOMAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,15 +945,31 @@
             if from_integration is not None:
                 body['fromIntegration'] = from_integration            
             
             response = session.post(path, json.dumps(body))
             return response
         except Exception as error:
             raise ApiResponseError(path, str(error))
+        
+    def bulk_clean_discount_limits(self, job_id, token=None):
+        path = self.url_v3 +f'/api/v3/admin/catalog/discount-limits/delete'
+        self.logger.info('Sending discount-limits delete for job id {}'.format(job_id))
 
+        try:
+            body = {
+                'syncJobId': job_id
+            }
+            session = self.__build_session(token)
+
+            response = session.delete(path, json.dumps(body))
+            
+            self.logger.info((response.status_code, response.json()))
+            return (response.status_code, response.json())
+        except Exception as error:
+            raise ApiResponseError(path, str(error))
     """
     Orders Endpoint
     """
     def get_orders(self, query):
         currentPage = 0
         totalPages = float('inf')
         orders = []
```

### Comparing `YOMAPI-0.1.8/setup.py` & `YOMAPI-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'YOMAPI',
   packages = ['YOMAPI'],
-  version = '0.1.8',
+  version = '0.1.9',
   license='MIT',
   description = 'A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS',
   author = 'Camilo Jiménez',
   author_email = 'camilo@youorder.me',
   url = 'https://github.com/user/reponame',
   # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz', 
   keywords = ['YOM-INTEGRATIONS'],   # Keywords that define your package best
```

### Comparing `YOMAPI-0.1.8/PKG-INFO` & `YOMAPI-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: YOMAPI
-Version: 0.1.8
+Version: 0.1.9
 Summary: A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS
 Home-page: https://github.com/user/reponame
 Author: Camilo Jiménez
 Author-email: camilo@youorder.me
 License: MIT
 Description: UNKNOWN
 Keywords: YOM-INTEGRATIONS
```

