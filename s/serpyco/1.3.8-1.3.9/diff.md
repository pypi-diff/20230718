# Comparing `tmp/serpyco-1.3.8.tar.gz` & `tmp/serpyco-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serpyco-1.3.8.tar", last modified: Thu Jun 23 12:49:13 2022, max compression
+gzip compressed data, was "dist/serpyco-1.3.9.tar", last modified: Mon Jul  4 09:42:42 2022, max compression
```

## Comparing `serpyco-1.3.8.tar` & `serpyco-1.3.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       31 2020-07-28 12:10:51.000000 serpyco-1.3.8/.coveragerc
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      117 2022-06-23 09:18:43.000000 serpyco-1.3.8/.gitignore
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      860 2022-06-23 09:18:43.000000 serpyco-1.3.8/.gitlab-ci.yml
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     7121 2022-06-23 12:37:01.000000 serpyco-1.3.8/CHANGELOG.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1137 2020-07-28 12:10:51.000000 serpyco-1.3.8/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      580 2020-07-28 12:10:51.000000 serpyco-1.3.8/Makefile
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     3301 2022-06-23 12:49:13.000000 serpyco-1.3.8/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2053 2020-07-28 12:10:51.000000 serpyco-1.3.8/README.rst
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5406 2020-07-28 12:10:51.000000 serpyco-1.3.8/conf.py
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/docs/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      173 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/api.rst
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1309 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/benchmark.rst
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/docs/examples/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      570 2020-07-28 12:40:23.000000 serpyco-1.3.8/docs/examples/complex_dump.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      429 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/examples/decorator.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1093 2020-07-28 12:40:23.000000 serpyco-1.3.8/docs/examples/encoder.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      454 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/examples/number_field.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      226 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/examples/simple_dump.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      461 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/examples/string_field.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    12717 2022-06-23 09:18:43.000000 serpyco-1.3.8/docs/getting_started.rst
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      252 2020-07-28 12:10:51.000000 serpyco-1.3.8/docs/index.rst
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      533 2020-07-28 12:10:51.000000 serpyco-1.3.8/example.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      641 2022-06-23 09:18:43.000000 serpyco-1.3.8/requirements.txt
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/serpyco/
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      990 2021-06-24 06:36:25.000000 serpyco-1.3.8/serpyco/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2168 2020-07-28 12:40:23.000000 serpyco-1.3.8/serpyco/decorator.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      105 2021-06-24 06:36:25.000000 serpyco-1.3.8/serpyco/encoder.pxd
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      296 2020-07-28 12:10:51.000000 serpyco-1.3.8/serpyco/encoder.pyi
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      670 2020-07-28 12:10:51.000000 serpyco-1.3.8/serpyco/encoder.pyx
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      627 2020-07-28 12:10:51.000000 serpyco-1.3.8/serpyco/exception.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    10030 2022-06-23 09:18:43.000000 serpyco-1.3.8/serpyco/field.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1521 2020-07-28 12:40:23.000000 serpyco-1.3.8/serpyco/mixin.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 09:18:43.000000 serpyco-1.3.8/serpyco/py.typed
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    19080 2022-06-23 09:18:43.000000 serpyco-1.3.8/serpyco/schema.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1741 2022-06-23 12:35:37.000000 serpyco-1.3.8/serpyco/serializer.pyi
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    31579 2022-06-23 12:35:37.000000 serpyco-1.3.8/serpyco/serializer.pyx
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     2901 2021-06-24 06:36:25.000000 serpyco-1.3.8/serpyco/util.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    11380 2022-06-23 09:18:43.000000 serpyco-1.3.8/serpyco/validator.py
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/serpyco.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3301 2022-06-23 12:49:12.000000 serpyco-1.3.8/serpyco.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      878 2022-06-23 12:49:13.000000 serpyco-1.3.8/serpyco.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2022-06-23 12:49:12.000000 serpyco-1.3.8/serpyco.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2020-07-28 12:33:08.000000 serpyco-1.3.8/serpyco.egg-info/not-zip-safe
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       94 2022-06-23 12:49:12.000000 serpyco-1.3.8/serpyco.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        8 2022-06-23 12:49:12.000000 serpyco-1.3.8/serpyco.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      385 2022-06-23 12:49:13.000000 serpyco-1.3.8/setup.cfg
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1540 2022-06-23 09:18:43.000000 serpyco-1.3.8/setup.py
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2022-06-23 12:49:13.000000 serpyco-1.3.8/tests/
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     2003 2021-06-24 06:36:25.000000 serpyco-1.3.8/tests/test_benchmarks.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)    54944 2022-06-23 12:27:05.000000 serpyco-1.3.8/tests/test_unit.py
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)       31 2022-07-04 09:37:35.000000 serpyco-1.3.9/.coveragerc
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      117 2022-07-04 09:37:35.000000 serpyco-1.3.9/.gitignore
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      860 2022-07-04 09:37:35.000000 serpyco-1.3.9/.gitlab-ci.yml
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     7337 2022-07-04 09:38:47.000000 serpyco-1.3.9/CHANGELOG.md
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     1137 2022-07-04 09:37:35.000000 serpyco-1.3.9/LICENSE
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      580 2022-07-04 09:37:35.000000 serpyco-1.3.9/Makefile
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     3301 2022-07-04 09:42:42.865543 serpyco-1.3.9/PKG-INFO
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     2053 2022-07-04 09:37:35.000000 serpyco-1.3.9/README.rst
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     5406 2022-07-04 09:37:35.000000 serpyco-1.3.9/conf.py
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/docs/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      173 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/api.rst
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     1309 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/benchmark.rst
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/docs/examples/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      570 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/complex_dump.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      429 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/decorator.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     1093 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/encoder.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      454 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/number_field.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      226 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/simple_dump.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      461 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/examples/string_field.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    12717 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/getting_started.rst
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      252 2022-07-04 09:37:35.000000 serpyco-1.3.9/docs/index.rst
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      835 2022-07-04 09:37:35.000000 serpyco-1.3.9/example.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      641 2022-07-04 09:37:35.000000 serpyco-1.3.9/requirements.txt
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/serpyco/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      990 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/__init__.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     2168 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/decorator.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      105 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/encoder.pxd
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      296 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/encoder.pyi
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      670 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/encoder.pyx
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      627 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/exception.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    10030 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/field.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     1521 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/mixin.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/py.typed
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    19080 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/schema.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     2644 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/serializer.pyi
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    31579 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/serializer.pyx
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     2901 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/util.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    11380 2022-07-04 09:37:35.000000 serpyco-1.3.9/serpyco/validator.py
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/serpyco.egg-info/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     3301 2022-07-04 09:42:42.000000 serpyco-1.3.9/serpyco.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      878 2022-07-04 09:42:42.000000 serpyco-1.3.9/serpyco.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        1 2022-07-04 09:42:42.000000 serpyco-1.3.9/serpyco.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        1 2022-07-04 09:41:51.000000 serpyco-1.3.9/serpyco.egg-info/not-zip-safe
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)       94 2022-07-04 09:42:42.000000 serpyco-1.3.9/serpyco.egg-info/requires.txt
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        8 2022-07-04 09:42:42.000000 serpyco-1.3.9/serpyco.egg-info/top_level.txt
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)      385 2022-07-04 09:42:42.865543 serpyco-1.3.9/setup.cfg
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     1540 2022-07-04 09:37:35.000000 serpyco-1.3.9/setup.py
+drwxrwxr-x   0 sebastiengrignard  (1001) sebastiengrignard  (1001)        0 2022-07-04 09:42:42.865543 serpyco-1.3.9/tests/
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)     2003 2022-07-04 09:37:35.000000 serpyco-1.3.9/tests/test_benchmarks.py
+-rw-rw-r--   0 sebastiengrignard  (1001) sebastiengrignard  (1001)    54944 2022-07-04 09:37:35.000000 serpyco-1.3.9/tests/test_unit.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `serpyco-1.3.8/.gitlab-ci.yml` & `serpyco-1.3.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/CHANGELOG.md` & `serpyco-1.3.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Serpyco changelog
 
+## v1.3.9
+
+- feat: update serializer.pyi to handle the `many` parameter in load and dump methods. This allows a better typing than having an `Union` as input/output of those methods. (courtesy of R. Pelloux-Prayer)
+
 ## v1.3.8
 
 - refactor: use `__dataclass_params__.frozen` to check whether a dataclass is frozen or not. This is more reliable than trying to set an attribute which can fail on custom dataclasses where `setattr` is redefined.
 
 ## v1.3.7
 
 - fix: support `NewType` by using their base type when serializing (courtesy of R. Pelloux-Prayer)
```

