# Comparing `tmp/USSCameraTools-0.1.1.tar.gz` & `tmp/USSCameraTools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "USSCameraTools-0.1.1.tar", last modified: Fri Jul 14 19:16:48 2023, max compression
+gzip compressed data, was "USSCameraTools-0.1.2.tar", last modified: Tue Jul 18 16:19:47 2023, max compression
```

## Comparing `USSCameraTools-0.1.1.tar` & `USSCameraTools-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/
--rw-rw-r--   0 bailey    (1000) bailey    (1000)      945 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/PKG-INFO
-drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/USSCameraTools/
--rw-rw-r--   0 bailey    (1000) bailey    (1000)       58 2023-07-14 17:24:01.000000 USSCameraTools-0.1.1/USSCameraTools/__init__.py
-drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/USSCameraTools.egg-info/
--rw-rw-r--   0 bailey    (1000) bailey    (1000)      945 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/PKG-INFO
--rw-rw-r--   0 bailey    (1000) bailey    (1000)      224 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/SOURCES.txt
--rw-rw-r--   0 bailey    (1000) bailey    (1000)        1 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/dependency_links.txt
--rw-rw-r--   0 bailey    (1000) bailey    (1000)       25 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/requires.txt
--rw-rw-r--   0 bailey    (1000) bailey    (1000)       15 2023-07-14 19:16:48.000000 USSCameraTools-0.1.1/USSCameraTools.egg-info/top_level.txt
--rw-rw-r--   0 bailey    (1000) bailey    (1000)       38 2023-07-14 19:16:48.186125 USSCameraTools-0.1.1/setup.cfg
--rw-rw-r--   0 bailey    (1000) bailey    (1000)     1101 2023-07-14 19:16:46.000000 USSCameraTools-0.1.1/setup.py
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-18 16:19:47.308110 USSCameraTools-0.1.2/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)     1012 2023-07-18 16:19:47.308110 USSCameraTools-0.1.2/PKG-INFO
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-18 16:19:47.308110 USSCameraTools-0.1.2/USSCameraTools/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       59 2023-07-18 16:09:06.000000 USSCameraTools-0.1.2/USSCameraTools/__init__.py
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)     8591 2023-07-14 18:58:24.000000 USSCameraTools-0.1.2/USSCameraTools/core.py
+drwxrwxr-x   0 bailey    (1000) bailey    (1000)        0 2023-07-18 16:19:47.308110 USSCameraTools-0.1.2/USSCameraTools.egg-info/
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)     1012 2023-07-18 16:19:47.000000 USSCameraTools-0.1.2/USSCameraTools.egg-info/PKG-INFO
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)      262 2023-07-18 16:19:47.000000 USSCameraTools-0.1.2/USSCameraTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)        1 2023-07-18 16:19:47.000000 USSCameraTools-0.1.2/USSCameraTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       31 2023-07-18 16:19:47.000000 USSCameraTools-0.1.2/USSCameraTools.egg-info/requires.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       15 2023-07-18 16:19:47.000000 USSCameraTools-0.1.2/USSCameraTools.egg-info/top_level.txt
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       97 2023-07-18 15:37:22.000000 USSCameraTools-0.1.2/pyproject.toml
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)       38 2023-07-18 16:19:47.308110 USSCameraTools-0.1.2/setup.cfg
+-rw-rw-r--   0 bailey    (1000) bailey    (1000)     1220 2023-07-18 16:18:35.000000 USSCameraTools-0.1.2/setup.py
```

### Comparing `USSCameraTools-0.1.1/PKG-INFO` & `USSCameraTools-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: USSCameraTools
-Version: 0.1.1
+Version: 0.1.2
 Summary: USSCamera: Python package for interacting with GigE cameras using the Harvesters library
-Home-page: UNKNOWN
-Author: USSVision
+Home-page: https://github.com/USSVision/USSCommonTools/tree/main/Packages/USSCameraTools
+Author: USS Vision
 Author-email: bhelfer@ussvision.com
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 USSCamera is a Python package that provides functionality to interact with GigE cameras using the Harvesters library. It allows you to easily connect to cameras, capture images, trigger the camera, and retrieve camera attributes.
```

### Comparing `USSCameraTools-0.1.1/USSCameraTools.egg-info/PKG-INFO` & `USSCameraTools-0.1.2/USSCameraTools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: USSCameraTools
-Version: 0.1.1
+Version: 0.1.2
 Summary: USSCamera: Python package for interacting with GigE cameras using the Harvesters library
-Home-page: UNKNOWN
-Author: USSVision
+Home-page: https://github.com/USSVision/USSCommonTools/tree/main/Packages/USSCameraTools
+Author: USS Vision
 Author-email: bhelfer@ussvision.com
-License: UNKNOWN
+License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 USSCamera is a Python package that provides functionality to interact with GigE cameras using the Harvesters library. It allows you to easily connect to cameras, capture images, trigger the camera, and retrieve camera attributes.
```

### Comparing `USSCameraTools-0.1.1/setup.py` & `USSCameraTools-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup
+from setuptools import setup,find_packages
 
 setup(
     name='USSCameraTools',
-    version='0.1.1',
+    version='0.1.2',
     description='USSCamera: Python package for interacting with GigE cameras using the Harvesters library',
     long_description='USSCamera is a Python package that provides functionality to interact with GigE cameras using the Harvesters library. It allows you to easily connect to cameras, capture images, trigger the camera, and retrieve camera attributes.',
     long_description_content_type='text/markdown',
-    author='USSVision',
+     url='https://github.com/USSVision/USSCommonTools/tree/main/Packages/USSCameraTools',
+    author='USS Vision',
     author_email='bhelfer@ussvision.com',
-    packages=['USSCameraTools'],
-    install_requires=[
-        'harvesters',
-        'opencv-python',
-    ],
+    license='MIT',
+    packages=find_packages(),
+    install_requires=['wheel','opencv-python','harvesters',],
+
     classifiers=[
         'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: Microsoft :: Windows :: Windows 10',
+        'License :: OSI Approved :: MIT License',  
         'Operating System :: POSIX :: Linux',
+        'Operating System :: Microsoft :: Windows :: Windows 10',         
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
     ],
 )
```

