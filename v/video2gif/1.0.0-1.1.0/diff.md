# Comparing `tmp/video2gif-1.0.0.tar.gz` & `tmp/video2gif-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video2gif-1.0.0.tar", max compression
+gzip compressed data, was "video2gif-1.1.0.tar", max compression
```

## Comparing `video2gif-1.0.0.tar` & `video2gif-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34523 2017-09-30 07:16:25.000000 video2gif-1.0.0/LICENSE
--rw-r--r--   0        0        0      248 2023-07-10 16:26:35.138429 video2gif-1.0.0/README.md
--rw-r--r--   0        0        0      615 2023-07-10 17:57:13.088588 video2gif-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 23:35:40.530776 video2gif-1.0.0/video2gif/__init__.py
--rw-r--r--   0        0        0     2204 2023-07-10 17:54:51.762697 video2gif-1.0.0/video2gif/main.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 video2gif-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-16 14:37:00.569535 video2gif-1.1.0/LICENSE
+-rw-r--r--   0        0        0      248 2023-07-16 14:37:00.569535 video2gif-1.1.0/README.md
+-rw-r--r--   0        0        0      615 2023-07-18 21:38:13.413635 video2gif-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 14:37:00.570535 video2gif-1.1.0/video2gif/__init__.py
+-rw-r--r--   0        0        0     2352 2023-07-18 21:38:13.428635 video2gif-1.1.0/video2gif/main.py
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 video2gif-1.1.0/PKG-INFO
```

### Comparing `video2gif-1.0.0/LICENSE` & `video2gif-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `video2gif-1.0.0/pyproject.toml` & `video2gif-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video2gif"
-version = "1.0.0"
+version = "1.1.0"
 description = "a simple program that converts a video to gif. it will also download a video for you using yt-dlp. Depends on ffmpeg"
 authors = ["Mae Miller <maeborow@posteo.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 yt-dlp = "^2023.7.6"
```

### Comparing `video2gif-1.0.0/video2gif/main.py` & `video2gif-1.1.0/video2gif/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,25 @@
 import validators
 import yt_dlp
 
 parser = argparse.ArgumentParser()
 parser.add_argument("video", help="url or path of the video you'd like to gif-ify")
 parser.add_argument("start", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="start time in minutes:seconds")
 parser.add_argument("end", type=lambda d: datetime.datetime.strptime(d, '%M:%S'), help="end time in minutes:seconds")
+parser.add_argument("--output", required=False, help="output file")
 args = parser.parse_args()
 
 start_sec = int(datetime.timedelta(minutes=args.start.minute, seconds=args.start.second).total_seconds())
 end_sec = int(datetime.timedelta(minutes=args.end.minute, seconds=args.end.second).total_seconds())
 
+if args.output:
+    outputFile = args.output
+else:
+    outputFile = "result/output.gif"
+
 if validators.url(args.video):
     URLS = [args.video]
     if os.path.exists("result/inter.mp4"):
         os.remove("result/inter.mp4")
     ydl_opts = {'final_ext': 'mkv',
                 'download_ranges': yt_dlp.utils.download_range_func([], [[start_sec, end_sec]]),
                 'format': 'bv*[ext=mp4]+ba[ext=vorbis]/b[ext=mp4] / bv*+ba/b',
@@ -38,15 +44,15 @@
             ffmpeg.input('result/palettegen_full.png'),
 
          ],
          filter_name='paletteuse',
          dither='heckbert',
          new='False',
          )
-stream = ffmpeg.output(stream, 'result/output.gif', framerate=30)
+stream = ffmpeg.output(stream, outputFile, framerate=30)
 
 
 def run() -> None:
     stream.run(overwrite_output=True)
     if os.path.exists("result/inter.mp4"):
         os.remove("result/inter.mp4")
     if os.path.exists("result/inter-scale.mp4"):
```

### Comparing `video2gif-1.0.0/PKG-INFO` & `video2gif-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video2gif
-Version: 1.0.0
+Version: 1.1.0
 Summary: a simple program that converts a video to gif. it will also download a video for you using yt-dlp. Depends on ffmpeg
 Author: Mae Miller
 Author-email: maeborow@posteo.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
```

