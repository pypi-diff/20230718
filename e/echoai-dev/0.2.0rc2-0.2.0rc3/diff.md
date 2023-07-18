# Comparing `tmp/echoai-dev-0.2.0rc2.tar.gz` & `tmp/echoai-dev-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoai-dev-0.2.0rc2.tar", last modified: Tue Apr 11 07:16:50 2023, max compression
+gzip compressed data, was "echoai-dev-0.2.0rc3.tar", last modified: Tue Jul 18 05:23:54 2023, max compression
```

## Comparing `echoai-dev-0.2.0rc2.tar` & `echoai-dev-0.2.0rc3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:16:50.121872 echoai-dev-0.2.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 07:16:50.121872 echoai-dev-0.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:16:50.117872 echoai-dev-0.2.0rc2/echoai/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/echoai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:16:50.117872 echoai-dev-0.2.0rc2/echoai/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/echoai/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/echoai/clients/langchain_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/echoai/clients/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/echoai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:16:50.121872 echoai-dev-0.2.0rc2/echoai_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 07:16:50.000000 echoai-dev-0.2.0rc2/echoai_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:16:50.121872 echoai-dev-0.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-11 07:16:39.000000 echoai-dev-0.2.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/echoai/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/echoai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/echoai/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/echoai/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/echoai/clients/langchain_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/echoai/clients/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/echoai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/echoai_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 05:23:54.000000 echoai-dev-0.2.0rc3/echoai_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:23:54.337171 echoai-dev-0.2.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-18 05:23:43.000000 echoai-dev-0.2.0rc3/setup.py
```

### Comparing `echoai-dev-0.2.0rc2/LICENSE.txt` & `echoai-dev-0.2.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.2.0rc2/PKG-INFO` & `echoai-dev-0.2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoai-dev
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: The command line tool to interface with Generative AI.
 Author: Fabio Dr.No Nonato
 Author-email: echoaidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `echoai-dev-0.2.0rc2/README.md` & `echoai-dev-0.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.2.0rc2/echoai/clients/langchain_client.py` & `echoai-dev-0.2.0rc3/echoai/clients/langchain_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from langchain.llms import OpenAI, AzureOpenAI
-from langchain.callbacks.base import CallbackManager
+from langchain.callbacks.manager import CallbackManager
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 import openai
 import os
 
 from langchain.prompts import (
     ChatPromptTemplate, 
     MessagesPlaceholder,
```

### Comparing `echoai-dev-0.2.0rc2/echoai/clients/openai_client.py` & `echoai-dev-0.2.0rc3/echoai/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.2.0rc2/echoai/main.py` & `echoai-dev-0.2.0rc3/echoai/main.py`

 * *Files identical despite different names*

### Comparing `echoai-dev-0.2.0rc2/echoai_dev.egg-info/PKG-INFO` & `echoai-dev-0.2.0rc3/echoai_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoai-dev
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: The command line tool to interface with Generative AI.
 Author: Fabio Dr.No Nonato
 Author-email: echoaidev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `echoai-dev-0.2.0rc2/setup.py` & `echoai-dev-0.2.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 commit_sha = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip().decode()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="echoai-dev",
-    version=f"0.2.0rc2",
+    version=f"0.2.0rc3",
     author="Fabio Dr.No Nonato",
     author_email="echoaidev@gmail.com",
     description="The command line tool to interface with Generative AI.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

