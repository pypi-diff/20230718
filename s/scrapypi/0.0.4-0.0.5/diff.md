# Comparing `tmp/scrapypi-0.0.4.tar.gz` & `tmp/scrapypi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapypi-0.0.4.tar", last modified: Tue Jul 18 12:18:56 2023, max compression
+gzip compressed data, was "scrapypi-0.0.5.tar", last modified: Tue Jul 18 13:06:01 2023, max compression
```

## Comparing `scrapypi-0.0.4.tar` & `scrapypi-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 12:18:56.223688 scrapypi-0.0.4/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      354 2023-07-18 12:18:01.000000 scrapypi-0.0.4/CHANGELOG.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-07-17 13:44:26.000000 scrapypi-0.0.4/LICENCE.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.4/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2311 2023-07-18 12:18:56.219685 scrapypi-0.0.4/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1380 2023-07-18 12:16:23.000000 scrapypi-0.0.4/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 12:18:56.215682 scrapypi-0.0.4/scrapypi/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-18 12:13:53.000000 scrapypi-0.0.4/scrapypi/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3907 2023-07-18 12:10:22.000000 scrapypi-0.0.4/scrapypi/handler.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2268 2023-07-18 12:10:55.000000 scrapypi-0.0.4/scrapypi/scrapypi.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 12:18:56.219685 scrapypi-0.0.4/scrapypi/stubs/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-17 12:33:53.000000 scrapypi-0.0.4/scrapypi/stubs/__init__.pyi
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      230 2023-07-17 15:49:11.000000 scrapypi-0.0.4/scrapypi/stubs/scrapypi.pyi
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 12:18:56.219685 scrapypi-0.0.4/scrapypi.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2311 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      367 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       24 2023-07-18 12:18:55.000000 scrapypi-0.0.4/scrapypi.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-18 12:18:56.223688 scrapypi-0.0.4/setup.cfg
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2023 2023-07-18 12:17:00.000000 scrapypi-0.0.4/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 13:06:01.085674 scrapypi-0.0.5/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      427 2023-07-18 13:04:06.000000 scrapypi-0.0.5/CHANGELOG.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-07-17 13:44:26.000000 scrapypi-0.0.5/LICENCE.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       30 2023-07-16 19:52:28.000000 scrapypi-0.0.5/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2384 2023-07-18 13:06:01.085674 scrapypi-0.0.5/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1380 2023-07-18 12:16:23.000000 scrapypi-0.0.5/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 13:06:01.081680 scrapypi-0.0.5/scrapypi/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-18 13:05:11.000000 scrapypi-0.0.5/scrapypi/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3907 2023-07-18 12:10:22.000000 scrapypi-0.0.5/scrapypi/handler.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2304 2023-07-18 13:02:35.000000 scrapypi-0.0.5/scrapypi/scrapypi.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 13:06:01.085674 scrapypi-0.0.5/scrapypi/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       23 2023-07-17 12:33:53.000000 scrapypi-0.0.5/scrapypi/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      230 2023-07-17 15:49:11.000000 scrapypi-0.0.5/scrapypi/stubs/scrapypi.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 13:06:01.085674 scrapypi-0.0.5/scrapypi.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2384 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      367 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        5 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       24 2023-07-18 13:06:00.000000 scrapypi-0.0.5/scrapypi.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-18 13:06:01.085674 scrapypi-0.0.5/setup.cfg
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2023 2023-07-18 13:05:00.000000 scrapypi-0.0.5/setup.py
```

### Comparing `scrapypi-0.0.4/LICENCE.txt` & `scrapypi-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.4/PKG-INFO` & `scrapypi-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -77,7 +77,11 @@
 > [ ADDED ]  
 > [+] Package download statistics  
 > [+] More Package info
 
 > **0.0.4** -- [ 18 JULY 2023 ]  
 > [ FIXED ]  
 > [+] - windows support
+
+> **0.0.5** -- [ 18 JULY 2023 ]  
+> [ FIXED ]  
+> [+] - temp file furge
```

### Comparing `scrapypi-0.0.4/README.md` & `scrapypi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.4/scrapypi/handler.py` & `scrapypi-0.0.5/scrapypi/handler.py`

 * *Files identical despite different names*

### Comparing `scrapypi-0.0.4/scrapypi/scrapypi.py` & `scrapypi-0.0.5/scrapypi/scrapypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,25 +24,27 @@
         with open(filename, 'r', errors='ignore') as file:
             file = file.readlines()
             
             line = [line for line in file if f"{module_name} " in line and "title" not in line]
             line = line[0].strip()
             version = line.split()[-1]
 
-            clean()
+        clean()
         return module_name, version
     except:
         ...
 
 
 class stats:
     def __init__(self, name: str = None, url: str = None):
         dataset['with_mirrors'] = scan_stats(name, url, mode='a')
+        clean()
         dataset['without_mirrors'] = scan_stats(name, url, mode='s')
-
+        clean()
+        
     def get_total(self):
         return get_total()
     
     def dataset(self):
         return dataset
```

### Comparing `scrapypi-0.0.4/scrapypi.egg-info/PKG-INFO` & `scrapypi-0.0.5/scrapypi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapypi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get PyPi Package information.
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: GNU LGPLv3
 Keywords: pypi,information,package,module,stats,info,scrape
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -77,7 +77,11 @@
 > [ ADDED ]  
 > [+] Package download statistics  
 > [+] More Package info
 
 > **0.0.4** -- [ 18 JULY 2023 ]  
 > [ FIXED ]  
 > [+] - windows support
+
+> **0.0.5** -- [ 18 JULY 2023 ]  
+> [ FIXED ]  
+> [+] - temp file furge
```

### Comparing `scrapypi-0.0.4/setup.py` & `scrapypi-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Get PyPi Package information.'
 KEYWORDS = ['pypi', 'information', 'package', 'module', 'stats', 'info', 'scrape']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

