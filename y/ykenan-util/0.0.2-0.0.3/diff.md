# Comparing `tmp/ykenan_util-0.0.2.tar.gz` & `tmp/ykenan_util-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_util-0.0.2.tar", last modified: Tue Jul 18 04:05:35 2023, max compression
+gzip compressed data, was "ykenan_util-0.0.3.tar", last modified: Tue Jul 18 04:14:17 2023, max compression
```

## Comparing `ykenan_util-0.0.2.tar` & `ykenan_util-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.636060 ykenan_util-0.0.2/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      801 2023-07-18 04:05:35.635060 ykenan_util-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.2/README.md
--rw-rw-rw-   0        0        0      653 2023-07-18 04:01:11.000000 ykenan_util-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 04:05:35.636060 ykenan_util-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.622060 ykenan_util-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.626061 ykenan_util-0.0.2/src/ykenan_util/
--rw-rw-rw-   0        0        0     6543 2023-07-18 04:05:06.000000 ykenan_util-0.0.2/src/ykenan_util/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.2/src/ykenan_util/snowflake.py
-drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.634060 ykenan_util-0.0.2/src/ykenan_util.egg-info/
--rw-rw-rw-   0        0        0      801 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.125547 ykenan_util-0.0.3/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      801 2023-07-18 04:14:17.124547 ykenan_util-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.3/README.md
+-rw-rw-rw-   0        0        0      653 2023-07-18 04:13:57.000000 ykenan_util-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 04:14:17.125547 ykenan_util-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.106547 ykenan_util-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.109546 ykenan_util-0.0.3/src/ykenan_util/
+-rw-rw-rw-   0        0        0     6559 2023-07-18 04:13:49.000000 ykenan_util-0.0.3/src/ykenan_util/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.3/src/ykenan_util/snowflake.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.123546 ykenan_util-0.0.3/src/ykenan_util.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/top_level.txt
```

### Comparing `ykenan_util-0.0.2/LICENSE` & `ykenan_util-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.2/PKG-INFO` & `ykenan_util-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_util-0.0.2/pyproject.toml` & `ykenan_util-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "selenium>=4.10.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_util"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "util", "tool"]
 description = "Tool class"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_util-0.0.2/src/ykenan_util/__init__.py` & `ykenan_util-0.0.3/src/ykenan_util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,32 +29,32 @@
     """
     初始化文件
     """
 
     def __init__(self,
                  driver=None,
                  wait=None,
-                 is_show=False,
-                 is_refresh=False,
+                 is_show: bool = False,
+                 is_refresh: bool = False,
                  log_file: str = "YKenan_util",
                  is_form_log_file: bool = True):
         """
         Initialization creation information, public information
         :param driver: 引擎
         :param wait: selenium 等待
         :param is_show: 是否启动无头模式
         :param is_refresh: 是否刷新页面
         :param log_file: Path to form a log file
         :param is_form_log_file: Is a log file formed
         """
         self.log = Logger(name="YKenan_util", log_path=log_file, is_form_file=is_form_log_file)
-        self.driver = driver if driver else self.init_driver()
-        self.wait = wait if wait else WebDriverWait(self.driver, 10)
         self.is_show = is_show
         self.is_refresh = is_refresh
+        self.driver = driver if driver else self.init_driver()
+        self.wait = wait if wait else WebDriverWait(self.driver, 10)
 
     @staticmethod
     def generate_unique_id() -> str:
         """
         形成数据库中的表
         """
         uuid_: str = str(uuid.uuid1())
```

### Comparing `ykenan_util-0.0.2/src/ykenan_util/snowflake.py` & `ykenan_util-0.0.3/src/ykenan_util/snowflake.py`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.2/src/ykenan_util.egg-info/PKG-INFO` & `ykenan_util-0.0.3/src/ykenan_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

