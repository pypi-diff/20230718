# Comparing `tmp/notion-dump-kernel-0.2.2.tar.gz` & `tmp/notion-dump-kernel-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-dump-kernel-0.2.2.tar", last modified: Fri Feb 10 04:13:09 2023, max compression
+gzip compressed data, was "notion-dump-kernel-0.2.3.tar", last modified: Tue Jul 18 02:56:53 2023, max compression
```

## Comparing `notion-dump-kernel-0.2.2.tar` & `notion-dump-kernel-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.819756 notion-dump-kernel-0.2.2/
--rw-rw-rw-   0        0        0     1087 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       84 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.767751 notion-dump-kernel-0.2.2/NotionDump/
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.781750 notion-dump-kernel-0.2.2/NotionDump/Dump/
--rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/Dump/__init__.py
--rw-rw-rw-   0        0        0     1716 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/Dump/block.py
--rw-rw-rw-   0        0        0     4033 2023-02-10 03:57:23.000000 notion-dump-kernel-0.2.2/NotionDump/Dump/database.py
--rw-rw-rw-   0        0        0     3734 2023-01-29 12:24:34.000000 notion-dump-kernel-0.2.2/NotionDump/Dump/dump.py
--rw-rw-rw-   0        0        0     2893 2023-01-29 13:11:01.000000 notion-dump-kernel-0.2.2/NotionDump/Dump/page.py
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.786749 notion-dump-kernel-0.2.2/NotionDump/Notion/
--rw-rw-rw-   0        0        0     2848 2023-01-30 05:16:48.000000 notion-dump-kernel-0.2.2/NotionDump/Notion/Buffer.py
--rw-rw-rw-   0        0        0    15647 2023-02-10 03:58:45.000000 notion-dump-kernel-0.2.2/NotionDump/Notion/Notion.py
--rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/Notion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.793750 notion-dump-kernel-0.2.2/NotionDump/Parser/
--rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/Parser/__init__.py
--rw-rw-rw-   0        0        0    49022 2023-02-07 04:07:05.000000 notion-dump-kernel-0.2.2/NotionDump/Parser/base_parser.py
--rw-rw-rw-   0        0        0    14198 2023-02-07 04:05:59.000000 notion-dump-kernel-0.2.2/NotionDump/Parser/block_parser.py
--rw-rw-rw-   0        0        0    11154 2023-02-02 12:23:47.000000 notion-dump-kernel-0.2.2/NotionDump/Parser/database_parser.py
--rw-rw-rw-   0        0        0     8308 2023-01-30 05:42:41.000000 notion-dump-kernel-0.2.2/NotionDump/Parser/mix_parser.py
--rw-rw-rw-   0        0        0     3604 2023-01-30 06:00:03.000000 notion-dump-kernel-0.2.2/NotionDump/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.802750 notion-dump-kernel-0.2.2/NotionDump/utils/
--rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/utils/__init__.py
--rw-rw-rw-   0        0        0    10133 2023-02-10 03:59:12.000000 notion-dump-kernel-0.2.2/NotionDump/utils/common_op.py
--rw-rw-rw-   0        0        0     3951 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/utils/content_format.py
--rw-rw-rw-   0        0        0      515 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/NotionDump/utils/internal_var.py
--rw-rw-rw-   0        0        0      982 2023-02-10 04:13:09.819756 notion-dump-kernel-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     5500 2023-01-30 04:58:37.000000 notion-dump-kernel-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.807750 notion-dump-kernel-0.2.2/examples/
--rw-rw-rw-   0        0        0     2019 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/examples/block_dump.py
--rw-rw-rw-   0        0        0     2783 2023-02-01 12:35:41.000000 notion-dump-kernel-0.2.2/examples/db_dump.py
--rw-rw-rw-   0        0        0     1703 2023-01-30 06:16:05.000000 notion-dump-kernel-0.2.2/examples/page_dump.py
-drwxrwxrwx   0        0        0        0 2023-02-10 04:13:09.818755 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/
--rw-rw-rw-   0        0        0      982 2023-02-10 04:13:09.000000 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2023-02-10 04:13:09.000000 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 04:13:09.000000 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-02-10 04:13:09.000000 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-10 04:13:09.000000 notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       35 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-10 04:13:09.819756 notion-dump-kernel-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1932 2023-02-10 04:12:03.000000 notion-dump-kernel-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.746733 notion-dump-kernel-0.2.3/
+-rw-rw-rw-   0        0        0     1087 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       84 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.732734 notion-dump-kernel-0.2.3/NotionDump/
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.734734 notion-dump-kernel-0.2.3/NotionDump/Dump/
+-rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/Dump/__init__.py
+-rw-rw-rw-   0        0        0     1716 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/Dump/block.py
+-rw-rw-rw-   0        0        0     4033 2023-02-10 03:57:23.000000 notion-dump-kernel-0.2.3/NotionDump/Dump/database.py
+-rw-rw-rw-   0        0        0     3734 2023-01-29 12:24:34.000000 notion-dump-kernel-0.2.3/NotionDump/Dump/dump.py
+-rw-rw-rw-   0        0        0     2893 2023-01-29 13:11:01.000000 notion-dump-kernel-0.2.3/NotionDump/Dump/page.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.736734 notion-dump-kernel-0.2.3/NotionDump/Notion/
+-rw-rw-rw-   0        0        0     2848 2023-01-30 05:16:48.000000 notion-dump-kernel-0.2.3/NotionDump/Notion/Buffer.py
+-rw-rw-rw-   0        0        0    15647 2023-02-10 03:58:45.000000 notion-dump-kernel-0.2.3/NotionDump/Notion/Notion.py
+-rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/Notion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.738735 notion-dump-kernel-0.2.3/NotionDump/Parser/
+-rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/Parser/__init__.py
+-rw-rw-rw-   0        0        0    49022 2023-02-07 04:07:05.000000 notion-dump-kernel-0.2.3/NotionDump/Parser/base_parser.py
+-rw-rw-rw-   0        0        0    14198 2023-02-07 04:05:59.000000 notion-dump-kernel-0.2.3/NotionDump/Parser/block_parser.py
+-rw-rw-rw-   0        0        0    11154 2023-02-02 12:23:47.000000 notion-dump-kernel-0.2.3/NotionDump/Parser/database_parser.py
+-rw-rw-rw-   0        0        0     8308 2023-01-30 05:42:41.000000 notion-dump-kernel-0.2.3/NotionDump/Parser/mix_parser.py
+-rw-rw-rw-   0        0        0     4153 2023-07-18 02:56:43.000000 notion-dump-kernel-0.2.3/NotionDump/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.740734 notion-dump-kernel-0.2.3/NotionDump/utils/
+-rw-rw-rw-   0        0        0        0 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/utils/__init__.py
+-rw-rw-rw-   0        0        0     9838 2023-02-22 14:17:48.000000 notion-dump-kernel-0.2.3/NotionDump/utils/common_op.py
+-rw-rw-rw-   0        0        0     3951 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/utils/content_format.py
+-rw-rw-rw-   0        0        0      515 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/NotionDump/utils/internal_var.py
+-rw-rw-rw-   0        0        0      982 2023-07-18 02:56:53.746733 notion-dump-kernel-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5500 2023-01-30 04:58:37.000000 notion-dump-kernel-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.742735 notion-dump-kernel-0.2.3/examples/
+-rw-rw-rw-   0        0        0     2019 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/examples/block_dump.py
+-rw-rw-rw-   0        0        0     2783 2023-02-01 12:35:41.000000 notion-dump-kernel-0.2.3/examples/db_dump.py
+-rw-rw-rw-   0        0        0     1703 2023-01-30 06:16:05.000000 notion-dump-kernel-0.2.3/examples/page_dump.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:56:53.745734 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/
+-rw-rw-rw-   0        0        0      982 2023-07-18 02:56:53.000000 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2023-07-18 02:56:53.000000 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:56:53.000000 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-18 02:56:53.000000 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 02:56:53.000000 notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       35 2022-12-12 07:18:07.000000 notion-dump-kernel-0.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:56:53.746733 notion-dump-kernel-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1932 2023-07-18 02:55:21.000000 notion-dump-kernel-0.2.3/setup.py
```

### Comparing `notion-dump-kernel-0.2.2/LICENSE` & `notion-dump-kernel-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Dump/block.py` & `notion-dump-kernel-0.2.3/NotionDump/Dump/block.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Dump/database.py` & `notion-dump-kernel-0.2.3/NotionDump/Dump/database.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Dump/dump.py` & `notion-dump-kernel-0.2.3/NotionDump/Dump/dump.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Dump/page.py` & `notion-dump-kernel-0.2.3/NotionDump/Dump/page.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Notion/Buffer.py` & `notion-dump-kernel-0.2.3/NotionDump/Notion/Buffer.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Notion/Notion.py` & `notion-dump-kernel-0.2.3/NotionDump/Notion/Notion.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Parser/base_parser.py` & `notion-dump-kernel-0.2.3/NotionDump/Parser/base_parser.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Parser/block_parser.py` & `notion-dump-kernel-0.2.3/NotionDump/Parser/block_parser.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Parser/database_parser.py` & `notion-dump-kernel-0.2.3/NotionDump/Parser/database_parser.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/Parser/mix_parser.py` & `notion-dump-kernel-0.2.3/NotionDump/Parser/mix_parser.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/__init__.py` & `notion-dump-kernel-0.2.3/NotionDump/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # author: delta1037
 # Date: 2022/01/08
 # mail:geniusrabbit@qq.com
 
 __author__ = "delta1037 <geniusrabbit@qq.com>"
