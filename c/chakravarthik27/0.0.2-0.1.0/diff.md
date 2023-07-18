# Comparing `tmp/chakravarthik27-0.0.2.tar.gz` & `tmp/chakravarthik27-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chakravarthik27-0.0.2.tar", last modified: Wed Dec 28 18:12:50 2022, max compression
+gzip compressed data, was "chakravarthik27-0.1.0.tar", max compression
```

## Comparing `chakravarthik27-0.0.2.tar` & `chakravarthik27-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,4 @@
-drwxrwxrwx   0        0        0        0 2022-12-28 18:12:50.027011 chakravarthik27-0.0.2/
--rw-rw-rw-   0        0        0     1064 2022-12-28 16:45:06.000000 chakravarthik27-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      676 2022-12-28 18:12:50.021430 chakravarthik27-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       60 2022-12-28 17:26:09.000000 chakravarthik27-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-28 18:12:49.997357 chakravarthik27-0.0.2/chakravarthik27/
--rw-rw-rw-   0        0        0       39 2022-12-28 18:12:05.000000 chakravarthik27-0.0.2/chakravarthik27/__init__.py
--rw-rw-rw-   0        0        0      315 2022-12-28 17:29:34.000000 chakravarthik27-0.0.2/chakravarthik27/searchresults.py
-drwxrwxrwx   0        0        0        0 2022-12-28 18:12:50.019083 chakravarthik27-0.0.2/chakravarthik27.egg-info/
--rw-rw-rw-   0        0        0      676 2022-12-28 18:12:49.000000 chakravarthik27-0.0.2/chakravarthik27.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-12-28 18:12:49.000000 chakravarthik27-0.0.2/chakravarthik27.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-28 18:12:49.000000 chakravarthik27-0.0.2/chakravarthik27.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-12-28 18:12:49.000000 chakravarthik27-0.0.2/chakravarthik27.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-12-28 18:12:49.000000 chakravarthik27-0.0.2/chakravarthik27.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-28 18:12:50.027011 chakravarthik27-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2022-12-28 17:58:29.000000 chakravarthik27-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:25:18.294329 chakravarthik27-0.1.0/chakravarthik27/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-18 06:25:18.302328 chakravarthik27-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-18 06:25:18.294329 chakravarthik27-0.1.0/README.md
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 chakravarthik27-0.1.0/PKG-INFO
```

