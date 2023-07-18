# Comparing `tmp/guardshield-1.1.0.tar.gz` & `tmp/guardshield-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\guardshield-1.1.0.tar", last modified: Tue Jul 18 16:11:18 2023, max compression
+gzip compressed data, was "dist\guardshield-1.1.1.tar", last modified: Tue Jul 18 16:36:30 2023, max compression
```

## Comparing `guardshield-1.1.0.tar` & `guardshield-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 16:11:18.800427 guardshield-1.1.0/
--rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     5775 2023-07-18 16:11:18.799430 guardshield-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5311 2023-07-18 16:11:16.000000 guardshield-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 16:11:18.790454 guardshield-1.1.0/guardshield/
--rw-rw-rw-   0        0        0       89 2023-07-18 16:10:44.000000 guardshield-1.1.0/guardshield/__init__.py
--rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.1.0/guardshield/dll_bytes.py
--rw-rw-rw-   0        0        0     4840 2023-07-18 15:55:17.000000 guardshield-1.1.0/guardshield/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 16:11:18.797435 guardshield-1.1.0/guardshield.egg-info/
--rw-rw-rw-   0        0        0     5775 2023-07-18 16:11:18.000000 guardshield-1.1.0/guardshield.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-18 16:11:18.000000 guardshield-1.1.0/guardshield.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 16:11:18.000000 guardshield-1.1.0/guardshield.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 16:11:18.000000 guardshield-1.1.0/guardshield.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-07-18 16:11:18.000000 guardshield-1.1.0/guardshield.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 16:11:18.800427 guardshield-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      585 2023-07-18 16:11:07.000000 guardshield-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:36:29.999607 guardshield-1.1.1/
+-rw-rw-rw-   0        0        0     1061 2023-05-18 23:20:40.000000 guardshield-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5782 2023-07-18 16:36:29.998579 guardshield-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5311 2023-07-18 16:11:16.000000 guardshield-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 16:36:29.987609 guardshield-1.1.1/guardshield/
+-rw-rw-rw-   0        0        0      131 2023-07-18 16:31:57.000000 guardshield-1.1.1/guardshield/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:36:29.997582 guardshield-1.1.1/guardshield/core/
+-rw-rw-rw-   0        0        0     2078 2023-07-18 16:31:56.000000 guardshield-1.1.1/guardshield/core/cheatengine.py
+-rw-rw-rw-   0        0        0    58627 2023-07-08 20:13:23.000000 guardshield-1.1.1/guardshield/dll_bytes.py
+-rw-rw-rw-   0        0        0     4840 2023-07-18 16:32:01.000000 guardshield-1.1.1/guardshield/main.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:36:29.995587 guardshield-1.1.1/guardshield.egg-info/
+-rw-rw-rw-   0        0        0     5782 2023-07-18 16:36:29.000000 guardshield-1.1.1/guardshield.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-18 16:36:29.000000 guardshield-1.1.1/guardshield.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:36:29.000000 guardshield-1.1.1/guardshield.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 16:36:29.000000 guardshield-1.1.1/guardshield.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-07-18 16:36:29.000000 guardshield-1.1.1/guardshield.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 16:36:29.999607 guardshield-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-07-18 16:36:09.000000 guardshield-1.1.1/setup.py
```

### Comparing `guardshield-1.1.0/LICENSE` & `guardshield-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guardshield-1.1.0/PKG-INFO` & `guardshield-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guardshield
-Version: 1.1.0
-Summary: Security lib
+Version: 1.1.1
+Summary: Python security lib
 Home-page: https://github.com/OxynDev/ExcerSec
 Author: Oxyn
 Author-email: oxyn.dev@gmail.com
 License: MIT
 Keywords: python anti debugger security exe
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guardshield-1.1.0/README.md` & `guardshield-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `guardshield-1.1.0/guardshield/dll_bytes.py` & `guardshield-1.1.1/guardshield/dll_bytes.py`

 * *Files identical despite different names*

### Comparing `guardshield-1.1.0/guardshield/main.py` & `guardshield-1.1.1/guardshield/main.py`

 * *Files identical despite different names*

### Comparing `guardshield-1.1.0/guardshield.egg-info/PKG-INFO` & `guardshield-1.1.1/guardshield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: guardshield
-Version: 1.1.0
-Summary: Security lib
+Version: 1.1.1
+Summary: Python security lib
 Home-page: https://github.com/OxynDev/ExcerSec
 Author: Oxyn
 Author-email: oxyn.dev@gmail.com
 License: MIT
 Keywords: python anti debugger security exe
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `guardshield-1.1.0/setup.py` & `guardshield-1.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import setuptools, os
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name="guardshield",
-    version="1.1.0",
+    version="1.1.1",
     author="Oxyn",
     author_email="oxyn.dev@gmail.com",
-    description="Security lib",
-    keywords = "python anti debugger security exe",
+    description="Python security lib",
+    keywords="python anti debugger security exe",
     packages=setuptools.find_packages(),
     include_package_data=True,
     url='https://github.com/OxynDev/ExcerSec',
     zip_safe=False,
     license='MIT',
     long_description=read('README.md'),
-    long_description_content_type='text/markdown'
-)
+    long_description_content_type='text/markdown',
+    data_files=[('guardshield/core', ['guardshield/core/cheatengine.py'])],
+)
```

