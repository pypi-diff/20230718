# Comparing `tmp/garth-0.1.4.tar.gz` & `tmp/garth-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.1.4.tar", last modified: Tue Jul 18 12:47:51 2023, max compression
+gzip compressed data, was "garth-0.1.5.tar", last modified: Tue Jul 18 12:50:59 2023, max compression
```

## Comparing `garth-0.1.4.tar` & `garth-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.4/README.md
--rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.4/garth/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.4/garth/auth_token.py
--rw-r--r--   0        0        0     2676 2023-07-18 12:47:12.835198 garth-0.1.4/garth/http.py
--rw-r--r--   0        0        0     2523 2023-07-18 12:39:28.223048 garth-0.1.4/garth/sso.py
--rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.4/garth/version.py
--rw-r--r--   0        0        0      531 2023-07-18 12:47:51.483806 garth-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 garth-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-07-12 03:23:05.160417 garth-0.1.5/README.md
+-rw-r--r--   0        0        0      107 2023-07-18 12:37:25.559230 garth-0.1.5/garth/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 12:40:02.512828 garth-0.1.5/garth/auth_token.py
+-rw-r--r--   0        0        0     2676 2023-07-18 12:47:12.835198 garth-0.1.5/garth/http.py
+-rw-r--r--   0        0        0     2523 2023-07-18 12:39:28.223048 garth-0.1.5/garth/sso.py
+-rw-r--r--   0        0        0        0 2023-07-16 18:57:56.389343 garth-0.1.5/garth/version.py
+-rw-r--r--   0        0        0      512 2023-07-18 12:50:59.550039 garth-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 garth-0.1.5/PKG-INFO
```

### Comparing `garth-0.1.4/garth/auth_token.py` & `garth-0.1.5/garth/auth_token.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.4/garth/http.py` & `garth-0.1.5/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.4/garth/sso.py` & `garth-0.1.5/garth/sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.1.4/pyproject.toml` & `garth-0.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [project]
 name = "garth"
-version = "0.1.4"
+version = "0.1.5"
 description = "Garmin SSO auth"
 authors = [
     { name = "Matin Tamizi", email = "mtamizi@duck.com" },
 ]
 dependencies = [
-    "fire>=0.5.0",
     "requests>=2.27.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

