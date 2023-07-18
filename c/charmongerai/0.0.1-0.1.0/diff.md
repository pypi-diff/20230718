# Comparing `tmp/charmongerai-0.0.1.tar.gz` & `tmp/charmongerai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmongerai-0.0.1.tar", last modified: Mon Jul 17 04:13:05 2023, max compression
+gzip compressed data, was "charmongerai-0.1.0.tar", last modified: Tue Jul 18 08:35:18 2023, max compression
```

## Comparing `charmongerai-0.0.1.tar` & `charmongerai-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-17 04:13:05.432812 charmongerai-0.0.1/
--rw-r--r--   0 vdutts7    (501) staff       (20)    11360 2023-07-17 04:12:47.000000 charmongerai-0.0.1/LICENSE.txt
--rw-r--r--   0 vdutts7    (501) staff       (20)      514 2023-07-17 04:13:05.432572 charmongerai-0.0.1/PKG-INFO
--rw-r--r--   0 vdutts7    (501) staff       (20)       21 2023-07-17 04:12:46.000000 charmongerai-0.0.1/README.md
--rw-r--r--   0 vdutts7    (501) staff       (20)      612 2023-07-17 04:12:48.000000 charmongerai-0.0.1/pyproject.toml
--rw-r--r--   0 vdutts7    (501) staff       (20)       38 2023-07-17 04:13:05.432859 charmongerai-0.0.1/setup.cfg
-drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-17 04:13:05.430030 charmongerai-0.0.1/src/
-drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-17 04:13:05.431643 charmongerai-0.0.1/src/charmongerai/
--rw-rw-r--   0 vdutts7    (501) staff       (20)       38 2023-07-17 04:04:35.000000 charmongerai-0.0.1/src/charmongerai/__init__.py
--rw-rw-r--   0 vdutts7    (501) staff       (20)     2041 2023-07-17 04:04:35.000000 charmongerai-0.0.1/src/charmongerai/charmongerai.py
--rw-rw-r--   0 vdutts7    (501) staff       (20)     4074 2023-07-17 04:04:35.000000 charmongerai-0.0.1/src/charmongerai/cli.py
--rw-rw-r--   0 vdutts7    (501) staff       (20)     1124 2023-07-17 04:04:35.000000 charmongerai-0.0.1/src/charmongerai/config.py
--rw-rw-r--   0 vdutts7    (501) staff       (20)     1535 2023-07-17 04:04:35.000000 charmongerai-0.0.1/src/charmongerai/util.py
-drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-17 04:13:05.432313 charmongerai-0.0.1/src/charmongerai.egg-info/
--rw-r--r--   0 vdutts7    (501) staff       (20)      514 2023-07-17 04:13:05.000000 charmongerai-0.0.1/src/charmongerai.egg-info/PKG-INFO
--rw-r--r--   0 vdutts7    (501) staff       (20)      334 2023-07-17 04:13:05.000000 charmongerai-0.0.1/src/charmongerai.egg-info/SOURCES.txt
--rw-r--r--   0 vdutts7    (501) staff       (20)        1 2023-07-17 04:13:05.000000 charmongerai-0.0.1/src/charmongerai.egg-info/dependency_links.txt
--rw-r--r--   0 vdutts7    (501) staff       (20)       13 2023-07-17 04:13:05.000000 charmongerai-0.0.1/src/charmongerai.egg-info/top_level.txt
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.652191 charmongerai-0.1.0/
+-rw-r--r--   0 vdutts7    (501) staff       (20)       72 2023-07-18 07:43:54.000000 charmongerai-0.1.0/.gitignore
+-rw-r--r--   0 vdutts7    (501) staff       (20)    11360 2023-07-18 07:43:50.000000 charmongerai-0.1.0/LICENSE.txt
+-rw-r--r--   0 vdutts7    (501) staff       (20)      825 2023-07-18 08:35:18.651941 charmongerai-0.1.0/PKG-INFO
+-rw-r--r--   0 vdutts7    (501) staff       (20)      341 2023-07-18 08:23:33.000000 charmongerai-0.1.0/README.md
+-rw-r--r--   0 vdutts7    (501) staff       (20)      613 2023-07-18 08:23:27.000000 charmongerai-0.1.0/pyproject.toml
+-rw-r--r--   0 vdutts7    (501) staff       (20)       38 2023-07-18 08:35:18.652246 charmongerai-0.1.0/setup.cfg
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.648387 charmongerai-0.1.0/src/
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.650469 charmongerai-0.1.0/src/charmongerai/
+-rw-r--r--   0 vdutts7    (501) staff       (20)       38 2023-07-18 07:40:43.000000 charmongerai-0.1.0/src/charmongerai/__init__.py
+-rw-r--r--   0 vdutts7    (501) staff       (20)     6504 2023-07-18 08:23:34.000000 charmongerai-0.1.0/src/charmongerai/charmongerai.py
+-rw-r--r--   0 vdutts7    (501) staff       (20)     8505 2023-07-18 08:00:37.000000 charmongerai-0.1.0/src/charmongerai/cli.py
+-rw-r--r--   0 vdutts7    (501) staff       (20)     1721 2023-07-18 07:55:55.000000 charmongerai-0.1.0/src/charmongerai/config.py
+-rw-r--r--   0 vdutts7    (501) staff       (20)     1348 2023-07-18 08:00:33.000000 charmongerai-0.1.0/src/charmongerai/context.py
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.651332 charmongerai-0.1.0/src/charmongerai/discord/
+-rw-rw-r--   0 vdutts7    (501) staff       (20)       47 2023-07-18 07:48:06.000000 charmongerai-0.1.0/src/charmongerai/discord/__init__.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)      335 2023-07-18 07:48:06.000000 charmongerai-0.1.0/src/charmongerai/discord/client.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)     2161 2023-07-18 08:00:20.000000 charmongerai-0.1.0/src/charmongerai/model.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)     1065 2023-07-18 07:57:27.000000 charmongerai-0.1.0/src/charmongerai/retriever.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)     3388 2023-07-18 08:00:09.000000 charmongerai-0.1.0/src/charmongerai/settings.py
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.651690 charmongerai-0.1.0/src/charmongerai/simulation/
+-rw-rw-r--   0 vdutts7    (501) staff       (20)        0 2023-07-18 07:48:06.000000 charmongerai-0.1.0/src/charmongerai/simulation/__init__.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)    14895 2023-07-18 08:23:24.000000 charmongerai-0.1.0/src/charmongerai/simulation/agent.py
+-rw-rw-r--   0 vdutts7    (501) staff       (20)     4767 2023-07-18 08:23:25.000000 charmongerai-0.1.0/src/charmongerai/simulation/simulation.py
+-rw-r--r--   0 vdutts7    (501) staff       (20)     2207 2023-07-18 08:03:51.000000 charmongerai-0.1.0/src/charmongerai/util.py
+drwxr-xr-x   0 vdutts7    (501) staff       (20)        0 2023-07-18 08:35:18.651067 charmongerai-0.1.0/src/charmongerai.egg-info/
+-rw-r--r--   0 vdutts7    (501) staff       (20)      825 2023-07-18 08:35:18.000000 charmongerai-0.1.0/src/charmongerai.egg-info/PKG-INFO
+-rw-r--r--   0 vdutts7    (501) staff       (20)      649 2023-07-18 08:35:18.000000 charmongerai-0.1.0/src/charmongerai.egg-info/SOURCES.txt
+-rw-r--r--   0 vdutts7    (501) staff       (20)        1 2023-07-18 08:35:18.000000 charmongerai-0.1.0/src/charmongerai.egg-info/dependency_links.txt
+-rw-r--r--   0 vdutts7    (501) staff       (20)       13 2023-07-18 08:35:18.000000 charmongerai-0.1.0/src/charmongerai.egg-info/top_level.txt
```

### Comparing `charmongerai-0.0.1/LICENSE.txt` & `charmongerai-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `charmongerai-0.0.1/PKG-INFO` & `charmongerai-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Metadata-Version: 2.1
 Name: charmongerai
-Version: 0.0.1
+Version: 0.1.0
 Summary: AI Characters
 Author-email: vdutts7 <me@vdutts7.com>
 Project-URL: Homepage, https://github.com/vdutts7/charmonger-ai
 Project-URL: Bug Tracker, https://github.com/vdutts7/charmonger-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyPi ~ charmongerai
+# 👹 CharmongerAI - Bring Your Characters to Life
+
+`CharmongerAI` illustrates the lifelike nature of LLM entities, better known as agents. 
+
+Using the `charmongerai` package, users can quickly get started creating virtual fantasies, 
+scenarios, and online conversations with their own characters.
+
+🔗 https://www.charmonger.ai/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `charmongerai-0.0.1/pyproject.toml` & `charmongerai-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm[toml]>=6.2",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "charmongerai"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="vdutts7", email="me@vdutts7.com" },
 ]
 description = "AI Characters"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -20,7 +20,8 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/vdutts7/charmonger-ai"
 "Bug Tracker" = "https://github.com/vdutts7/charmonger-ai/issues"
