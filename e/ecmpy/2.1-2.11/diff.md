# Comparing `tmp/ECMPY-2.1.tar.gz` & `tmp/ecmpy-2.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ECMPY-2.1.tar", last modified: Tue Jul 18 05:24:51 2023, max compression
+gzip compressed data, was "ecmpy-2.11.tar", last modified: Tue Jul 18 06:14:24 2023, max compression
```

## Comparing `ECMPY-2.1.tar` & `ecmpy-2.11.tar`

### file list

```diff
@@ -1,12 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:24:51.222522 ECMPY-2.1/
-drwxrwxrwx   0        0        0        0 2023-07-18 05:24:51.222522 ECMPY-2.1/ECMPY.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      137 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:24:51.000000 ECMPY-2.1/ECMPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      223 2023-07-18 05:24:51.222522 ECMPY-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      700 2023-06-21 06:18:48.000000 ECMPY-2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 05:24:51.222522 ECMPY-2.1/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-07-18 05:24:32.000000 ECMPY-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:14:24.239674 ecmpy-2.11/
+-rw-rw-rw-   0        0        0      224 2023-07-18 06:14:24.239674 ecmpy-2.11/PKG-INFO
+-rw-rw-rw-   0        0        0      700 2023-06-21 06:18:48.000000 ecmpy-2.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 06:14:24.230549 ecmpy-2.11/ecmpy/
+-rw-rw-rw-   0        0        0    93279 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/AutoPACMEN_function.py
+-rw-rw-rw-   0        0        0   120059 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/ECMpy_function.py
+-rw-rw-rw-   0        0        0       19 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/__init__.py
+-rw-rw-rw-   0        0        0     4718 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/get_ecGEM_onestop.py
+-rw-rw-rw-   0        0        0     8905 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/model.py
+-rw-rw-rw-   0        0        0     9605 2023-07-10 07:56:31.000000 ecmpy-2.11/ecmpy/prediction_for_input.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:14:24.239674 ecmpy-2.11/ecmpy.egg-info/
+-rw-rw-rw-   0        0        0      224 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      137 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 06:14:24.000000 ecmpy-2.11/ecmpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 06:14:24.239674 ecmpy-2.11/setup.cfg
+-rw-rw-rw-   0        0        0      777 2023-07-18 06:14:04.000000 ecmpy-2.11/setup.py
```

### Comparing `ECMPY-2.1/README.md` & `ecmpy-2.11/README.md`

 * *Files identical despite different names*

### Comparing `ECMPY-2.1/setup.py` & `ecmpy-2.11/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup   
 
-setup(name='ECMPY',
-    version='2.1',
+setup(name='ecmpy',
+    version='2.11',
     description='Automated construction of enzyme constraint models using ECMpy workflow',
     author='TIB BioDesign Center',
     url = 'https://github.com/A-runaaaa/ecmpy',
     license='MIT',
     packages=find_packages(),
     zip_safe=False,
     include_package_data=True,
```

