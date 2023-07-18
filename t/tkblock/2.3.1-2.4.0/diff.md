# Comparing `tmp/tkblock-2.3.1.tar.gz` & `tmp/tkblock-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-2.3.1.tar", last modified: Wed Jul 12 15:33:03 2023, max compression
+gzip compressed data, was "tkblock-2.4.0.tar", last modified: Tue Jul 18 14:40:26 2023, max compression
```

## Comparing `tkblock-2.3.1.tar` & `tkblock-2.4.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.161235 tkblock-2.3.1/
--rw-rw-rw-   0        0        0     1077 2023-06-02 17:09:00.000000 tkblock-2.3.1/LICENSE
--rw-rw-rw-   0        0        0    15304 2023-07-12 15:33:03.160269 tkblock-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    14580 2023-06-02 11:06:20.000000 tkblock-2.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 15:33:03.162233 tkblock-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-07-12 15:32:18.000000 tkblock-2.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.146208 tkblock-2.3.1/tkblock/
--rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/__init__.py
--rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_framework.py
--rw-rw-rw-   0        0        0    41449 2023-06-18 14:16:06.000000 tkblock-2.3.1/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_util.py
--rw-rw-rw-   0        0        0     3750 2023-06-02 18:21:40.000000 tkblock-2.3.1/tkblock/block_waiting_screen.py
--rw-rw-rw-   0        0        0     1574 2023-06-18 14:21:05.000000 tkblock-2.3.1/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.3.1/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.3.1/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.158240 tkblock-2.3.1/tkblock.egg-info/
--rw-rw-rw-   0        0        0    15304 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:40:26.717123 tkblock-2.4.0/
+-rw-rw-rw-   0        0        0     1077 2023-06-02 17:09:00.000000 tkblock-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0    15304 2023-07-18 14:40:26.717123 tkblock-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14580 2023-06-02 11:06:20.000000 tkblock-2.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 14:40:26.717123 tkblock-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-07-18 14:40:09.000000 tkblock-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:40:26.701501 tkblock-2.4.0/tkblock/
+-rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.4.0/tkblock/__init__.py
+-rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.4.0/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.4.0/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0    42799 2023-07-18 14:36:31.000000 tkblock-2.4.0/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.4.0/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     4843 2023-07-18 14:30:17.000000 tkblock-2.4.0/tkblock/block_waiting_screen.py
+-rw-rw-rw-   0        0        0     1574 2023-06-18 14:21:05.000000 tkblock-2.4.0/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.4.0/tkblock/layout.py
+-rw-rw-rw-   0        0        0     7822 2023-07-13 14:38:20.000000 tkblock-2.4.0/tkblock/logger.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.4.0/tkblock/scrollbar.py
+-rw-rw-rw-   0        0        0     1098 2023-07-18 14:37:58.000000 tkblock-2.4.0/tkblock/thread_stop.py
+-rw-rw-rw-   0        0        0     1438 2023-07-18 14:30:55.000000 tkblock-2.4.0/tkblock/traceback.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:40:26.717123 tkblock-2.4.0/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    15304 2023-07-18 14:40:26.000000 tkblock-2.4.0/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-07-18 14:40:26.000000 tkblock-2.4.0/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:40:26.000000 tkblock-2.4.0/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-18 14:40:26.000000 tkblock-2.4.0/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-2.3.1/LICENSE` & `tkblock-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/PKG-INFO` & `tkblock-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.3.1
+Version: 2.4.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tkblock-2.3.1/README.md` & `tkblock-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/setup.py` & `tkblock-2.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="2.3.1",
+    version="2.4.0",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-2.3.1/tkblock/__init__.py` & `tkblock-2.4.0/tkblock/__init__.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/tkblock/block_framebase.py` & `tkblock-2.4.0/tkblock/block_framebase.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/tkblock/block_framework.py` & `tkblock-2.4.0/tkblock/block_framework.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/tkblock/block_service.py` & `tkblock-2.4.0/tkblock/block_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 # -*- coding: utf-8 -*-
 # kuri_pome
 """BlockService
 
 このクラスを使用することでblock指定でwidgetを配置することができる。
 """
 import threading
+import traceback
 from typing import Any
 from functools import wraps, partial
 
 from .canvas import ResizingCanvas
 from .block_framebase import *
 from .layout import Layout
