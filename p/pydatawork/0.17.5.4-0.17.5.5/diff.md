# Comparing `tmp/pydatawork-0.17.5.4.tar.gz` & `tmp/pydatawork-0.17.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.17.5.4.tar", last modified: Sat Jul  8 15:04:29 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.17.5.5.tar", last modified: Tue Jul 18 09:23:21 2023, max compression
```

## Comparing `pydatawork-0.17.5.4.tar` & `pydatawork-0.17.5.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.4/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52293 2023-07-08 15:02:17.000000 pydatawork-0.17.5.4/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-08 15:04:29.000000 pydatawork-0.17.5.4/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-08 15:04:22.000000 pydatawork-0.17.5.4/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    16977 2023-07-08 15:03:51.000000 pydatawork-0.17.5.5/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    22240 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)    52890 2023-07-18 09:19:37.000000 pydatawork-0.17.5.5/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-07-18 09:23:21.000000 pydatawork-0.17.5.5/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      796 2023-07-18 09:20:01.000000 pydatawork-0.17.5.5/setup.py
```

### Comparing `pydatawork-0.17.5.4/PKG-INFO` & `pydatawork-0.17.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.4
+Version: 0.17.5.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.5.4/README.md` & `pydatawork-0.17.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pydatawork-0.17.5.4/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.17.5.5/pydatawork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.17.5.4
+Version: 0.17.5.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         pydatawork功能建议收集表：
```

### Comparing `pydatawork-0.17.5.4/pydatawork.py` & `pydatawork-0.17.5.5/pydatawork.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,61 +81,77 @@
         # print("\t\t3.data analysis")
         # print("\t\t4.查找")
         # print("\t\t5.工作台")
         # print("\t\t6.知识库")
         # print("\t\t7.数据库")
         # print("\t\t8.联系与帮助")
         # print("\t\t0.退出")
-        print("1.basic functions", end="")
-        print("\t2.data processing", end="")
-        print("\t3.data analysis")
-        print("4.查找", end="")
-        print("\t5.工作台", end="")
-        print("\t6.知识库", end="")
-        print("\t7.数据库", end="")
-        print("\t8.联系与帮助")
+        # print("1.basic functions", end="")
+        # print("\t2.data processing", end="")
+        # print("\t3.data analysis")
+        # print("4.查找", end="")
+        # print("\t5.工作台", end="")
+        # print("\t6.知识库", end="")
+        # print("\t7.数据库", end="")
+        # print("\t8.联系与帮助")
+        # print("0.退出")
+        # print("--------------------------------------------------------------------")
+        print("1.basic functions")
+        print("2.data processing")
+        print("3.data analysis")
+        print("4.查找")
+        print("5.工作台")
+        print("6.知识库")
+        print("7.数据库")
+        print("8.联系与帮助")
         print("0.退出")
         print("--------------------------------------------------------------------")
 
     def basic_functions():
         while True:
-            print("""basic functions:
-            file_split
-            get_current_folder_name
-            get_file_name
-            copy_files, copy_all_files, copy_files_by_keyword
-            move_files, move_all_files, move_files_by_keyword
-            renamer_folder_numeric_serialize
-            """)
+            print("basic functions:")
+            print("file_split")
+            print("get_current_folder_name")
+            print("get_file_name")
+            print("copy_files")
+            print("copy_all_files")
+            print("copy_files_by_keyword")
+            print("move_files")
+            print("move_all_files")
+            print("move_files_by_keyword")
+            print("rename_by_re") 
+            print("rename_by_insert_keyword()")
+            print("renamer_folder_numeric_serialize")
+
             answer = input("输入 n/N 退出，按 回车 继续...\n") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
 
     def data_processing():
         while True:
-            print("""data processing:
-            obsidian_move_md_or_canvas_linked_images
-            obsidian_bookmarks_merge_and_deduplicate
-            get_weibo
-            """)
+            print("data processing:")
+            print("obsidian_move_md_or_canvas_linked_images")
+            print("obsidian_bookmarks_merge_and_deduplicate")
+            print("get_weibo")
+
             answer = input("输入 n/N 退出，按 回车 继续...\n") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
 
 
     def data_analysis():
         while True:
-            print("""data analysis:
-            game_number_guessing
-            get_BMI
-            """)
+            print("data analysis:")
+            print("game_number_guessing")
+            print("get_BMI")
+
             answer = input("输入 n/N 退出，按 回车 继续...\n") # @知识卡片 输入时没有指定input的值的类型，所以，当输入的值为空值时，不会报错。如果指定了int，输入空值就会直接报错，无法进入下一步判断。
             if answer == "n" or answer == "N": # 仅当输入n/N直接退出。要继续，直接回车就行
                 exit()
             else:
                 break # @知识卡片 在这里要继续使用，本质上就是退出当前的循环，所以，直接break
```

### Comparing `pydatawork-0.17.5.4/setup.py` & `pydatawork-0.17.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.17.5.4',
+    version='0.17.5.5',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

