# Comparing `tmp/booze-0.3.0.tar.gz` & `tmp/booze-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booze-0.3.0.tar", max compression
+gzip compressed data, was "booze-0.4.0.tar", max compression
```

## Comparing `booze-0.3.0.tar` & `booze-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-18 04:43:34.768812 booze-0.3.0/README.md
--rw-r--r--   0        0        0      426 2023-07-18 16:05:55.241411 booze-0.3.0/booze/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-18 18:52:22.180647 booze-0.3.0/booze/base.py
--rw-r--r--   0        0        0     3808 2023-07-18 21:04:53.190145 booze-0.3.0/booze/coercer.py
--rw-r--r--   0        0        0      548 2023-07-18 19:20:33.481035 booze-0.3.0/booze/errors.py
--rw-r--r--   0        0        0     2822 2023-07-18 19:03:25.524342 booze-0.3.0/booze/test_coercer.py
--rw-r--r--   0        0        0     2146 2023-07-18 19:26:29.535386 booze-0.3.0/booze/test_errors.py
--rw-r--r--   0        0        0     4478 2023-07-18 19:08:47.403397 booze-0.3.0/booze/validators.py
--rw-r--r--   0        0        0      283 2023-07-18 21:07:07.249323 booze-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      374 1970-01-01 00:00:00.000000 booze-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 04:43:34.768812 booze-0.4.0/README.md
+-rw-r--r--   0        0        0      426 2023-07-18 16:05:55.241411 booze-0.4.0/booze/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-18 18:52:22.180647 booze-0.4.0/booze/base.py
+-rw-r--r--   0        0        0     3808 2023-07-18 21:04:53.190145 booze-0.4.0/booze/coercer.py
+-rw-r--r--   0        0        0      548 2023-07-18 19:20:33.481035 booze-0.4.0/booze/errors.py
+-rw-r--r--   0        0        0     2822 2023-07-18 19:03:25.524342 booze-0.4.0/booze/test_coercer.py
+-rw-r--r--   0        0        0     2146 2023-07-18 19:26:29.535386 booze-0.4.0/booze/test_errors.py
+-rw-r--r--   0        0        0     4478 2023-07-18 19:08:47.403397 booze-0.4.0/booze/validators.py
+-rw-r--r--   0        0        0      321 2023-07-18 21:09:39.776965 booze-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 booze-0.4.0/PKG-INFO
```

### Comparing `booze-0.3.0/booze/base.py` & `booze-0.4.0/booze/base.py`

 * *Files identical despite different names*

### Comparing `booze-0.3.0/booze/coercer.py` & `booze-0.4.0/booze/coercer.py`

 * *Files identical despite different names*

### Comparing `booze-0.3.0/booze/errors.py` & `booze-0.4.0/booze/errors.py`

 * *Files identical despite different names*

### Comparing `booze-0.3.0/booze/test_coercer.py` & `booze-0.4.0/booze/test_coercer.py`

 * *Files identical despite different names*

### Comparing `booze-0.3.0/booze/test_errors.py` & `booze-0.4.0/booze/test_errors.py`

 * *Files identical despite different names*

### Comparing `booze-0.3.0/booze/validators.py` & `booze-0.4.0/booze/validators.py`

 * *Files identical despite different names*

