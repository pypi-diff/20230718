# Comparing `tmp/exchangecurrency-0.6.0.tar.gz` & `tmp/exchangecurrency-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchangecurrency-0.6.0.tar", max compression
+gzip compressed data, was "exchangecurrency-0.7.0.tar", max compression
```

## Comparing `exchangecurrency-0.6.0.tar` & `exchangecurrency-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-07-18 09:02:38.526476 exchangecurrency-0.6.0/LICENSE
--rw-r--r--   0        0        0      418 2023-07-18 08:38:40.891621 exchangecurrency-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 08:17:43.155573 exchangecurrency-0.6.0/exchangecurrency/__init__.py
--rw-r--r--   0        0        0      429 2023-07-18 10:13:31.969587 exchangecurrency-0.6.0/exchangecurrency/cli.py
--rw-r--r--   0        0        0      298 2023-07-18 08:51:28.452251 exchangecurrency-0.6.0/exchangecurrency/rates.py
--rw-r--r--   0        0        0      436 2023-07-18 10:13:49.147062 exchangecurrency-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 exchangecurrency-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 09:02:38.526476 exchangecurrency-0.7.0/LICENSE
+-rw-r--r--   0        0        0      418 2023-07-18 08:38:40.891621 exchangecurrency-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 08:17:43.155573 exchangecurrency-0.7.0/exchangecurrency/__init__.py
+-rw-r--r--   0        0        0      446 2023-07-18 10:15:25.066583 exchangecurrency-0.7.0/exchangecurrency/cli.py
+-rw-r--r--   0        0        0      298 2023-07-18 08:51:28.452251 exchangecurrency-0.7.0/exchangecurrency/rates.py
+-rw-r--r--   0        0        0      436 2023-07-18 10:15:31.388382 exchangecurrency-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 exchangecurrency-0.7.0/PKG-INFO
```

### Comparing `exchangecurrency-0.6.0/LICENSE` & `exchangecurrency-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchangecurrency-0.6.0/PKG-INFO` & `exchangecurrency-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangecurrency
-Version: 0.6.0
+Version: 0.7.0
 Summary: cli tool to convert currencies and get rates
 Author: mojoee
 Author-email: 47809126+mojoee@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

