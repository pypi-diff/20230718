# Comparing `tmp/viur_cli-1.0.8.tar.gz` & `tmp/viur_cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.8.tar", last modified: Tue Jul 11 16:56:52 2023, max compression
+gzip compressed data, was "viur_cli-1.0.9.tar", last modified: Wed Jul 12 05:08:50 2023, max compression
```

## Comparing `viur_cli-1.0.8.tar` & `viur_cli-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 16:56:36.000000 viur_cli-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 16:56:52.370766 viur_cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-11 16:56:36.000000 viur_cli-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 16:56:36.000000 viur_cli-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 16:56:52.370766 viur_cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 16:56:36.000000 viur_cli-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.358766 viur_cli-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/npm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.370766 viur_cli-1.0.8/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:56:36.000000 viur_cli-1.0.8/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:56:52.366766 viur_cli-1.0.8/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 16:56:52.000000 viur_cli-1.0.8/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.354654 viur_cli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-12 05:08:41.000000 viur_cli-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-12 05:08:50.354654 viur_cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-12 05:08:41.000000 viur_cli-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 05:08:41.000000 viur_cli-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-12 05:08:50.354654 viur_cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-12 05:08:41.000000 viur_cli-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.350654 viur_cli-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.350654 viur_cli-1.0.9/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.354654 viur_cli-1.0.9/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.354654 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.354654 viur_cli-1.0.9/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 05:08:41.000000 viur_cli-1.0.9/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 05:08:50.350654 viur_cli-1.0.9/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 05:08:50.000000 viur_cli-1.0.9/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.8/LICENSE` & `viur_cli-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/PKG-INFO` & `viur_cli-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 1.0.8 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 1.0.9 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.8/README.md` & `viur_cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/setup.cfg` & `viur_cli-1.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/build.py` & `viur_cli-1.0.9/src/viur_cli/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Performs build steps configured within the project, or creates any necessary steps for a project deployment build.
 """
 
-import click, os, zipfile, shutil, urllib, json
-from urllib.request import urlretrieve
-from . import cli, conf, utils, get_config, write_config
+import click, os
+from . import cli, conf, utils
 
 
 def _build(cfg, name, build_cfg, additional_args):
     """Internal function to perform steps required for a given build configuration.
 
     :param cfg: The project configuration (default, or project-specific)
     :param name: Name of the app to build.
@@ -71,22 +70,22 @@
 
     match build_cfg["kind"]:
         # for flare and npm, drop the target folder and node_modules (npm)
         case "flare" | "npm":
             if target_dir := build_cfg.get("target"):
                 target_dir = os.path.join(cfg["distribution_folder"], target_dir)
                 utils.echo_info(f"  - dropping {target_dir}")
-                shutil.rmtree(target_dir)
+                utils.rmdir(target_dir)
 
             if build_cfg["kind"] == "npm":
                 # todo: Later, call "npm run clean" or a similar command when it exists
 
                 node_modules = os.path.join(cfg["sources_folder"], build_cfg["source"], "node_modules")
                 utils.echo_info(f"  - dropping {node_modules}")
-                shutil.rmtree(os.path.join(node_modules))
+                utils.rmdir(os.path.join(node_modules))
 
         case "exec":
             pass
 
         case other:
             utils.echo_fatal(f"Unknown build kind {other!r}")
```

### Comparing `viur_cli-1.0.8/src/viur_cli/cli.py` & `viur_cli-1.0.9/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/conf.py` & `viur_cli-1.0.9/src/viur_cli/conf.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/deploy.py` & `viur_cli-1.0.9/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/flare.py` & `viur_cli-1.0.9/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/install.py` & `viur_cli-1.0.9/src/viur_cli/install.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/local.py` & `viur_cli-1.0.9/src/viur_cli/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import click, os, shutil, subprocess, json
+import click, os, shutil, subprocess
 from . import cli, echo_error, get_config, utils
 from .install import vi as vi_install
 
 
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("name", default='develop')
 @click.argument("additional_args", nargs=-1)
@@ -13,15 +13,15 @@
     if name not in projectConfig:
         echo_error(f"{name} is not a valid config name.")
         return
 
     conf = projectConfig["default"].copy()
     conf.update(projectConfig[name])
 
-    os.system(f'app_server -A={conf["application_name"]} {conf["distribution_folder"]} {" ".join(additional_args)}')
+    utils.system(f'app_server -A={conf["application_name"]} {conf["distribution_folder"]} {" ".join(additional_args)}')
 
 
 @cli.command()
 def env():
     """check local Environment"""
     valid_icon = "\U00002714"
     failed_icon = "\U0000274C"
@@ -119,57 +119,59 @@
 @cli.command()
 @click.argument("version", default="latest")
 @click.option('--next', '-n', 'next_',  is_flag=True, default=False)
 def vi(version, next_):
     """DEPRECATED please use viur install vi"""
     utils.echo_info("DEPRECATED please use: viur install vi")
     if next_:
