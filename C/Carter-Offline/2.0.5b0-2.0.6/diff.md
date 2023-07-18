# Comparing `tmp/Carter-Offline-2.0.5b0.tar.gz` & `tmp/Carter-Offline-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-2.0.5b0.tar", last modified: Mon Jul 17 14:41:48 2023, max compression
+gzip compressed data, was "Carter-Offline-2.0.6.tar", last modified: Tue Jul 18 18:31:44 2023, max compression
```

## Comparing `Carter-Offline-2.0.5b0.tar` & `Carter-Offline-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:41:48.105469 Carter-Offline-2.0.5b0/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:41:48.101708 Carter-Offline-2.0.5b0/CarterOffline/
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:41:48.102242 Carter-Offline-2.0.5b0/CarterOffline/Carter-Offline-SubFolder/
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.5b0/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
--rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.5b0/CarterOffline/Carter-Offline-SubFolder/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)    10343 2023-07-17 14:41:21.000000 Carter-Offline-2.0.5b0/CarterOffline/__init__.py
--rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.5b0/CarterOffline/chat.py
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-09 19:53:02.000000 Carter-Offline-2.0.5b0/CarterOffline/main.py
-drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-17 14:41:48.105142 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/
--rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:41:48.000000 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)      387 2023-07-17 14:41:48.000000 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-17 14:41:48.000000 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-17 14:41:48.000000 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-17 14:41:48.000000 Carter-Offline-2.0.5b0/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.5b0/LICENSE
--rw-r--r--   0 cipher     (501) staff       (20)     2094 2023-07-17 14:41:48.105337 Carter-Offline-2.0.5b0/PKG-INFO
--rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.5b0/README.md
--rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-17 14:41:48.105505 Carter-Offline-2.0.5b0/setup.cfg
--rw-r--r--   0 cipher     (501) staff       (20)     1324 2023-07-17 14:41:37.000000 Carter-Offline-2.0.5b0/setup.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.410636 Carter-Offline-2.0.6/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.400371 Carter-Offline-2.0.6/CarterOffline/
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.401682 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:07:05.000000 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/JanexSub.py
+-rw-r--r--   0 cipher     (501) staff       (20)        0 2023-07-09 16:20:34.000000 Carter-Offline-2.0.6/CarterOffline/Carter-Offline-SubFolder/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)       20 2023-07-18 18:26:41.000000 Carter-Offline-2.0.6/CarterOffline/__init__.py
+-rw-r--r--   0 cipher     (501) staff       (20)      260 2023-07-07 20:07:57.000000 Carter-Offline-2.0.6/CarterOffline/chat.py
+-rw-r--r--   0 cipher     (501) staff       (20)    10343 2023-07-18 18:26:48.000000 Carter-Offline-2.0.6/CarterOffline/main.py
+drwxr-xr-x   0 cipher     (501) staff       (20)        0 2023-07-18 18:31:44.409987 Carter-Offline-2.0.6/Carter_Offline.egg-info/
+-rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)      576 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 cipher     (501) staff       (20)        1 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       22 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 cipher     (501) staff       (20)       14 2023-07-18 18:31:44.000000 Carter-Offline-2.0.6/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 cipher     (501) staff       (20)     2950 2023-07-07 12:33:15.000000 Carter-Offline-2.0.6/LICENSE
+-rw-r--r--   0 cipher     (501) staff       (20)     2092 2023-07-18 18:31:44.410483 Carter-Offline-2.0.6/PKG-INFO
+-rw-r--r--   0 cipher     (501) staff       (20)     1705 2023-07-17 13:27:25.000000 Carter-Offline-2.0.6/README.md
+-rw-r--r--   0 cipher     (501) staff       (20)       38 2023-07-18 18:31:44.410708 Carter-Offline-2.0.6/setup.cfg
+-rw-r--r--   0 cipher     (501) staff       (20)     1322 2023-07-18 18:30:19.000000 Carter-Offline-2.0.6/setup.py
```

### Comparing `Carter-Offline-2.0.5b0/CarterOffline/__init__.py` & `Carter-Offline-2.0.6/CarterOffline/main.py`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.5b0/Carter_Offline.egg-info/PKG-INFO` & `Carter-Offline-2.0.6/Carter_Offline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.5b0
+Version: 2.0.6
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.5b0/LICENSE` & `Carter-Offline-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.5b0/PKG-INFO` & `Carter-Offline-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Carter-Offline
-Version: 2.0.5b0
+Version: 2.0.6
 Home-page: https://github.com/Cipher58
 Download-URL: https://github.com/Cipher58/Carter-Offline/
 Author: Cipher58
 Author-email: cipher58public@gmail.com
 License: Lily 1.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `Carter-Offline-2.0.5b0/README.md` & `Carter-Offline-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Carter-Offline-2.0.5b0/setup.py` & `Carter-Offline-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     # Here is the module name.
     name="Carter-Offline",
 
     # version of the module
-    version="2.0.5b0",
+    version="2.0.6",
 
     # Name of Author
     author="Cipher58",
 
     download_url = 'https://github.com/Cipher58/Carter-Offline/',
 
     # your Email address
```

