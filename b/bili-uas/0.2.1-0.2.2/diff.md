# Comparing `tmp/bili-uas-0.2.1.tar.gz` & `tmp/bili-uas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.2.1.tar", last modified: Mon Jul 17 14:01:55 2023, max compression
+gzip compressed data, was "bili-uas-0.2.2.tar", last modified: Mon Jul 17 14:08:01 2023, max compression
```

## Comparing `bili-uas-0.2.1.tar` & `bili-uas-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.794275 bili-uas-0.2.1/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.787826 bili-uas-0.2.1/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.2.1/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2371 2023-07-17 13:47:56.000000 bili-uas-0.2.1/Bili_UAS/bili_config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     6867 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/bili_live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3238 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/bili_login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3350 2023-07-17 12:53:20.000000 bili-uas-0.2.1/Bili_UAS/bili_user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2964 2023-07-17 12:38:07.000000 bili-uas-0.2.1/Bili_UAS/bili_video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.788656 bili-uas-0.2.1/Bili_UAS/cli/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-17 12:26:30.000000 bili-uas-0.2.1/Bili_UAS/cli/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4298 2023-07-17 12:47:31.000000 bili-uas-0.2.1/Bili_UAS/cli/live_cli.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1277 2023-07-17 12:46:40.000000 bili-uas-0.2.1/Bili_UAS/cli/user_cli.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1502 2023-07-17 12:46:40.000000 bili-uas-0.2.1/Bili_UAS/cli/video_cli.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.789123 bili-uas-0.2.1/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.2.1/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2886 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)    13416 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4670 2023-07-17 12:38:07.000000 bili-uas-0.2.1/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.791877 bili-uas-0.2.1/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.2.1/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2366 2023-07-17 13:38:58.000000 bili-uas-0.2.1/Bili_UAS/utils/config_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    63669 2023-07-17 12:17:57.000000 bili-uas-0.2.1/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2224 2023-07-17 12:23:11.000000 bili-uas-0.2.1/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.2.1/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18336 2023-07-17 12:53:20.000000 bili-uas-0.2.1/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-07-15 12:01:05.000000 bili-uas-0.2.1/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    22842 2023-07-15 13:04:58.000000 bili-uas-0.2.1/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.793063 bili-uas-0.2.1/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.2.1/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.2.1/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4148 2023-07-15 12:42:36.000000 bili-uas-0.2.1/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.2.1/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:01:55.794139 bili-uas-0.2.1/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.2.1/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.793947 bili-uas-0.2.1/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      890 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-17 14:01:55.794326 bili-uas-0.2.1/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     2042 2023-07-17 14:01:28.000000 bili-uas-0.2.1/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.976683 bili-uas-0.2.2/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.971852 bili-uas-0.2.2/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.2.2/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2371 2023-07-17 13:47:56.000000 bili-uas-0.2.2/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     6867 2023-07-17 14:01:28.000000 bili-uas-0.2.2/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3238 2023-07-17 14:01:28.000000 bili-uas-0.2.2/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3350 2023-07-17 12:53:20.000000 bili-uas-0.2.2/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2964 2023-07-17 12:38:07.000000 bili-uas-0.2.2/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.972577 bili-uas-0.2.2/Bili_UAS/cli/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-17 12:26:30.000000 bili-uas-0.2.2/Bili_UAS/cli/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4298 2023-07-17 12:47:31.000000 bili-uas-0.2.2/Bili_UAS/cli/live_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1277 2023-07-17 12:46:40.000000 bili-uas-0.2.2/Bili_UAS/cli/user_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1502 2023-07-17 12:46:40.000000 bili-uas-0.2.2/Bili_UAS/cli/video_cli.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.973174 bili-uas-0.2.2/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.2.2/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2752 2023-07-17 14:06:49.000000 bili-uas-0.2.2/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    13416 2023-07-17 14:01:28.000000 bili-uas-0.2.2/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4670 2023-07-17 12:38:07.000000 bili-uas-0.2.2/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.974925 bili-uas-0.2.2/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.2.2/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2390 2023-07-17 14:06:49.000000 bili-uas-0.2.2/Bili_UAS/utils/config_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    63669 2023-07-17 12:17:57.000000 bili-uas-0.2.2/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2224 2023-07-17 12:23:11.000000 bili-uas-0.2.2/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.2.2/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18336 2023-07-17 12:53:20.000000 bili-uas-0.2.2/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-07-15 12:01:05.000000 bili-uas-0.2.2/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    22842 2023-07-15 13:04:58.000000 bili-uas-0.2.2/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.975580 bili-uas-0.2.2/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.2.2/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.2.2/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4124 2023-07-17 14:04:41.000000 bili-uas-0.2.2/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.2.2/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:08:01.976553 bili-uas-0.2.2/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.2.2/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:08:01.976364 bili-uas-0.2.2/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      890 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-17 14:08:01.000000 bili-uas-0.2.2/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-17 14:08:01.976730 bili-uas-0.2.2/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     2042 2023-07-17 14:06:49.000000 bili-uas-0.2.2/setup.py
```

### Comparing `bili-uas-0.2.1/Bili_UAS/bili_config.py` & `bili-uas-0.2.2/Bili_UAS/bili_config.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/bili_live.py` & `bili-uas-0.2.2/Bili_UAS/bili_live.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/bili_login.py` & `bili-uas-0.2.2/Bili_UAS/bili_login.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/bili_user.py` & `bili-uas-0.2.2/Bili_UAS/bili_user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/bili_video.py` & `bili-uas-0.2.2/Bili_UAS/bili_video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/cli/live_cli.py` & `bili-uas-0.2.2/Bili_UAS/cli/live_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/cli/user_cli.py` & `bili-uas-0.2.2/Bili_UAS/cli/user_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/cli/video_cli.py` & `bili-uas-0.2.2/Bili_UAS/cli/video_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/scripts/config.py` & `bili-uas-0.2.2/Bili_UAS/scripts/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 Bili_UAS.scripts.config
 
 This module provides the function to save and read working path and danmu mark.
 """
 
 
 from __future__ import annotations
-from Bili_UAS.writer import log_writer as wlw
 import os
 
 
-@wlw.async_separate()
 async def save_work_dir_to_txt(work_dir: str, language: str) -> None:
     """
     Save working path to file.
 
     Args:
         work_dir: working directory of program
         language: the language of program prompts
