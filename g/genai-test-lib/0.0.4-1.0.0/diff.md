# Comparing `tmp/genai_test_lib-0.0.4.tar.gz` & `tmp/genai_test_lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genai_test_lib-0.0.4.tar", last modified: Tue Jul 18 09:11:53 2023, max compression
+gzip compressed data, was "genai_test_lib-1.0.0.tar", last modified: Tue Jul 18 09:12:37 2023, max compression
```

## Comparing `genai_test_lib-0.0.4.tar` & `genai_test_lib-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:11:53.657256 genai_test_lib-0.0.4/
--rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 09:11:53.657102 genai_test_lib-0.0.4/PKG-INFO
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:11:53.651701 genai_test_lib-0.0.4/genai_test_lib/
--rw-r--r--   0 atul       (501) staff       (20)      111 2023-07-18 09:09:05.000000 genai_test_lib-0.0.4/genai_test_lib/__init__.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:11:53.656710 genai_test_lib-0.0.4/genai_test_lib/text_comparision/
--rw-r--r--   0 atul       (501) staff       (20)       77 2023-07-18 09:09:05.000000 genai_test_lib-0.0.4/genai_test_lib/text_comparision/__init__.py
--rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-0.0.4/genai_test_lib/text_comparision/output_parser.py
--rw-r--r--   0 atul       (501) staff       (20)     2201 2023-07-18 08:56:05.000000 genai_test_lib-0.0.4/genai_test_lib/text_comparision/text_compare.py
-drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:11:53.656062 genai_test_lib-0.0.4/genai_test_lib.egg-info/
--rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/PKG-INFO
--rw-r--r--   0 atul       (501) staff       (20)      402 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/SOURCES.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/dependency_links.txt
--rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/not-zip-safe
--rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/requires.txt
--rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-18 09:11:53.000000 genai_test_lib-0.0.4/genai_test_lib.egg-info/top_level.txt
--rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-18 09:11:53.657306 genai_test_lib-0.0.4/setup.cfg
--rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-18 09:11:42.000000 genai_test_lib-0.0.4/setup.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:12:37.858678 genai_test_lib-1.0.0/
+-rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 09:12:37.858490 genai_test_lib-1.0.0/PKG-INFO
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:12:37.856106 genai_test_lib-1.0.0/genai_test_lib/
+-rw-r--r--   0 atul       (501) staff       (20)      111 2023-07-18 09:09:05.000000 genai_test_lib-1.0.0/genai_test_lib/__init__.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:12:37.858205 genai_test_lib-1.0.0/genai_test_lib/text_comparision/
+-rw-r--r--   0 atul       (501) staff       (20)       77 2023-07-18 09:09:05.000000 genai_test_lib-1.0.0/genai_test_lib/text_comparision/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)      594 2023-07-18 08:00:17.000000 genai_test_lib-1.0.0/genai_test_lib/text_comparision/output_parser.py
+-rw-r--r--   0 atul       (501) staff       (20)     2201 2023-07-18 08:56:05.000000 genai_test_lib-1.0.0/genai_test_lib/text_comparision/text_compare.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-07-18 09:12:37.857451 genai_test_lib-1.0.0/genai_test_lib.egg-info/
+-rw-r--r--   0 atul       (501) staff       (20)      188 2023-07-18 09:12:37.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)      402 2023-07-18 09:12:37.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 09:12:37.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-07-18 09:11:53.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/not-zip-safe
+-rw-r--r--   0 atul       (501) staff       (20)       17 2023-07-18 09:12:37.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/requires.txt
+-rw-r--r--   0 atul       (501) staff       (20)       15 2023-07-18 09:12:37.000000 genai_test_lib-1.0.0/genai_test_lib.egg-info/top_level.txt
+-rw-r--r--   0 atul       (501) staff       (20)       38 2023-07-18 09:12:37.858832 genai_test_lib-1.0.0/setup.cfg
+-rw-r--r--   0 atul       (501) staff       (20)      238 2023-07-18 09:12:33.000000 genai_test_lib-1.0.0/setup.py
```

### Comparing `genai_test_lib-0.0.4/genai_test_lib/text_comparision/output_parser.py` & `genai_test_lib-1.0.0/genai_test_lib/text_comparision/output_parser.py`

 * *Files identical despite different names*

### Comparing `genai_test_lib-0.0.4/genai_test_lib/text_comparision/text_compare.py` & `genai_test_lib-1.0.0/genai_test_lib/text_comparision/text_compare.py`

 * *Files identical despite different names*

