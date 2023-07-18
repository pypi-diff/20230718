# Comparing `tmp/ykenan_util-0.0.3.tar.gz` & `tmp/ykenan_util-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_util-0.0.3.tar", last modified: Tue Jul 18 04:14:17 2023, max compression
+gzip compressed data, was "ykenan_util-0.0.4.tar", last modified: Tue Jul 18 10:44:18 2023, max compression
```

## Comparing `ykenan_util-0.0.3.tar` & `ykenan_util-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.125547 ykenan_util-0.0.3/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      801 2023-07-18 04:14:17.124547 ykenan_util-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.3/README.md
--rw-rw-rw-   0        0        0      653 2023-07-18 04:13:57.000000 ykenan_util-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 04:14:17.125547 ykenan_util-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.106547 ykenan_util-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.109546 ykenan_util-0.0.3/src/ykenan_util/
--rw-rw-rw-   0        0        0     6559 2023-07-18 04:13:49.000000 ykenan_util-0.0.3/src/ykenan_util/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.3/src/ykenan_util/snowflake.py
-drwxrwxrwx   0        0        0        0 2023-07-18 04:14:17.123546 ykenan_util-0.0.3/src/ykenan_util.egg-info/
--rw-rw-rw-   0        0        0      801 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 04:14:17.000000 ykenan_util-0.0.3/src/ykenan_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 10:44:18.572168 ykenan_util-0.0.4/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      801 2023-07-18 10:44:18.572168 ykenan_util-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.4/README.md
+-rw-rw-rw-   0        0        0      653 2023-07-18 10:43:51.000000 ykenan_util-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:44:18.572168 ykenan_util-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 10:44:18.555153 ykenan_util-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 10:44:18.558153 ykenan_util-0.0.4/src/ykenan_util/
+-rw-rw-rw-   0        0        0     6824 2023-07-18 10:38:57.000000 ykenan_util-0.0.4/src/ykenan_util/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.4/src/ykenan_util/snowflake.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:44:18.571151 ykenan_util-0.0.4/src/ykenan_util.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-07-18 10:44:18.000000 ykenan_util-0.0.4/src/ykenan_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-18 10:44:18.000000 ykenan_util-0.0.4/src/ykenan_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:44:18.000000 ykenan_util-0.0.4/src/ykenan_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-18 10:44:18.000000 ykenan_util-0.0.4/src/ykenan_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 10:44:18.000000 ykenan_util-0.0.4/src/ykenan_util.egg-info/top_level.txt
```

### Comparing `ykenan_util-0.0.3/LICENSE` & `ykenan_util-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.3/PKG-INFO` & `ykenan_util-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_util
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_util-0.0.3/pyproject.toml` & `ykenan_util-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "selenium>=4.10.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_util"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "util", "tool"]
 description = "Tool class"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_util-0.0.3/src/ykenan_util/__init__.py` & `ykenan_util-0.0.4/src/ykenan_util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
+
 import os
 import random
 import re
 import time
 import uuid
 
 from ykenan_log import Logger
@@ -26,98 +27,34 @@
 
 
 class Util:
     """
     初始化文件
     """
 
-    def __init__(self,
-                 driver=None,
-                 wait=None,
-                 is_show: bool = False,
-                 is_refresh: bool = False,
-                 log_file: str = "YKenan_util",
-                 is_form_log_file: bool = True):
+    def __init__(self, log_file: str = "YKenan_util", is_form_log_file: bool = True):
         """
         Initialization creation information, public information
-        :param driver: 引擎
-        :param wait: selenium 等待
-        :param is_show: 是否启动无头模式
-        :param is_refresh: 是否刷新页面
         :param log_file: Path to form a log file
         :param is_form_log_file: Is a log file formed
         """
         self.log = Logger(name="YKenan_util", log_path=log_file, is_form_file=is_form_log_file)
-        self.is_show = is_show
-        self.is_refresh = is_refresh
-        self.driver = driver if driver else self.init_driver()
-        self.wait = wait if wait else WebDriverWait(self.driver, 10)
 
     @staticmethod
     def generate_unique_id() -> str:
         """
         形成数据库中的表
         """
         uuid_: str = str(uuid.uuid1())
         uuid__: str = re.sub("-", "", uuid_)
         id_: int = round(random.Random().random() * 100 % 31)
         unique: str = uuid__ + IdWorker().generator(str(id_))
         # 正常长度不会大于 62, 防止意外, 数据库存储长度为 pow(2,6)
         return unique[1:62]
 