@@ -40,15 +38,14 @@
         os.mkdir(log_out_dir)
     if language == "en":
         print("INFO: Working path saved successfully.")
     else:
         print("INFO: 工作路径保存成功。")
 
 
-@wlw.async_separate()
 async def save_danmu_mark_to_txt(danmu_mark: list[str], language: str) -> None:
     """
     Save danmu mark to file.
 
     Args:
         danmu_mark: danmu mark list
         language: the language of program prompts
@@ -59,15 +56,14 @@
             f.write(mark + "\n")
     if language == "en":
         print("INFO: Danmu mark saved successfully.")
     else:
         print("INFO: 弹幕标记保存成功。")
 
 
-@wlw.async_separate()
 async def save_ffmpeg_path_to_txt(ffmpeg_path: str, language: str) -> None:
     """
     Save ffmpeg path to file.
 
     Args:
         ffmpeg_path: the path of ffmpeg
         language: the language of program prompts
@@ -77,15 +73,14 @@
         f.write(ffmpeg_path + "\n")
     if language == "en":
         print("INFO: ffmpeg path saved successfully.")
     else:
         print("INFO: ffmpeg路径保存成功。")
 
 
-@wlw.async_separate()
 async def save_language_to_txt(language: str) -> None:
     """
     Save language to file.
 
     Args:
         language: the language of program prompts
     """
```

### Comparing `bili-uas-0.2.1/Bili_UAS/scripts/log_in.py` & `bili-uas-0.2.2/Bili_UAS/scripts/log_in.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/scripts/video.py` & `bili-uas-0.2.2/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/config_utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/config_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,17 @@
             raise wam.FileMissError("No historical working path found, please specify the working path.")
         else:
             raise wam.FileMissError("未找到记录工作路径的文件, 请指定工作路径.")
     else:
         with open(config_file, "r") as f:
             work_dir: str = f.readline().removesuffix("\n")
         if language == "en":
-            print("Historical working path found, using historical working path.")
+            print("INFO: Historical working path found, using historical working path.")
         else:
-            print("找到历史工作路径, 使用历史工作路径.")
+            print("INFO: 找到历史工作路径, 使用历史工作路径.")
         return work_dir
 
 
 async def load_ffmpeg_path_from_txt() -> str:
     """
     Load the ffmpeg path.
 
@@ -66,11 +66,11 @@
             raise wam.FileMissError("No file found to record ffmpeg path, please specify the ffmpeg path.")
         else:
             raise wam.FileMissError("未找到记录ffmpeg路径的文件, 请指定ffmpeg路径.")
     else:
         with open(ffmpeg_file, "r") as f:
             ffmpeg: str = f.readline().removesuffix("\n")
         if language == "en":
-            print("Historical ffmpeg path found, using historical ffmpeg path.")
+            print("INFO: Historical ffmpeg path found, using historical ffmpeg path.")
         else:
-            print("找到历史ffmpeg路径, 使用历史ffmpeg路径.")
+            print("INFO: 找到历史ffmpeg路径, 使用历史ffmpeg路径.")
         return ffmpeg
```

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/live_utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/live_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/search_utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/user_utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/utils/video_utils.py` & `bili-uas-0.2.2/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/Bili_UAS/writer/log_writer.py` & `bili-uas-0.2.2/Bili_UAS/writer/log_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 
     Args:
         number: the number of separator characters
     """
     def decorator(func):
         @wraps(func)
         async def wrapper(*args, **kwargs):
-            print("\n")
             print("\033[32m" + "-" * number + "\033[0m")
             result = await func(*args, **kwargs)
             print("\033[32m" + "-" * number + "\033[0m")
             print("\n")
             return result
         return wrapper
     return decorator
```

### Comparing `bili-uas-0.2.1/LICENSE` & `bili-uas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/PKG-INFO` & `bili-uas-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.2.1
+Version: 0.2.2
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.2.1/README.md` & `bili-uas-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.2.2/bili_uas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.2.1
+Version: 0.2.2
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.2.1/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.2.2/bili_uas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.1/setup.py` & `bili-uas-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1',
     'openpyxl~=3.1.2']
 
 setup(
     name='bili-uas',
-    version='0.2.1',
+    version='0.2.2',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

