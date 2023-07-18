# Comparing `tmp/bugout-0.2.8.tar.gz` & `tmp/bugout-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugout-0.2.8.tar", last modified: Tue May 30 10:05:47 2023, max compression
+gzip compressed data, was "bugout-0.2.9.tar", last modified: Mon Jun 19 06:58:22 2023, max compression
```

## Comparing `bugout-0.2.8.tar` & `bugout-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.395813 bugout-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 10:05:29.000000 bugout-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 10:05:47.395813 bugout-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-30 10:05:29.000000 bugout-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.391814 bugout-0.2.8/bugout/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34157 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/humbug.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/journal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.395813 bugout-0.2.8/bugout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:05:38.000000 bugout-0.2.8/bugout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:05:47.395813 bugout-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-30 10:05:29.000000 bugout-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:58:22.842862 bugout-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-19 06:58:08.000000 bugout-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-19 06:58:22.842862 bugout-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-19 06:58:08.000000 bugout-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:58:22.842862 bugout-0.2.9/bugout/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34157 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/humbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-06-19 06:58:08.000000 bugout-0.2.9/bugout/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:58:22.842862 bugout-0.2.9/bugout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:58:13.000000 bugout-0.2.9/bugout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 06:58:22.000000 bugout-0.2.9/bugout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:58:22.842862 bugout-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-19 06:58:08.000000 bugout-0.2.9/setup.py
```

### Comparing `bugout-0.2.8/LICENSE` & `bugout-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/PKG-INFO` & `bugout-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.8/README.md` & `bugout-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/__main__.py` & `bugout-0.2.9/bugout/__main__.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/app.py` & `bugout-0.2.9/bugout/app.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/calls.py` & `bugout-0.2.9/bugout/calls.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/data.py` & `bugout-0.2.9/bugout/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,14 +258,17 @@
     content_url: str
     title: str
     content: Optional[str]
     tags: List[str]
     created_at: str
     updated_at: str
     score: float
+    context_type: Optional[str] = None
+    context_url: Optional[str] = None
+    context_id: Optional[str] = None
 
 
 class BugoutSearchResults(BaseModel):
     total_results: int
     offset: int
     next_offset: Optional[int]
     max_score: float
```

### Comparing `bugout-0.2.8/bugout/exceptions.py` & `bugout-0.2.9/bugout/exceptions.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/group.py` & `bugout-0.2.9/bugout/group.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/humbug.py` & `bugout-0.2.9/bugout/humbug.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/jobs.py` & `bugout-0.2.9/bugout/jobs.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/journal.py` & `bugout-0.2.9/bugout/journal.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/resource.py` & `bugout-0.2.9/bugout/resource.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/settings.py` & `bugout-0.2.9/bugout/settings.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout/user.py` & `bugout-0.2.9/bugout/user.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.8/bugout.egg-info/PKG-INFO` & `bugout-0.2.9/bugout.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.8/setup.py` & `bugout-0.2.9/setup.py`

 * *Files identical despite different names*

