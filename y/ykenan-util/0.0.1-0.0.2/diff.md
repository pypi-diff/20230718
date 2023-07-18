# Comparing `tmp/ykenan_util-0.0.1.tar.gz` & `tmp/ykenan_util-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_util-0.0.1.tar", last modified: Tue Jul 18 03:42:44 2023, max compression
+gzip compressed data, was "ykenan_util-0.0.2.tar", last modified: Tue Jul 18 04:05:35 2023, max compression
```

## Comparing `ykenan_util-0.0.1.tar` & `ykenan_util-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:44.970586 ykenan_util-0.0.1/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      801 2023-07-18 03:42:44.970586 ykenan_util-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.1/README.md
--rw-rw-rw-   0        0        0      653 2023-07-18 03:35:40.000000 ykenan_util-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 03:42:44.970586 ykenan_util-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:44.956543 ykenan_util-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:44.960515 ykenan_util-0.0.1/src/ykenan_util/
--rw-rw-rw-   0        0        0     5125 2023-07-18 03:42:23.000000 ykenan_util-0.0.1/src/ykenan_util/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.1/src/ykenan_util/snowflake.py
-drwxrwxrwx   0        0        0        0 2023-07-18 03:42:44.969544 ykenan_util-0.0.1/src/ykenan_util.egg-info/
--rw-rw-rw-   0        0        0      801 2023-07-18 03:42:44.000000 ykenan_util-0.0.1/src/ykenan_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-18 03:42:44.000000 ykenan_util-0.0.1/src/ykenan_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 03:42:44.000000 ykenan_util-0.0.1/src/ykenan_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-18 03:42:44.000000 ykenan_util-0.0.1/src/ykenan_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 03:42:44.000000 ykenan_util-0.0.1/src/ykenan_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.636060 ykenan_util-0.0.2/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_util-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_util-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      801 2023-07-18 04:05:35.635060 ykenan_util-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-18 03:24:02.000000 ykenan_util-0.0.2/README.md
+-rw-rw-rw-   0        0        0      653 2023-07-18 04:01:11.000000 ykenan_util-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2023-07-18 03:35:39.000000 ykenan_util-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 04:05:35.636060 ykenan_util-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.622060 ykenan_util-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.626061 ykenan_util-0.0.2/src/ykenan_util/
+-rw-rw-rw-   0        0        0     6543 2023-07-18 04:05:06.000000 ykenan_util-0.0.2/src/ykenan_util/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-07-18 03:21:52.000000 ykenan_util-0.0.2/src/ykenan_util/snowflake.py
+drwxrwxrwx   0        0        0        0 2023-07-18 04:05:35.634060 ykenan_util-0.0.2/src/ykenan_util.egg-info/
+-rw-rw-rw-   0        0        0      801 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 04:05:35.000000 ykenan_util-0.0.2/src/ykenan_util.egg-info/top_level.txt
```

### Comparing `ykenan_util-0.0.1/LICENSE` & `ykenan_util-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.1/PKG-INFO` & `ykenan_util-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_util
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_util-0.0.1/pyproject.toml` & `ykenan_util-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "selenium>=4.10.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_util"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "util", "tool"]
 description = "Tool class"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_util-0.0.1/src/ykenan_util/__init__.py` & `ykenan_util-0.0.2/src/ykenan_util/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 import uuid
 
 from ykenan_log import Logger
 
 from selenium.webdriver import Firefox
 from selenium.webdriver import FirefoxOptions
 from selenium.webdriver.common.by import By
+from selenium.webdriver.support.wait import WebDriverWait
 # noinspection PyPep8Naming
 from selenium.webdriver.support import expected_conditions as EC
 
 from ykenan_util.snowflake import IdWorker
 
 '''
  * @Author       : YKenan
  * @Description  : Util class
 '''
 
+SPECIAL_SYMBOLS: str = "[ |)>=,%;&#:'<(/\\\\+-]+"
+
 
 class Util:
     """
     初始化文件
     """
 
     def __init__(self,
@@ -40,16 +43,16 @@
         :param wait: selenium 等待
         :param is_show: 是否启动无头模式
         :param is_refresh: 是否刷新页面
         :param log_file: Path to form a log file
         :param is_form_log_file: Is a log file formed
         """
         self.log = Logger(name="YKenan_util", log_path=log_file, is_form_file=is_form_log_file)
-        self.wait = wait
-        self.driver = driver
+        self.driver = driver if driver else self.init_driver()
+        self.wait = wait if wait else WebDriverWait(self.driver, 10)
         self.is_show = is_show
         self.is_refresh = is_refresh
 
     @staticmethod
     def generate_unique_id() -> str:
         """
         形成数据库中的表
@@ -146,7 +149,52 @@
         while True:
             if info_split[i] is None or info_split[i] == "":
                 break
             info_list.append(info_split[i])
             i += 1
         self.log.info(f">>>>>>>>> end 执行 {command} 命令 >>>>>>>>>")
         return info_list
+
+    @staticmethod
+    def format_str_abbr(str_name: str):
+        str_split = re.split(SPECIAL_SYMBOLS, str_name)
+        str_sample = ""
+        if len(str_split) > 1:
+            for t_s in str_split:
+                if t_s is not None and t_s != "":
+                    str_sample += t_s[0].capitalize()
+        else:
+            str_sample = str_name
+        return str_sample
+
+    @staticmethod
+    def get_number(str_: str) -> int:
+        """
+        冲字符串中获取数量
+        :param str_:
+        :return:
+        """
+        re_compile = re.compile("[0-9]+")
+        page_number = re.findall(re_compile, str_)[0]
+        return int(page_number)
+
+    @staticmethod
+    def remove_r_n(str_: str, repl: str = " | ") -> str:
+        """
+        移除 \r \n
+        :param str_:
+        :param repl:
+        :return:
+        """
+        return re.sub("[\r\n]+", repl, str_)
+
+    @staticmethod
+    def single_line(info_list: list):
+        """
+        生成添加行的信息
+        :param info_list:
+        :return:
+        """
+        line_one: str = ''
+        for col in info_list:
+            line_one += f"{str(col)}\t"
+        return f"{line_one.strip()}\n"
```

### Comparing `ykenan_util-0.0.1/src/ykenan_util/snowflake.py` & `ykenan_util-0.0.2/src/ykenan_util/snowflake.py`

 * *Files identical despite different names*

### Comparing `ykenan_util-0.0.1/src/ykenan_util.egg-info/PKG-INFO` & `ykenan_util-0.0.2/src/ykenan_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-util
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tool class
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_util
 Keywords: ykenan,util,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

