# Comparing `tmp/nics-3.0.0b0.tar.gz` & `tmp/nics-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-odb5mm82/nics-3.0.0b0.tar", last modified: Tue Jul 18 18:04:44 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-v1fqc1sb/nics-3.0.0b1.tar", last modified: Tue Jul 18 18:27:54 2023, max compression
```

## Comparing `nics-3.0.0b0.tar` & `nics-3.0.0b1.tar`

### file list

```diff
@@ -1,64 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 18:04:37.000000 nics-3.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 18:04:37.000000 nics-3.0.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:04:44.000000 nics-3.0.0b0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_init/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/ensure_nics_env_can_be_installed.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/get_user_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_init/loading/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/copy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/loading/workflow_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_init/print_outro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/cmd_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/cmd_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/404.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/settings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/logo200.png
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/2 - Pages/page.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/template/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics/main/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/ensure_a_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/favicon_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/is_nics_initialized.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics/main/utils/page404_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:04:44.000000 nics-3.0.0b0/nics_compiler/compiler/customize/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_config_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_constants_sass.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_favicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/custom_nav_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/customize/update_docs_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-18 18:04:37.000000 nics-3.0.0b0/nics_compiler/compiler/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 18:04:37.000000 nics-3.0.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 18:04:37.000000 nics-3.0.0b0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 18:04:44.000000 nics-3.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 18:04:37.000000 nics-3.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 18:27:46.000000 nics-3.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 18:27:46.000000 nics-3.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:27:54.000000 nics-3.0.0b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/cmd_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/ensure_nics_env_can_be_installed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/cmd_init/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/loading/copy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/loading/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/loading/workflow_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_init/print_outro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/cmd_upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/cmd_upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/settings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/template/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/template/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/2 - Pages/logo200.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/2 - Pages/page.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/template/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/template/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics/main/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/utils/ensure_a_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/utils/favicon_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/utils/is_nics_initialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 18:27:46.000000 nics-3.0.0b1/nics/main/utils/page404_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 18:27:54.000000 nics-3.0.0b1/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 18:27:46.000000 nics-3.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 18:27:46.000000 nics-3.0.0b1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 18:27:54.000000 nics-3.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 18:27:46.000000 nics-3.0.0b1/setup.py
```

### Comparing `nics-3.0.0b0/LICENSE` & `nics-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/PKG-INFO` & `nics-3.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-3.0.0b0/nics/main/__init__.py` & `nics-3.0.0b1/nics/main/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import logging
 
 from nics.main.constants import __version__
 from nics.main.cmd_init import run as run_init
 from nics.main.cmd_upgrade import run as run_upgrade
 
 