### Comparing `serpyco-1.3.8/LICENSE` & `serpyco-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/Makefile` & `serpyco-1.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/PKG-INFO` & `serpyco-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: serpyco
-Version: 1.3.8
+Version: 1.3.9
 Summary: Fast serialization of dataclasses using Cython
 Home-page: https://gitlab.com/sgrignard/serpyco
 Author: Sébastien Grignard
 Author-email: pub@amakaze.org
 License: MIT
 Description: ============================================
         Serpyco: a serializer for python dataclasses
```

### Comparing `serpyco-1.3.8/README.rst` & `serpyco-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/conf.py` & `serpyco-1.3.9/conf.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/docs/benchmark.rst` & `serpyco-1.3.9/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/docs/examples/complex_dump.py` & `serpyco-1.3.9/docs/examples/complex_dump.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/docs/examples/encoder.py` & `serpyco-1.3.9/docs/examples/encoder.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/docs/getting_started.rst` & `serpyco-1.3.9/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/requirements.txt` & `serpyco-1.3.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/__init__.py` & `serpyco-1.3.9/serpyco/__init__.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/decorator.py` & `serpyco-1.3.9/serpyco/decorator.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/encoder.pyx` & `serpyco-1.3.9/serpyco/encoder.pyx`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/exception.py` & `serpyco-1.3.9/serpyco/exception.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/field.py` & `serpyco-1.3.9/serpyco/field.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/mixin.py` & `serpyco-1.3.9/serpyco/mixin.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/schema.py` & `serpyco-1.3.9/serpyco/schema.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/serializer.pyi` & `serpyco-1.3.9/serpyco/serializer.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,82 @@
 import typing
 
 from .encoder import FieldEncoder
 from .util import JsonDict
 
 D = typing.TypeVar("D")
 
-DictOrIterable = typing.Union[JsonDict, typing.Iterable[JsonDict]]
-DictOrList = typing.Union[JsonDict, typing.List[JsonDict]]
-
 class Serializer(typing.Generic[D]):
     def __init__(
         self,
         dataclass: typing.Type[D],
-        omit_none: bool = True,
-        type_encoders: typing.Optional[typing.Dict[type, FieldEncoder]] = None,
-        only: typing.Optional[typing.List[str]] = None,
-        exclude: typing.Optional[typing.List[str]] = None,
-        strict: bool = False,
-        load_as_type: typing.Optional[type] = None,
+        omit_none: bool = ...,
+        type_encoders: typing.Optional[typing.Dict[type, FieldEncoder]] = ...,
+        only: typing.Optional[typing.List[str]] = ...,
+        exclude: typing.Optional[typing.List[str]] = ...,
+        strict: bool = ...,
+        load_as_type: typing.Optional[type] = ...,
     ) -> None: ...
-    def json_schema(self, many: bool = False) -> JsonDict: ...
+    def json_schema(self, many: bool = ...) -> JsonDict: ...
     def get_dict_path(self, obj_path: typing.Sequence[str]) -> typing.List[str]: ...
     def get_object_path(self, dict_path: typing.Sequence[str]) -> typing.List[str]: ...
     @classmethod
     def register_global_type(
         cls, field_type: typing.Any, encoder: FieldEncoder
     ) -> None: ...
     @classmethod
     def unregister_global_type(cls, field_type: typing.Any) -> None: ...
     def dataclass(self) -> type: ...
+    @typing.overload
+    def dump(
+        self,
+        obj: typing.Iterable[D],
+        validate: bool = ...,
+        many: typing.Literal[True] = ...,
+    ) -> typing.List[JsonDict]: ...
+    @typing.overload
+    def dump(
+        self,
+        obj: D,
+        validate: bool = ...,
+        many: typing.Literal[False] = ...,
+    ) -> JsonDict: ...
+    @typing.overload
     def dump(
         self,
         obj: typing.Union[D, typing.Iterable[D]],
-        validate: bool = False,
-        many: bool = False,
-    ) -> DictOrList: ...
+        validate: bool = ...,
+        many: bool = ...,
+    ) -> typing.Union[JsonDict, typing.List[JsonDict]]: ...
+    @typing.overload
     def load(
-        self, data: DictOrIterable, validate: bool = True, many: bool = False
+        self,
+        data: typing.Iterable[JsonDict],
+        validate: bool = ...,
+        many: typing.Literal[True] = ...,
+    ) -> typing.List[D]: ...
+    @typing.overload
+    def load(
+        self, data: JsonDict, validate: bool = ..., many: typing.Literal[False] = ...
+    ) -> D: ...
+    @typing.overload
+    def load(
+        self, data: JsonDict, validate: bool = ..., many: bool = ...
     ) -> typing.Union[D, typing.List[D]]: ...
     def dump_json(
         self,
         obj: typing.Union[D, typing.Iterable[D]],
-        validate: bool = False,
-        many: bool = False,
+        validate: bool = ...,
+        many: bool = ...,
     ) -> str: ...
+    @typing.overload
     def load_json(
-        self, js: str, validate: bool = True, many: bool = False
-    ) -> typing.Union[D, typing.List[D]]: ...
+        self, js: str, validate: bool = ..., many: typing.Literal[False] = ...
+    ) -> D: ...
+    @typing.overload
+    def load_json(
+        self, js: str, validate: bool = ..., many: typing.Literal[True] = ...
+    ) -> typing.List[D]: ...
+    @typing.overload
+    def load_json(
+        self, js: str, validate: bool = ..., many: bool = ...
+    ) -> typing.Union[typing.List[D], D]: ...
```

### Comparing `serpyco-1.3.8/serpyco/serializer.pyx` & `serpyco-1.3.9/serpyco/serializer.pyx`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/util.py` & `serpyco-1.3.9/serpyco/util.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco/validator.py` & `serpyco-1.3.9/serpyco/validator.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/serpyco.egg-info/PKG-INFO` & `serpyco-1.3.9/serpyco.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: serpyco
-Version: 1.3.8
+Version: 1.3.9
 Summary: Fast serialization of dataclasses using Cython
 Home-page: https://gitlab.com/sgrignard/serpyco
 Author: Sébastien Grignard
 Author-email: pub@amakaze.org
 License: MIT
 Description: ============================================
         Serpyco: a serializer for python dataclasses
```

### Comparing `serpyco-1.3.8/serpyco.egg-info/SOURCES.txt` & `serpyco-1.3.9/serpyco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/setup.py` & `serpyco-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/tests/test_benchmarks.py` & `serpyco-1.3.9/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `serpyco-1.3.8/tests/test_unit.py` & `serpyco-1.3.9/tests/test_unit.py`

 * *Files identical despite different names*

