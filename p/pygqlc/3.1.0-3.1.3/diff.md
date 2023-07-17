# Comparing `tmp/pygqlc-3.1.0.tar.gz` & `tmp/pygqlc-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygqlc-3.1.0.tar", last modified: Fri Apr 21 18:46:37 2023, max compression
+gzip compressed data, was "pygqlc-3.1.3.tar", max compression
```

## Comparing `pygqlc-3.1.0.tar` & `pygqlc-3.1.3.tar`

### file list

```diff
@@ -1,28 +1,14 @@
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.524084 pygqlc-3.1.0/
--rw-r--r--   0 baruc      (501) staff       (20)     1074 2021-12-22 16:29:04.000000 pygqlc-3.1.0/LICENCE
--rw-r--r--   0 baruc      (501) staff       (20)       30 2023-02-14 17:33:49.000000 pygqlc-3.1.0/MANIFEST.in
--rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-04-21 18:46:37.523876 pygqlc-3.1.0/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)     4434 2023-02-10 19:11:02.000000 pygqlc-3.1.0/README.md
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.521825 pygqlc-3.1.0/pygqlc/
--rw-r--r--   0 baruc      (501) staff       (20)    25872 2023-04-21 18:46:19.000000 pygqlc-3.1.0/pygqlc/GraphQLClient.py
--rw-r--r--   0 baruc      (501) staff       (20)     4941 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/MutationBatch.py
--rw-r--r--   0 baruc      (501) staff       (20)     2795 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/MutationParser.py
--rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/QueryBatch.py
--rw-r--r--   0 baruc      (501) staff       (20)      761 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/QueryParser.py
--rw-r--r--   0 baruc      (501) staff       (20)      124 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/SubscriptionParser.py
--rw-r--r--   0 baruc      (501) staff       (20)      338 2023-02-14 17:35:44.000000 pygqlc-3.1.0/pygqlc/__init__.py
--rw-r--r--   0 baruc      (501) staff       (20)      338 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/__main__.py
--rw-r--r--   0 baruc      (501) staff       (20)       22 2023-04-21 18:46:19.000000 pygqlc-3.1.0/pygqlc/__version__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.523633 pygqlc-3.1.0/pygqlc/helper_modules/
--rw-r--r--   0 baruc      (501) staff       (20)      362 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/helper_modules/Singleton.py
--rw-r--r--   0 baruc      (501) staff       (20)        0 2021-12-22 16:29:04.000000 pygqlc-3.1.0/pygqlc/helper_modules/__init__.py
-drwxr-xr-x   0 baruc      (501) staff       (20)        0 2023-04-21 18:46:37.523254 pygqlc-3.1.0/pygqlc.egg-info/
--rw-r--r--   0 baruc      (501) staff       (20)     4702 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/PKG-INFO
--rw-r--r--   0 baruc      (501) staff       (20)      523 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/SOURCES.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/dependency_links.txt
--rw-r--r--   0 baruc      (501) staff       (20)       48 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/entry_points.txt
--rw-r--r--   0 baruc      (501) staff       (20)        1 2023-02-10 19:03:06.000000 pygqlc-3.1.0/pygqlc.egg-info/not-zip-safe
--rw-r--r--   0 baruc      (501) staff       (20)       81 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/requires.txt
--rw-r--r--   0 baruc      (501) staff       (20)        7 2023-04-21 18:46:37.000000 pygqlc-3.1.0/pygqlc.egg-info/top_level.txt
--rw-r--r--   0 baruc      (501) staff       (20)       38 2023-04-21 18:46:37.524141 pygqlc-3.1.0/setup.cfg
--rw-r--r--   0 baruc      (501) staff       (20)     1914 2023-02-22 19:53:02.000000 pygqlc-3.1.0/setup.py
+-rw-r--r--   0        0        0     4434 2023-02-10 19:11:02.590061 pygqlc-3.1.3/README.md
+-rw-r--r--   0        0        0    25872 2023-04-21 18:46:19.761900 pygqlc-3.1.3/pygqlc/GraphQLClient.py
+-rw-r--r--   0        0        0     4941 2021-12-22 16:29:04.043942 pygqlc-3.1.3/pygqlc/MutationBatch.py
+-rw-r--r--   0        0        0     2795 2021-12-22 16:29:04.044073 pygqlc-3.1.3/pygqlc/MutationParser.py
+-rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044124 pygqlc-3.1.3/pygqlc/QueryBatch.py
+-rw-r--r--   0        0        0      761 2021-12-22 16:29:04.044246 pygqlc-3.1.3/pygqlc/QueryParser.py
+-rw-r--r--   0        0        0      124 2021-12-22 16:29:04.044355 pygqlc-3.1.3/pygqlc/SubscriptionParser.py
+-rw-r--r--   0        0        0      293 2023-07-17 17:17:28.772924 pygqlc-3.1.3/pygqlc/__init__.py
+-rw-r--r--   0        0        0      338 2021-12-22 16:29:04.044601 pygqlc-3.1.3/pygqlc/__main__.py
+-rw-r--r--   0        0        0       21 2023-07-17 17:19:07.657179 pygqlc-3.1.3/pygqlc/__version__.py
+-rw-r--r--   0        0        0      362 2021-12-22 16:29:04.044775 pygqlc-3.1.3/pygqlc/helper_modules/Singleton.py
+-rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044829 pygqlc-3.1.3/pygqlc/helper_modules/__init__.py
+-rw-r--r--   0        0        0      683 2023-07-17 17:19:07.651867 pygqlc-3.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5047 1970-01-01 00:00:00.000000 pygqlc-3.1.3/PKG-INFO
```

### Comparing `pygqlc-3.1.0/PKG-INFO` & `pygqlc-3.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pygqlc
-Version: 3.1.0
-Summary: GraphQL API Client for python language
-Home-page: https://github.com/valiot/pygqlc
-Author: Valiot
-Author-email: hiring@valiot.io
-Keywords: pygqlc
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # pygqlc
 Python client for graphql APIs
 
 ### Scope
 This is an open source project, please feel free to fork it and PR to contribute with the community!
 Repo for the project: https://github.com/valiot/pygqlc
