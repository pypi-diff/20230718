# Comparing `tmp/deltalake-redis-lock-0.0.1a6.tar.gz` & `tmp/deltalake-redis-lock-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake-redis-lock-0.0.1a6.tar", max compression
+gzip compressed data, was "deltalake-redis-lock-0.0.1a7.tar", max compression
```

## Comparing `deltalake-redis-lock-0.0.1a6.tar` & `deltalake-redis-lock-0.0.1a7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a6/LICENSE
--rw-r--r--   0        0        0     2592 2023-07-16 09:04:06.785162 deltalake-redis-lock-0.0.1a6/README.md
--rw-r--r--   0        0        0      594 2023-07-16 08:58:58.292361 deltalake-redis-lock-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a6/src/__init__.py
--rw-r--r--   0        0        0     3051 2023-07-16 08:58:19.312467 deltalake-redis-lock-0.0.1a6/src/deltalake_redis_lock.py
--rw-r--r--   0        0        0      122 2023-07-16 08:58:19.308691 deltalake-redis-lock-0.0.1a6/src/global_lock.py
--rw-r--r--   0        0        0     2135 2023-07-15 14:28:54.446711 deltalake-redis-lock-0.0.1a6/src/redis_lock_object_store.py
--rw-r--r--   0        0        0     3496 2023-07-16 09:04:41.918074 deltalake-redis-lock-0.0.1a6/setup.py
--rw-r--r--   0        0        0     3285 2023-07-16 09:04:41.918368 deltalake-redis-lock-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-14 15:51:34.636636 deltalake-redis-lock-0.0.1a7/LICENSE
+-rw-r--r--   0        0        0     8694 2023-07-18 21:37:46.140095 deltalake-redis-lock-0.0.1a7/README.md
+-rw-r--r--   0        0        0      594 2023-07-18 21:37:46.140791 deltalake-redis-lock-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 15:52:45.562904 deltalake-redis-lock-0.0.1a7/src/__init__.py
+-rw-r--r--   0        0        0     8498 2023-07-18 21:37:46.141144 deltalake-redis-lock-0.0.1a7/src/deltalake_redis_lock.py
+-rw-r--r--   0        0        0      122 2023-07-16 08:58:19.308691 deltalake-redis-lock-0.0.1a7/src/global_lock.py
+-rw-r--r--   0        0        0     2135 2023-07-15 14:28:54.446711 deltalake-redis-lock-0.0.1a7/src/redis_lock_object_store.py
+-rw-r--r--   0        0        0     9776 2023-07-18 21:37:49.769572 deltalake-redis-lock-0.0.1a7/setup.py
+-rw-r--r--   0        0        0     9387 2023-07-18 21:37:49.770022 deltalake-redis-lock-0.0.1a7/PKG-INFO
```

### Comparing `deltalake-redis-lock-0.0.1a6/LICENSE` & `deltalake-redis-lock-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `deltalake-redis-lock-0.0.1a6/pyproject.toml` & `deltalake-redis-lock-0.0.1a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltalake-redis-lock"
-version = "0.0.1-alpha.6"
+version = "0.0.1-alpha.7"
 description = "deltalake-redis-lock"
 authors = ["Simon Thelin"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/wrapbytes/deltalake-redis-lock"
 repository = "https://github.com/wrapbytes/deltalake-redis-lock"
 packages = [
```

### Comparing `deltalake-redis-lock-0.0.1a6/src/redis_lock_object_store.py` & `deltalake-redis-lock-0.0.1a7/src/redis_lock_object_store.py`

 * *Files identical despite different names*

