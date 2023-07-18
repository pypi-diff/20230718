# Comparing `tmp/orbitalcyber-sdk-0.1.1.tar.gz` & `tmp/orbitalcyber-sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Rylan Merritt\Development\orbitalcyber-python-sdk\dist\.tmp-mb5zxv8n\orbitalcyber-sdk-0.1.1.tar", last modified: Tue Jul 18 20:28:50 2023, max compression
+gzip compressed data, was "C:\Users\Rylan Merritt\Development\orbitalcyber-python-sdk\dist\.tmp-zkdju5ji\orbitalcyber-sdk-0.1.2.tar", last modified: Tue Jul 18 20:47:28 2023, max compression
```

## Comparing `orbitalcyber-sdk-0.1.1.tar` & `orbitalcyber-sdk-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:28:50.158384 orbitalcyber-sdk-0.1.1/
--rw-rw-rw-   0        0        0     1117 2023-06-30 20:41:54.000000 orbitalcyber-sdk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      522 2023-07-18 20:28:50.157384 orbitalcyber-sdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-06-30 20:41:54.000000 orbitalcyber-sdk-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 20:28:50.141888 orbitalcyber-sdk-0.1.1/orbitalcyber/
--rw-rw-rw-   0        0        0     4616 2023-07-05 19:47:36.000000 orbitalcyber-sdk-0.1.1/orbitalcyber/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:28:50.144269 orbitalcyber-sdk-0.1.1/orbitalcyber/exceptions/
--rw-rw-rw-   0        0        0      802 2023-07-05 19:33:34.000000 orbitalcyber-sdk-0.1.1/orbitalcyber/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:28:50.156457 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/
--rw-rw-rw-   0        0        0      522 2023-07-18 20:28:50.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-07-18 20:28:50.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:28:50.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-05 19:28:48.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-18 20:28:50.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 20:28:50.000000 orbitalcyber-sdk-0.1.1/orbitalcyber_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 20:28:50.158469 orbitalcyber-sdk-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-07-18 20:28:36.000000 orbitalcyber-sdk-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:47:28.754013 orbitalcyber-sdk-0.1.2/
+-rw-rw-rw-   0        0        0     1117 2023-06-30 20:41:54.000000 orbitalcyber-sdk-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1714 2023-07-18 20:47:28.753013 orbitalcyber-sdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1299 2023-07-18 20:45:45.000000 orbitalcyber-sdk-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 20:47:28.729848 orbitalcyber-sdk-0.1.2/orbitalcyber/
+-rw-rw-rw-   0        0        0     4616 2023-07-05 19:47:36.000000 orbitalcyber-sdk-0.1.2/orbitalcyber/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:47:28.737913 orbitalcyber-sdk-0.1.2/orbitalcyber/exceptions/
+-rw-rw-rw-   0        0        0      802 2023-07-05 19:33:34.000000 orbitalcyber-sdk-0.1.2/orbitalcyber/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:47:28.752067 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1714 2023-07-18 20:47:28.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-18 20:47:28.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 20:47:28.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-05 19:28:48.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-18 20:47:28.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 20:47:28.000000 orbitalcyber-sdk-0.1.2/orbitalcyber_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 20:47:28.755015 orbitalcyber-sdk-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-07-18 20:47:10.000000 orbitalcyber-sdk-0.1.2/setup.py
```

### Comparing `orbitalcyber-sdk-0.1.1/LICENSE` & `orbitalcyber-sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitalcyber-sdk-0.1.1/orbitalcyber/__init__.py` & `orbitalcyber-sdk-0.1.2/orbitalcyber/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitalcyber-sdk-0.1.1/orbitalcyber/exceptions/__init__.py` & `orbitalcyber-sdk-0.1.2/orbitalcyber/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitalcyber-sdk-0.1.1/setup.py` & `orbitalcyber-sdk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 requires = ['requests']
 setup(name='orbitalcyber-sdk',
-      version='0.1.1',
+      version='0.1.2',
       description='This package provides an SDK that can be used to jumpstart projects that interact with the OrbitalCyber API',
       url='https://github.com/Sage-Infrastructure-Solutions-Group-Inc/orbitalcyber-python-sdk',
       author='Rylan Merritt',
       author_email='rmerritt@sageisg.com',
       license='MIT',
       install_requires=requires,
       packages=find_packages(),
```

