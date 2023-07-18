# Comparing `tmp/RapidMangaDL-0.1.1.tar.gz` & `tmp/RapidMangaDL-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RapidMangaDL-0.1.1.tar", last modified: Tue Jul 18 18:01:12 2023, max compression
+gzip compressed data, was "RapidMangaDL-0.1.2.tar", last modified: Tue Jul 18 18:05:55 2023, max compression
```

## Comparing `RapidMangaDL-0.1.1.tar` & `RapidMangaDL-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.328463 RapidMangaDL-0.1.1/
--rw-rw-rw-   0        0        0     6826 2023-07-18 18:01:12.327463 RapidMangaDL-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5422 2023-07-18 18:00:01.000000 RapidMangaDL-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.209468 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/
--rw-rw-rw-   0        0        0     6826 2023-07-18 18:01:10.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-07-18 18:01:11.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 18:01:10.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-18 18:01:10.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      232 2023-07-18 18:01:10.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-18 18:01:10.000000 RapidMangaDL-0.1.1/RapidMangaDL.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.228463 RapidMangaDL-0.1.1/manga_dl/
--rw-rw-rw-   0        0        0      102 2023-07-18 07:16:20.000000 RapidMangaDL-0.1.1/manga_dl/__init__.py
--rw-rw-rw-   0        0        0     6652 2023-07-18 17:00:52.000000 RapidMangaDL-0.1.1/manga_dl/app.py
--rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.1.1/manga_dl/jsconfig.json
--rw-rw-rw-   0        0        0     7753 2023-07-18 17:10:20.000000 RapidMangaDL-0.1.1/manga_dl/main.py
--rw-rw-rw-   0        0        0    27381 2023-07-18 17:31:48.000000 RapidMangaDL-0.1.1/manga_dl/manga.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.238464 RapidMangaDL-0.1.1/manga_dl/manga_sources/
--rw-rw-rw-   0        0        0      557 2023-07-18 08:07:56.000000 RapidMangaDL-0.1.1/manga_dl/manga_sources/__init__.py
--rw-rw-rw-   0        0        0     3698 2023-07-18 15:02:19.000000 RapidMangaDL-0.1.1/manga_dl/manga_sources/base_source.py
--rw-rw-rw-   0        0        0    20701 2023-07-18 17:57:05.000000 RapidMangaDL-0.1.1/manga_dl/manga_sources/source1.py
--rw-rw-rw-   0        0        0    12656 2023-07-18 17:22:33.000000 RapidMangaDL-0.1.1/manga_dl/manga_sources/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.279464 RapidMangaDL-0.1.1/manga_dl/public/
--rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.1.1/manga_dl/public/bootstrap530.css
--rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.1.1/manga_dl/public/bootstrap530.js
--rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.1.1/manga_dl/public/error.png
--rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.1.1/manga_dl/public/jquery321.js
--rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.1.1/manga_dl/public/loading-fast.gif
--rw-rw-rw-   0        0        0     6613 2023-07-18 13:56:46.000000 RapidMangaDL-0.1.1/manga_dl/public/manga.js
--rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.1.1/manga_dl/public/search.js
--rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.1.1/manga_dl/public/style.css
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.296461 RapidMangaDL-0.1.1/manga_dl/templates/
--rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.1.1/manga_dl/templates/chapter.html
--rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.1.1/manga_dl/templates/layout.html
--rw-rw-rw-   0        0        0    13075 2023-07-18 16:19:30.000000 RapidMangaDL-0.1.1/manga_dl/templates/manga.html
--rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.1.1/manga_dl/templates/search.html
-drwxrwxrwx   0        0        0        0 2023-07-18 18:01:12.325465 RapidMangaDL-0.1.1/manga_dl/tools/
--rw-rw-rw-   0        0        0      183 2023-07-17 14:00:50.000000 RapidMangaDL-0.1.1/manga_dl/tools/__init__.py
--rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.1.1/manga_dl/tools/create_pdf.py
--rw-rw-rw-   0        0        0     9652 2023-07-17 09:15:36.000000 RapidMangaDL-0.1.1/manga_dl/tools/download.py
--rw-rw-rw-   0        0        0     6697 2023-07-17 14:54:43.000000 RapidMangaDL-0.1.1/manga_dl/tools/downloader2.py
--rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.1.1/manga_dl/tools/downloader3.py
--rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.1.1/manga_dl/tools/exceptions.py
--rw-rw-rw-   0        0        0     7137 2023-07-17 14:19:26.000000 RapidMangaDL-0.1.1/manga_dl/tools/flask_cloudflared.py
--rw-rw-rw-   0        0        0     1308 2023-07-18 07:58:37.000000 RapidMangaDL-0.1.1/manga_dl/tools/models.py
--rw-rw-rw-   0        0        0     7582 2023-07-18 17:37:20.000000 RapidMangaDL-0.1.1/manga_dl/tools/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-18 18:01:12.329463 RapidMangaDL-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2187 2023-07-18 18:00:34.000000 RapidMangaDL-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.629864 RapidMangaDL-0.1.2/
+-rw-rw-rw-   0        0        0     6826 2023-07-18 18:05:55.617869 RapidMangaDL-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5422 2023-07-18 18:00:01.000000 RapidMangaDL-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.464865 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/
+-rw-rw-rw-   0        0        0     6826 2023-07-18 18:05:53.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-07-18 18:05:54.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:05:53.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-18 18:05:53.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      257 2023-07-18 18:05:53.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 18:05:53.000000 RapidMangaDL-0.1.2/RapidMangaDL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.478864 RapidMangaDL-0.1.2/manga_dl/
+-rw-rw-rw-   0        0        0      102 2023-07-18 07:16:20.000000 RapidMangaDL-0.1.2/manga_dl/__init__.py
+-rw-rw-rw-   0        0        0     6652 2023-07-18 17:00:52.000000 RapidMangaDL-0.1.2/manga_dl/app.py
+-rw-rw-rw-   0        0        0      309 2023-07-11 07:46:25.000000 RapidMangaDL-0.1.2/manga_dl/jsconfig.json
+-rw-rw-rw-   0        0        0     7753 2023-07-18 17:10:20.000000 RapidMangaDL-0.1.2/manga_dl/main.py
+-rw-rw-rw-   0        0        0    27381 2023-07-18 17:31:48.000000 RapidMangaDL-0.1.2/manga_dl/manga.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.492866 RapidMangaDL-0.1.2/manga_dl/manga_sources/
+-rw-rw-rw-   0        0        0      557 2023-07-18 08:07:56.000000 RapidMangaDL-0.1.2/manga_dl/manga_sources/__init__.py
+-rw-rw-rw-   0        0        0     3698 2023-07-18 15:02:19.000000 RapidMangaDL-0.1.2/manga_dl/manga_sources/base_source.py
+-rw-rw-rw-   0        0        0    20701 2023-07-18 17:57:05.000000 RapidMangaDL-0.1.2/manga_dl/manga_sources/source1.py
+-rw-rw-rw-   0        0        0    12656 2023-07-18 17:22:33.000000 RapidMangaDL-0.1.2/manga_dl/manga_sources/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.532863 RapidMangaDL-0.1.2/manga_dl/public/
+-rw-rw-rw-   0        0        0   232918 2023-07-11 11:05:36.000000 RapidMangaDL-0.1.2/manga_dl/public/bootstrap530.css
+-rw-rw-rw-   0        0        0    80427 2023-07-11 11:07:47.000000 RapidMangaDL-0.1.2/manga_dl/public/bootstrap530.js
+-rw-rw-rw-   0        0        0    65212 2023-07-10 06:53:05.000000 RapidMangaDL-0.1.2/manga_dl/public/error.png
+-rw-rw-rw-   0        0        0    86663 2023-07-11 11:07:20.000000 RapidMangaDL-0.1.2/manga_dl/public/jquery321.js
+-rw-rw-rw-   0        0        0   215111 2023-07-11 11:38:35.000000 RapidMangaDL-0.1.2/manga_dl/public/loading-fast.gif
+-rw-rw-rw-   0        0        0     6613 2023-07-18 13:56:46.000000 RapidMangaDL-0.1.2/manga_dl/public/manga.js
+-rw-rw-rw-   0        0        0     3421 2023-07-16 14:02:35.000000 RapidMangaDL-0.1.2/manga_dl/public/search.js
+-rw-rw-rw-   0        0        0     4075 2023-07-16 08:35:36.000000 RapidMangaDL-0.1.2/manga_dl/public/style.css
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.548861 RapidMangaDL-0.1.2/manga_dl/templates/
+-rw-rw-rw-   0        0        0     3699 2023-07-14 18:32:29.000000 RapidMangaDL-0.1.2/manga_dl/templates/chapter.html
+-rw-rw-rw-   0        0        0     3200 2023-07-16 13:24:25.000000 RapidMangaDL-0.1.2/manga_dl/templates/layout.html
+-rw-rw-rw-   0        0        0    13075 2023-07-18 16:19:30.000000 RapidMangaDL-0.1.2/manga_dl/templates/manga.html
+-rw-rw-rw-   0        0        0     2287 2023-07-16 14:00:18.000000 RapidMangaDL-0.1.2/manga_dl/templates/search.html
+drwxrwxrwx   0        0        0        0 2023-07-18 18:05:55.613864 RapidMangaDL-0.1.2/manga_dl/tools/
+-rw-rw-rw-   0        0        0      183 2023-07-17 14:00:50.000000 RapidMangaDL-0.1.2/manga_dl/tools/__init__.py
+-rw-rw-rw-   0        0        0     8192 2023-07-13 14:27:12.000000 RapidMangaDL-0.1.2/manga_dl/tools/create_pdf.py
+-rw-rw-rw-   0        0        0     9652 2023-07-17 09:15:36.000000 RapidMangaDL-0.1.2/manga_dl/tools/download.py
+-rw-rw-rw-   0        0        0     6697 2023-07-17 14:54:43.000000 RapidMangaDL-0.1.2/manga_dl/tools/downloader2.py
+-rw-rw-rw-   0        0        0     8588 2023-07-14 13:14:30.000000 RapidMangaDL-0.1.2/manga_dl/tools/downloader3.py
+-rw-rw-rw-   0        0        0      188 2023-07-16 05:40:17.000000 RapidMangaDL-0.1.2/manga_dl/tools/exceptions.py
+-rw-rw-rw-   0        0        0     7137 2023-07-17 14:19:26.000000 RapidMangaDL-0.1.2/manga_dl/tools/flask_cloudflared.py
+-rw-rw-rw-   0        0        0     1308 2023-07-18 07:58:37.000000 RapidMangaDL-0.1.2/manga_dl/tools/models.py
+-rw-rw-rw-   0        0        0     7582 2023-07-18 17:37:20.000000 RapidMangaDL-0.1.2/manga_dl/tools/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:05:55.629864 RapidMangaDL-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2187 2023-07-18 18:05:20.000000 RapidMangaDL-0.1.2/setup.py
```

### Comparing `RapidMangaDL-0.1.1/PKG-INFO` & `RapidMangaDL-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.1.1
+Version: 0.1.2
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
```

### Comparing `RapidMangaDL-0.1.1/README.md` & `RapidMangaDL-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/RapidMangaDL.egg-info/PKG-INFO` & `RapidMangaDL-0.1.2/RapidMangaDL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RapidMangaDL
-Version: 0.1.1
+Version: 0.1.2
 Summary: Swiftly download manga from multiple sources.
 Home-page: https://github.com/shhossain/RapidMangaDL
 Author: sifat
 Author-email: hossain0338@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/shhossain/RapidMangaDL
 Project-URL: Issue Tracker, https://github.com/shhossain/RapidMangaDL/issues
