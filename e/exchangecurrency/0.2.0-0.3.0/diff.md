# Comparing `tmp/exchangecurrency-0.2.0.tar.gz` & `tmp/exchangecurrency-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchangecurrency-0.2.0.tar", max compression
+gzip compressed data, was "exchangecurrency-0.3.0.tar", max compression
```

## Comparing `exchangecurrency-0.2.0.tar` & `exchangecurrency-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-07-18 09:02:38.526476 exchangecurrency-0.2.0/LICENSE
--rw-r--r--   0        0        0      418 2023-07-18 08:38:40.891621 exchangecurrency-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 08:17:43.155573 exchangecurrency-0.2.0/exchangecurrency/__init__.py
--rw-r--r--   0        0        0      412 2023-07-18 08:52:27.241316 exchangecurrency-0.2.0/exchangecurrency/cli.py
--rw-r--r--   0        0        0      267 2023-07-18 09:11:08.771175 exchangecurrency-0.2.0/exchangecurrency/config.py
--rw-r--r--   0        0        0      298 2023-07-18 08:51:28.452251 exchangecurrency-0.2.0/exchangecurrency/rates.py
--rw-r--r--   0        0        0      434 2023-07-18 09:46:58.598195 exchangecurrency-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 exchangecurrency-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 09:02:38.526476 exchangecurrency-0.3.0/LICENSE
+-rw-r--r--   0        0        0      418 2023-07-18 08:38:40.891621 exchangecurrency-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 08:17:43.155573 exchangecurrency-0.3.0/exchangecurrency/__init__.py
+-rw-r--r--   0        0        0      412 2023-07-18 09:54:17.392470 exchangecurrency-0.3.0/exchangecurrency/cli.py
+-rw-r--r--   0        0        0      267 2023-07-18 09:11:08.771175 exchangecurrency-0.3.0/exchangecurrency/config.py
+-rw-r--r--   0        0        0      298 2023-07-18 08:51:28.452251 exchangecurrency-0.3.0/exchangecurrency/rates.py
+-rw-r--r--   0        0        0      419 2023-07-18 09:57:09.641675 exchangecurrency-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 exchangecurrency-0.3.0/PKG-INFO
```

### Comparing `exchangecurrency-0.2.0/LICENSE` & `exchangecurrency-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exchangecurrency-0.2.0/PKG-INFO` & `exchangecurrency-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchangecurrency
-Version: 0.2.0
+Version: 0.3.0
 Summary: cli tool to convert currencies and get rates
 Author: mojoee
 Author-email: 47809126+mojoee@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

