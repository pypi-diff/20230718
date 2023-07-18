# Comparing `tmp/easysec-0.0.1.tar.gz` & `tmp/easysec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easysec-0.0.1.tar", last modified: Tue Jul 18 12:16:46 2023, max compression
+gzip compressed data, was "easysec-0.0.2.tar", last modified: Tue Jul 18 12:19:51 2023, max compression
```

## Comparing `easysec-0.0.1.tar` & `easysec-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:16:46.183256 easysec-0.0.1/
--rw-r--r--   0 guille     (501) staff       (20)      562 2023-07-18 12:16:46.183132 easysec-0.0.1/PKG-INFO
--rw-r--r--   0 guille     (501) staff       (20)     2055 2023-07-18 12:10:44.000000 easysec-0.0.1/README.md
-drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:16:46.182093 easysec-0.0.1/easysec/
--rw-r--r--   0 guille     (501) staff       (20)       35 2023-07-12 16:22:23.000000 easysec-0.0.1/easysec/__init__.py
--rw-r--r--   0 guille     (501) staff       (20)     5878 2023-07-16 11:02:27.000000 easysec-0.0.1/easysec/easysec.py
-drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:16:46.182938 easysec-0.0.1/easysec.egg-info/
--rw-r--r--   0 guille     (501) staff       (20)      562 2023-07-18 12:16:46.000000 easysec-0.0.1/easysec.egg-info/PKG-INFO
--rw-r--r--   0 guille     (501) staff       (20)      211 2023-07-18 12:16:46.000000 easysec-0.0.1/easysec.egg-info/SOURCES.txt
--rw-r--r--   0 guille     (501) staff       (20)        1 2023-07-18 12:16:46.000000 easysec-0.0.1/easysec.egg-info/dependency_links.txt
--rw-r--r--   0 guille     (501) staff       (20)       21 2023-07-18 12:16:46.000000 easysec-0.0.1/easysec.egg-info/requires.txt
--rw-r--r--   0 guille     (501) staff       (20)        8 2023-07-18 12:16:46.000000 easysec-0.0.1/easysec.egg-info/top_level.txt
--rw-r--r--   0 guille     (501) staff       (20)       38 2023-07-18 12:16:46.183304 easysec-0.0.1/setup.cfg
--rw-r--r--   0 guille     (501) staff       (20)      920 2023-07-18 12:13:01.000000 easysec-0.0.1/setup.py
+drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:19:51.761940 easysec-0.0.2/
+-rw-r--r--   0 guille     (501) staff       (20)      562 2023-07-18 12:19:51.761834 easysec-0.0.2/PKG-INFO
+-rw-r--r--   0 guille     (501) staff       (20)     2055 2023-07-18 12:10:44.000000 easysec-0.0.2/README.md
+drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:19:51.760954 easysec-0.0.2/easysec/
+-rw-r--r--   0 guille     (501) staff       (20)       35 2023-07-12 16:22:23.000000 easysec-0.0.2/easysec/__init__.py
+-rw-r--r--   0 guille     (501) staff       (20)     5878 2023-07-16 11:02:27.000000 easysec-0.0.2/easysec/easysec.py
+drwxr-xr-x   0 guille     (501) staff       (20)        0 2023-07-18 12:19:51.761656 easysec-0.0.2/easysec.egg-info/
+-rw-r--r--   0 guille     (501) staff       (20)      562 2023-07-18 12:19:51.000000 easysec-0.0.2/easysec.egg-info/PKG-INFO
+-rw-r--r--   0 guille     (501) staff       (20)      211 2023-07-18 12:19:51.000000 easysec-0.0.2/easysec.egg-info/SOURCES.txt
+-rw-r--r--   0 guille     (501) staff       (20)        1 2023-07-18 12:19:51.000000 easysec-0.0.2/easysec.egg-info/dependency_links.txt
+-rw-r--r--   0 guille     (501) staff       (20)        7 2023-07-18 12:19:51.000000 easysec-0.0.2/easysec.egg-info/requires.txt
+-rw-r--r--   0 guille     (501) staff       (20)        8 2023-07-18 12:19:51.000000 easysec-0.0.2/easysec.egg-info/top_level.txt
+-rw-r--r--   0 guille     (501) staff       (20)       38 2023-07-18 12:19:51.761981 easysec-0.0.2/setup.cfg
+-rw-r--r--   0 guille     (501) staff       (20)      900 2023-07-18 12:18:52.000000 easysec-0.0.2/setup.py
```

### Comparing `easysec-0.0.1/PKG-INFO` & `easysec-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: easysec
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to import data from SEC.gov.
 Home-page: UNKNOWN
 Author: Guillermo Vizcaíno Román
 Author-email: <guillevzn@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,sec,database,API
```

### Comparing `easysec-0.0.1/README.md` & `easysec-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easysec-0.0.1/easysec/easysec.py` & `easysec-0.0.2/easysec/easysec.py`

 * *Files identical despite different names*

### Comparing `easysec-0.0.1/easysec.egg-info/PKG-INFO` & `easysec-0.0.2/easysec.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: easysec
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to import data from SEC.gov.
 Home-page: UNKNOWN
 Author: Guillermo Vizcaíno Román
 Author-email: <guillevzn@gmail.com>
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,sec,database,API
```

### Comparing `easysec-0.0.1/setup.py` & `easysec-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Python library to import data from SEC.gov.'
 
 # Setting up
 setup(
     name="easysec",
     version=VERSION,
     author="Guillermo Vizcaíno Román",
     author_email="<guillevzn@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['pandas', 'requests', 'json'],
+    install_requires=['pandas'],
     keywords=['python', 'sec', 'database', 'API' ],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