+
```

### Comparing `charmongerai-0.0.1/src/charmongerai/config.py` & `charmongerai-0.1.0/src/charmongerai/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,54 @@
 import os
 from pathlib import Path
-from charmongerai.util import set_json_value, load_json_value
+
+from charmongerai.util import load_json_value, set_json_value
+
 
 def set_openai_token(token: str):
     config_dir = Path(Path.home(), ".charmongerai")
     if not config_dir.exists():
         config_dir.mkdir(parents=True)
     config_file = Path(config_dir, "config.json")
     set_json_value(config_file, "openai_token", token)
 
 
 def set_pinecone_token(token: str):
     config_dir = Path(Path.home(), ".charmongerai")
     if not config_dir.exists():
         config_dir.mkdir(parents=True)
     config_file = Path(config_dir, "config.json")
-    set_json_value(config_file, "pinecone_token", token)
+    set_json_value(config_file, "openai_token", token)
+
+
+def set_discord_token(token: str):
+    config_dir = Path(Path.home(), ".charmongerai")
+    if not config_dir.exists():
+        config_dir.mkdir(parents=True)
+    config_file = Path(config_dir, "config.json")
+    set_json_value(config_file, "discord_token", token)
 
 
 def load_pinecone_token() -> str:
     config_dir = Path(Path.home(), ".charmongerai")
     if not config_dir.exists():
         return ""
     config_file = Path(config_dir, "config.json")
     return load_json_value(config_file, "pinecone_token", "")
 
 
 def load_openai_token() -> str:
