# Comparing `tmp/ezsmdeploy-1.93.dev0.tar.gz` & `tmp/ezsmdeploy-1.95.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploy-1.93.dev0.tar", last modified: Fri Jul 14 05:39:19 2023, max compression
+gzip compressed data, was "ezsmdeploy-1.95.dev0.tar", last modified: Tue Jul 18 17:33:24 2023, max compression
```

## Comparing `ezsmdeploy-1.93.dev0.tar` & `ezsmdeploy-1.95.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 05:39:19.149633 ezsmdeploy-1.93.dev0/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18951 2023-07-14 05:39:19.149633 ezsmdeploy-1.93.dev0/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18461 2023-07-14 05:37:34.000000 ezsmdeploy-1.93.dev0/README.rst
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 05:39:19.145633 ezsmdeploy-1.93.dev0/ezsmdeploy/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48678 2023-07-14 05:37:54.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 05:39:19.149633 ezsmdeploy-1.93.dev0/ezsmdeploy/data/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/Dockerfile
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/build-docker.sh
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/conversation.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/cost.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/instancetypes.csv
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/model_handler.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/nginx.conf
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/predictor.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/serve
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/smlocust.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/train
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/data/wsgi.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-08 14:37:12.000000 ezsmdeploy-1.93.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-14 05:39:19.145633 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    18951 2023-07-14 05:39:19.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-14 05:39:19.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-14 05:39:19.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-13 20:11:33.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/not-zip-safe
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-14 05:39:19.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-14 05:39:19.000000 ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-14 05:39:19.149633 ezsmdeploy-1.93.dev0/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-14 05:37:59.000000 ezsmdeploy-1.93.dev0/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       26 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19108 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/README.rst
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/ezsmdeploy/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    48678 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/ezsmdeploy/data/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2100 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/Dockerfile
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1934 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1390 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/build-docker.sh
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1603 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/conversation.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1361 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/cost.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      884 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      576 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1797 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/model_handler.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      719 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/nginx.conf
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2090 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/predictor.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2429 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/serve
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1409 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/smlocust.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      432 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/train
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      202 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/data/wsgi.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      733 2023-07-18 17:32:09.000000 ezsmdeploy-1.95.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    19598 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      696 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/not-zip-safe
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      129 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-07-18 17:33:24.000000 ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-07-18 17:33:24.173803 ezsmdeploy-1.95.dev0/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1274 2023-07-18 17:32:54.000000 ezsmdeploy-1.95.dev0/setup.py
```

### Comparing `ezsmdeploy-1.93.dev0/PKG-INFO` & `ezsmdeploy-1.95.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploy
-Version: 1.93.dev0
+Version: 1.95.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -58,17 +58,24 @@
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
+    - TheBloke/dromedary-65b-lora-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
+    - CalderaAI/30B-Lazarus, ml.g5.16xlarge
+    - huggyllama/llama-65b, ml.g5.16xlarge
+    - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
+    - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
+    - 
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -303,15 +310,22 @@
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
 ~~~~~~~~~~~~~~~~~~~~~
 
-EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface. Genreral guidance:
+
+
+1. Jumpstart models - `foundation_model=True`
+2. Large huggingface models - `foundation_model=True, huggingface_model=True`
+3. Small huggingface models - `huggingface_model=True`
+4. Tiny models - `serverless=True`
+
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
```

### Comparing `ezsmdeploy-1.93.dev0/README.rst` & `ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ezsmdeploy
+Version: 1.95.dev0
+Summary: SageMaker custom deployments made easy
+Home-page: https://pypi.python.org/pypi/ezsmdeploy
+Author: Shreyas Subramanian
+Author-email: subshrey@amazon.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Provides-Extra: locust
+
 ====================================================
 Ezsmdeploy - SageMaker custom deployments made easy
 ====================================================
 
 .. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: Latest Version
@@ -43,17 +58,24 @@
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
+    - TheBloke/dromedary-65b-lora-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
+    - CalderaAI/30B-Lazarus, ml.g5.16xlarge
+    - huggyllama/llama-65b, ml.g5.16xlarge
+    - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
+    - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
+    - 
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -288,15 +310,22 @@
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
 ~~~~~~~~~~~~~~~~~~~~~
 
-EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface. Genreral guidance:
+
+
+1. Jumpstart models - `foundation_model=True`
+2. Large huggingface models - `foundation_model=True, huggingface_model=True`
+3. Small huggingface models - `huggingface_model=True`
+4. Tiny models - `serverless=True`
+
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
```

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/__init__.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/serve` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploy-1.95.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/PKG-INFO` & `ezsmdeploy-1.95.dev0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ezsmdeploy
-Version: 1.93.dev0
-Summary: SageMaker custom deployments made easy
-Home-page: https://pypi.python.org/pypi/ezsmdeploy
-Author: Shreyas Subramanian
-Author-email: subshrey@amazon.com
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Provides-Extra: locust
-
 ====================================================
 Ezsmdeploy - SageMaker custom deployments made easy
 ====================================================
 
 .. image:: https://img.shields.io/pypi/v/ezsmdeploy.svg
    :target: https://pypi.python.org/pypi/ezsmdeploy
    :alt: Latest Version
@@ -58,17 +43,24 @@
 2. Added support for Huggingface hub models
 3. Added OpenChatKit support for appropriate chat models
 4. Tested the following:
     - tiiuae/falcon-40b-instruct, ml.g4dn.12xlarge
     - tiiuae/falcon-7b-instruct, ml.g5.16xlarge
     - WizardLM/WizardLM-7B-V1.0", ml.g5.16xlarge
     - TheBloke/wizardLM-7B-HF, ml.g4dn.4xlarge
+    - TheBloke/dromedary-65b-lora-HF, ml.g4dn.4xlarge
     - togethercomputer/RedPajama-INCITE-Chat-3B-v1, ml.g4dn.4xlarge
     - openchat/openchat, ml.g5.24xlarge
     - facebook/galactica-6.7b, ml.g5.16xlarge
+    - CalderaAI/30B-Lazarus, ml.g5.16xlarge
+    - huggyllama/llama-65b, ml.g5.16xlarge
+    - ausboss/llama-30b-supercot, ml.g4dn.4xlarge
+    - MetaIX/GPT4-X-Alpasta-30b, ml.g4dn.4xlarge
+    - 
+    - Also tried several small/tiny models from huggingface on Serverless - (distilbert / dynamic-tinybert / deepset/tinyroberta-squad2 / facebook/detr-resnet-50) 
 
 
 V 1.x release notes
 -------------------
 1. Updated to use >v2.x of SageMaker SDK
 2. Fixed failing docker builds
 3. Tested with test notebook
@@ -303,15 +295,22 @@
 
 Note that when using the Multi model mode, the payload comes in as a dictionary and the raw bytes sent in can be accessed using payload[0]['body']; In flask based deployments, you can just use payload as it is (comes in as bytes)
 
 
 Large Language models
 ~~~~~~~~~~~~~~~~~~~~~
 
-EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface:
+EzSMDeploy supports deploying foundation models through Jumpstart as well as huggingface. Genreral guidance:
+
+
+1. Jumpstart models - `foundation_model=True`
+2. Large huggingface models - `foundation_model=True, huggingface_model=True`
+3. Small huggingface models - `huggingface_model=True`
+4. Tiny models - `serverless=True`
+
 
 To deploy models using Jumpstart:
 
 ::
 
     ezonsm = ezsmdeploy.Deploy(model = "huggingface-text2text-flan-ul2-bf16",
                                foundation_model=True)
```

### Comparing `ezsmdeploy-1.93.dev0/ezsmdeploy.egg-info/SOURCES.txt` & `ezsmdeploy-1.95.dev0/ezsmdeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploy-1.93.dev0/setup.py` & `ezsmdeploy-1.95.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploy',
-      version='1.93dev',
+      version='1.95dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
       package_data={'ezsmdeploy': ['data/*']},
       include_package_data=True,
       extras_require = extras,
-      install_requires=["sagemaker==2.171.0","yaspin==0.16.0","shortuuid==1.0.1","sagemaker-studio-image-build==0.5.0", "boto3>=1.14.12"],
+      install_requires=["sagemaker==2.173.0","yaspin==0.16.0","shortuuid==1.0.1","sagemaker-studio-image-build==0.5.0", "boto3>=1.14.12"],
       zip_safe=False,
       classifiers=['Development Status :: 3 - Alpha',
                    "Intended Audience :: Developers",
                    "Natural Language :: English",
                    "License :: OSI Approved :: Apache Software License",
                    "Programming Language :: Python"],
       long_description=read("README.rst")
```

