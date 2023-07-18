# Comparing `tmp/agentbrowser-0.1.0.tar.gz` & `tmp/agentbrowser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentbrowser-0.1.0.tar", last modified: Mon Jul 10 20:11:44 2023, max compression
+gzip compressed data, was "agentbrowser-0.1.1.tar", last modified: Mon Jul 10 20:13:52 2023, max compression
```

## Comparing `agentbrowser-0.1.0.tar` & `agentbrowser-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:11:44.919179 agentbrowser-0.1.0/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-08 17:50:31.000000 agentbrowser-0.1.0/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     3663 2023-07-10 20:11:44.918995 agentbrowser-0.1.0/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     3058 2023-07-10 20:09:51.000000 agentbrowser-0.1.0/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:11:44.917422 agentbrowser-0.1.0/agentbrowser/
--rw-r--r--   0 shawwalters   (501) staff       (20)      593 2023-07-10 20:11:41.000000 agentbrowser-0.1.0/agentbrowser/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5410 2023-07-10 20:02:45.000000 agentbrowser-0.1.0/agentbrowser/browser.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     1374 2023-07-10 20:10:54.000000 agentbrowser-0.1.0/agentbrowser/browser_test.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:11:44.918666 agentbrowser-0.1.0/agentbrowser.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     3663 2023-07-10 20:11:44.000000 agentbrowser-0.1.0/agentbrowser.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      283 2023-07-10 20:11:44.000000 agentbrowser-0.1.0/agentbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 20:11:44.000000 agentbrowser-0.1.0/agentbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        9 2023-07-10 20:11:44.000000 agentbrowser-0.1.0/agentbrowser.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       13 2023-07-10 20:11:44.000000 agentbrowser-0.1.0/agentbrowser.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 20:11:44.919231 agentbrowser-0.1.0/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1260 2023-07-10 20:11:41.000000 agentbrowser-0.1.0/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:13:52.674192 agentbrowser-0.1.1/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-08 17:50:31.000000 agentbrowser-0.1.1/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3674 2023-07-10 20:13:52.674032 agentbrowser-0.1.1/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3058 2023-07-10 20:09:51.000000 agentbrowser-0.1.1/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:13:52.672477 agentbrowser-0.1.1/agentbrowser/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      609 2023-07-10 20:13:48.000000 agentbrowser-0.1.1/agentbrowser/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5410 2023-07-10 20:02:45.000000 agentbrowser-0.1.1/agentbrowser/browser.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1374 2023-07-10 20:10:54.000000 agentbrowser-0.1.1/agentbrowser/browser_test.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-10 20:13:52.673801 agentbrowser-0.1.1/agentbrowser.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     3674 2023-07-10 20:13:52.000000 agentbrowser-0.1.1/agentbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      283 2023-07-10 20:13:52.000000 agentbrowser-0.1.1/agentbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-10 20:13:52.000000 agentbrowser-0.1.1/agentbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       10 2023-07-10 20:13:52.000000 agentbrowser-0.1.1/agentbrowser.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       13 2023-07-10 20:13:52.000000 agentbrowser-0.1.1/agentbrowser.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-10 20:13:52.674246 agentbrowser-0.1.1/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1257 2023-07-10 20:13:48.000000 agentbrowser-0.1.1/setup.py
```

### Comparing `agentbrowser-0.1.0/LICENSE` & `agentbrowser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.1.0/PKG-INFO` & `agentbrowser-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: agentbrowser
-Version: 0.1.0
-Summary: Easy-to-use agent memory, powered by chromadb
+Version: 0.1.1
+Summary: A browser for your agent, built on Chrome and Pyppeteer.
 Home-page: https://github.com/lalalune/agentbrowser
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agentbrowser-0.1.0/README.md` & `agentbrowser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.1.0/agentbrowser/__init__.py` & `agentbrowser-0.1.1/agentbrowser/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 agentbrowser
 
-Simple agent memory, powered by chromadb
+A browser for your agent, built on Chrome and Pyppeteer.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Moon (https://github.com/lalalune)"
 __credits__ = "https://github.com/lalalune/agentbrowser"
 
 from .browser import (
     get_browser,
     init_browser,
     create_page,
```

### Comparing `agentbrowser-0.1.0/agentbrowser/browser.py` & `agentbrowser-0.1.1/agentbrowser/browser.py`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.1.0/agentbrowser/browser_test.py` & `agentbrowser-0.1.1/agentbrowser/browser_test.py`

 * *Files identical despite different names*

### Comparing `agentbrowser-0.1.0/agentbrowser.egg-info/PKG-INFO` & `agentbrowser-0.1.1/agentbrowser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: agentbrowser
-Version: 0.1.0
-Summary: Easy-to-use agent memory, powered by chromadb
+Version: 0.1.1
+Summary: A browser for your agent, built on Chrome and Pyppeteer.
 Home-page: https://github.com/lalalune/agentbrowser
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `agentbrowser-0.1.0/setup.py` & `agentbrowser-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from setuptools import setup
 
 long_description = ""
 with open("README.md", "r") as fh:
     long_description = fh.read()
     # search for any lines that contain <img and remove them
-    long_description = long_description.split('\n')
-    long_description = [line for line in long_description if not '<img' in line]
+    long_description = long_description.split("\n")
+    long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
-    long_description = '\n'.join(long_description)
-    
+    long_description = "\n".join(long_description)
+
 
 setup(
-    name='agentbrowser',
-    version='0.1.0',
-    description='Easy-to-use agent memory, powered by chromadb',
+    name="agentbrowser",
+    version='0.1.1',
+    description="A browser for your agent, built on Chrome and Pyppeteer.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
-    url='https://github.com/lalalune/agentbrowser',
-    author='Moon',
-    author_email='shawmakesmagic@gmail.com',
-    license='MIT',
-    packages=['agentbrowser'],
-    install_requires=['chromadb'],
-    readme = "README.md",
+    url="https://github.com/lalalune/agentbrowser",
+    author="Moon",
+    author_email="shawmakesmagic@gmail.com",
+    license="MIT",
+    packages=["agentbrowser"],
+    install_requires=["pyppeteer"],
+    readme="README.md",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',  
-        'Operating System :: POSIX :: Linux',        
-        'Programming Language :: Python :: 3',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: Microsoft :: Windows'
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
     ],
 )
```

