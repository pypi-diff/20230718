# Comparing `tmp/tools_wzy-0.0.2.tar.gz` & `tmp/tools_wzy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools_wzy-0.0.2.tar", last modified: Tue Jul 18 02:17:53 2023, max compression
+gzip compressed data, was "tools_wzy-0.0.3.tar", last modified: Tue Jul 18 02:21:59 2023, max compression
```

## Comparing `tools_wzy-0.0.2.tar` & `tools_wzy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 02:17:53.006486 tools_wzy-0.0.2/
--rw-rw-rw-   0        0        0      329 2023-07-18 02:17:53.006486 tools_wzy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-18 02:17:53.006486 tools_wzy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-07-18 02:17:46.000000 tools_wzy-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:17:53.001503 tools_wzy-0.0.2/tools_wzy/
--rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.2/tools_wzy/__init__.py
--rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.2/tools_wzy/node_coverage.py
--rw-rw-rw-   0        0        0     5153 2023-07-18 01:18:44.000000 tools_wzy-0.0.2/tools_wzy/yolo_need.py
-drwxrwxrwx   0        0        0        0 2023-07-18 02:17:53.005489 tools_wzy-0.0.2/tools_wzy.egg-info/
--rw-rw-rw-   0        0        0      329 2023-07-18 02:17:52.000000 tools_wzy-0.0.2/tools_wzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-18 02:17:52.000000 tools_wzy-0.0.2/tools_wzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 02:17:52.000000 tools_wzy-0.0.2/tools_wzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-18 02:17:52.000000 tools_wzy-0.0.2/tools_wzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 02:17:52.000000 tools_wzy-0.0.2/tools_wzy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:21:59.983336 tools_wzy-0.0.3/
+-rw-rw-rw-   0        0        0      308 2023-07-18 02:21:59.983336 tools_wzy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:21:59.983336 tools_wzy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1030 2023-07-18 02:21:52.000000 tools_wzy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:21:59.979350 tools_wzy-0.0.3/tools_wzy/
+-rw-rw-rw-   0        0        0        0 2023-07-13 09:07:59.000000 tools_wzy-0.0.3/tools_wzy/__init__.py
+-rw-rw-rw-   0        0        0     9507 2023-07-17 06:15:57.000000 tools_wzy-0.0.3/tools_wzy/node_coverage.py
+-rw-rw-rw-   0        0        0     5153 2023-07-18 01:18:44.000000 tools_wzy-0.0.3/tools_wzy/yolo_need.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:21:59.982339 tools_wzy-0.0.3/tools_wzy.egg-info/
+-rw-rw-rw-   0        0        0      308 2023-07-18 02:21:59.000000 tools_wzy-0.0.3/tools_wzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-07-18 02:21:59.000000 tools_wzy-0.0.3/tools_wzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:21:59.000000 tools_wzy-0.0.3/tools_wzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 02:21:59.000000 tools_wzy-0.0.3/tools_wzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 02:21:59.000000 tools_wzy-0.0.3/tools_wzy.egg-info/top_level.txt
```

### Comparing `tools_wzy-0.0.2/setup.py` & `tools_wzy-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # Created Time:  2023-07-18
 #############################################
 
 from setuptools import setup, find_packages            #这个包没有的可以pip一下
 
 setup(
     name = "tools_wzy",      #这里是pip项目发布的名称
-    version = "0.0.2",  #版本号，数值大的会优先被pip
+    version = "0.0.3",  #版本号，数值大的会优先被pip
     keywords = ["pip", "tools_wzy"],
     description = "Some python tools for work from Zhiyuan",
-    long_description = "Some python tools for work from Zhiyuan, improve the FastICA",
+    long_description = "Some python tools for work from Zhiyuan",
     license = "MIT Licence",
 
     url = "https://gitee.com/Zhiyuan_WZY",     #项目相关文件地址，一般是github
     author = "Zhiyuan Wang",
     author_email = "2073834696@qq.com",
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = ["pandas", "json", "datetime", "xml"]          #这个项目需要的第三方库
+    install_requires = ["pandas", "datetime"]          #这个项目需要的第三方库
 )
```

### Comparing `tools_wzy-0.0.2/tools_wzy/node_coverage.py` & `tools_wzy-0.0.3/tools_wzy/node_coverage.py`

 * *Files identical despite different names*

### Comparing `tools_wzy-0.0.2/tools_wzy/yolo_need.py` & `tools_wzy-0.0.3/tools_wzy/yolo_need.py`

 * *Files identical despite different names*

