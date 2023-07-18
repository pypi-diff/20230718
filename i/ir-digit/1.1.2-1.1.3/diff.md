# Comparing `tmp/ir_digit-1.1.2.tar.gz` & `tmp/ir_digit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ir_digit-1.1.2.tar", last modified: Tue Jul 18 11:58:00 2023, max compression
+gzip compressed data, was "ir_digit-1.1.3.tar", last modified: Tue Jul 18 11:59:33 2023, max compression
```

## Comparing `ir_digit-1.1.2.tar` & `ir_digit-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:00.180497 ir_digit-1.1.2/
--rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-1.1.2/LICENSE
--rw-rw-rw-   0        0        0       32 2023-03-28 12:17:48.000000 ir_digit-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      516 2023-07-18 11:58:00.178490 ir_digit-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:00.155491 ir_digit-1.1.2/digit/
--rw-rw-rw-   0        0        0      244 2023-06-30 08:41:10.000000 ir_digit-1.1.2/digit/__init__.py
--rw-rw-rw-   0        0        0     3536 2023-07-07 06:05:06.000000 ir_digit-1.1.2/digit/base_data.py
--rw-rw-rw-   0        0        0     1786 2023-06-01 06:11:19.000000 ir_digit-1.1.2/digit/child_base_data.py
--rw-rw-rw-   0        0        0     3206 2023-07-07 06:26:49.000000 ir_digit-1.1.2/digit/core.py
--rw-rw-rw-   0        0        0     7223 2023-07-13 12:35:06.000000 ir_digit-1.1.2/digit/data.py
--rw-rw-rw-   0        0        0     4985 2023-07-13 12:22:34.000000 ir_digit-1.1.2/digit/download.py
--rw-rw-rw-   0        0        0      252 2023-06-01 09:12:08.000000 ir_digit-1.1.2/digit/info.json
--rw-rw-rw-   0        0        0     2143 2023-07-18 11:56:16.000000 ir_digit-1.1.2/digit/info.py
--rw-rw-rw-   0        0        0     4899 2023-07-13 12:22:10.000000 ir_digit-1.1.2/digit/query.py
--rw-rw-rw-   0        0        0     2937 2023-07-13 07:20:47.000000 ir_digit-1.1.2/digit/scripts.py
--rw-rw-rw-   0        0        0     2315 2023-07-13 09:53:29.000000 ir_digit-1.1.2/digit/setting.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:58:00.175584 ir_digit-1.1.2/ir_digit.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 11:57:59.000000 ir_digit-1.1.2/ir_digit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 11:58:00.180497 ir_digit-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-07-18 11:57:27.000000 ir_digit-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:59:33.107030 ir_digit-1.1.3/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 06:34:05.000000 ir_digit-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0       32 2023-03-28 12:17:48.000000 ir_digit-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      516 2023-07-18 11:59:33.106047 ir_digit-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-27 07:07:49.000000 ir_digit-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 11:59:33.083027 ir_digit-1.1.3/digit/
+-rw-rw-rw-   0        0        0      244 2023-06-30 08:41:10.000000 ir_digit-1.1.3/digit/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-07-07 06:05:06.000000 ir_digit-1.1.3/digit/base_data.py
+-rw-rw-rw-   0        0        0     1786 2023-06-01 06:11:19.000000 ir_digit-1.1.3/digit/child_base_data.py
+-rw-rw-rw-   0        0        0     3206 2023-07-07 06:26:49.000000 ir_digit-1.1.3/digit/core.py
+-rw-rw-rw-   0        0        0     7223 2023-07-13 12:35:06.000000 ir_digit-1.1.3/digit/data.py
+-rw-rw-rw-   0        0        0     4985 2023-07-13 12:22:34.000000 ir_digit-1.1.3/digit/download.py
+-rw-rw-rw-   0        0        0      252 2023-06-01 09:12:08.000000 ir_digit-1.1.3/digit/info.json
+-rw-rw-rw-   0        0        0     2143 2023-07-18 11:56:16.000000 ir_digit-1.1.3/digit/info.py
+-rw-rw-rw-   0        0        0     4899 2023-07-13 12:22:10.000000 ir_digit-1.1.3/digit/query.py
+-rw-rw-rw-   0        0        0     2937 2023-07-13 07:20:47.000000 ir_digit-1.1.3/digit/scripts.py
+-rw-rw-rw-   0        0        0     2315 2023-07-13 09:53:29.000000 ir_digit-1.1.3/digit/setting.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:59:33.103048 ir_digit-1.1.3/ir_digit.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 11:59:32.000000 ir_digit-1.1.3/ir_digit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:59:33.107030 ir_digit-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      989 2023-07-18 11:59:22.000000 ir_digit-1.1.3/setup.py
```

### Comparing `ir_digit-1.1.2/LICENSE` & `ir_digit-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/PKG-INFO` & `ir_digit-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ir_digit
-Version: 1.1.2
+Version: 1.1.3
 Summary: digit package
 Home-page: https://master--ir-digit-redocs.netlify.app/
 Author: FKLiu
 Author-email: fkliu001@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ir_digit-1.1.2/digit/base_data.py` & `ir_digit-1.1.3/digit/base_data.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/child_base_data.py` & `ir_digit-1.1.3/digit/child_base_data.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/core.py` & `ir_digit-1.1.3/digit/core.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/data.py` & `ir_digit-1.1.3/digit/data.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/download.py` & `ir_digit-1.1.3/digit/download.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/info.py` & `ir_digit-1.1.3/digit/info.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/query.py` & `ir_digit-1.1.3/digit/query.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/scripts.py` & `ir_digit-1.1.3/digit/scripts.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/digit/setting.py` & `ir_digit-1.1.3/digit/setting.py`

 * *Files identical despite different names*

### Comparing `ir_digit-1.1.2/ir_digit.egg-info/PKG-INFO` & `ir_digit-1.1.3/ir_digit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ir-digit
-Version: 1.1.2
+Version: 1.1.3
 Summary: digit package
 Home-page: https://master--ir-digit-redocs.netlify.app/
 Author: FKLiu
 Author-email: fkliu001@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ir_digit-1.1.2/setup.py` & `ir_digit-1.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import setuptools
 
 
 setuptools.setup(
     name="ir_digit",
-    version="1.1.2",
+    version="1.1.3",
     author="FKLiu",
     author_email="fkliu001@outlook.com",
     description="digit package",
     long_description="digit package 与 digit web 配套使用，下载其digit web中的数据资源并在本地运行",
     long_description_content_type="text",
     url="https://master--ir-digit-redocs.netlify.app/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires = [
         "gitpython",
         "numpy",
         "pandas",
         "matplotlib",
         "seaborn",
-        "jieba"
+        "jieba",
+        "requests"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

