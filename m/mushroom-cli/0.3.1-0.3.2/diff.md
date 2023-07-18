# Comparing `tmp/mushroom_cli-0.3.1.tar.gz` & `tmp/mushroom_cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mushroom_cli-0.3.1.tar", last modified: Thu Jul 13 03:10:55 2023, max compression
+gzip compressed data, was "mushroom_cli-0.3.2.tar", last modified: Tue Jul 18 03:39:49 2023, max compression
```

## Comparing `mushroom_cli-0.3.1.tar` & `mushroom_cli-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/
--rw-r--r--   0 chentian  (1005) fapon     (1000)     1066 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/LICENSE.txt
--rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/PKG-INFO
--rw-r--r--   0 chentian  (1005) fapon     (1000)     5786 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/README.md
-drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/mushroom/
--rw-r--r--   0 chentian  (1005) fapon     (1000)      173 2023-07-13 03:08:06.000000 mushroom_cli-0.3.1/mushroom/__init__.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)     6439 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_builder.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)       49 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_exceptions.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)      969 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/arg_textwrap.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)     1285 2023-07-13 02:05:40.000000 mushroom_cli-0.3.1/mushroom/args_fetch.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)     1622 2023-07-13 02:16:32.000000 mushroom_cli-0.3.1/mushroom/core.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)     1788 2023-07-13 02:08:59.000000 mushroom_cli-0.3.1/mushroom/func_parser.py
--rw-r--r--   0 chentian  (1005) fapon     (1000)     3524 2023-07-13 03:01:10.000000 mushroom_cli-0.3.1/mushroom/traceback_module.py
-drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-13 03:10:55.773348 mushroom_cli-0.3.1/mushroom_cli.egg-info/
--rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/PKG-INFO
--rw-r--r--   0 chentian  (1005) fapon     (1000)      409 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/SOURCES.txt
--rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/dependency_links.txt
--rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-13 03:06:01.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/not-zip-safe
--rw-r--r--   0 chentian  (1005) fapon     (1000)        9 2023-07-13 03:10:55.000000 mushroom_cli-0.3.1/mushroom_cli.egg-info/top_level.txt
--rw-r--r--   0 chentian  (1005) fapon     (1000)       79 2023-07-13 03:10:55.777349 mushroom_cli-0.3.1/setup.cfg
--rw-r--r--   0 chentian  (1005) fapon     (1000)      339 2023-07-13 03:08:00.000000 mushroom_cli-0.3.1/setup.py
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-18 03:39:49.380506 mushroom_cli-0.3.2/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1066 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/LICENSE.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-18 03:39:49.380506 mushroom_cli-0.3.2/PKG-INFO
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     5786 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/README.md
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-18 03:39:49.368506 mushroom_cli-0.3.2/mushroom/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      173 2023-07-14 08:27:27.000000 mushroom_cli-0.3.2/mushroom/__init__.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     6439 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/mushroom/arg_builder.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)       49 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/mushroom/arg_exceptions.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      969 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/mushroom/arg_textwrap.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1285 2023-07-13 02:05:40.000000 mushroom_cli-0.3.2/mushroom/args_fetch.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1622 2023-07-13 02:16:32.000000 mushroom_cli-0.3.2/mushroom/core.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     1788 2023-07-13 02:08:59.000000 mushroom_cli-0.3.2/mushroom/func_parser.py
+-rw-r--r--   0 chentian  (1005) fapon     (1000)     3692 2023-07-14 08:57:52.000000 mushroom_cli-0.3.2/mushroom/traceback_module.py
+drwxr-xr-x   0 chentian  (1005) fapon     (1000)        0 2023-07-18 03:39:49.376506 mushroom_cli-0.3.2/mushroom_cli.egg-info/
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      250 2023-07-18 03:39:49.000000 mushroom_cli-0.3.2/mushroom_cli.egg-info/PKG-INFO
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      409 2023-07-18 03:39:49.000000 mushroom_cli-0.3.2/mushroom_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-18 03:39:49.000000 mushroom_cli-0.3.2/mushroom_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        1 2023-07-13 03:06:01.000000 mushroom_cli-0.3.2/mushroom_cli.egg-info/not-zip-safe
+-rw-r--r--   0 chentian  (1005) fapon     (1000)        9 2023-07-18 03:39:49.000000 mushroom_cli-0.3.2/mushroom_cli.egg-info/top_level.txt
+-rw-r--r--   0 chentian  (1005) fapon     (1000)       79 2023-07-18 03:39:49.380506 mushroom_cli-0.3.2/setup.cfg
+-rw-r--r--   0 chentian  (1005) fapon     (1000)      339 2023-07-14 08:27:33.000000 mushroom_cli-0.3.2/setup.py
```

### Comparing `mushroom_cli-0.3.1/LICENSE.txt` & `mushroom_cli-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/README.md` & `mushroom_cli-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/arg_builder.py` & `mushroom_cli-0.3.2/mushroom/arg_builder.py`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/arg_textwrap.py` & `mushroom_cli-0.3.2/mushroom/arg_textwrap.py`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/args_fetch.py` & `mushroom_cli-0.3.2/mushroom/args_fetch.py`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/core.py` & `mushroom_cli-0.3.2/mushroom/core.py`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/func_parser.py` & `mushroom_cli-0.3.2/mushroom/func_parser.py`

 * *Files identical despite different names*

### Comparing `mushroom_cli-0.3.1/mushroom/traceback_module.py` & `mushroom_cli-0.3.2/mushroom/traceback_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import traceback
 
 
 USAGE_DOC = """
     输入以下指令执行对应动作:
     ?,h,help : 打印帮助
     print {value_name}: 打印{value_name}的值
     list {global, [local]}: 打印所有变量名(不包含隐藏变量),默认打印local
@@ -11,17 +12,21 @@
     back,b : 跳回上一层的堆栈
     step,s : 往下跳一层堆栈
     q,quit,exit: 退出程序
 """
 
 
 def global_excepthook(ttype,tvalue,ttraceback):
