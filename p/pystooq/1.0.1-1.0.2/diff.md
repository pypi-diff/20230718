# Comparing `tmp/pystooq-1.0.1.tar.gz` & `tmp/pystooq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystooq-1.0.1.tar", last modified: Tue Jul 18 19:33:25 2023, max compression
+gzip compressed data, was "pystooq-1.0.2.tar", last modified: Tue Jul 18 19:46:53 2023, max compression
```

## Comparing `pystooq-1.0.1.tar` & `pystooq-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:33:25.508336 pystooq-1.0.1/
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1062 2023-07-18 19:18:17.000000 pystooq-1.0.1/LICENSE.txt
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     2004 2023-07-18 19:33:25.508071 pystooq-1.0.1/PKG-INFO
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1755 2023-07-18 19:03:25.000000 pystooq-1.0.1/README.md
-drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:33:25.491250 pystooq-1.0.1/pystooq/
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)       71 2023-06-30 12:39:54.000000 pystooq-1.0.1/pystooq/__init__.py
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1926 2023-06-30 12:29:04.000000 pystooq-1.0.1/pystooq/stooq_data_fetcher.py
-drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:33:25.507615 pystooq-1.0.1/pystooq.egg-info/
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     2004 2023-07-18 19:33:25.000000 pystooq-1.0.1/pystooq.egg-info/PKG-INFO
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)      234 2023-07-18 19:33:25.000000 pystooq-1.0.1/pystooq.egg-info/SOURCES.txt
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)        1 2023-07-18 19:33:25.000000 pystooq-1.0.1/pystooq.egg-info/dependency_links.txt
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)      131 2023-07-18 19:33:25.000000 pystooq-1.0.1/pystooq.egg-info/requires.txt
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)        8 2023-07-18 19:33:25.000000 pystooq-1.0.1/pystooq.egg-info/top_level.txt
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)       38 2023-07-18 19:33:25.508426 pystooq-1.0.1/setup.cfg
--rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1008 2023-07-18 19:31:11.000000 pystooq-1.0.1/setup.py
+drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:46:53.460797 pystooq-1.0.2/
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1062 2023-07-18 19:18:17.000000 pystooq-1.0.2/LICENSE.txt
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)     2004 2023-07-18 19:46:53.460406 pystooq-1.0.2/PKG-INFO
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1755 2023-07-18 19:03:25.000000 pystooq-1.0.2/README.md
+drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:46:53.455634 pystooq-1.0.2/pystooq/
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)       71 2023-06-30 12:39:54.000000 pystooq-1.0.2/pystooq/__init__.py
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)     1926 2023-06-30 12:29:04.000000 pystooq-1.0.2/pystooq/stooq_data_fetcher.py
+drwxr-xr-x   0 arturwegrzyn   (501) staff       (20)        0 2023-07-18 19:46:53.459067 pystooq-1.0.2/pystooq.egg-info/
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)     2004 2023-07-18 19:46:53.000000 pystooq-1.0.2/pystooq.egg-info/PKG-INFO
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)      234 2023-07-18 19:46:53.000000 pystooq-1.0.2/pystooq.egg-info/SOURCES.txt
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)        1 2023-07-18 19:46:53.000000 pystooq-1.0.2/pystooq.egg-info/dependency_links.txt
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)      131 2023-07-18 19:46:53.000000 pystooq-1.0.2/pystooq.egg-info/requires.txt
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)        8 2023-07-18 19:46:53.000000 pystooq-1.0.2/pystooq.egg-info/top_level.txt
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)       38 2023-07-18 19:46:53.460906 pystooq-1.0.2/setup.cfg
+-rw-r--r--   0 arturwegrzyn   (501) staff       (20)      630 2023-07-18 19:46:46.000000 pystooq-1.0.2/setup.py
```

### Comparing `pystooq-1.0.1/LICENSE.txt` & `pystooq-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pystooq-1.0.1/PKG-INFO` & `pystooq-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystooq
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for fetching of data from Stooq.com
 Home-page: UNKNOWN
 Author: Artur Wegrzyn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pystooq-1.0.1/README.md` & `pystooq-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pystooq-1.0.1/pystooq/stooq_data_fetcher.py` & `pystooq-1.0.2/pystooq/stooq_data_fetcher.py`

 * *Files identical despite different names*

### Comparing `pystooq-1.0.1/pystooq.egg-info/PKG-INFO` & `pystooq-1.0.2/pystooq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystooq
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package for fetching of data from Stooq.com
 Home-page: UNKNOWN
 Author: Artur Wegrzyn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