-__version__ = "0.2.1"
+__version__ = "0.2.3"
+
+from NotionDump import utils
 
 # 临时存放文件夹
 TMP_DIR = "./.tmp/"
 
 # Markdown的分割条语法
 MD_DIVIDER = "------"
 MD_BOOL_TRUE = "✓"
@@ -19,14 +21,35 @@
 
 # 日志输出模式
 DUMP_MODE_DEBUG = 0
 DUMP_MODE_DEFAULT = 1
 DUMP_MODE_SILENT = 2
 DUMP_MODE = DUMP_MODE_DEFAULT
 
+
+# 日志控制器
+class NotionBackupLogger:
+    def __init__(self):
+        self.prefix = "[NotionDump] "
+        self.log_fd = open("notion-export-kernel-debug.log", "a+", encoding='utf-8')
+
+    def log_debug(self, log_str):
+        self.log_info(log_str)
+
+        # debug内容写入到文件
+        self.log_fd.write(str(log_str) + "\n")
+        self.log_fd.flush()
+
+    def log_info(self, log_str):
+        print(self.prefix, end='')
+        print(log_str)
+
+
+LOGGER = NotionBackupLogger()
+
 # 导出的类型
 DUMP_TYPE_BLOCK = 1
 DUMP_TYPE_PAGE = 2
 DUMP_TYPE_DB_TABLE = 4
 
 # 解析的类型：分为Markdown和纯文本
 PARSER_TYPE_MD = 0
