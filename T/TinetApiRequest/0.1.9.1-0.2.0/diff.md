# Comparing `tmp/TinetApiRequest-0.1.9.1.tar.gz` & `tmp/TinetApiRequest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TinetApiRequest-0.1.9.1.tar", last modified: Tue Jul 18 07:10:42 2023, max compression
+gzip compressed data, was "dist\TinetApiRequest-0.2.0.tar", last modified: Tue Jul 18 07:14:52 2023, max compression
```

## Comparing `TinetApiRequest-0.1.9.1.tar` & `TinetApiRequest-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/
--rw-rw-rw-   0        0        0      274 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-0.1.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/
--rw-rw-rw-   0        0        0      274 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/TinetApiRequest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-07-18 07:04:56.000000 TinetApiRequest-0.1.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:10:42.000000 TinetApiRequest-0.1.9.1/tinet/
--rw-rw-rw-   0        0        0    21950 2023-07-18 07:04:01.000000 TinetApiRequest-0.1.9.1/tinet/APIRequest.py
--rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-0.1.9.1/tinet/ApiConfig.py
--rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/LogUtil.py
--rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/RequestUtil.py
--rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.1.9.1/tinet/SignUtil.py
--rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.1.9.1/tinet/YamlUtil.py
--rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.1.9.1/tinet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/
+-rw-rw-rw-   0        0        0      272 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-07-14 02:58:39.000000 TinetApiRequest-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/TinetApiRequest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      653 2023-07-18 07:14:44.000000 TinetApiRequest-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:14:52.000000 TinetApiRequest-0.2.0/tinet/
+-rw-rw-rw-   0        0        0    21950 2023-07-18 07:04:01.000000 TinetApiRequest-0.2.0/tinet/APIRequest.py
+-rw-rw-rw-   0        0        0     6911 2023-07-17 07:53:30.000000 TinetApiRequest-0.2.0/tinet/ApiConfig.py
+-rw-rw-rw-   0        0        0     1082 2023-07-11 08:50:04.000000 TinetApiRequest-0.2.0/tinet/LogUtil.py
+-rw-rw-rw-   0        0        0     2658 2023-07-11 08:50:04.000000 TinetApiRequest-0.2.0/tinet/RequestUtil.py
+-rw-rw-rw-   0        0        0     2958 2023-07-11 08:50:04.000000 TinetApiRequest-0.2.0/tinet/SignUtil.py
+-rw-rw-rw-   0        0        0     7314 2023-06-13 08:06:01.000000 TinetApiRequest-0.2.0/tinet/YamlUtil.py
+-rw-rw-rw-   0        0        0      164 2023-06-09 08:49:02.000000 TinetApiRequest-0.2.0/tinet/__init__.py
```

### Comparing `TinetApiRequest-0.1.9.1/README.md` & `TinetApiRequest-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/setup.py` & `TinetApiRequest-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 BASE_DIR = Path(__file__).parent
 with open(Path(BASE_DIR, "requirements.txt"), "r") as file:
     required_packages = [ln.strip() for ln in file.readlines()]
 
 # Define our package
 setup(
     name="TinetApiRequest",
-    version="0.1.9.1",
+    version="0.2.0",
     description="天润接口测试库",
     author="天润-测试",
     author_email="zhupeng@ti-net.com.cn",
     url="https://www.ti-net.com.cn/",
     python_requires=">=3.7",
     packages=find_namespace_packages(),
     install_requires=[required_packages],
```

### Comparing `TinetApiRequest-0.1.9.1/tinet/APIRequest.py` & `TinetApiRequest-0.2.0/tinet/APIRequest.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/tinet/ApiConfig.py` & `TinetApiRequest-0.2.0/tinet/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/tinet/LogUtil.py` & `TinetApiRequest-0.2.0/tinet/LogUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/tinet/RequestUtil.py` & `TinetApiRequest-0.2.0/tinet/RequestUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/tinet/SignUtil.py` & `TinetApiRequest-0.2.0/tinet/SignUtil.py`

 * *Files identical despite different names*

### Comparing `TinetApiRequest-0.1.9.1/tinet/YamlUtil.py` & `TinetApiRequest-0.2.0/tinet/YamlUtil.py`

 * *Files identical despite different names*