```

### Comparing `RapidMangaDL-0.1.1/RapidMangaDL.egg-info/SOURCES.txt` & `RapidMangaDL-0.1.2/RapidMangaDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/app.py` & `RapidMangaDL-0.1.2/manga_dl/app.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/main.py` & `RapidMangaDL-0.1.2/manga_dl/main.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/manga.py` & `RapidMangaDL-0.1.2/manga_dl/manga.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/manga_sources/__init__.py` & `RapidMangaDL-0.1.2/manga_dl/manga_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/manga_sources/base_source.py` & `RapidMangaDL-0.1.2/manga_dl/manga_sources/base_source.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/manga_sources/source1.py` & `RapidMangaDL-0.1.2/manga_dl/manga_sources/source1.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/manga_sources/utils.py` & `RapidMangaDL-0.1.2/manga_dl/manga_sources/utils.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/bootstrap530.css` & `RapidMangaDL-0.1.2/manga_dl/public/bootstrap530.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/bootstrap530.js` & `RapidMangaDL-0.1.2/manga_dl/public/bootstrap530.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/error.png` & `RapidMangaDL-0.1.2/manga_dl/public/error.png`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/jquery321.js` & `RapidMangaDL-0.1.2/manga_dl/public/jquery321.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/loading-fast.gif` & `RapidMangaDL-0.1.2/manga_dl/public/loading-fast.gif`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/manga.js` & `RapidMangaDL-0.1.2/manga_dl/public/manga.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/search.js` & `RapidMangaDL-0.1.2/manga_dl/public/search.js`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/public/style.css` & `RapidMangaDL-0.1.2/manga_dl/public/style.css`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/templates/chapter.html` & `RapidMangaDL-0.1.2/manga_dl/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/templates/layout.html` & `RapidMangaDL-0.1.2/manga_dl/templates/layout.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/templates/manga.html` & `RapidMangaDL-0.1.2/manga_dl/templates/manga.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/templates/search.html` & `RapidMangaDL-0.1.2/manga_dl/templates/search.html`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/create_pdf.py` & `RapidMangaDL-0.1.2/manga_dl/tools/create_pdf.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/download.py` & `RapidMangaDL-0.1.2/manga_dl/tools/download.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/downloader2.py` & `RapidMangaDL-0.1.2/manga_dl/tools/downloader2.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/downloader3.py` & `RapidMangaDL-0.1.2/manga_dl/tools/downloader3.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/flask_cloudflared.py` & `RapidMangaDL-0.1.2/manga_dl/tools/flask_cloudflared.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/models.py` & `RapidMangaDL-0.1.2/manga_dl/tools/models.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/manga_dl/tools/utils.py` & `RapidMangaDL-0.1.2/manga_dl/tools/utils.py`

 * *Files identical despite different names*

### Comparing `RapidMangaDL-0.1.1/setup.py` & `RapidMangaDL-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # setup.py
 from setuptools import setup, find_packages
 
 package_name = "RapidMangaDL"
-package_version = "0.1.1"
+package_version = "0.1.2"
 package_description = "Swiftly download manga from multiple sources."
 package_author = "sifat"
 package_author_email = "hossain0338@gmail.com"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

