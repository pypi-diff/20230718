# Comparing `tmp/nonebot_plugin_capoo-0.1.3.tar.gz` & `tmp/nonebot_plugin_capoo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_capoo-0.1.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_capoo-0.1.4.tar", max compression
```

## Comparing `nonebot_plugin_capoo-0.1.3.tar` & `nonebot_plugin_capoo-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/LICENSE
--rw-r--r--   0        0        0     3934 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/README.md
--rw-r--r--   0        0        0     4524 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/__init__.py
--rw-r--r--   0        0        0      520 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/config.py
--rw-r--r--   0        0        0     2805 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/download.py
--rw-r--r--   0        0        0      469 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/sqlite.py
--rw-r--r--   0        0        0      603 2023-07-13 06:56:28.843663 nonebot_plugin_capoo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3934 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/README.md
+-rw-r--r--   0        0        0     4558 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/__init__.py
+-rw-r--r--   0        0        0      520 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/config.py
+-rw-r--r--   0        0        0     2805 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/download.py
+-rw-r--r--   0        0        0      469 2023-07-18 07:13:29.981538 nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/sqlite.py
+-rw-r--r--   0        0        0      603 2023-07-18 07:13:29.985538 nonebot_plugin_capoo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 nonebot_plugin_capoo-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_capoo-0.1.3/LICENSE` & `nonebot_plugin_capoo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.3/README.md` & `nonebot_plugin_capoo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/__init__.py` & `nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 )
             continue
             
         data = resp.content
         fmd5 = hashlib.md5(data).hexdigest()
 
         capoo_cur_picnum = len( os.listdir(str(capoo_pic2_path)) )
-        if not check_md5(conn, cursor, fmd5, capoo_pic2 + str(capoo_cur_picnum + 1)) :
+        if not check_md5(conn, cursor, fmd5, f"{capoo_pic2}/{capoo_filename.format(index=str(capoo_cur_picnum + 1))}") :
             await add.send(pic + 
                             Message('\n这张已经有了，不能重复添加！')   
                         )
         else:
             capoo_cur_picnum = capoo_cur_picnum + 1
             file_name = capoo_filename.format(index=str(capoo_cur_picnum))
             file_path = capoo_pic2_path / file_name
```

### Comparing `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/config.py` & `nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.3/nonebot_plugin_capoo/download.py` & `nonebot_plugin_capoo-0.1.4/nonebot_plugin_capoo/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_capoo-0.1.3/pyproject.toml` & `nonebot_plugin_capoo-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-capoo"
-version = "0.1.3"
+version = "0.1.4"
 description = "一个发送 capoo 表情包的插件"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_capoo"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-capoo"
 repository = "https://github.com/HuParry/nonebot-plugin-capoo"
```

### Comparing `nonebot_plugin_capoo-0.1.3/PKG-INFO` & `nonebot_plugin_capoo-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-capoo
-Version: 0.1.3
+Version: 0.1.4
 Summary: 一个发送 capoo 表情包的插件
 Home-page: https://github.com/HuParry/nonebot-plugin-capoo
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-capoo Version: 0.1.4 Summary:
 ä¸ä¸ªåé capoo è¡¨æåçæä»¶ Home-page: https://github.com/HuParry/
 nonebot-plugin-capoo License: MIT Author: HuParry Author-email:
 huparry@outlook.com Requires-Python: >=3.8 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: asyncio (>=3.4.3)
```