```

### Comparing `notion-dump-kernel-0.2.2/NotionDump/utils/common_op.py` & `notion-dump-kernel-0.2.3/NotionDump/utils/common_op.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,22 +206,12 @@
     if last_type == "table_row" and now_type == "table_row":
         return False
     return True
 
 
 def debug_log(debug_str, level=NotionDump.DUMP_MODE_DEBUG):
     if NotionDump.DUMP_MODE == NotionDump.DUMP_MODE_DEBUG:
-        # debug 模式啥都打印出来
-        print("[NotionDump] ", end='')
-        print(debug_str)
-
-        # debug内容写入到文件
-        log_fd = open("notion-export-kernel-debug.log", "a+", encoding='utf-8')
-        log_fd.write(str(debug_str) + "\n")
-        log_fd.flush()
-        log_fd.close()
-
+        NotionDump.LOGGER.log_debug(debug_str)
     elif NotionDump.DUMP_MODE == NotionDump.DUMP_MODE_DEFAULT and level == NotionDump.DUMP_MODE_DEFAULT:
         # 默认模式 对 level进行过滤
-        print("[NotionDump] ", end='')
-        print(debug_str)
+        NotionDump.LOGGER.log_info(debug_str)
     # 静默模式什么都不输出
```

### Comparing `notion-dump-kernel-0.2.2/NotionDump/utils/content_format.py` & `notion-dump-kernel-0.2.3/NotionDump/utils/content_format.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/NotionDump/utils/internal_var.py` & `notion-dump-kernel-0.2.3/NotionDump/utils/internal_var.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/PKG-INFO` & `notion-dump-kernel-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-dump-kernel
-Version: 0.2.2
+Version: 0.2.3
 Summary: Freely available tools for export Notion page and database.
 Home-page: https://github.com/delta1037/notion-export-kernel
 Author: delta1037
 Author-email: geniusrabbit@qq.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/delta1037/notion-export-kernel/blob/main/README.md
 Project-URL: Source, https://github.com/delta1037/notion-export-kernel
```

### Comparing `notion-dump-kernel-0.2.2/README.md` & `notion-dump-kernel-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/examples/block_dump.py` & `notion-dump-kernel-0.2.3/examples/block_dump.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/examples/db_dump.py` & `notion-dump-kernel-0.2.3/examples/db_dump.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/examples/page_dump.py` & `notion-dump-kernel-0.2.3/examples/page_dump.py`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/PKG-INFO` & `notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-dump-kernel
-Version: 0.2.2
+Version: 0.2.3
 Summary: Freely available tools for export Notion page and database.
 Home-page: https://github.com/delta1037/notion-export-kernel
 Author: delta1037
 Author-email: geniusrabbit@qq.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/delta1037/notion-export-kernel/blob/main/README.md
 Project-URL: Source, https://github.com/delta1037/notion-export-kernel
```

### Comparing `notion-dump-kernel-0.2.2/notion_dump_kernel.egg-info/SOURCES.txt` & `notion-dump-kernel-0.2.3/notion_dump_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `notion-dump-kernel-0.2.2/setup.py` & `notion-dump-kernel-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 REQUIRES = ["notion-client>=0.8.0"]
 
 # with open("README_En.md", encoding="utf-8") as handle:
 #    readme_rst = handle.read()
 
 setup(
     name="notion-dump-kernel",
-    version="0.2.2",
+    version="0.2.3",
     author="delta1037",
     author_email="geniusrabbit@qq.com",
     url="https://github.com/delta1037/notion-export-kernel",
     description="Freely available tools for export Notion page and database.",
     project_urls={
         "Documentation": "https://github.com/delta1037/notion-export-kernel/blob/main/README.md",
         "Source": "https://github.com/delta1037/notion-export-kernel",
```

