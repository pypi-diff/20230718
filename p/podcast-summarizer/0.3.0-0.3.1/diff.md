# Comparing `tmp/podcast_summarizer-0.3.0.tar.gz` & `tmp/podcast_summarizer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_summarizer-0.3.0.tar", max compression
+gzip compressed data, was "podcast_summarizer-0.3.1.tar", max compression
```

## Comparing `podcast_summarizer-0.3.0.tar` & `podcast_summarizer-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.3.0/LICENSE
--rw-r--r--   0        0        0     1580 2023-07-18 01:18:54.523862 podcast_summarizer-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-13 05:22:24.279790 podcast_summarizer-0.3.0/podcast_summarizer/__init__.py
--rw-r--r--   0        0        0     3472 2023-07-18 03:04:14.700888 podcast_summarizer-0.3.0/podcast_summarizer/cli.py
--rw-r--r--   0        0        0     4148 2023-07-18 03:04:19.424968 podcast_summarizer-0.3.0/podcast_summarizer/summarizer.py
--rw-r--r--   0        0        0     3139 2023-07-18 02:57:53.246365 podcast_summarizer-0.3.0/podcast_summarizer/youtube.py
--rw-r--r--   0        0        0      683 2023-07-18 03:05:33.164302 podcast_summarizer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2390 1970-01-01 00:00:00.000000 podcast_summarizer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-13 00:12:43.694813 podcast_summarizer-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1580 2023-07-18 01:18:54.523862 podcast_summarizer-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 05:22:24.279790 podcast_summarizer-0.3.1/podcast_summarizer/__init__.py
+-rw-r--r--   0        0        0     3472 2023-07-18 03:04:14.700888 podcast_summarizer-0.3.1/podcast_summarizer/cli.py
+-rw-r--r--   0        0        0     4148 2023-07-18 03:04:19.424968 podcast_summarizer-0.3.1/podcast_summarizer/summarizer.py
+-rw-r--r--   0        0        0     3139 2023-07-18 02:57:53.246365 podcast_summarizer-0.3.1/podcast_summarizer/youtube.py
+-rw-r--r--   0        0        0      646 2023-07-18 03:07:29.515809 podcast_summarizer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2359 1970-01-01 00:00:00.000000 podcast_summarizer-0.3.1/PKG-INFO
```

### Comparing `podcast_summarizer-0.3.0/LICENSE` & `podcast_summarizer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.3.0/README.md` & `podcast_summarizer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.3.0/podcast_summarizer/cli.py` & `podcast_summarizer-0.3.1/podcast_summarizer/cli.py`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.3.0/podcast_summarizer/summarizer.py` & `podcast_summarizer-0.3.1/podcast_summarizer/summarizer.py`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.3.0/podcast_summarizer/youtube.py` & `podcast_summarizer-0.3.1/podcast_summarizer/youtube.py`

 * *Files identical despite different names*

### Comparing `podcast_summarizer-0.3.0/PKG-INFO` & `podcast_summarizer-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: podcast-summarizer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Summarizes podcasts.
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: openai-whisper @ git+https://github.com/openai/whisper.git
+Requires-Dist: openai-whisper (==20230314)
 Requires-Dist: tiktoken (==0.3.3)
 Requires-Dist: webvtt-py (>=0.4.6,<0.5.0)
 Requires-Dist: yt-dlp (>=2023.7.6,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # podcast-summarizer
```

