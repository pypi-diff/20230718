# Comparing `tmp/PSIcheck-0.0.6.tar.gz` & `tmp/PSIcheck-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSIcheck-0.0.6.tar", last modified: Tue Jul 18 06:43:59 2023, max compression
+gzip compressed data, was "PSIcheck-0.0.7.tar", last modified: Tue Jul 18 06:48:34 2023, max compression
```

## Comparing `PSIcheck-0.0.6.tar` & `PSIcheck-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:43:59.472897 PSIcheck-0.0.6/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:43:59.462848 PSIcheck-0.0.6/PKG-INFO
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:43:59.179431 PSIcheck-0.0.6/PSIcheck/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.6/PSIcheck/__init__.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)      844 2023-07-18 06:43:12.000000 PSIcheck-0.0.6/PSIcheck/get_parser.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.6/PSIcheck/screen_for_magPro.py
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:43:59.408578 PSIcheck-0.0.6/PSIcheck.egg-info/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:43:58.000000 PSIcheck-0.0.6/PSIcheck.egg-info/PKG-INFO
--rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 06:43:59.000000 PSIcheck-0.0.6/PSIcheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 06:43:58.000000 PSIcheck-0.0.6/PSIcheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 06:43:58.000000 PSIcheck-0.0.6/PSIcheck.egg-info/entry_points.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 06:43:58.000000 PSIcheck-0.0.6/PSIcheck.egg-info/requires.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 06:43:58.000000 PSIcheck-0.0.6/PSIcheck.egg-info/top_level.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 06:43:59.474909 PSIcheck-0.0.6/setup.cfg
--rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 06:43:31.000000 PSIcheck-0.0.6/setup.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:48:34.583774 PSIcheck-0.0.7/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:48:34.577005 PSIcheck-0.0.7/PKG-INFO
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:48:34.235029 PSIcheck-0.0.7/PSIcheck/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.7/PSIcheck/__init__.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      747 2023-07-18 06:47:58.000000 PSIcheck-0.0.7/PSIcheck/get_parser.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.7/PSIcheck/screen_for_magPro.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:48:34.522266 PSIcheck-0.0.7/PSIcheck.egg-info/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:48:33.000000 PSIcheck-0.0.7/PSIcheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 06:48:34.000000 PSIcheck-0.0.7/PSIcheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 06:48:33.000000 PSIcheck-0.0.7/PSIcheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 06:48:33.000000 PSIcheck-0.0.7/PSIcheck.egg-info/entry_points.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 06:48:33.000000 PSIcheck-0.0.7/PSIcheck.egg-info/requires.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 06:48:33.000000 PSIcheck-0.0.7/PSIcheck.egg-info/top_level.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 06:48:34.586778 PSIcheck-0.0.7/setup.cfg
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 06:48:16.000000 PSIcheck-0.0.7/setup.py
```

### Comparing `PSIcheck-0.0.6/PSIcheck/get_parser.py` & `PSIcheck-0.0.7/PSIcheck/get_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     CEND = '\33[0m'
     CRED = '\33[31m'
     CGREEN = '\33[32m'
     CYELLOW = '\33[33m'
     parser = argparse.ArgumentParser(
              prog="PSIcheck", 
              epilog=f"""
-                {CBOLD}Usage{CEND}
-                -----------------
-                    {CRED}$ {CGREEN}PSIcheck{CEND} PsiResultPath
+{CBOLD}Usage{CEND}
 
-                Runjia Ji, 2023
-                """
+    {CRED}$ {CGREEN}PSIcheck{CEND} PsiResultPath
+
+Runjia Ji, 2023
+"""
             )
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.6', help='show PSIcheck version number and exit')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.7', help='show PSIcheck version number and exit')
     parser.add_argument('PsiResultPath', type=str, help='directory stores PSI-Blast results')
     parser.add_argument('-gbk','--GenbankFilesPath', type=str, help='directory stores Genbank files')
 
     args = parser.parse_args()
     return args
```

### Comparing `PSIcheck-0.0.6/PSIcheck/screen_for_magPro.py` & `PSIcheck-0.0.7/PSIcheck/screen_for_magPro.py`

 * *Files identical despite different names*

### Comparing `PSIcheck-0.0.6/setup.py` & `PSIcheck-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PSIcheck',
-    version='0.0.6',
+    version='0.0.7',
     description="check PSI-Blast result",
     author='Runjia Ji',
     author_email='jirunjia@gmail.com',
     # py_modules=["magcluster", 'args', 'capture_args', 'maga', 'magm', 'magsc', 'main'],
     # package_dir={'': 'src'},
     packages=find_packages(),
     classifiers=[
```

