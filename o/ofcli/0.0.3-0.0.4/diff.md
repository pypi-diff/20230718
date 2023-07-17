# Comparing `tmp/ofcli-0.0.3.tar.gz` & `tmp/ofcli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofcli-0.0.3.tar", last modified: Wed Jul  5 23:28:18 2023, max compression
+gzip compressed data, was "ofcli-0.0.4.tar", last modified: Mon Jul 17 22:39:22 2023, max compression
```

## Comparing `ofcli-0.0.3.tar` & `ofcli-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/
--rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-07-05 23:28:18.423761 ofcli-0.0.3/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      359 2023-06-23 09:35:20.000000 ofcli-0.0.3/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.0.3/pyproject.toml
--rw-r--r--   0 diana     (1000) diana     (1000)     1512 2023-07-05 23:28:18.423761 ofcli-0.0.3/setup.cfg
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/src/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-05 23:28:18.423761 ofcli-0.0.3/src/ofcli.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)     1688 2023-07-05 23:28:17.000000 ofcli-0.0.3/src/ofcli.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-05 23:28:17.000000 ofcli-0.0.3/src/ofcli.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-05 23:28:18.000000 ofcli-0.0.3/src/ofcli.egg-info/top_level.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4590 2023-07-17 22:39:22.253432 ofcli-0.0.4/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)     3261 2023-07-17 13:16:19.000000 ofcli-0.0.4/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.0.4/pyproject.toml
+-rw-r--r--   0 diana     (1000) diana     (1000)     1570 2023-07-17 22:39:22.256765 ofcli-0.0.4/setup.cfg
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/src/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/src/ofcli.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4590 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/top_level.txt
```

### Comparing `ofcli-0.0.3/setup.cfg` & `ofcli-0.0.4/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ofcli
-version = 0.0.3
+version = file: src/ofcli/VERSION
 summary = helper CLI tool for OIDC federation exploration
 description = helper tool for OIDC federation exploration
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Diana Gudu
 author_email = gudu@kit.edu
 home_page = https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
@@ -45,14 +45,17 @@
 	requests
 	cryptojwt
 	pygraphviz
 package_dir = 
 	=src
 packages = find:
 
+[options.package_data]
+ofcli = VERSION
+
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

