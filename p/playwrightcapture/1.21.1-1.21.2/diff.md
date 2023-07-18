# Comparing `tmp/playwrightcapture-1.21.1.tar.gz` & `tmp/playwrightcapture-1.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.21.1.tar", max compression
+gzip compressed data, was "playwrightcapture-1.21.2.tar", max compression
```

## Comparing `playwrightcapture-1.21.1.tar` & `playwrightcapture-1.21.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.21.1/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.21.1/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.21.1/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    37961 2023-07-04 14:22:13.898654 playwrightcapture-1.21.1/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.21.1/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.21.1/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.21.1/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1840 2023-07-06 13:08:27.903638 playwrightcapture-1.21.1/pyproject.toml
--rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 playwrightcapture-1.21.1/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.21.2/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.21.2/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.21.2/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    37961 2023-07-04 14:22:13.898654 playwrightcapture-1.21.2/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.21.2/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.21.2/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.21.2/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1840 2023-07-18 07:51:12.103879 playwrightcapture-1.21.2/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 playwrightcapture-1.21.2/PKG-INFO
```

### Comparing `playwrightcapture-1.21.1/LICENSE` & `playwrightcapture-1.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.1/README.md` & `playwrightcapture-1.21.2/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.1/playwrightcapture/capture.py` & `playwrightcapture-1.21.2/playwrightcapture/capture.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.1/playwrightcapture/helpers.py` & `playwrightcapture-1.21.2/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.1/pyproject.toml` & `playwrightcapture-1.21.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.21.1"
+version = "1.21.2"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -17,15 +17,15 @@
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
-playwright = "^1.35.0"
+playwright = "^1.36.0"
 dateparser = "^1.1.8"
 beautifulsoup4 = {version= "^4.12.2", extras = ["lxml"]}
 w3lib = "^2.1.1"
 requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
 pytz = {"version" = "^2023.3", python = "<3.9"}
```

### Comparing `playwrightcapture-1.21.1/PKG-INFO` & `playwrightcapture-1.21.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.21.1
+Version: 1.21.2
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
 Requires-Dist: beautifulsoup4[lxml] (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
-Requires-Dist: playwright (>=1.35.0,<2.0.0)
+Requires-Dist: playwright (>=1.36.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2023.3,<2024.0) ; python_version < "3.9"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: tzdata (>=2023.3,<2024.0)
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
 Description-Content-Type: text/markdown
```

