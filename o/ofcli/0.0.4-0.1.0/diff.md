# Comparing `tmp/ofcli-0.0.4.tar.gz` & `tmp/ofcli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofcli-0.0.4.tar", last modified: Mon Jul 17 22:39:22 2023, max compression
+gzip compressed data, was "ofcli-0.1.0.tar", last modified: Tue Jul 18 10:50:42 2023, max compression
```

## Comparing `ofcli-0.0.4.tar` & `ofcli-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/
--rw-r--r--   0 diana     (1000) diana     (1000)     4590 2023-07-17 22:39:22.253432 ofcli-0.0.4/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)     3261 2023-07-17 13:16:19.000000 ofcli-0.0.4/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.0.4/pyproject.toml
--rw-r--r--   0 diana     (1000) diana     (1000)     1570 2023-07-17 22:39:22.256765 ofcli-0.0.4/setup.cfg
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/src/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-17 22:39:22.253432 ofcli-0.0.4/src/ofcli.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)     4590 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-17 22:39:21.000000 ofcli-0.0.4/src/ofcli.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-17 22:39:22.000000 ofcli-0.0.4/src/ofcli.egg-info/top_level.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-18 10:50:42.683079 ofcli-0.1.0/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-07-18 10:50:42.683079 ofcli-0.1.0/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)     3279 2023-07-17 22:44:14.000000 ofcli-0.1.0/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)      106 2023-06-25 09:29:29.000000 ofcli-0.1.0/pyproject.toml
+-rw-r--r--   0 diana     (1000) diana     (1000)     1570 2023-07-18 10:50:42.683079 ofcli-0.1.0/setup.cfg
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-18 10:50:42.679746 ofcli-0.1.0/src/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-07-18 10:50:42.683079 ofcli-0.1.0/src/ofcli.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)     4608 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)      234 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       46 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       50 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-07-18 10:50:42.000000 ofcli-0.1.0/src/ofcli.egg-info/top_level.txt
```

### Comparing `ofcli-0.0.4/PKG-INFO` & `ofcli-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.0.4
+Version: 0.1.0
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
@@ -95,18 +95,18 @@
   --help                      Show this message and exit.
 ```
 
 ## Development
 
 ### Installing the development version
 
-The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
+The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
 
 ```bash
-git clone https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
+git clone https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli
 cd ofcli
 pip install -e .
 ```
 
 ### Versioning
 
 Versions are managed by `bump2version`. To bump the version, run:
```

### Comparing `ofcli-0.0.4/README.md` & `ofcli-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -64,18 +64,18 @@
   --help                      Show this message and exit.
 ```
 
 ## Development
 
 ### Installing the development version
 
-The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
+The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
 
 ```bash
-git clone https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
+git clone https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli
 cd ofcli
 pip install -e .
 ```
 
 ### Versioning
 
 Versions are managed by `bump2version`. To bump the version, run:
```

### Comparing `ofcli-0.0.4/setup.cfg` & `ofcli-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ofcli-0.0.4/src/ofcli.egg-info/PKG-INFO` & `ofcli-0.1.0/src/ofcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofcli
-Version: 0.0.4
+Version: 0.1.0
 Summary: helper CLI tool for OIDC federation exploration
 Home-page: https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
 Author: Diana Gudu
 Author-email: gudu@kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli/issues
 Classifier: Development Status :: 3 - Alpha
@@ -95,18 +95,18 @@
   --help                      Show this message and exit.
 ```
 
 ## Development
 
 ### Installing the development version
 
-The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
+The development version of `ofcli` can be installed from the `main` branch of the [git repository](https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli) and can be installed as follows (note the `-e` switch to install it in editable or "develop mode"):
 
 ```bash
-git clone https://gitlab.geant.org/TI_Incubator/oidcfed/ofcli
+git clone https://gitlab.software.geant.org/TI_Incubator/oidcfed/ofcli
 cd ofcli
 pip install -e .
 ```
 
 ### Versioning
 
 Versions are managed by `bump2version`. To bump the version, run:
```

