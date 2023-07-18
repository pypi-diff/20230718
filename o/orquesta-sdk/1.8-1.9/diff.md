# Comparing `tmp/orquesta_sdk-1.8.tar.gz` & `tmp/orquesta_sdk-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquesta_sdk-1.8.tar", max compression
+gzip compressed data, was "orquesta_sdk-1.9.tar", max compression
```

## Comparing `orquesta_sdk-1.8.tar` & `orquesta_sdk-1.9.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0     1066 2022-06-23 16:02:23.428425 orquesta_sdk-1.8/LICENSE
--rw-r--r--   0        0        0     1231 2023-02-09 07:42:49.216931 orquesta_sdk-1.8/README.md
--rw-r--r--   0        0        0       37 2023-02-09 06:49:12.342103 orquesta_sdk-1.8/orquesta_sdk/__init__.py
--rw-r--r--   0        0        0     1041 2023-02-09 07:39:32.349397 orquesta_sdk-1.8/orquesta_sdk/base_client.py
--rw-r--r--   0        0        0      931 2023-02-09 06:54:32.098548 orquesta_sdk-1.8/orquesta_sdk/orquesta.py
--rw-r--r--   0        0        0       67 2023-02-09 06:38:22.357177 orquesta_sdk-1.8/orquesta_sdk/utils.py
--rw-r--r--   0        0        0       20 2023-02-09 07:43:02.627240 orquesta_sdk-1.8/orquesta_sdk/version.py
--rw-r--r--   0        0        0     1370 2023-02-09 07:43:02.630938 orquesta_sdk-1.8/pyproject.toml
--rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 orquesta_sdk-1.8/setup.py
--rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 orquesta_sdk-1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-06-23 16:02:23.428425 orquesta_sdk-1.9/LICENSE
+-rw-r--r--   0        0        0     2990 2023-06-05 16:40:06.729964 orquesta_sdk-1.9/README.md
+-rw-r--r--   0        0        0       35 2023-06-04 19:28:37.740808 orquesta_sdk-1.9/orquesta_sdk/__init__.py
+-rw-r--r--   0        0        0     1348 2023-06-04 20:03:55.892741 orquesta_sdk-1.9/orquesta_sdk/cache.py
+-rw-r--r--   0        0        0      858 2023-06-05 16:37:28.653231 orquesta_sdk-1.9/orquesta_sdk/client.py
+-rw-r--r--   0        0        0     2468 2023-06-04 20:35:14.659538 orquesta_sdk-1.9/orquesta_sdk/prompts.py
+-rw-r--r--   0        0        0      574 2023-06-04 20:05:16.034254 orquesta_sdk-1.9/orquesta_sdk/request.py
+-rw-r--r--   0        0        0     1724 2023-06-04 20:02:22.932515 orquesta_sdk-1.9/orquesta_sdk/result.py
+-rw-r--r--   0        0        0      160 2023-06-04 19:18:37.948329 orquesta_sdk-1.9/orquesta_sdk/rule_type.py
+-rw-r--r--   0        0        0     1732 2023-06-04 20:06:35.320064 orquesta_sdk-1.9/orquesta_sdk/rules.py
+-rw-r--r--   0        0        0      650 2023-06-04 18:59:40.277740 orquesta_sdk-1.9/orquesta_sdk/utils.py
+-rw-r--r--   0        0        0       20 2023-06-04 18:37:34.646081 orquesta_sdk-1.9/orquesta_sdk/version.py
+-rw-r--r--   0        0        0     1370 2023-06-04 18:36:52.950066 orquesta_sdk-1.9/pyproject.toml
+-rw-r--r--   0        0        0     3889 1970-01-01 00:00:00.000000 orquesta_sdk-1.9/PKG-INFO
```

### Comparing `orquesta_sdk-1.8/LICENSE` & `orquesta_sdk-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `orquesta_sdk-1.8/pyproject.toml` & `orquesta_sdk-1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orquesta_sdk"
-version = "1.8"
+version = "1.9"
 description = "No-code business rules and remote configurations"
 authors = ["Orquesta <info@orquesta.dev>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