```

### Comparing `pygqlc-3.1.0/README.md` & `pygqlc-3.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pygqlc
+Version: 3.1.3
+Summary: Python client for graphql APIs
+Author: Baruc Almaguer
+Author-email: baruc.almaguer@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: certifi (==2022.12.07)
+Requires-Dist: pydash (>=5.0,<6.0)
+Requires-Dist: requests (>=2.26,<3.0)
+Requires-Dist: tenacity (>=6.3,<7.0)
+Requires-Dist: websocket-client (==0.54.0)
+Description-Content-Type: text/markdown
+
 # pygqlc
 Python client for graphql APIs
 
 ### Scope
 This is an open source project, please feel free to fork it and PR to contribute with the community!
 Repo for the project: https://github.com/valiot/pygqlc
 
@@ -194,7 +212,8 @@
 You can set a websocket timeout to keep subscriptions alive. 
 
 Use `gql.setTimeoutWebsocket(seconds)`, or directly in the environment `gql.addEnvironment(timeoutWebsocket=seconds)`. Default timeoutWebsocket is 60 seconds
 
 ### for mantainers:
 deploy using:
 `python setup.py sdist bdist_wheel && python -m twine upload dist/* --skip-existing # UPLOAD TO PYPI`
+
```

### Comparing `pygqlc-3.1.0/pygqlc/GraphQLClient.py` & `pygqlc-3.1.3/pygqlc/GraphQLClient.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.0/pygqlc/MutationBatch.py` & `pygqlc-3.1.3/pygqlc/MutationBatch.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.0/pygqlc/MutationParser.py` & `pygqlc-3.1.3/pygqlc/MutationParser.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.0/pygqlc/QueryParser.py` & `pygqlc-3.1.3/pygqlc/QueryParser.py`

 * *Files identical despite different names*