+from .traceback import TracebackCatch
+from .thread_stop import StoppableThread
 from .scrollbar import Scrollbar
 from .block_framework import BlockFramework
 from .block_waiting_screen import BlockWaitingScreen
 
 
 def wait_processe(frame=None):
     """処理の完了を待つ。その間、待機描画処理を行う。
@@ -30,29 +33,41 @@
         def wait_processe(*args, **kwargs):
             root = BlockService.root if frame is None else frame
             result = [None]
             is_force_finish = [False]
             wait_screen = BlockWaitingScreen(root, is_force_finish)
 
             def _execute(result, wait_screen, func, *args, **kwargs):
-                result[0] = func(*args, **kwargs)
-                wait_screen.end_thread()
-
-            # # スレッドを実行して、関数を実行
-            wait_thread = threading.Thread(target=wait_screen.start_thread)
-            # wait_thread.daemon = False
+                try:
+                    result[0] = func(*args, **kwargs)
+                    wait_screen.end_thread()
+                except:
+                    # run_threadが何かしらのエラーが発生したとき
+                    for t in threading.enumerate():
+                        if t.name == "wait_thread":
+                            # TracebackCatchのloggerはエラーログファイル出力をするので、そちらに出力
+                            TracebackCatch.logger.error(traceback.format_exc())
+                            # 待機画面を終了させるためのフラグ更新
+                            wait_screen.is_spin = False
+
+            # 待機画面のスレッド
+            wait_thread = threading.Thread(
+                name="wait_thread", target=wait_screen.start_thread
+            )
             wait_thread.start()
-            # run_thread = threading.Thread(target=partial(_execute, result, wait_screen, func, args=args, kwargs=kwargs), args=args, kwargs=kwargs)
-            run_thread = threading.Thread(
+            # mainとなる処理を実行するスレッド
+            run_thread = StoppableThread(
+                name="run_thread",
                 target=partial(_execute, result, wait_screen, func),
                 args=args,
                 kwargs=kwargs,
             )
-            # run_thread.daemon = True
             run_thread.start()
+            # mainスレッドはそのままtkinterのloopさせる。
+            # waitスレッドが終了後にダイアログが終了し、mainスレッドがイベント受付開始をし、resultの値をアクセスする
             return result[0]
 
         return wait_processe
 
     return wrapper
 
 
@@ -66,28 +81,38 @@
         cls,
         title: str,
         max_col: int,
         max_row: int,
         width: int,
         height: int,
         is_debug=False,
+        is_output_file_error=True,
+        error_output_destination=None,
     ) -> BlockFramework:
         """コンストラクタ
 
         Args:
             title (str): rootのタイトル名
             max_col (int): defaultとなる分割する列数
             max_row (int): defaultとなる分割する行数
             width (int): フレームの横幅
             height (int): フレームの縦幅
             is_debug (bool, optional): デバッグモードならTrue
