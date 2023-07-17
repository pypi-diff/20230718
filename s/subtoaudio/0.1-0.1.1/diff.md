# Comparing `tmp/subtoaudio-0.1.tar.gz` & `tmp/subtoaudio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtoaudio-0.1.tar", last modified: Mon Jul 17 22:56:57 2023, max compression
+gzip compressed data, was "subtoaudio-0.1.1.tar", last modified: Mon Jul 17 23:08:57 2023, max compression
```

## Comparing `subtoaudio-0.1.tar` & `subtoaudio-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 22:56:57.649658 subtoaudio-0.1/
--rw-rw-rw-   0        0        0    16725 2023-07-17 08:09:14.000000 subtoaudio-0.1/LICENSE
--rw-rw-rw-   0        0        0     2765 2023-07-17 22:56:57.649658 subtoaudio-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2119 2023-07-17 22:56:28.000000 subtoaudio-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 22:56:57.649658 subtoaudio-0.1/setup.cfg
--rw-rw-rw-   0        0        0      951 2023-07-17 08:09:14.000000 subtoaudio-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:56:57.618458 subtoaudio-0.1/subtoaudio/
--rw-rw-rw-   0        0        0       34 2023-07-17 08:09:14.000000 subtoaudio-0.1/subtoaudio/__init__.py
--rw-rw-rw-   0        0        0     5037 2023-07-17 08:09:14.000000 subtoaudio-0.1/subtoaudio/subtoaudio.py
-drwxrwxrwx   0        0        0        0 2023-07-17 22:56:57.634058 subtoaudio-0.1/subtoaudio.egg-info/
--rw-rw-rw-   0        0        0     2765 2023-07-17 22:56:56.000000 subtoaudio-0.1/subtoaudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-17 22:56:57.000000 subtoaudio-0.1/subtoaudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 22:56:56.000000 subtoaudio-0.1/subtoaudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-17 22:56:56.000000 subtoaudio-0.1/subtoaudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 22:56:56.000000 subtoaudio-0.1/subtoaudio.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/
+-rw-rw-rw-   0        0        0    16725 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2732 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2084 2023-07-17 23:06:54.000000 subtoaudio-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-07-17 23:07:37.000000 subtoaudio-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.946174 subtoaudio-0.1.1/subtoaudio/
+-rw-rw-rw-   0        0        0       34 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/subtoaudio/__init__.py
+-rw-rw-rw-   0        0        0     5037 2023-07-17 08:09:14.000000 subtoaudio-0.1.1/subtoaudio/subtoaudio.py
+drwxrwxrwx   0        0        0        0 2023-07-17 23:08:56.992974 subtoaudio-0.1.1/subtoaudio.egg-info/
+-rw-rw-rw-   0        0        0     2732 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 23:08:56.000000 subtoaudio-0.1.1/subtoaudio.egg-info/top_level.txt
```

### Comparing `subtoaudio-0.1/LICENSE` & `subtoaudio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `subtoaudio-0.1/PKG-INFO` & `subtoaudio-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1
+Version: 0.1.1
 Summary: Generate audio or speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
-pip install git+https://github.com/bnsantoso/sub-to-audio
+pip install subtoaudio
 ```
 ffmpeg on linux
 ```bash
 apt-get install ffmpeg
 ```
 ## Example usage
```

### Comparing `subtoaudio-0.1/README.md` & `subtoaudio-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
-pip install git+https://github.com/bnsantoso/sub-to-audio
+pip install subtoaudio
 ```
 ffmpeg on linux
 ```bash
 apt-get install ffmpeg
 ```
 ## Example usage
```

### Comparing `subtoaudio-0.1/setup.py` & `subtoaudio-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     README = readme_file.read()
 
 setup(
     name="subtoaudio",
     packages=find_packages(exclude=[]),
-    version="0.1",
+    version="0.1.1",
     license="MPL 2.0",
     description="Generate audio or speech from any subtitle file",
     author="Bagas NS",
     author_email="bagassantoso71@gmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bnsantoso/",
```

### Comparing `subtoaudio-0.1/subtoaudio/subtoaudio.py` & `subtoaudio-0.1.1/subtoaudio/subtoaudio.py`

 * *Files identical despite different names*

### Comparing `subtoaudio-0.1/subtoaudio.egg-info/PKG-INFO` & `subtoaudio-0.1.1/subtoaudio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtoaudio
-Version: 0.1
+Version: 0.1.1
 Summary: Generate audio or speech from any subtitle file
 Home-page: https://github.com/bnsantoso/
 Author: Bagas NS
 Author-email: bagassantoso71@gmail.com
 License: MPL 2.0
 Keywords: subtitle,tts,text to audio,subtitle to audio,subtitle to speech
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 
 ## Installation
 
 ```bash
 pip install git+https://github.com/bnsantoso/sub-to-audio
 ```
 ```bash
-pip install git+https://github.com/bnsantoso/sub-to-audio
+pip install subtoaudio
 ```
 ffmpeg on linux
 ```bash
 apt-get install ffmpeg
 ```
 ## Example usage
```

