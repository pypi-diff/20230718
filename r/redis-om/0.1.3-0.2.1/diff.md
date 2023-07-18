# Comparing `tmp/redis_om-0.1.3.tar.gz` & `tmp/redis_om-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_om-0.1.3.tar", max compression
+gzip compressed data, was "redis_om-0.2.1.tar", max compression
```

## Comparing `redis_om-0.1.3.tar` & `redis_om-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1071 2023-07-12 10:27:59.001163 redis_om-0.1.3/LICENSE
--rw-r--r--   0        0        0    13137 2023-07-12 10:27:59.001163 redis_om-0.1.3/README.md
--rw-r--r--   0        0        0      463 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/__init__.py
--rw-r--r--   0        0        0      806 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/_compat.py
--rw-r--r--   0        0        0       35 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/async_redis.py
--rw-r--r--   0        0        0      751 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/checks.py
--rw-r--r--   0        0        0      524 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/connections.py
--rw-r--r--   0        0        0      223 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 10:27:59.001163 redis_om-0.1.3/aredis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      448 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6513 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5204 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    69588 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/model.py
--rw-r--r--   0        0        0     2210 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2140 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/render_tree.py
--rw-r--r--   0        0        0      824 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/sync_redis.py
--rw-r--r--   0        0        0      218 2023-07-12 10:27:59.005164 redis_om-0.1.3/aredis_om/util.py
--rw-r--r--   0        0        0     3717 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/connections.md
--rw-r--r--   0        0        0     6704 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/errors.md
--rw-r--r--   0        0        0     7510 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/fastapi_integration.md
--rw-r--r--   0        0        0    21897 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/getting_started.md
--rw-r--r--   0        0        0      973 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/index.md
--rw-r--r--   0        0        0    11595 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/models.md
--rw-r--r--   0        0        0     1674 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/redis_modules.md
--rw-r--r--   0        0        0     3688 2023-07-12 10:27:59.005164 redis_om-0.1.3/docs/validation.md
--rw-r--r--   0        0        0     3577 2023-07-12 10:27:59.005164 redis_om-0.1.3/images/logo.svg
--rw-r--r--   0        0        0     1822 2023-07-12 10:27:59.489192 redis_om-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      462 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/__init__.py
--rw-r--r--   0        0        0      806 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/_compat.py
--rw-r--r--   0        0        0       35 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/async_redis.py
--rw-r--r--   0        0        0      714 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/checks.py
--rw-r--r--   0        0        0      524 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/connections.py
--rw-r--r--   0        0        0      223 2023-07-12 10:28:57.940643 redis_om-0.1.3/redis_om/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 10:28:57.952644 redis_om-0.1.3/redis_om/model/cli/__init__.py
--rw-r--r--   0        0        0      446 2023-07-12 10:28:57.952644 redis_om-0.1.3/redis_om/model/cli/migrate.py
--rw-r--r--   0        0        0     6513 2023-07-12 10:28:57.940643 redis_om-0.1.3/redis_om/model/encoders.py
--rw-r--r--   0        0        0        0 2023-07-12 10:28:57.948643 redis_om-0.1.3/redis_om/model/migrations/__init__.py
--rw-r--r--   0        0        0     5101 2023-07-12 10:28:57.948643 redis_om-0.1.3/redis_om/model/migrations/migrator.py
--rw-r--r--   0        0        0    69263 2023-07-12 10:28:57.932643 redis_om-0.1.3/redis_om/model/model.py
--rw-r--r--   0        0        0     2209 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/model/query_resolver.py
--rw-r--r--   0        0        0     2140 2023-07-12 10:28:57.944643 redis_om-0.1.3/redis_om/model/render_tree.py
--rw-r--r--   0        0        0      824 2023-07-12 10:28:57.864638 redis_om-0.1.3/redis_om/model/token_escaper.py
--rw-r--r--   0        0        0       13 2023-07-12 10:28:57.856638 redis_om-0.1.3/redis_om/sync_redis.py
--rw-r--r--   0        0        0      212 2023-07-12 10:28:57.860638 redis_om-0.1.3/redis_om/util.py
--rw-r--r--   0        0        0    14617 1970-01-01 00:00:00.000000 redis_om-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-18 14:52:41.875387 redis_om-0.2.1/LICENSE
+-rw-r--r--   0        0        0    13124 2023-07-18 14:52:41.875387 redis_om-0.2.1/README.md
+-rw-r--r--   0        0        0      463 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/_compat.py
+-rw-r--r--   0        0        0       35 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/async_redis.py
+-rw-r--r--   0        0        0      751 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/checks.py
+-rw-r--r--   0        0        0      524 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/connections.py
+-rw-r--r--   0        0        0      223 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6513 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5204 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    69588 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/model.py
+-rw-r--r--   0        0        0     2210 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2140 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/render_tree.py
+-rw-r--r--   0        0        0      824 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/sync_redis.py
+-rw-r--r--   0        0        0      218 2023-07-18 14:52:41.875387 redis_om-0.2.1/aredis_om/util.py
+-rw-r--r--   0        0        0     3717 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/connections.md
+-rw-r--r--   0        0        0     6704 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/errors.md
+-rw-r--r--   0        0        0     7510 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/fastapi_integration.md
+-rw-r--r--   0        0        0    21897 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/getting_started.md
+-rw-r--r--   0        0        0      973 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/index.md
+-rw-r--r--   0        0        0    11595 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/models.md
+-rw-r--r--   0        0        0     1674 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/redis_modules.md
+-rw-r--r--   0        0        0     3688 2023-07-18 14:52:41.875387 redis_om-0.2.1/docs/validation.md
+-rw-r--r--   0        0        0     3577 2023-07-18 14:52:41.875387 redis_om-0.2.1/images/logo.svg
+-rw-r--r--   0        0        0     1822 2023-07-18 14:52:42.279394 redis_om-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-07-18 14:53:33.063929 redis_om-0.2.1/redis_om/__init__.py
+-rw-r--r--   0        0        0      806 2023-07-18 14:53:33.059929 redis_om-0.2.1/redis_om/_compat.py
+-rw-r--r--   0        0        0       35 2023-07-18 14:53:33.059929 redis_om-0.2.1/redis_om/async_redis.py
+-rw-r--r--   0        0        0      714 2023-07-18 14:53:33.063929 redis_om-0.2.1/redis_om/checks.py
+-rw-r--r--   0        0        0      524 2023-07-18 14:53:33.059929 redis_om-0.2.1/redis_om/connections.py
+-rw-r--r--   0        0        0      223 2023-07-18 14:53:33.131930 redis_om-0.2.1/redis_om/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:53:33.139930 redis_om-0.2.1/redis_om/model/cli/__init__.py
+-rw-r--r--   0        0        0      446 2023-07-18 14:53:33.139930 redis_om-0.2.1/redis_om/model/cli/migrate.py
+-rw-r--r--   0        0        0     6513 2023-07-18 14:53:33.131930 redis_om-0.2.1/redis_om/model/encoders.py
+-rw-r--r--   0        0        0        0 2023-07-18 14:53:33.139930 redis_om-0.2.1/redis_om/model/migrations/__init__.py
+-rw-r--r--   0        0        0     5101 2023-07-18 14:53:33.139930 redis_om-0.2.1/redis_om/model/migrations/migrator.py
+-rw-r--r--   0        0        0    69263 2023-07-18 14:53:33.127930 redis_om-0.2.1/redis_om/model/model.py
+-rw-r--r--   0        0        0     2209 2023-07-18 14:53:33.063929 redis_om-0.2.1/redis_om/model/query_resolver.py
+-rw-r--r--   0        0        0     2140 2023-07-18 14:53:33.135930 redis_om-0.2.1/redis_om/model/render_tree.py
+-rw-r--r--   0        0        0      824 2023-07-18 14:53:33.067930 redis_om-0.2.1/redis_om/model/token_escaper.py
+-rw-r--r--   0        0        0       13 2023-07-18 14:53:33.059929 redis_om-0.2.1/redis_om/sync_redis.py
+-rw-r--r--   0        0        0      212 2023-07-18 14:53:33.063929 redis_om-0.2.1/redis_om/util.py
+-rw-r--r--   0        0        0    14604 1970-01-01 00:00:00.000000 redis_om-0.2.1/PKG-INFO
```

### Comparing `redis_om-0.1.3/LICENSE` & `redis_om-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/README.md` & `redis_om-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 
 Redis OM uses the [MIT license][license-url].
 
 <!-- Badges -->
 
 [version-svg]: https://img.shields.io/pypi/v/redis-om?style=flat-square
 [package-url]: https://pypi.org/project/redis-om/