+            is_output_file_error (bool, optional): エラーをファイル出力するか
+            error_output_destination (str, optional): エラーの出力先パス
 
         Returns:
             BlockFramework: 大本のrootとなるFrameを継承したクラスのインスタンス
         """
+        if is_output_file_error:
+            tk.CallWrapper = TracebackCatch
+            if error_output_destination is None:
+                TracebackCatch.init_logger()
+            else:
+                TracebackCatch.init_logger(file_path=error_output_destination)
         cls.root: BlockFramework = BlockFramework(
             max_col, max_row, width, height, is_debug=is_debug
         )
         cls.root.grid_rowconfigure(0, weight=1)
         cls.root.grid_columnconfigure(0, weight=1)
         cls.root.title(title)
         return cls.root
```

### Comparing `tkblock-2.3.1/tkblock/block_waiting_screen.py` & `tkblock-2.4.0/tkblock/block_waiting_screen.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,92 @@
 #!/usr/local/bin/python
 # -*- coding: utf-8 -*-
 # kuri_pome
 """BlockWaitingScreen"""
 import time
+import threading
 import tkinter as tk
 from tkinter import messagebox
 
+from .logger import create_logger
+
+
+logger = create_logger(__name__, level="debug")
+
+FILL_COLOERS = ["white", "black", "red", "green", "blue", "cyan", "yellow", "magenta"]
 
-FILL_COLOERS = ['white', 'black', 'red', 'green', 'blue', 'cyan', 'yellow', 'magenta']
 
 class BlockWaitingScreen:
     """BlockWaitingScreenクラスは、Tkinterウィンドウにウェイト画面を表示するために使用されます。"""
+
     def __init__(self, master, is_force_finish, width=400, height=300):
         self.roop_index = 0
         self.top = tk.Toplevel(master)
         self.top.title("Wait Screen")
         self.top.geometry("{}x{}".format(width, height))
-        
+
         # このWindowsが閉じられたとき
         def click_close():
-            if messagebox.askokcancel("確認", "想定外の動き！ばぐるかも！本当に閉じていいですか？"):
-                self.stop()
-                self.is_thread_run = True
+            if messagebox.askokcancel("確認", "強制終了。\n処理途中のデータが破壊される可能性あり\n本当に閉じていいですか？"):
+                is_force_finish[0] = True
+                for t in threading.enumerate():
+                    if t.name == "run_thread":
+                        t.raise_exception()
+                        logger.info("強制停止しました。")
+                self.is_thread_run = False
                 self.end_thread()
-                self.top.destroy()
+            else:
+                logger.info("強制停止しませんでした。")
+
         self.top.protocol("WM_DELETE_WINDOW", click_close)
 
         # 回転する円描画用のキャンバスを作成
         self.canvas = tk.Canvas(self.top, width=100, height=100)
         self.canvas.place(relx=0.5, rely=0.4, anchor="center")
-        self.arc = self.canvas.create_arc(10, 10, 90, 90, start=0, extent=40, outline="magenta")
-        
+        self.arc = self.canvas.create_arc(
+            10, 10, 90, 90, start=0, extent=40, outline="magenta"
+        )
+
         # 強制終了ボタン
         def _execute_finish():
             is_force_finish[0] = True
-            # raise Exception("gega")
-        self.button = tk.Button(self.top, width=100, height=5, text="強制終了[未実装]", command=_execute_finish)
+            for t in threading.enumerate():
+                if t.name == "run_thread":
+                    t.raise_exception()
+                    logger.info("強制停止しました。")
+            self.is_thread_run = False
+            self.end_thread()
+
+        self.button = tk.Button(
+            self.top,
+            width=100,
+            height=5,
+            text="強制終了。\n処理途中のデータが破壊される可能性あり",
+            command=_execute_finish,
+        )
         self.button.place(relx=0.5, rely=0.9, anchor="center")
 
-
         # キャンバスの描画を回転させるspinメソッドを定期的に実行
         self.angle = 0
         self.delay = 0.1
         self.is_spin = True
         self.is_thread_run = False
 
     def _spin(self):
         """canvas.create_arc()で描いた円を回転させるアニメーションを実行"""
         if self.is_spin:
             self.canvas.delete(self.arc)
-            self.canvas.create_arc(10, 10, 90, 90, start=self.angle, extent=40, fill="red", width=5)
+            self.canvas.create_arc(
+                10, 10, 90, 90, start=self.angle, extent=40, fill="red", width=5
+            )
             self.angle += 40
-        self.top.after(int(self.delay * 1000), self._spin)
-        
+            self.top.after(int(self.delay * 1000), self._spin)
+        else:
+            self.is_thread_run = False
+            self.end_thread()
 
     def start(self):
         """BlockWaitingScreenを表示する"""
         self._spin()
         self.top.update_idletasks()
         self.top.update()
 
@@ -68,36 +98,43 @@
         self.is_thread_run = True
         fill_colors = FILL_COLOERS.copy()
         while self.is_spin:
             if self.angle < 360:
                 if len(fill_colors) == 0:
                     fill_colors = FILL_COLOERS.copy()
                 color = fill_colors.pop()
-                self.canvas.create_arc(10, 10, 90, 90, start=self.angle, extent=40, fill=color, outline=color)
+                self.canvas.create_arc(
+                    10,
+                    10,
+                    90,
+                    90,
+                    start=self.angle,
+                    extent=40,
+                    fill=color,
+                    outline=color,
+                )
                 self.angle += 40
             else:
                 self.canvas.delete("all")
                 self.angle = 0
             time.sleep(0.5)
             self.roop_index += 1
             self.top.update_idletasks()
         self.is_thread_run = False
+        self.end_thread()
 
     def end_thread(self):
         """BlockWaitingScreenの円アニメーションを停止する
-        
+
         start_thread
         """
         self.is_spin = False
         while self.is_thread_run:
             time.sleep(0.1)
         self.top.destroy()
 
-
     def restart(self):
         """BlockWaitingScreenの円アニメーションを再開する"""
         self.is_spin = True
-        
+
     def destroy(self):
         self.top.destroy()
-
-
```

### Comparing `tkblock-2.3.1/tkblock/canvas.py` & `tkblock-2.4.0/tkblock/canvas.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.1/tkblock.egg-info/PKG-INFO` & `tkblock-2.4.0/tkblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.3.1
+Version: 2.4.0
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