-    def init_driver(self):
-        """
-        浏览器引擎初始化
-        :return: 浏览器引擎
-        """
-        options = FirefoxOptions()
-        # 设置不加载
-        options.page_load_strategy = 'normal'
-        # 是否设置为无头模式
-        if self.is_show:
-            # 设置火狐为 headless 无界面模式
-            options.add_argument("--headless")
-            options.add_argument("--disable-gpu")
-        # 实例化浏览器对象
-        return Firefox(options=options)
-
-    def refresh_handle(self):
-        """
-        窗口处理, 对 selenium 跳转 URL 的处理
-        :return: None
-        """
-        time.sleep(1)
-        # 得到跳转之前的页面
-        original_window = self.driver.current_window_handle
-        # 获取所有的窗口
-        handles = self.driver.window_handles
-        # 切换窗口
-        for handle in handles:
-            if handle != original_window:
-                # 关闭前面的窗口
-                self.driver.close()
-                self.driver.switch_to.window(handle)
-        # 刷新和沉睡是为了防止得到的页面代码不全
-        time.sleep(1)
-        if self.is_refresh:
-            self.driver.refresh()
-
-    def is_element_exist(self, xpath):
-        """
-        判断某个标签是否存在
-        :param xpath: xpath 解析的路径
-        :return: 是否存在 true: 存在
-        """
-        try:
-            self.wait.until(EC.presence_of_element_located((By.XPATH, xpath)))
-            return True
-        except Exception as e:
-            self.log.debug(f"标签不存在: {e.args}")
-            return False
-
     def circle_run(self, title_, callback, refresh, i=0):
         """
         回调函数 主要用户 selenium 访问进行获取相关信息为获取到进行重新获取
         :param title_: 是 callback 函数的参数信息
         :param callback: 回调的第一个函数, 主要的执行函数
         :param refresh: 回调的第二个函数, 当第一个 callback 函数出现错误时候进行一定的刷新循环
         :param i: 循环的次数, 也就是 callback 函数执行错误的次数
@@ -194,7 +131,80 @@
         :param info_list:
         :return:
         """
         line_one: str = ''
         for col in info_list:
             line_one += f"{str(col)}\t"
         return f"{line_one.strip()}\n"
+
+
+class FirefoxSelenium:
+
+    def __init__(self,
+                 driver=None,
+                 wait=None,
+                 is_show: bool = False,
+                 is_refresh: bool = False,
+                 log_file: str = "YKenan_util",
+                 is_form_log_file: bool = True):
+        """
+        Selenium Util
+        :param driver: 引擎
+        :param wait: selenium 等待
+        :param is_show: 是否启动无头模式
+        :param is_refresh: 是否刷新页面
+        """
+        self.log = Logger(name="YKenan_util", log_path=log_file, is_form_file=is_form_log_file)
+        self.is_show = is_show
+        self.is_refresh = is_refresh
+        self.driver = driver if driver else self.init_driver()
+        self.wait = wait if wait else WebDriverWait(self.driver, 10)
+
+    def init_driver(self):
+        """
+        浏览器引擎初始化
+        :return: 浏览器引擎
+        """
+        options = FirefoxOptions()
+        # 设置不加载
+        options.page_load_strategy = 'normal'
+        # 是否设置为无头模式
+        if self.is_show:
+            # 设置火狐为 headless 无界面模式
+            options.add_argument("--headless")
+            options.add_argument("--disable-gpu")
+        # 实例化浏览器对象
+        return Firefox(options=options)
+
+    def refresh_handle(self):
+        """
+        窗口处理, 对 selenium 跳转 URL 的处理
+        :return: None
+        """
+        time.sleep(1)
+        # 得到跳转之前的页面
+        original_window = self.driver.current_window_handle
+        # 获取所有的窗口
+        handles = self.driver.window_handles
+        # 切换窗口
+        for handle in handles:
+            if handle != original_window:
+                # 关闭前面的窗口
+                self.driver.close()
+                self.driver.switch_to.window(handle)
+        # 刷新和沉睡是为了防止得到的页面代码不全
+        time.sleep(1)
+        if self.is_refresh:
+            self.driver.refresh()
+
+    def is_element_exist(self, xpath):
+        """
+        判断某个标签是否存在
+        :param xpath: xpath 解析的路径
+        :return: 是否存在 true: 存在
+        """
+        try:
+            self.wait.until(EC.presence_of_element_located((By.XPATH, xpath)))
+            return True
+        except Exception as e:
+            self.log.debug(f"标签不存在: {e.args}")
+            return False
```

### Comparing `ykenan_util-0.0.3/src/ykenan_util/snowflake.py` & `ykenan_util-0.0.4/src/ykenan_util/snowflake.py`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.3/src/ykenan_util.egg-info/PKG-INFO` & `ykenan_util-0.0.4/src/ykenan_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-util
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

