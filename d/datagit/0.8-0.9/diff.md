# Comparing `tmp/datagit-0.8.tar.gz` & `tmp/datagit-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagit-0.8.tar", last modified: Tue Jul  4 09:25:47 2023, max compression
+gzip compressed data, was "datagit-0.9.tar", last modified: Tue Jul  4 12:42:18 2023, max compression
```

## Comparing `datagit-0.8.tar` & `datagit-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.755957 datagit-0.8/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-04 09:25:47.755800 datagit-0.8/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-04 08:55:47.000000 datagit-0.8/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.754719 datagit-0.8/datagit/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-07-04 08:55:47.000000 datagit-0.8/datagit/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2336 2023-07-04 08:55:47.000000 datagit-0.8/datagit/dataset_helpers.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     9804 2023-07-04 09:24:12.000000 datagit-0.8/datagit/github_connector.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-07-04 08:55:47.000000 datagit-0.8/datagit/query_builder.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 09:25:47.755560 datagit-0.8/datagit.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     3145 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-04 09:25:47.000000 datagit-0.8/datagit.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-04 09:25:47.756013 datagit-0.8/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      648 2023-07-04 09:25:34.000000 datagit-0.8/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 12:42:18.274848 datagit-0.9/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3172 2023-07-04 12:42:18.274691 datagit-0.9/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2745 2023-07-04 12:39:12.000000 datagit-0.9/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 12:42:18.273598 datagit-0.9/datagit/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-07-04 08:55:47.000000 datagit-0.9/datagit/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2336 2023-07-04 08:55:47.000000 datagit-0.9/datagit/dataset_helpers.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     9804 2023-07-04 12:32:35.000000 datagit-0.9/datagit/github_connector.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      721 2023-07-04 08:55:47.000000 datagit-0.9/datagit/query_builder.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-07-04 12:42:18.274448 datagit-0.9/datagit.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     3172 2023-07-04 12:42:18.000000 datagit-0.9/datagit.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      272 2023-07-04 12:42:18.000000 datagit-0.9/datagit.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-07-04 12:42:18.000000 datagit-0.9/datagit.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       16 2023-07-04 12:42:18.000000 datagit-0.9/datagit.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        8 2023-07-04 12:42:18.000000 datagit-0.9/datagit.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-07-04 12:42:18.274902 datagit-0.9/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      675 2023-07-04 12:42:10.000000 datagit-0.9/setup.py
```

### Comparing `datagit-0.8/PKG-INFO` & `datagit-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.8
+Version: 0.9
 Summary: Git based metric store
-Home-page: https://github.com/data-drift/datagit
+Home-page: https://github.com/data-drift/data-drift/tree/main/tools/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `datagit-0.8/README.md` & `datagit-0.9/README.md`

 * *Files identical despite different names*

### Comparing `datagit-0.8/datagit/dataset_helpers.py` & `datagit-0.9/datagit/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `datagit-0.8/datagit/github_connector.py` & `datagit-0.9/datagit/github_connector.py`

 * *Files identical despite different names*

### Comparing `datagit-0.8/datagit/query_builder.py` & `datagit-0.9/datagit/query_builder.py`

 * *Files identical despite different names*

### Comparing `datagit-0.8/datagit.egg-info/PKG-INFO` & `datagit-0.9/datagit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: datagit
-Version: 0.8
+Version: 0.9
 Summary: Git based metric store
-Home-page: https://github.com/data-drift/datagit
+Home-page: https://github.com/data-drift/data-drift/tree/main/tools/datagit
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `datagit-0.8/setup.py` & `datagit-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="datagit",
-    version="0.8",
+    version="0.9",
     packages=find_packages(),
     author="Sammy Teillet",
     author_email="sammy.teillet@gmail.com",
     description="Git based metric store",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url="https://github.com/data-drift/datagit",
+    url="https://github.com/data-drift/data-drift/tree/main/tools/datagit",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
```

