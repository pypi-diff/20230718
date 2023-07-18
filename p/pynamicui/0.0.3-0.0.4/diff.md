# Comparing `tmp/pynamicui-0.0.3.tar.gz` & `tmp/pynamicui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.3.tar", last modified: Tue Jul 18 07:42:25 2023, max compression
+gzip compressed data, was "pynamicui-0.0.4.tar", last modified: Tue Jul 18 20:52:35 2023, max compression
```

## Comparing `pynamicui-0.0.3.tar` & `pynamicui-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.385733 pynamicui-0.0.3/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      775 2023-07-18 07:42:25.385733 pynamicui-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    17583 2023-07-18 07:39:19.000000 pynamicui-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.303646 pynamicui-0.0.3/pynamicui/
--rw-rw-rw-   0        0        0      386 2023-07-18 07:40:33.000000 pynamicui-0.0.3/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.356649 pynamicui-0.0.3/pynamicui/createDom/
--rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.3/pynamicui/createDom/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.3/pynamicui/createDom/createDom.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.374733 pynamicui-0.0.3/pynamicui/createElement/
--rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.3/pynamicui/createElement/__init__.py
--rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.3/pynamicui/createElement/createElement.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.382736 pynamicui-0.0.3/pynamicui/createStylesheet/
--rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.3/pynamicui/createStylesheet/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.3/pynamicui/createStylesheet/createStylesheet.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.337647 pynamicui-0.0.3/pynamicui.egg-info/
--rw-rw-rw-   0        0        0      775 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      779 2023-07-18 07:41:55.000000 pynamicui-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1185 2023-07-18 07:42:25.389735 pynamicui-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.514414 pynamicui-0.0.4/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      479 2023-07-18 20:52:35.515412 pynamicui-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4342 2023-07-18 08:45:35.000000 pynamicui-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.388892 pynamicui-0.0.4/pynamicui/
+-rw-rw-rw-   0        0        0      386 2023-07-18 20:51:38.000000 pynamicui-0.0.4/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.454410 pynamicui-0.0.4/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.4/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.4/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.478406 pynamicui-0.0.4/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.4/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.4/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.511414 pynamicui-0.0.4/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.4/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.4/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:52:35.429405 pynamicui-0.0.4/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 20:52:35.000000 pynamicui-0.0.4/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      779 2023-07-18 20:51:46.000000 pynamicui-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      904 2023-07-18 20:52:35.518413 pynamicui-0.0.4/setup.cfg
```

### Comparing `pynamicui-0.0.3/LICENSE` & `pynamicui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.3/pynamicui/createDom/createDom.py` & `pynamicui-0.0.4/pynamicui/createDom/createDom.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.3/pynamicui/createElement/createElement.py` & `pynamicui-0.0.4/pynamicui/createElement/createElement.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.3/pynamicui/createStylesheet/createStylesheet.py` & `pynamicui-0.0.4/pynamicui/createStylesheet/createStylesheet.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.3/pyproject.toml` & `pynamicui-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.3"
+current = "0.0.4"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

