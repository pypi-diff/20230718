# Comparing `tmp/ADattribution-0.0.3.tar.gz` & `tmp/ADattribution-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADattribution-0.0.3.tar", last modified: Thu Apr  6 06:55:16 2023, max compression
+gzip compressed data, was "ADattribution-0.0.4.tar", last modified: Tue Jul 18 08:27:48 2023, max compression
```

## Comparing `ADattribution-0.0.3.tar` & `ADattribution-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-04-06 06:55:16.255942 ADattribution-0.0.3/
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-04-06 06:55:16.254839 ADattribution-0.0.3/ADattribution/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     5833 2023-04-06 06:54:37.000000 ADattribution-0.0.3/ADattribution/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1107 2023-02-28 08:40:57.000000 ADattribution-0.0.3/ADattribution/adq_postback.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-04-06 06:55:16.255683 ADattribution-0.0.3/ADattribution.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      747 2023-04-06 06:55:16.000000 ADattribution-0.0.3/ADattribution.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      266 2023-04-06 06:55:16.000000 ADattribution-0.0.3/ADattribution.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-04-06 06:55:16.000000 ADattribution-0.0.3/ADattribution.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       35 2023-04-06 06:55:16.000000 ADattribution-0.0.3/ADattribution.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       14 2023-04-06 06:55:16.000000 ADattribution-0.0.3/ADattribution.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-04-06 06:34:13.000000 ADattribution-0.0.3/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)      747 2023-04-06 06:55:16.255843 ADattribution-0.0.3/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      390 2023-04-06 06:35:18.000000 ADattribution-0.0.3/README.md
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-04-06 06:55:16.255986 ADattribution-0.0.3/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      906 2023-04-06 06:54:37.000000 ADattribution-0.0.3/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-18 08:27:48.607354 ADattribution-0.0.4/
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-18 08:27:48.606275 ADattribution-0.0.4/ADattribution/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     5868 2023-07-18 08:25:38.000000 ADattribution-0.0.4/ADattribution/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1107 2023-02-28 08:40:57.000000 ADattribution-0.0.4/ADattribution/adq_postback.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4514 2023-07-18 08:25:38.000000 ADattribution-0.0.4/ADattribution/oceanengine_postback.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-18 08:27:48.607077 ADattribution-0.0.4/ADattribution.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2023-07-18 08:27:48.000000 ADattribution-0.0.4/ADattribution.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      304 2023-07-18 08:27:48.000000 ADattribution-0.0.4/ADattribution.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-18 08:27:48.000000 ADattribution-0.0.4/ADattribution.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       35 2023-07-18 08:27:48.000000 ADattribution-0.0.4/ADattribution.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       14 2023-07-18 08:27:48.000000 ADattribution-0.0.4/ADattribution.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1067 2023-04-06 06:34:13.000000 ADattribution-0.0.4/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      756 2023-07-18 08:27:48.607244 ADattribution-0.0.4/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      390 2023-04-06 06:35:18.000000 ADattribution-0.0.4/README.md
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-18 08:27:48.607408 ADattribution-0.0.4/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      915 2023-07-18 08:26:04.000000 ADattribution-0.0.4/setup.py
```

### Comparing `ADattribution-0.0.3/ADattribution/__init__.py` & `ADattribution-0.0.4/ADattribution/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @ e-mail : zeroseeker@foxmail.com
 @ GitHub : https://github.com/ZeroSeeker
 @ Gitee : https://gitee.com/ZeroSeeker
 """
 from ua_parser import user_agent_parser
 from difflib import SequenceMatcher
 from . import adq_postback
+from . import oceanengine_postback
 
 
 def similarity(
         x: str,
         y: str
 ) -> float:
     """
```

### Comparing `ADattribution-0.0.3/ADattribution/adq_postback.py` & `ADattribution-0.0.4/ADattribution/adq_postback.py`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.3/ADattribution.egg-info/PKG-INFO` & `ADattribution-0.0.4/ADattribution.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ADattribution
-Version: 0.0.3
-Summary: make it easy to use AD
+Version: 0.0.4
+Summary: make it easy to use AD postback
 Home-page: https://gitee.com/ZeroSeeker/ADattribution
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ADattribution-0.0.3/LICENSE` & `ADattribution-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ADattribution-0.0.3/PKG-INFO` & `ADattribution-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ADattribution
-Version: 0.0.3
-Summary: make it easy to use AD
+Version: 0.0.4
+Summary: make it easy to use AD postback
 Home-page: https://gitee.com/ZeroSeeker/ADattribution
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ADattribution-0.0.3/setup.py` & `ADattribution-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ADattribution",
-    version="0.0.3",
+    version="0.0.4",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
-    description="make it easy to use AD",
+    description="make it easy to use AD postback",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/ADattribution",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         # "License :: OSI Approved :: MIT License",
```