-logging.basicConfig(format='[%(asctime)s] <%(levelname)s>: %(message)s', datefmt='%H:%M:%S')
+logging.basicConfig(format='[%(asctime)s] %(levelname)s: %(message)s', datefmt='%H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
 def main():
 
     parser = argparse.ArgumentParser(
         usage=(
             '\n'
             '├─ Run `nics init`   : Set up NICS environment\n'
             '└─ Run `nics upgrade`: Reconfigure NICS environment'
         ),
         formatter_class=argparse.RawTextHelpFormatter  # to use line breaks (\n) in the help message
     )
     parser.add_argument('-v', '--version', action='version', version=f'nics-{__version__}', help='show software version')
-    parser.add_argument('-L', '--log-level', dest='log_level', choices=['debug', 'info', 'warning', 'error'], default='info')
+    parser.add_argument('-L', dest='log_level', choices=['debug', 'info', 'warning', 'error'], default='info', help='Set the log level (default: %(default)s)')
     parser.add_argument('cmd', choices=['init', 'upgrade'], help=argparse.SUPPRESS)  # `help=argparse.SUPPRESS` to hide the default help message
 
     args = parser.parse_args()
     logger.setLevel(getattr(logging, args.log_level.upper()))
 
     logger.debug(f'Running {repr(args.cmd)} command.')
     if args.cmd == 'init':
```

### Comparing `nics-3.0.0b0/nics/main/cmd_init/__init__.py` & `nics-3.0.0b1/nics/main/cmd_init/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/ensure_nics_env_can_be_installed.py` & `nics-3.0.0b1/nics/main/cmd_init/ensure_nics_env_can_be_installed.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/get_user_details.py` & `nics-3.0.0b1/nics/main/cmd_init/get_user_details.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/loading/__init__.py` & `nics-3.0.0b1/nics/main/cmd_init/loading/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/loading/settings_writer.py` & `nics-3.0.0b1/nics/main/cmd_init/loading/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/loading/workflow_writer.py` & `nics-3.0.0b1/nics/main/cmd_init/loading/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/cmd_init/print_outro.py` & `nics-3.0.0b1/nics/main/cmd_init/print_outro.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/constants.py` & `nics-3.0.0b1/nics/main/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ROOT_DIR_PTH = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 DIST_DIR_PTH = os.path.join(ROOT_DIR_PTH, 'nics')
 MAIN_DIR_PTH = os.path.join(ROOT_DIR_PTH, 'nics', 'main')
 NICS_COMPILER_DIR_PTH = os.path.join(ROOT_DIR_PTH, 'nics-compiler')
 
-TEMPLATE_DOCS_DIR_PTH = os.path.join(ROOT_DIR_PTH, 'nics', 'template')
+TEMPLATE_DOCS_DIR_PTH = os.path.join(ROOT_DIR_PTH, 'nics', 'main', 'template')
 TEMPLATE_WEB_DIR_PTH  = os.path.join(ROOT_DIR_PTH, 'nics-compiler', 'template')
 
 SETTINGS_KEYS = [
     'author',
     'color_hue',
     'lowercase_the_url',
     'show_credit',
```

### Comparing `nics-3.0.0b0/nics/main/template/tree/2 - Pages/logo200.png` & `nics-3.0.0b1/nics/main/template/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/utils/favicon_maker.py` & `nics-3.0.0b1/nics/main/utils/favicon_maker.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/utils/is_nics_initialized.py` & `nics-3.0.0b1/nics/main/utils/is_nics_initialized.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics/main/utils/page404_maker.py` & `nics-3.0.0b1/nics/main/utils/page404_maker.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b0/nics.egg-info/PKG-INFO` & `nics-3.0.0b1/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 3.0.0b0
+Version: 3.0.0b1
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-3.0.0b0/nics.egg-info/SOURCES.txt` & `nics-3.0.0b1/nics.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,8 @@
 nics/main/template/tree/2 - Pages/logo200.png
 nics/main/template/tree/2 - Pages/page.md
 nics/main/template/tree/7 - FAQs/1 - Question1.md
 nics/main/template/tree/7 - FAQs/index.md
 nics/main/utils/ensure_a_git_repo.py
 nics/main/utils/favicon_maker.py
 nics/main/utils/is_nics_initialized.py
-nics/main/utils/page404_maker.py
-nics_compiler/compiler/__init__.py
-nics_compiler/compiler/__main__.py
-nics_compiler/compiler/docking.py
-nics_compiler/compiler/customize/__init__.py
-nics_compiler/compiler/customize/custom_config_yml.py
-nics_compiler/compiler/customize/custom_constants_sass.py
-nics_compiler/compiler/customize/custom_favicon.py
-nics_compiler/compiler/customize/custom_nav_html.py
-nics_compiler/compiler/customize/update_docs_tree.py
+nics/main/utils/page404_maker.py
```

### Comparing `nics-3.0.0b0/pyproject.toml` & `nics-3.0.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "3.0.0b0"
+version = "3.0.0b1"
 description = "Automated markdown-based documentation page workflow"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
@@ -28,15 +28,15 @@
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "archive*",
     "assets*",
     "docs*",
-    "nics-compiler*",
+    "nics_compiler*",
     "tests*",
 ]
 
 
 [project.urls]
 Documentation = "https://nvfp.github.io/now-i-can-sleep/docs"
 "Report bugs" = "https://github.com/nvfp/now-i-can-sleep/issues"
```

### Comparing `nics-3.0.0b0/readme.md` & `nics-3.0.0b1/readme.md`

 * *Files identical despite different names*

