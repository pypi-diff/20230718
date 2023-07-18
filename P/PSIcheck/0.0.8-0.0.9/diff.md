# Comparing `tmp/PSIcheck-0.0.8.tar.gz` & `tmp/PSIcheck-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSIcheck-0.0.8.tar", last modified: Tue Jul 18 06:50:22 2023, max compression
+gzip compressed data, was "PSIcheck-0.0.9.tar", last modified: Tue Jul 18 07:00:30 2023, max compression
```

## Comparing `PSIcheck-0.0.8.tar` & `PSIcheck-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:50:22.167302 PSIcheck-0.0.8/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:50:22.160529 PSIcheck-0.0.8/PKG-INFO
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:50:21.823526 PSIcheck-0.0.8/PSIcheck/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.8/PSIcheck/__init__.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)      753 2023-07-18 06:49:50.000000 PSIcheck-0.0.8/PSIcheck/get_parser.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.8/PSIcheck/screen_for_magPro.py
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:50:22.112929 PSIcheck-0.0.8/PSIcheck.egg-info/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/PKG-INFO
--rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/entry_points.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/requires.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 06:50:21.000000 PSIcheck-0.0.8/PSIcheck.egg-info/top_level.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 06:50:22.168314 PSIcheck-0.0.8/setup.cfg
--rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 06:49:56.000000 PSIcheck-0.0.8/setup.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:30.004214 PSIcheck-0.0.9/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 07:00:29.994243 PSIcheck-0.0.9/PKG-INFO
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:29.640404 PSIcheck-0.0.9/PSIcheck/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.9/PSIcheck/__init__.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      772 2023-07-18 07:00:14.000000 PSIcheck-0.0.9/PSIcheck/get_parser.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.9/PSIcheck/screen_for_magPro.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 07:00:29.939827 PSIcheck-0.0.9/PSIcheck.egg-info/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/entry_points.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/requires.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 07:00:29.000000 PSIcheck-0.0.9/PSIcheck.egg-info/top_level.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 07:00:30.006127 PSIcheck-0.0.9/setup.cfg
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 07:00:07.000000 PSIcheck-0.0.9/setup.py
```

### Comparing `PSIcheck-0.0.8/PSIcheck/get_parser.py` & `PSIcheck-0.0.9/PSIcheck/get_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 def get_parser():
     import argparse
     CBOLD = '\33[1m'
     CEND = '\33[0m'
     CRED = '\33[31m'
     CGREEN = '\33[32m'
-    CYELLOW = '\33[33m'
     parser = argparse.ArgumentParser(
              prog="PSIcheck", 
+             formatter_class=argparse.RawTextHelpFormatter,
              epilog=f"""
-
-{CBOLD}Usage{CEND}
-
+{CBOLD}Usage：{CEND}
 
     {CRED}$ {CGREEN}PSIcheck{CEND} PsiResultPath
 
-
 Runjia Ji, 2023
-"""
-            )
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.8', help='show PSIcheck version number and exit')
+""")
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.9', help='show PSIcheck version number and exit')
     parser.add_argument('PsiResultPath', type=str, help='directory stores PSI-Blast results')
     parser.add_argument('-gbk','--GenbankFilesPath', type=str, help='directory stores Genbank files')
 
     args = parser.parse_args()
     return args
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PSIcheck-0.0.8/PSIcheck/screen_for_magPro.py` & `PSIcheck-0.0.9/PSIcheck/screen_for_magPro.py`

 * *Files identical despite different names*

### Comparing `PSIcheck-0.0.8/setup.py` & `PSIcheck-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PSIcheck',
-    version='0.0.8',
+    version='0.0.9',
     description="check PSI-Blast result",
     author='Runjia Ji',
     author_email='jirunjia@gmail.com',
     # py_modules=["magcluster", 'args', 'capture_args', 'maga', 'magm', 'magsc', 'main'],
     # package_dir={'': 'src'},
     packages=find_packages(),
     classifiers=[
```

