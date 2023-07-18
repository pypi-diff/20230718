# Comparing `tmp/neuralpit-2.0.5.tar.gz` & `tmp/neuralpit-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-2.0.5.tar", last modified: Wed Jul 12 10:23:16 2023, max compression
+gzip compressed data, was "neuralpit-2.0.7.tar", last modified: Tue Jul 18 03:21:29 2023, max compression
```

## Comparing `neuralpit-2.0.5.tar` & `neuralpit-2.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:22:45.000000 neuralpit-2.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-12 10:23:16.070674 neuralpit-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-12 10:22:45.000000 neuralpit-2.0.5/README.md
--rw-r--r--   0 root         (0) root         (0)      963 2023-07-12 10:22:45.000000 neuralpit-2.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:23:16.070674 neuralpit-2.0.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.066674 neuralpit-2.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/conversation.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-07-12 10:22:45.000000 neuralpit-2.0.5/src/neuralpit/services/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-12 10:23:16.000000 neuralpit-2.0.5/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:23:16.070674 neuralpit-2.0.5/test/
--rw-r--r--   0 root         (0) root         (0)      411 2023-07-12 10:22:45.000000 neuralpit-2.0.5/test/testCreateConversation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.588756 neuralpit-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 03:20:59.000000 neuralpit-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-18 03:21:29.588756 neuralpit-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-18 03:20:59.000000 neuralpit-2.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-18 03:20:59.000000 neuralpit-2.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 03:21:29.588756 neuralpit-2.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.584756 neuralpit-2.0.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.584756 neuralpit-2.0.7/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-18 03:20:59.000000 neuralpit-2.0.7/src/neuralpit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.588756 neuralpit-2.0.7/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 03:20:59.000000 neuralpit-2.0.7/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-07-18 03:20:59.000000 neuralpit-2.0.7/src/neuralpit/services/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      571 2023-07-18 03:20:59.000000 neuralpit-2.0.7/src/neuralpit/services/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.584756 neuralpit-2.0.7/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-18 03:21:29.000000 neuralpit-2.0.7/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-18 03:21:29.000000 neuralpit-2.0.7/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 03:21:29.000000 neuralpit-2.0.7/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-18 03:21:29.000000 neuralpit-2.0.7/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-18 03:21:29.000000 neuralpit-2.0.7/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 03:21:29.588756 neuralpit-2.0.7/test/
+-rw-r--r--   0 root         (0) root         (0)      411 2023-07-18 03:20:59.000000 neuralpit-2.0.7/test/testCreateConversation.py
```

### Comparing `neuralpit-2.0.5/PKG-INFO` & `neuralpit-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.5
+Version: 2.0.7
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-2.0.5/pyproject.toml` & `neuralpit-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "2.0.5"
+version = "2.0.7"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-2.0.5/src/neuralpit/__init__.py` & `neuralpit-2.0.7/src/neuralpit/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.5/src/neuralpit/services/conversation.py` & `neuralpit-2.0.7/src/neuralpit/services/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,24 @@
     def deleteConversation(self, conversation_id):
         delete_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         delete_call = requests.delete(delete_url, headers = headers)
         return True
     
     def addConversationDocumentFromNeuralPitStorage(self, conversation_id, bucket, keys:List[str]):
-        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/neuralpit_document')
+        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/neuralpit_platform_file')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
         post_call = requests.post(post_url, headers = headers, json = [{'bucket': bucket, 'key': key} for key in keys])
         resp =  json.loads(post_call.content)
         return resp
     
     def addConversationDocumentFromLocalFile(self, conversation_id, file:any):
-        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/local_document')
+        post_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/local_file')
         headers = {'x-api-key':self.api_key}
-        upload_files = {'file':file}
+        upload_files = {'file':(file.name,file)}
         post_call = requests.post(post_url, headers = headers, files = upload_files)
         resp =  json.loads(post_call.content)
         return resp
     
     def deleteConversationDocument(self, conversation_id, document_id):
         delete_url = urljoin(self.api_endpoint,f'/conversation/{conversation_id}/document/{document_id}')
         headers = {'x-api-key':self.api_key, 'Content-Type':'application/json'}
```

### Comparing `neuralpit-2.0.5/src/neuralpit/services/conversion.py` & `neuralpit-2.0.7/src/neuralpit/services/conversion.py`

 * *Files identical despite different names*

### Comparing `neuralpit-2.0.5/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-2.0.7/src/neuralpit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 2.0.5
+Version: 2.0.7
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