-[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/ci?style=flat-square
+[ci-svg]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml/badge.svg
 [ci-url]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml
 [license-image]: https://img.shields.io/badge/license-mit-green.svg?style=flat-square
 [license-url]: LICENSE
 <!-- Links -->
 
 [redis-om-website]: https://developer.redis.com
 [redis-om-js]: https://github.com/redis-om/redis-om-js
```

### Comparing `redis_om-0.1.3/aredis_om/_compat.py` & `redis_om-0.2.1/aredis_om/_compat.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/checks.py` & `redis_om-0.2.1/aredis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/connections.py` & `redis_om-0.2.1/aredis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/encoders.py` & `redis_om-0.2.1/aredis_om/model/encoders.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/migrations/migrator.py` & `redis_om-0.2.1/aredis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/model.py` & `redis_om-0.2.1/aredis_om/model/model.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/query_resolver.py` & `redis_om-0.2.1/aredis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/render_tree.py` & `redis_om-0.2.1/aredis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/aredis_om/model/token_escaper.py` & `redis_om-0.2.1/aredis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/connections.md` & `redis_om-0.2.1/docs/connections.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/errors.md` & `redis_om-0.2.1/docs/errors.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/fastapi_integration.md` & `redis_om-0.2.1/docs/fastapi_integration.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/getting_started.md` & `redis_om-0.2.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/index.md` & `redis_om-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/models.md` & `redis_om-0.2.1/docs/models.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/redis_modules.md` & `redis_om-0.2.1/docs/redis_modules.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/docs/validation.md` & `redis_om-0.2.1/docs/validation.md`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/images/logo.svg` & `redis_om-0.2.1/images/logo.svg`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/pyproject.toml` & `redis_om-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-om"
-version = "0.1.3"
+version = "0.2.1"
 description = "Object mappings, and more, for Redis."
 authors = [ "Redis OSS <oss@redis.com>" ]
 maintainers = [ "Redis OSS <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/redis/redis-om-python"
 classifiers = [
```

### Comparing `redis_om-0.1.3/redis_om/_compat.py` & `redis_om-0.2.1/redis_om/_compat.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/checks.py` & `redis_om-0.2.1/redis_om/checks.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/connections.py` & `redis_om-0.2.1/redis_om/connections.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/encoders.py` & `redis_om-0.2.1/redis_om/model/encoders.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/migrations/migrator.py` & `redis_om-0.2.1/redis_om/model/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/model.py` & `redis_om-0.2.1/redis_om/model/model.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/query_resolver.py` & `redis_om-0.2.1/redis_om/model/query_resolver.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/render_tree.py` & `redis_om-0.2.1/redis_om/model/render_tree.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/redis_om/model/token_escaper.py` & `redis_om-0.2.1/redis_om/model/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redis_om-0.1.3/PKG-INFO` & `redis_om-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-om
-Version: 0.1.3
+Version: 0.2.1
 Summary: Object mappings, and more, for Redis.
 Home-page: https://github.com/redis/redis-om-python
 License: BSD-3-Clause
 Author: Redis OSS
 Author-email: oss@redis.com
 Maintainer: Redis OSS
 Maintainer-email: oss@redis.com
@@ -419,15 +419,15 @@
 
 Redis OM uses the [MIT license][license-url].
 
 <!-- Badges -->
 
 [version-svg]: https://img.shields.io/pypi/v/redis-om?style=flat-square
 [package-url]: https://pypi.org/project/redis-om/
-[ci-svg]: https://img.shields.io/github/workflow/status/redis/redis-om-python/ci?style=flat-square
+[ci-svg]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml/badge.svg
 [ci-url]: https://github.com/redis/redis-om-python/actions/workflows/ci.yml
 [license-image]: https://img.shields.io/badge/license-mit-green.svg?style=flat-square
 [license-url]: LICENSE
 <!-- Links -->
 
 [redis-om-website]: https://developer.redis.com
 [redis-om-js]: https://github.com/redis-om/redis-om-js
```