-        os.system(f'viur install vi --next')
+        utils.system(f'viur install vi --next')
     else:
-        os.system(f'viur install vi')
+        utils.system(f'viur install vi')
 
 @cli.command()
 @click.option('--dev', '-d', is_flag=True, default=False)
 def check(dev):
     """do security checks"""
     if do_checks(dev):
         utils.echo_info("\U00002714 No vulnerabilities found.")
 
 def do_checks(dev=True):
+    all_checks_passed = True
 
-    all_checks_passed=True
-    result = subprocess.check_output(['pipenv', 'check','--output', 'minimal','--continue-on-error']).decode("utf-8")
-    if "0 vulnerabilities found." in result:
-        pass
-    else:
-        os.system("pipenv check")
-        all_checks_passed=False
+    # Check Pipenv vulnerabilities
+
+    result = subprocess.check_output("pipenv check --output minimal --continue-on-error".split())
+    if "0 vulnerabilities found." not in result.decode("utf-8"):
+        utils.system("pipenv check")
+        all_checks_passed = False
 
     if dev:
-        result = subprocess.check_output(['pipenv', 'check','--output', 'minimal', "--categories", "develop",'--continue-on-error']).decode("utf-8")
-        if "0 vulnerabilities found." in result:
-            pass
-        else:
-            os.system("pipenv check --categories develop")
-            all_checks_passed=False
+        result = subprocess.check_output(
+            "pipenv check --output minimal --categories develop --continue-on-error".split()
+        )
+
+        if "0 vulnerabilities found." not in result.decode("utf-8"):
+            utils.system("pipenv check --categories develop")
+            all_checks_passed = False
 
+    # Check npm vulnerabilities for all npm builds
 
     projectConfig = get_config()
     cfg = projectConfig["default"].copy()
     if builds_cfg := cfg.get("builds"):
         if npm_apps := [k for k,v in builds_cfg.items() if builds_cfg[k]["kind"] == "npm"]:
             for name in npm_apps:
+                path = os.path.join(cfg["sources_folder"], builds_cfg[name]["source"])
+
                 if dev:
-                    result = subprocess.check_output(['npm', 'audit','--prefix',cfg["sources_folder"]+builds_cfg[name]["source"]]).decode("utf-8")
+                    result = subprocess.check_output(("npm", "audit", "--prefix", path))
                 else:
-                    result = subprocess.check_output(['npm', 'audit','--omit','dev', '--prefix',cfg["sources_folder"]+builds_cfg[name]["source"]]).decode("utf-8")
-                if "found 0 vulnerabilities" in result:
+                    result = subprocess.check_output(("npm", "audit", "--omit", "dev", "--prefix", path))
+
+                if "found 0 vulnerabilities" in result.decode("utf-8"):
                     pass
                 else:
                     utils.echo_info(f"checking {name}...")
-                    os.system(f'cd {cfg["sources_folder"]}{builds_cfg[name]["source"]} && npm audit')
-                    all_checks_passed=False
-
-    if all_checks_passed:
-        return True
+                    utils.system(f'cd {path} && npm audit')
+                    all_checks_passed = False
 
-    return False
+    return all_checks_passed
```

### Comparing `viur_cli-1.0.8/src/viur_cli/npm.py` & `viur_cli-1.0.9/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.9/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.9/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.9/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.9/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/setup.py` & `viur_cli-1.0.9/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/tool.py` & `viur_cli-1.0.9/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.8/src/viur_cli/utils.py` & `viur_cli-1.0.9/src/viur_cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,27 @@
-import os, click, sys, typing, datetime, getpass
+import os, shutil, click, sys, typing, datetime, getpass
+
+
+def rmdir(dir):
+    """Secure and error-prone recursive removal of entire folders.
+
+    Does only allow to remove folders inside the project folder, so that a misconfiguration, wanted or not,
+    cannot delete the entire home folder or similar.
+    """
+    # Verify the dir is part of the current folder
+    dir = os.path.abspath(dir)
+    wdir = os.getcwd()
+    if wdir != os.path.commonpath((wdir, dir)):
+        echo_fatal(f"Illegal path configuration, won't remove {dir!r}")
+
+    # Remove it
+    try:
+        shutil.rmtree(dir)
+    except FileNotFoundError:
+        pass
 
 
 def system(cmd):
     """Performs an os.system() call with the given command, but throws an echo_fatal on error and stops viur-cli."""
     if os.system(cmd) != 0:
         echo_fatal(f"Failed to execute {cmd!r}")
```

### Comparing `viur_cli-1.0.8/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-1.0.9/src/viur_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-cli
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-cli Version: 1.0.8 Summary: Command-line
+Metadata-Version: 2.1 Name: viur-cli Version: 1.0.9 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.8/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.9/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

