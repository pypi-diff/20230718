# Comparing `tmp/fourdigits-cli-1.2.1.tar.gz` & `tmp/fourdigits-cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourdigits-cli-1.2.1.tar", last modified: Tue Jun 20 08:05:17 2023, max compression
+gzip compressed data, was "fourdigits-cli-1.3.0.tar", last modified: Tue Jul 18 12:43:18 2023, max compression
```

## Comparing `fourdigits-cli-1.2.1.tar` & `fourdigits-cli-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.970934 fourdigits-cli-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-20 08:05:17.970934 fourdigits-cli-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.967934 fourdigits-cli-1.2.1/fourdigits_cli/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.969934 fourdigits-cli-1.2.1/fourdigits_cli/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5511 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/commands/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/commands/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.970934 fourdigits-cli-1.2.1/fourdigits_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/utils/docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/fourdigits_cli/utils/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.969934 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      625 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 08:05:17.000000 fourdigits-cli-1.2.1/fourdigits_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-20 08:05:17.971934 fourdigits-cli-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 08:05:17.970934 fourdigits-cli-1.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-20 08:04:12.000000 fourdigits-cli-1.2.1/tests/test_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.270327 fourdigits-cli-1.3.0/fourdigits_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.272328 fourdigits-cli-1.3.0/fourdigits_cli/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5511 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/commands/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.273327 fourdigits-cli-1.3.0/fourdigits_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/fourdigits_cli/utils/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.272328 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      625 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-18 12:43:18.000000 fourdigits-cli-1.3.0/fourdigits_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:43:18.274327 fourdigits-cli-1.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-07-18 12:42:13.000000 fourdigits-cli-1.3.0/tests/test_settings.py
```

### Comparing `fourdigits-cli-1.2.1/PKG-INFO` & `fourdigits-cli-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.2.1
+Version: 1.3.0
 Summary: FourDigits CLI tool
-Requires-Python: >= 3.7
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
 
 A command line tool to make development and deployment easier within Four Digits.
```

### Comparing `fourdigits-cli-1.2.1/README.md` & `fourdigits-cli-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/cli.py` & `fourdigits-cli-1.3.0/fourdigits_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/commands/docker.py` & `fourdigits-cli-1.3.0/fourdigits_cli/commands/docker.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/commands/gitlab.py` & `fourdigits-cli-1.3.0/fourdigits_cli/commands/gitlab.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/settings.py` & `fourdigits-cli-1.3.0/fourdigits_cli/settings.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/utils/docker.py` & `fourdigits-cli-1.3.0/fourdigits_cli/utils/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import subprocess
 
 logger = logging.getLogger(__name__)
 
 
 class DockerException(Exception):
     pass
@@ -75,27 +76,30 @@
         build_tag="",
         cache_from=None,
     ):
         logger.info(f"Docker build image {tag}")
         logger.info(f" - file={file}")
         logger.info(f" - context={context}")
         logger.info(f" - target={target}")
+        pip_extra_index_url = os.getenv(
+            "PIP_EXTRA_INDEX_URL", "https://overmind.fourdigits.nl/products/simple/"
+        )
         return self.run(
             list(
                 filter(
                     None,
                     [
                         "build",
                         "--pull",
                         f"--target={target}" if target else None,
                         f"--tag={tag}",
                         f"--file={file}",
                         f"--cache-from={cache_from}" if cache_from else None,
-                        "--build-arg",
-                        f"TAG={build_tag}",
+                        f"--build-arg=TAG={build_tag}",
+                        f"--build-arg=PIP_EXTRA_INDEX_URL={pip_extra_index_url}",
                         context,
                     ],
                 )
             )
         )
 
     def image_tag(self, tag, new_tag):
```

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli/utils/git.py` & `fourdigits-cli-1.3.0/fourdigits_cli/utils/git.py`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli.egg-info/PKG-INFO` & `fourdigits-cli-1.3.0/fourdigits_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fourdigits-cli
-Version: 1.2.1
+Version: 1.3.0
 Summary: FourDigits CLI tool
-Requires-Python: >= 3.7
+Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # FourDigits CLI
 
 A command line tool to make development and deployment easier within Four Digits.
```

### Comparing `fourdigits-cli-1.2.1/fourdigits_cli.egg-info/SOURCES.txt` & `fourdigits-cli-1.3.0/fourdigits_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourdigits-cli-1.2.1/setup.py` & `fourdigits-cli-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     packages=find_packages(include=["fourdigits_cli", "fourdigits_cli.*"]),
     entry_points={
         "console_scripts": [
             "fd = fourdigits_cli.cli:main",
             "fourdigits = fourdigits_cli.cli:main",
         ]
     },
-    python_requires=">= 3.7",
+    python_requires=">= 3.9",
     install_requires=[
         "click~=8.1.3",
         "tomli~=2.0.1",
         "packaging",
     ],
     extras_require={
         "dev": [
```

### Comparing `fourdigits-cli-1.2.1/tests/test_settings.py` & `fourdigits-cli-1.3.0/tests/test_settings.py`

 * *Files identical despite different names*