-    print("错误类型：{}".format(ttype))
-    print("错误信息：{}".format(tvalue))
-
+    print("错误类型：\033[91m {} \033[0m".format(ttype))
+    print("错误信息：\033[91m {} \033[0m".format(tvalue))
+    print("=" * 30)
+    traceback_details = traceback.format_exception(ttype,tvalue,ttraceback)
+    traceback_string = "".join(traceback_details)
+    print(traceback_string)
+    print("=" * 30)
     stacks = []
     while ttraceback:
         stacks.append(ttraceback)
         ttraceback = ttraceback.tb_next
     interactive_ter(stacks[::-1])
 
 
@@ -30,15 +35,15 @@
     idx = 0
     stacks_depth = len(stacks)
 
     f = stacks[idx].tb_frame
     global_values = f.f_globals
     local_values = f.f_locals
     while True:
-        cmd = input(">> ").strip()
+        cmd = input("\033[92m >> \033[0m").strip()
         if cmd in ("?", "h", "help"):
             print(USAGE_DOC)
         elif cmd.startswith("print"):
             var_name = cmd.split()[-1]
             print_var_func(var_name, global_values, local_values)
         elif cmd.startswith("list"):
             cmd = cmd.split()
@@ -47,17 +52,17 @@
             elif cmd[-1] == "global":
                 print_all_var(global_values, filter_func=lambda x: not x.startswith("__"))
             else:
                 print("Invaild option: {}".format(" ".join(cmd[1:])))
         elif cmd.startswith("all"):
             cmd = cmd.split()
             if len(cmd) == 1 or cmd[-1] == "local":
-                print_all_var(local_values, filter_func=lambda x: not x.startswith("__"))
+                print_all_var(local_values)
             elif cmd[-1] == "global":
-                print_all_var(global_values, filter_func=lambda x: not x.startswith("__"))
+                print_all_var(global_values)
             else:
                 print("Invaild option: {}".format(" ".join(cmd[1:])))
         elif cmd == "show":
             print(f)
         elif cmd in ("back", "b"):
             if idx >= stacks_depth - 1:
                 print("无法再返回上一层")
```

