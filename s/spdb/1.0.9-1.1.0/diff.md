# Comparing `tmp/spdb-1.0.9.tar.gz` & `tmp/spdb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdb-1.0.9.tar", last modified: Mon Jul 17 17:09:26 2023, max compression
+gzip compressed data, was "spdb-1.1.0.tar", last modified: Tue Jul 18 13:14:12 2023, max compression
```

## Comparing `spdb-1.0.9.tar` & `spdb-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.0.9/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2910 2023-07-17 17:09:26.646797 spdb-1.0.9/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2427 2023-07-17 17:08:59.000000 spdb-1.0.9/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-17 17:09:15.000000 spdb-1.0.9/pyproject.toml
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-17 17:09:26.646797 spdb-1.0.9/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-17 17:09:12.000000 spdb-1.0.9/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/spdb/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      170 2023-07-17 10:29:25.000000 spdb-1.0.9/spdb/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1596 2023-07-17 12:41:12.000000 spdb-1.0.9/spdb/db.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.0.9/spdb/generator_utils.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.0.9/spdb/otp.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      325 2023-07-17 12:10:08.000000 spdb-1.0.9/spdb/text_validator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 12:46:37.000000 spdb-1.0.9/spdb/token_generator.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.0.9/spdb/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-17 17:09:26.646797 spdb-1.0.9/spdb.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2910 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      332 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-17 10:51:25.000000 spdb-1.0.9/spdb.egg-info/not-zip-safe
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/requires.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-17 17:09:26.000000 spdb-1.0.9/spdb.egg-info/top_level.txt
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 13:14:12.755664 spdb-1.1.0/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2023-07-17 12:15:45.000000 spdb-1.1.0/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 13:14:12.755664 spdb-1.1.0/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4986 2023-07-18 12:48:35.000000 spdb-1.1.0/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      468 2023-07-18 11:41:08.000000 spdb-1.1.0/pyproject.toml
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2023-07-18 13:14:12.755664 spdb-1.1.0/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      246 2023-07-18 11:41:11.000000 spdb-1.1.0/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 13:14:12.752331 spdb-1.1.0/spdb/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      229 2023-07-18 12:50:28.000000 spdb-1.1.0/spdb/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2555 2023-07-18 11:02:16.000000 spdb-1.1.0/spdb/db.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      596 2023-07-17 12:49:27.000000 spdb-1.1.0/spdb/generator_utils.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1047 2023-07-17 12:49:07.000000 spdb-1.1.0/spdb/otp.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1366 2023-07-18 13:08:42.000000 spdb-1.1.0/spdb/quotes.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2223 2023-07-18 12:58:01.000000 spdb-1.1.0/spdb/restr.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      370 2023-07-18 13:07:31.000000 spdb-1.1.0/spdb/textvalidator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      654 2023-07-17 17:51:56.000000 spdb-1.1.0/spdb/token_generator.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       34 2023-07-17 10:29:15.000000 spdb-1.1.0/spdb/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2023-07-18 13:14:12.755664 spdb-1.1.0/spdb.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5469 2023-07-18 13:14:12.000000 spdb-1.1.0/spdb.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      360 2023-07-18 13:14:12.000000 spdb-1.1.0/spdb.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 13:14:12.000000 spdb-1.1.0/spdb.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2023-07-18 11:02:48.000000 spdb-1.1.0/spdb.egg-info/not-zip-safe
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       13 2023-07-18 13:14:12.000000 spdb-1.1.0/spdb.egg-info/requires.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        5 2023-07-18 13:14:12.000000 spdb-1.1.0/spdb.egg-info/top_level.txt
```

### Comparing `spdb-1.0.9/LICENSE` & `spdb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spdb-1.0.9/spdb/generator_utils.py` & `spdb-1.1.0/spdb/generator_utils.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.9/spdb/otp.py` & `spdb-1.1.0/spdb/otp.py`

 * *Files identical despite different names*

### Comparing `spdb-1.0.9/spdb/token_generator.py` & `spdb-1.1.0/spdb/token_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class TokenGenerator:
 	def __init__(self, code: str):
 		self.code = code
 
 
-	def gen(self, type: str, ID: str, key: str) -> stc:
+	def gen(self, type: str, ID: str, key: str) -> str:
 		return f'{self.code}.t.{type}.{ID}:{generator_utils.sha256(ID+generator_utils.sha256(key))}_{generator_utils.sha256(generator_utils.sha256(key)+ID+generator_utils.random_sha256())}'
 
 	@staticmethod
 	def parse_token(token: str) -> dict:
 		return {
 			'code': token.split('.')[0],
 			'type': token.split('.')[2],
```

