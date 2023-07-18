# Comparing `tmp/gspot_django_auth-0.1.1.tar.gz` & `tmp/gspot_django_auth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspot_django_auth-0.1.1.tar", last modified: Tue Jul 18 11:11:59 2023, max compression
+gzip compressed data, was "gspot_django_auth-0.1.2.tar", last modified: Tue Jul 18 13:52:42 2023, max compression
```

## Comparing `gspot_django_auth-0.1.1.tar` & `gspot_django_auth-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 11:11:59.231309 gspot_django_auth-0.1.1/
--rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.1/LICENSE
--rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.1/MANIFEST.in
--rw-r--r--   0 vitya      (501) staff       (20)     1313 2023-07-18 11:11:59.231386 gspot_django_auth-0.1.1/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      718 2023-07-18 11:10:16.000000 gspot_django_auth-0.1.1/README.md
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 11:11:59.228747 gspot_django_auth-0.1.1/gspot_django_auth/
--rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.1/gspot_django_auth/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.1/gspot_django_auth/authentication.py
--rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.1/gspot_django_auth/exceptions.py
--rw-r--r--   0 vitya      (501) staff       (20)     1244 2023-07-08 19:21:47.000000 gspot_django_auth-0.1.1/gspot_django_auth/models.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 11:11:59.231038 gspot_django_auth-0.1.1/gspot_django_auth/permissions/
--rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.1/gspot_django_auth/permissions/__init__.py
--rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.1/gspot_django_auth/permissions/permissons.py
--rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.1/gspot_django_auth/permissions/validators.py
--rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.1/gspot_django_auth/permissions/verifiers.py
--rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.1/gspot_django_auth/redis_client.py
--rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.1/gspot_django_auth/token.py
-drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 11:11:59.229888 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/
--rw-r--r--   0 vitya      (501) staff       (20)     1313 2023-07-18 11:11:59.000000 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/PKG-INFO
--rw-r--r--   0 vitya      (501) staff       (20)      627 2023-07-18 11:11:59.000000 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/SOURCES.txt
--rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-18 11:11:59.000000 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/dependency_links.txt
--rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-18 11:11:59.000000 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/requires.txt
--rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-18 11:11:59.000000 gspot_django_auth-0.1.1/gspot_django_auth.egg-info/top_level.txt
--rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-18 11:10:34.000000 gspot_django_auth-0.1.1/pyproject.toml
--rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-18 11:11:59.231700 gspot_django_auth-0.1.1/setup.cfg
--rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.1/setup.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.642207 gspot_django_auth-0.1.2/
+-rw-r--r--   0 vitya      (501) staff       (20)     1063 2023-06-20 19:08:32.000000 gspot_django_auth-0.1.2/LICENSE
+-rw-r--r--   0 vitya      (501) staff       (20)       34 2023-06-27 13:11:56.000000 gspot_django_auth-0.1.2/MANIFEST.in
+-rw-r--r--   0 vitya      (501) staff       (20)     4805 2023-07-18 13:52:42.642307 gspot_django_auth-0.1.2/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)     4209 2023-07-18 13:52:29.000000 gspot_django_auth-0.1.2/README.md
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.637994 gspot_django_auth-0.1.2/gspot_django_auth/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-06-27 13:10:00.000000 gspot_django_auth-0.1.2/gspot_django_auth/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1221 2023-07-08 19:28:37.000000 gspot_django_auth-0.1.2/gspot_django_auth/authentication.py
+-rw-r--r--   0 vitya      (501) staff       (20)      176 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.2/gspot_django_auth/exceptions.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.640237 gspot_django_auth-0.1.2/gspot_django_auth/management/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:34:18.000000 gspot_django_auth-0.1.2/gspot_django_auth/management/__init__.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.640542 gspot_django_auth-0.1.2/gspot_django_auth/management/commands/
+-rw-r--r--   0 vitya      (501) staff       (20)        0 2023-07-18 13:45:15.000000 gspot_django_auth-0.1.2/gspot_django_auth/management/commands/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     4835 2023-07-18 13:49:23.000000 gspot_django_auth-0.1.2/gspot_django_auth/management/commands/load_test_tokens.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1244 2023-07-08 19:21:47.000000 gspot_django_auth-0.1.2/gspot_django_auth/models.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.641892 gspot_django_auth-0.1.2/gspot_django_auth/permissions/
+-rw-r--r--   0 vitya      (501) staff       (20)      189 2023-07-08 19:43:37.000000 gspot_django_auth-0.1.2/gspot_django_auth/permissions/__init__.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1070 2023-07-08 19:08:49.000000 gspot_django_auth-0.1.2/gspot_django_auth/permissions/permissons.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1119 2023-07-03 13:21:53.000000 gspot_django_auth-0.1.2/gspot_django_auth/permissions/validators.py
+-rw-r--r--   0 vitya      (501) staff       (20)     1683 2023-07-07 20:05:39.000000 gspot_django_auth-0.1.2/gspot_django_auth/permissions/verifiers.py
+-rw-r--r--   0 vitya      (501) staff       (20)      781 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.2/gspot_django_auth/redis_client.py
+-rw-r--r--   0 vitya      (501) staff       (20)      243 2023-07-08 19:21:37.000000 gspot_django_auth-0.1.2/gspot_django_auth/token.py
+drwxr-xr-x   0 vitya      (501) staff       (20)        0 2023-07-18 13:52:42.640069 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/
+-rw-r--r--   0 vitya      (501) staff       (20)     4805 2023-07-18 13:52:42.000000 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/PKG-INFO
+-rw-r--r--   0 vitya      (501) staff       (20)      776 2023-07-18 13:52:42.000000 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 vitya      (501) staff       (20)        1 2023-07-18 13:52:42.000000 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      158 2023-07-18 13:52:42.000000 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/requires.txt
+-rw-r--r--   0 vitya      (501) staff       (20)       18 2023-07-18 13:52:42.000000 gspot_django_auth-0.1.2/gspot_django_auth.egg-info/top_level.txt
+-rw-r--r--   0 vitya      (501) staff       (20)      989 2023-07-18 13:52:39.000000 gspot_django_auth-0.1.2/pyproject.toml
+-rw-r--r--   0 vitya      (501) staff       (20)      702 2023-07-18 13:52:42.642764 gspot_django_auth-0.1.2/setup.cfg
+-rw-r--r--   0 vitya      (501) staff       (20)      168 2023-07-08 19:52:39.000000 gspot_django_auth-0.1.2/setup.py
```

### Comparing `gspot_django_auth-0.1.1/LICENSE` & `gspot_django_auth-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/authentication.py` & `gspot_django_auth-0.1.2/gspot_django_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/models.py` & `gspot_django_auth-0.1.2/gspot_django_auth/models.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/permissions/permissons.py` & `gspot_django_auth-0.1.2/gspot_django_auth/permissions/permissons.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/permissions/validators.py` & `gspot_django_auth-0.1.2/gspot_django_auth/permissions/validators.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/permissions/verifiers.py` & `gspot_django_auth-0.1.2/gspot_django_auth/permissions/verifiers.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/gspot_django_auth/redis_client.py` & `gspot_django_auth-0.1.2/gspot_django_auth/redis_client.py`

 * *Files identical despite different names*

### Comparing `gspot_django_auth-0.1.1/pyproject.toml` & `gspot_django_auth-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gspot_django_auth"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name = "oxpaoff", email = "kosenkoviktor11@gmail.com" },
 ]
 description = "A Django app for auth."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gspot_django_auth-0.1.1/setup.cfg` & `gspot_django_auth-0.1.2/setup.cfg`

 * *Files identical despite different names*

