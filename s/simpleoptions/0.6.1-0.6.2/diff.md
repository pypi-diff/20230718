# Comparing `tmp/simpleoptions-0.6.1.tar.gz` & `tmp/simpleoptions-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleoptions-0.6.1.tar", last modified: Tue Jul 18 15:38:43 2023, max compression
+gzip compressed data, was "simpleoptions-0.6.2.tar", last modified: Tue Jul 18 16:25:31 2023, max compression
```

## Comparing `simpleoptions-0.6.1.tar` & `simpleoptions-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.285380 simpleoptions-0.6.1/
--rw-rw-rw-   0        0        0     1090 2019-07-25 00:43:58.000000 simpleoptions-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-18 15:38:43.285380 simpleoptions-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4403 2023-03-30 12:13:28.000000 simpleoptions-0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 15:38:43.286380 simpleoptions-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-07-18 15:35:49.000000 simpleoptions-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.250871 simpleoptions-0.6.1/simpleoptions/
--rw-rw-rw-   0        0        0      217 2023-03-30 12:12:05.000000 simpleoptions-0.6.1/simpleoptions/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-06-21 14:46:48.000000 simpleoptions-0.6.1/simpleoptions/environment.py
--rw-rw-rw-   0        0        0     1619 2023-04-14 17:42:51.000000 simpleoptions-0.6.1/simpleoptions/option.py
--rw-rw-rw-   0        0        0    22676 2023-07-18 14:34:18.000000 simpleoptions-0.6.1/simpleoptions/options_agent.py
--rw-rw-rw-   0        0        0     2069 2023-04-18 12:35:11.000000 simpleoptions-0.6.1/simpleoptions/primitive_option.py
-drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.280380 simpleoptions-0.6.1/simpleoptions.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 15:38:43.000000 simpleoptions-0.6.1/simpleoptions.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 15:38:43.284381 simpleoptions-0.6.1/test/
--rw-rw-rw-   0        0        0     1327 2023-04-14 17:42:51.000000 simpleoptions-0.6.1/test/test_discounted_sum.py
--rw-rw-rw-   0        0        0     5007 2023-04-14 17:44:04.000000 simpleoptions-0.6.1/test/test_intra_option_update.py
--rw-rw-rw-   0        0        0     8620 2023-04-15 00:31:22.000000 simpleoptions-0.6.1/test/test_macro_q_update.py
--rw-rw-rw-   0        0        0    29384 2023-04-19 17:28:07.000000 simpleoptions-0.6.1/test/test_run_agent.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:25:31.366756 simpleoptions-0.6.2/
+-rw-rw-rw-   0        0        0     1090 2019-07-25 00:43:58.000000 simpleoptions-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-18 16:25:31.366756 simpleoptions-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4403 2023-03-30 12:13:28.000000 simpleoptions-0.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 16:25:31.367757 simpleoptions-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-07-18 16:25:03.000000 simpleoptions-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:25:31.329261 simpleoptions-0.6.2/simpleoptions/
+-rw-rw-rw-   0        0        0      217 2023-03-30 12:12:05.000000 simpleoptions-0.6.2/simpleoptions/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-06-21 14:46:48.000000 simpleoptions-0.6.2/simpleoptions/environment.py
+-rw-rw-rw-   0        0        0     1619 2023-04-14 17:42:51.000000 simpleoptions-0.6.2/simpleoptions/option.py
+-rw-rw-rw-   0        0        0    22676 2023-07-18 14:34:18.000000 simpleoptions-0.6.2/simpleoptions/options_agent.py
+-rw-rw-rw-   0        0        0     2069 2023-04-18 12:35:11.000000 simpleoptions-0.6.2/simpleoptions/primitive_option.py
+drwxrwxrwx   0        0        0        0 2023-07-18 16:25:31.361756 simpleoptions-0.6.2/simpleoptions.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-18 16:25:31.000000 simpleoptions-0.6.2/simpleoptions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-18 16:25:31.000000 simpleoptions-0.6.2/simpleoptions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 16:25:31.000000 simpleoptions-0.6.2/simpleoptions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 16:25:31.000000 simpleoptions-0.6.2/simpleoptions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 16:25:31.000000 simpleoptions-0.6.2/simpleoptions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 16:25:31.365757 simpleoptions-0.6.2/test/
+-rw-rw-rw-   0        0        0     1327 2023-04-14 17:42:51.000000 simpleoptions-0.6.2/test/test_discounted_sum.py
+-rw-rw-rw-   0        0        0     5007 2023-04-14 17:44:04.000000 simpleoptions-0.6.2/test/test_intra_option_update.py
+-rw-rw-rw-   0        0        0     8620 2023-04-15 00:31:22.000000 simpleoptions-0.6.2/test/test_macro_q_update.py
+-rw-rw-rw-   0        0        0    29384 2023-04-19 17:28:07.000000 simpleoptions-0.6.2/test/test_run_agent.py
```

### Comparing `simpleoptions-0.6.1/LICENSE` & `simpleoptions-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/PKG-INFO` & `simpleoptions-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleoptions
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package which provides a simple framework for working with Options in Reinforcement Learning.
 Home-page: https://github.com/Ueva/BaRL-SimpleOptions
 Author: Joshua Evans
 Author-email: jbe25@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleoptions-0.6.1/README.md` & `simpleoptions-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/setup.py` & `simpleoptions-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="simpleoptions",
-    version="0.6.1",
+    version="0.6.2",
     author="Joshua Evans",
     author_email="jbe25@bath.ac.uk",
     description="A package which provides a simple framework for working with Options in Reinforcement Learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ueva/BaRL-SimpleOptions",
     # packages=setuptools.find_packages(exclude=("example", "test")),
```

### Comparing `simpleoptions-0.6.1/simpleoptions/environment.py` & `simpleoptions-0.6.2/simpleoptions/environment.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/simpleoptions/option.py` & `simpleoptions-0.6.2/simpleoptions/option.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/simpleoptions/options_agent.py` & `simpleoptions-0.6.2/simpleoptions/options_agent.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/simpleoptions/primitive_option.py` & `simpleoptions-0.6.2/simpleoptions/primitive_option.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/simpleoptions.egg-info/PKG-INFO` & `simpleoptions-0.6.2/simpleoptions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleoptions
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package which provides a simple framework for working with Options in Reinforcement Learning.
 Home-page: https://github.com/Ueva/BaRL-SimpleOptions
 Author: Joshua Evans
 Author-email: jbe25@bath.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleoptions-0.6.1/test/test_discounted_sum.py` & `simpleoptions-0.6.2/test/test_discounted_sum.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/test/test_intra_option_update.py` & `simpleoptions-0.6.2/test/test_intra_option_update.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/test/test_macro_q_update.py` & `simpleoptions-0.6.2/test/test_macro_q_update.py`

 * *Files identical despite different names*

### Comparing `simpleoptions-0.6.1/test/test_run_agent.py` & `simpleoptions-0.6.2/test/test_run_agent.py`

 * *Files identical despite different names*

