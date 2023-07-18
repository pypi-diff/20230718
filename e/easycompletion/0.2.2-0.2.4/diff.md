# Comparing `tmp/easycompletion-0.2.2.tar.gz` & `tmp/easycompletion-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.2.tar", last modified: Sat Jul 15 00:36:29 2023, max compression
+gzip compressed data, was "easycompletion-0.2.4.tar", last modified: Tue Jul 18 14:06:59 2023, max compression
```

## Comparing `easycompletion-0.2.2.tar` & `easycompletion-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.275543 easycompletion-0.2.2/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.2.2/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-15 00:36:29.275373 easycompletion-0.2.2/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     6452 2023-07-14 09:03:44.000000 easycompletion-0.2.2/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.273554 easycompletion-0.2.2/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      776 2023-07-15 00:36:24.000000 easycompletion-0.2.2/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.2.2/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    14537 2023-07-14 09:00:43.000000 easycompletion-0.2.2/easycompletion/model.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5511 2023-07-15 00:35:11.000000 easycompletion-0.2.2/easycompletion/prompt.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.275107 easycompletion-0.2.2/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      319 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-15 00:36:29.275616 easycompletion-0.2.2/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1430 2023-07-15 00:36:24.000000 easycompletion-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:06:59.830449 easycompletion-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 14:06:40.000000 easycompletion-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-18 14:06:59.830449 easycompletion-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-18 14:06:40.000000 easycompletion-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:06:59.818448 easycompletion-0.2.4/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-18 14:06:40.000000 easycompletion-0.2.4/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 14:06:40.000000 easycompletion-0.2.4/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-07-18 14:06:40.000000 easycompletion-0.2.4/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-18 14:06:40.000000 easycompletion-0.2.4/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:06:59.830449 easycompletion-0.2.4/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-18 14:06:59.000000 easycompletion-0.2.4/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-18 14:06:59.000000 easycompletion-0.2.4/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:06:59.000000 easycompletion-0.2.4/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 14:06:59.000000 easycompletion-0.2.4/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:06:59.000000 easycompletion-0.2.4/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:06:59.830449 easycompletion-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-18 14:06:40.000000 easycompletion-0.2.4/setup.py
```

### Comparing `easycompletion-0.2.2/LICENSE` & `easycompletion-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.2/PKG-INFO` & `easycompletion-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.2
+Version: 0.2.4
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.2/README.md` & `easycompletion-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.2/easycompletion/model.py` & `easycompletion-0.2.4/easycompletion/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import time
 import openai
 import re
 import json
 import ast
 
 from dotenv import load_dotenv
@@ -187,15 +188,16 @@
 
     # Count tokens in the input text
     total_tokens = count_tokens(text, model=model)
 
     # If text is longer than chunk_length and model is not for long texts, switch to the long text model
     if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
-        print("Warning: Message is long. Using 16k model")
+        if not os.environ.get("SUPPRESS_WARNINGS"):
+            print("Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)")
 
     # If text is too long even for long text model, return None
     if total_tokens > (16384 - chunk_length):
         print("Error: Message too long")
         return {
             "text": None,
             usage: None,
@@ -334,15 +336,16 @@
     if functions is None:
         function_call_tokens = count_tokens(functions, model=model)
         total_tokens += function_call_tokens + 3  # Additional tokens for the user
 
     # Switch to a larger model if the message is too long for the default model
     if total_tokens > chunk_length and "16k" not in model:
         model = long_text_model
-        print("Warning: Message is long. Using 16k model")
+        if not os.environ.get("SUPPRESS_WARNINGS"):
+            print("Warning: Message is long. Using 16k model (to hide this message, set SUPPRESS_WARNINGS=1)")
 
     # Check if the total number of tokens exceeds the maximum allowable tokens for the model
     if total_tokens > (16384 - chunk_length):
         return {"error": "Message too long"}
 
     # Prepare the messages to be sent to the API
     messages = [{"role": "user", "content": text}]
```

### Comparing `easycompletion-0.2.2/easycompletion/prompt.py` & `easycompletion-0.2.4/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.2/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.2.4/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.2
+Version: 0.2.4
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.2/setup.py` & `easycompletion-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.2',
+    version='0.2.4',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

