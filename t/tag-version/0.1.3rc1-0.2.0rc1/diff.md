# Comparing `tmp/tag-version-0.1.3rc1.tar.gz` & `tmp/tag-version-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tag-version-0.1.3rc1.tar", last modified: Tue Jul 11 14:40:29 2023, max compression
+gzip compressed data, was "tag-version-0.2.0rc1.tar", last modified: Tue Jul 18 19:01:17 2023, max compression
```

## Comparing `tag-version-0.1.3rc1.tar` & `tag-version-0.2.0rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/
--rw-r--r--   0 root         (0) staff       (50)     5388 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/README.md
--rw-r--r--   0 root         (0) staff       (50)       38 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/setup.cfg
-drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/
-drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/
--rw-r--r--   0 root         (0) staff       (50)        1 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (50)      447 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (50)       61 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (50)      271 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (50)       11 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (50)       11 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/requires.txt
-drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tagversion/
--rw-r--r--   0 root         (0) staff       (50)      617 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/entrypoints.py
--rw-r--r--   0 root         (0) staff       (50)        0 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/__init__.py
--rw-r--r--   0 root         (0) staff       (50)     1709 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/argparse.py
--rw-r--r--   0 root         (0) staff       (50)      126 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/exceptions.py
--rw-r--r--   0 root         (0) staff       (50)    13650 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/git.py
--rw-r--r--   0 root         (0) staff       (50)     1834 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/write.py
--rw-r--r--   0 root         (0) staff       (50)     6481 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/version.py
--rw-r--r--   0 root         (0) staff       (50)      271 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/PKG-INFO
--rwxr-xr-x   0 root         (0) staff       (50)      623 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/setup.py
--rw-r--r--   0 root         (0) staff       (50)     1320 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5388 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      623 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/src/tag_version.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 19:01:17.000000 tag-version-0.2.0rc1/src/tag_version.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 19:01:17.736118 tag-version-0.2.0rc1/src/tagversion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/argparse.py
+-rw-r--r--   0 root         (0) root         (0)      617 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/entrypoints.py
+-rw-r--r--   0 root         (0) root         (0)      126 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13650 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/git.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/version.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-07-18 19:00:04.000000 tag-version-0.2.0rc1/src/tagversion/write.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tag-version-0.1.3rc1/README.md` & `tag-version-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/src/tagversion/entrypoints.py` & `tag-version-0.2.0rc1/src/tagversion/entrypoints.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/src/tagversion/argparse.py` & `tag-version-0.2.0rc1/src/tagversion/argparse.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/src/tagversion/git.py` & `tag-version-0.2.0rc1/src/tagversion/git.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/src/tagversion/write.py` & `tag-version-0.2.0rc1/src/tagversion/write.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/src/tagversion/version.py` & `tag-version-0.2.0rc1/src/tagversion/version.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.3rc1/setup.py` & `tag-version-0.2.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 SCRIPT_DIR = os.path.dirname(__file__)
 if not SCRIPT_DIR:
     SCRIPT_DIR = os.getcwd()
 
 
 setup(
     name="tag-version",
-    version="0.1.3rc1",
+    version="0.2.0rc1",
     description="semantic versioned git tags",
     author="DoubleVerify",
     author_email="code@doubleverify.com",
     url="https://github.com/openslate/tag-version",
     package_dir={"": "src"},
     packages=["tagversion"],
     install_requires=["sh==1.14.3"],
```

### Comparing `tag-version-0.1.3rc1/LICENSE` & `tag-version-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

