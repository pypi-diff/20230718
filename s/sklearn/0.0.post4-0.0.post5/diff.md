# Comparing `tmp/sklearn-0.0.post4.tar.gz` & `tmp/sklearn-0.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn-0.0.post4.tar", last modified: Thu Apr 13 12:50:40 2023, max compression
+gzip compressed data, was "sklearn-0.0.post5.tar", last modified: Wed May 10 10:12:01 2023, max compression
```

## Comparing `sklearn-0.0.post4.tar` & `sklearn-0.0.post5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-04-13 12:50:40.738130 sklearn-0.0.post4/
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-04-13 12:50:40.738130 sklearn-0.0.post4/PKG-INFO
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3340 2023-04-13 12:50:09.000000 sklearn-0.0.post4/README.md
--rw-r--r--   0 lesteve  (202587) sed      (26082)       38 2023-04-13 12:50:40.738130 sklearn-0.0.post4/setup.cfg
--rw-r--r--   0 lesteve  (202587) sed      (26082)     4085 2023-04-13 12:50:23.000000 sklearn-0.0.post4/setup.py
-drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-04-13 12:50:40.738130 sklearn-0.0.post4/sklearn.egg-info/
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/PKG-INFO
--rw-r--r--   0 lesteve  (202587) sed      (26082)      159 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)        1 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)       14 2023-04-13 12:50:40.000000 sklearn-0.0.post4/sklearn.egg-info/top_level.txt
--rw-r--r--   0 lesteve  (202587) sed      (26082)     3735 2022-11-07 13:41:13.000000 sklearn-0.0.post4/test_brownout.py
+drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-05-10 10:12:01.089918 sklearn-0.0.post5/
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-05-10 10:12:01.089918 sklearn-0.0.post5/PKG-INFO
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3340 2023-04-13 12:50:09.000000 sklearn-0.0.post5/README.md
+-rw-r--r--   0 lesteve  (202587) sed      (26082)       38 2023-05-10 10:12:01.089918 sklearn-0.0.post5/setup.cfg
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     4103 2023-05-10 09:44:14.000000 sklearn-0.0.post5/setup.py
+drwxr-xr-x   0 lesteve  (202587) sed      (26082)        0 2023-05-10 10:12:01.089918 sklearn-0.0.post5/sklearn.egg-info/
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3498 2023-05-10 10:12:01.000000 sklearn-0.0.post5/sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 lesteve  (202587) sed      (26082)      159 2023-05-10 10:12:01.000000 sklearn-0.0.post5/sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)        1 2023-05-10 10:12:01.000000 sklearn-0.0.post5/sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)       14 2023-05-10 10:12:01.000000 sklearn-0.0.post5/sklearn.egg-info/top_level.txt
+-rw-r--r--   0 lesteve  (202587) sed      (26082)     3735 2022-11-07 13:41:13.000000 sklearn-0.0.post5/test_brownout.py
```

### Comparing `sklearn-0.0.post4/PKG-INFO` & `sklearn-0.0.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn
-Version: 0.0.post4
+Version: 0.0.post5
 Summary: deprecated sklearn package, use scikit-learn instead
 Description-Content-Type: text/markdown
 
 # ⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
 
 ⚠️⚠️⚠️ The **`sklearn` PyPI package is deprecated use `scikit-learn` instead** ⚠️⚠️⚠️
```

### Comparing `sklearn-0.0.post4/README.md` & `sklearn-0.0.post5/README.md`

 * *Files identical despite different names*

### Comparing `sklearn-0.0.post4/setup.py` & `sklearn-0.0.post5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from datetime import datetime, MAXYEAR
 from collections import namedtuple
 
 from setuptools import setup
 
 
-with open("README.md") as f:
+with open("README.md", encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 
 def get_brownout_schedule():
     all_start_dates = [datetime(2022, 12, 1)] + [
         datetime(2023, 2 * i, 1) for i in range(1, 7)
     ]
@@ -101,9 +101,9 @@
         maybe_raise_error(checked_datetime)
 
     setup(
         description="deprecated sklearn package, use scikit-learn instead",
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         name="sklearn",
-        version="0.0.post4",
+        version="0.0.post5",
     )
```

### Comparing `sklearn-0.0.post4/sklearn.egg-info/PKG-INFO` & `sklearn-0.0.post5/sklearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn
-Version: 0.0.post4
+Version: 0.0.post5
 Summary: deprecated sklearn package, use scikit-learn instead
 Description-Content-Type: text/markdown
 
 # ⚠️⚠️⚠️ Summary ⚠️⚠️⚠️
 
 ⚠️⚠️⚠️ The **`sklearn` PyPI package is deprecated use `scikit-learn` instead** ⚠️⚠️⚠️
```

### Comparing `sklearn-0.0.post4/test_brownout.py` & `sklearn-0.0.post5/test_brownout.py`

 * *Files identical despite different names*

