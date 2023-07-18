# Comparing `tmp/pynamicui-0.0.1.tar.gz` & `tmp/pynamicui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pynamicui-0.0.2.tar", last modified: Tue Jul 18 07:36:37 2023, max compression
```

## Comparing `pynamicui-0.0.1.tar` & `pynamicui-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pynamicui-0.0.1/requirements.txt
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createDom/__init__.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createDom/createDom.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createElement/__init__.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createElement/createElement.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createStylesheet/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 pynamicui-0.0.1/src/pynamicui/createStylesheet/createStylesheet.py
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 pynamicui-0.0.1/tests/example.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pynamicui-0.0.1/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 pynamicui-0.0.1/LICENSE
--rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 pynamicui-0.0.1/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 pynamicui-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    17906 2020-02-02 00:00:00.000000 pynamicui-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.806503 pynamicui-0.0.2/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      775 2023-07-18 07:36:37.807505 pynamicui-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17677 2023-07-18 01:40:07.000000 pynamicui-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.760503 pynamicui-0.0.2/pynamicui/
+-rw-rw-rw-   0        0        0      386 2023-07-18 07:32:34.000000 pynamicui-0.0.2/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.804508 pynamicui-0.0.2/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      779 2023-07-18 07:32:57.000000 pynamicui-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1108 2023-07-18 07:36:37.811506 pynamicui-0.0.2/setup.cfg
```

### Comparing `pynamicui-0.0.1/LICENSE` & `pynamicui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.1/README.md` & `pynamicui-0.0.2/README.md`

 * *Files identical despite different names*

