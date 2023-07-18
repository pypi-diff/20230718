# Comparing `tmp/lavapayments-1.0.1.tar.gz` & `tmp/lavapayments-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavapayments-1.0.1.tar", last modified: Tue Jul 18 13:42:17 2023, max compression
+gzip compressed data, was "lavapayments-1.0.2.tar", last modified: Tue Jul 18 13:46:38 2023, max compression
```

## Comparing `lavapayments-1.0.1.tar` & `lavapayments-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:42:17.083760 lavapayments-1.0.1/
--rw-rw-rw-   0        0        0     1184 2023-07-18 13:42:17.083212 lavapayments-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 13:42:17.082200 lavapayments-1.0.1/lavapayments.egg-info/
--rw-rw-rw-   0        0        0     1184 2023-07-18 13:42:16.000000 lavapayments-1.0.1/lavapayments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-07-18 13:42:17.000000 lavapayments-1.0.1/lavapayments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:42:16.000000 lavapayments-1.0.1/lavapayments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 13:19:05.000000 lavapayments-1.0.1/lavapayments.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-07-18 13:42:16.000000 lavapayments-1.0.1/lavapayments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 13:42:17.083760 lavapayments-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-07-18 13:42:14.000000 lavapayments-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 13:46:38.469788 lavapayments-1.0.2/
+-rw-rw-rw-   0        0        0     1189 2023-07-18 13:46:38.468594 lavapayments-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 13:46:38.468594 lavapayments-1.0.2/lavapayments.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-07-18 13:46:38.000000 lavapayments-1.0.2/lavapayments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 13:46:38.469788 lavapayments-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-18 13:45:59.000000 lavapayments-1.0.2/setup.py
```

### Comparing `lavapayments-1.0.1/PKG-INFO` & `lavapayments-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lavapayments
-Version: 1.0.1
+Version: 1.0.2
 Summary: Библиотека для работы с Бизнес API Lava.ru
 Author-email: dimabykov189@gmail.com
 Requires: aiohttp
 Requires-Python: >=3.8
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 
 # LavaPayments
 **Python Библиотека для работы с Бизнес API Lava.ru**
 
 Преимущества
 ------------
 - Асинхронный враппер
```

### Comparing `lavapayments-1.0.1/lavapayments.egg-info/PKG-INFO` & `lavapayments-1.0.2/lavapayments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lavapayments
-Version: 1.0.1
+Version: 1.0.2
 Summary: Библиотека для работы с Бизнес API Lava.ru
 Author-email: dimabykov189@gmail.com
 Requires: aiohttp
 Requires-Python: >=3.8
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 
 # LavaPayments
 **Python Библиотека для работы с Бизнес API Lava.ru**
 
 Преимущества
 ------------
 - Асинхронный враппер
```