+    if "OPENAI_API_KEY" in os.environ:
+        return os.environ["OPENAI_API_KEY"]
     config_dir = Path(Path.home(), ".charmongerai")
     if not config_dir.exists():
         return ""
     config_file = Path(config_dir, "config.json")
     return load_json_value(config_file, "openai_token", "")
+
+
+def load_discord_token() -> str:
+    config_dir = Path(Path.home(), ".charmongerai")
+    if not config_dir.exists():
+        return ""
+    config_file = Path(config_dir, "config.json")
+    return load_json_value(config_file, "discord_token", "")
```

### Comparing `charmongerai-0.0.1/src/charmongerai.egg-info/PKG-INFO` & `charmongerai-0.1.0/src/charmongerai.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 Metadata-Version: 2.1
 Name: charmongerai
-Version: 0.0.1
+Version: 0.1.0
 Summary: AI Characters
 Author-email: vdutts7 <me@vdutts7.com>
 Project-URL: Homepage, https://github.com/vdutts7/charmonger-ai
 Project-URL: Bug Tracker, https://github.com/vdutts7/charmonger-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# PyPi ~ charmongerai
+# 👹 CharmongerAI - Bring Your Characters to Life
+
+`CharmongerAI` illustrates the lifelike nature of LLM entities, better known as agents. 
+
+Using the `charmongerai` package, users can quickly get started creating virtual fantasies, 
+scenarios, and online conversations with their own characters.
+
+🔗 https://www.charmonger.ai/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

