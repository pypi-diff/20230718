# Comparing `tmp/example_client-0.0.1.tar.gz` & `tmp/example_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_client-0.0.1.tar", last modified: Thu Jul 13 22:44:01 2023, max compression
+gzip compressed data, was "example_client-0.0.2.tar", last modified: Tue Jul 18 17:43:29 2023, max compression
```

## Comparing `example_client-0.0.1.tar` & `example_client-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-13 22:44:01.425242 example_client-0.0.1/
--rw-r--r--   0 wayne      (501) staff       (20)      319 2023-07-13 22:44:01.424723 example_client-0.0.1/PKG-INFO
-drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-13 22:44:01.421787 example_client-0.0.1/example_client/
--rw-r--r--   0 wayne      (501) staff       (20)     4081 2023-07-12 20:28:47.000000 example_client-0.0.1/example_client/__init__.py
-drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-13 22:44:01.423918 example_client-0.0.1/example_client.egg-info/
--rw-r--r--   0 wayne      (501) staff       (20)      319 2023-07-13 22:44:01.000000 example_client-0.0.1/example_client.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (501) staff       (20)      224 2023-07-13 22:44:01.000000 example_client-0.0.1/example_client.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (501) staff       (20)        1 2023-07-13 22:44:01.000000 example_client-0.0.1/example_client.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (501) staff       (20)      154 2023-07-13 22:44:01.000000 example_client-0.0.1/example_client.egg-info/requires.txt
--rw-r--r--   0 wayne      (501) staff       (20)       15 2023-07-13 22:44:01.000000 example_client-0.0.1/example_client.egg-info/top_level.txt
--rw-r--r--   0 wayne      (501) staff       (20)       38 2023-07-13 22:44:01.425493 example_client-0.0.1/setup.cfg
--rw-r--r--   0 wayne      (501) staff       (20)     1165 2023-07-13 22:43:47.000000 example_client-0.0.1/setup.py
+drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-18 17:43:29.632396 example_client-0.0.2/
+-rw-r--r--   0 wayne      (501) staff       (20)      319 2023-07-18 17:43:29.631824 example_client-0.0.2/PKG-INFO
+drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-18 17:43:29.627743 example_client-0.0.2/example_client/
+-rw-r--r--   0 wayne      (501) staff       (20)     4081 2023-07-18 17:40:47.000000 example_client-0.0.2/example_client/__init__.py
+drwxr-xr-x   0 wayne      (501) staff       (20)        0 2023-07-18 17:43:29.630935 example_client-0.0.2/example_client.egg-info/
+-rw-r--r--   0 wayne      (501) staff       (20)      319 2023-07-18 17:43:29.000000 example_client-0.0.2/example_client.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (501) staff       (20)      224 2023-07-18 17:43:29.000000 example_client-0.0.2/example_client.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (501) staff       (20)        1 2023-07-18 17:43:29.000000 example_client-0.0.2/example_client.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (501) staff       (20)      159 2023-07-18 17:43:29.000000 example_client-0.0.2/example_client.egg-info/requires.txt
+-rw-r--r--   0 wayne      (501) staff       (20)       15 2023-07-18 17:43:29.000000 example_client-0.0.2/example_client.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (501) staff       (20)       38 2023-07-18 17:43:29.632631 example_client-0.0.2/setup.cfg
+-rw-r--r--   0 wayne      (501) staff       (20)     1170 2023-07-18 17:43:13.000000 example_client-0.0.2/setup.py
```

### Comparing `example_client-0.0.1/example_client/__init__.py` & `example_client-0.0.2/example_client/__init__.py`

 * *Files identical despite different names*

### Comparing `example_client-0.0.1/setup.py` & `example_client-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 here = pathlib.Path(__file__).parent.resolve()
 readme = here / "readme.md"
 long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
 
 setup(
     name="example_client",
-    version="0.0.1",
+    version="0.0.2",
     description="Example Discovery Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BWRC-AMS-ML-Discovery",
     author="The Regents of the University of California",
     author_email="whh.bear@berkeley.edu",
     packages=find_packages(),
     python_requires=">=3.7, <4",
     install_requires=[
         "hdl21>=3.0.1",
         "python-dotenv==1.0.0",
-        "discovery_client==0.0.1",
+        "bwrc_discovery_client==0.0.1",
         "example_shared==0.0.1",
     ],
     extras_require={
         "dev": [
             "pytest==7.1",
             "coverage",
             "pytest-cov",
```

