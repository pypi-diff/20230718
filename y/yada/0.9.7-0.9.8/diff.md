# Comparing `tmp/yada-0.9.7.tar.gz` & `tmp/yada-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yada-0.9.7.tar", last modified: Wed Feb  3 19:38:56 2021, max compression
+gzip compressed data, was "yada-0.9.8.tar", last modified: Tue Jul 18 18:43:59 2023, max compression
```

## Comparing `yada-0.9.7.tar` & `yada-0.9.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.511376 yada-0.9.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (117)      571 2021-02-03 19:38:47.000000 yada-0.9.7/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (117)      991 2021-02-03 19:38:47.000000 yada-0.9.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (117)     1736 2021-02-03 19:38:47.000000 yada-0.9.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (117)      154 2021-02-03 19:38:47.000000 yada-0.9.7/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (117)      683 2021-02-03 19:38:56.515375 yada-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      234 2021-02-03 19:38:47.000000 yada-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (117)       63 2021-02-03 19:38:56.515375 yada-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)     1846 2021-02-03 19:38:47.000000 yada-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.511376 yada-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/src/yada/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/src/yada/cli/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)     8081 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (117)     1013 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/config.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/src/yada/data/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)      152 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/data/config.yaml
--rw-r--r--   0 runner    (1001) docker     (117)       43 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (117)      976 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/platform.py
--rw-r--r--   0 runner    (1001) docker     (117)     6164 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/repo.py
--rw-r--r--   0 runner    (1001) docker     (117)     3800 2021-02-03 19:38:47.000000 yada-0.9.7/src/yada/xdg.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/src/yada.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)      683 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      554 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       44 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (117)      330 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)        5 2021-02-03 19:38:56.000000 yada-0.9.7/src/yada.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-03 19:38:56.515375 yada-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (117)      449 2021-02-03 19:38:47.000000 yada-0.9.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (117)     1964 2021-02-03 19:38:47.000000 yada-0.9.7/tests/test_repo.py
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.135016 yada-0.9.8/
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.131514 yada-0.9.8/.github/
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.132630 yada-0.9.8/.github/workflows/
+-rw-r--r--   0 apetresc   (502) staff       (20)      571 2023-07-17 20:57:06.000000 yada-0.9.8/.github/workflows/package.yml
+-rw-r--r--   0 apetresc   (502) staff       (20)      991 2023-07-17 20:57:06.000000 yada-0.9.8/.github/workflows/test.yml
+-rw-r--r--   0 apetresc   (502) staff       (20)     1736 2023-07-17 20:57:06.000000 yada-0.9.8/.gitignore
+-rw-r--r--   0 apetresc   (502) staff       (20)      154 2023-07-17 20:57:06.000000 yada-0.9.8/.travis.yml
+-rw-r--r--   0 apetresc   (502) staff       (20)      579 2023-07-18 18:43:59.135100 yada-0.9.8/PKG-INFO
+-rw-r--r--   0 apetresc   (502) staff       (20)      234 2023-07-17 20:57:06.000000 yada-0.9.8/README.md
+-rw-r--r--   0 apetresc   (502) staff       (20)       63 2023-07-18 18:43:59.135376 yada-0.9.8/setup.cfg
+-rw-r--r--   0 apetresc   (502) staff       (20)     1891 2023-07-18 18:36:00.000000 yada-0.9.8/setup.py
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.131682 yada-0.9.8/src/
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.133324 yada-0.9.8/src/yada/
+-rw-r--r--   0 apetresc   (502) staff       (20)        0 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/__init__.py
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.134228 yada-0.9.8/src/yada/cli/
+-rw-r--r--   0 apetresc   (502) staff       (20)        0 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/cli/__init__.py
+-rw-r--r--   0 apetresc   (502) staff       (20)     8081 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/cli/main.py
+-rw-r--r--   0 apetresc   (502) staff       (20)     1013 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/config.py
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.134423 yada-0.9.8/src/yada/data/
+-rw-r--r--   0 apetresc   (502) staff       (20)        0 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/data/__init__.py
+-rw-r--r--   0 apetresc   (502) staff       (20)      152 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/data/config.yaml
+-rw-r--r--   0 apetresc   (502) staff       (20)       43 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/exceptions.py
+-rw-r--r--   0 apetresc   (502) staff       (20)      976 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/platform.py
+-rw-r--r--   0 apetresc   (502) staff       (20)     6164 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/repo.py
+-rw-r--r--   0 apetresc   (502) staff       (20)     3800 2023-07-17 20:57:06.000000 yada-0.9.8/src/yada/xdg.py
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.134020 yada-0.9.8/src/yada.egg-info/
+-rw-r--r--   0 apetresc   (502) staff       (20)      579 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/PKG-INFO
+-rw-r--r--   0 apetresc   (502) staff       (20)      554 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/SOURCES.txt
+-rw-r--r--   0 apetresc   (502) staff       (20)        1 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/dependency_links.txt
+-rw-r--r--   0 apetresc   (502) staff       (20)       43 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/entry_points.txt
+-rw-r--r--   0 apetresc   (502) staff       (20)      342 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/requires.txt
+-rw-r--r--   0 apetresc   (502) staff       (20)        5 2023-07-18 18:43:59.000000 yada-0.9.8/src/yada.egg-info/top_level.txt
+drwxr-xr-x   0 apetresc   (502) staff       (20)        0 2023-07-18 18:43:59.134874 yada-0.9.8/tests/
+-rw-r--r--   0 apetresc   (502) staff       (20)      449 2023-07-17 20:57:06.000000 yada-0.9.8/tests/test_cli.py
+-rw-r--r--   0 apetresc   (502) staff       (20)     1964 2023-07-17 20:57:06.000000 yada-0.9.8/tests/test_repo.py
```

### Comparing `yada-0.9.7/.github/workflows/package.yml` & `yada-0.9.8/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/.github/workflows/test.yml` & `yada-0.9.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/.gitignore` & `yada-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/setup.py` & `yada-0.9.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRES_PYTHON = '>=2.7.15, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*'
 
 REQUIRED = [
     'future>=0.16.0',
     'six>=1.10.0',
     'Click>=7.0,<8.0',
     'pathlib2==2.3.3;python_version<"3.4"',
-    'pyyaml>=3.12,<6.0',
+    "pyyaml!=6.0.0,!=5.4.0,!=5.4.1", # pyyaml is broken with cython 3
 ]
 
 SETUP_REQUIRED = [
     'setuptools_scm'
 ]
 
 EXTRAS = {
```

### Comparing `yada-0.9.7/src/yada/cli/main.py` & `yada-0.9.8/src/yada/cli/main.py`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/src/yada/config.py` & `yada-0.9.8/src/yada/config.py`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/src/yada/platform.py` & `yada-0.9.8/src/yada/platform.py`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/src/yada/repo.py` & `yada-0.9.8/src/yada/repo.py`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/src/yada/xdg.py` & `yada-0.9.8/src/yada/xdg.py`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/src/yada.egg-info/SOURCES.txt` & `yada-0.9.8/src/yada.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yada-0.9.7/tests/test_repo.py` & `yada-0.9.8/tests/test_repo.py`

 * *Files identical despite different names*

