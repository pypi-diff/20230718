# Comparing `tmp/nics-3.0.0b5.tar.gz` & `tmp/nics-3.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-3vkmc6n6/nics-3.0.0b5.tar", last modified: Tue Jul 18 20:25:29 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-iotu87ee/nics-3.0.0b6.tar", last modified: Tue Jul 18 20:31:56 2023, max compression
```

## Comparing `nics-3.0.0b5.tar` & `nics-3.0.0b6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 20:25:23.000000 nics-3.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 20:25:23.000000 nics-3.0.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 20:25:29.000000 nics-3.0.0b5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/cmd_init/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/ensure_nics_env_can_be_installed.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/get_user_details.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/cmd_init/loading/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/loading/copy_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/loading/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/loading/workflow_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_init/print_outro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/cmd_upgrade/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_upgrade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_upgrade/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_upgrade/gather_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/cmd_upgrade/where_is_the_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/404.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/settings.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/template/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/1 - Page1.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/template/tree/2 - Pages/
--rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/2 - Pages/logo200.png
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/2 - Pages/page.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/template/tree/7 - FAQs/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/7 - FAQs/1 - Question1.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/7 - FAQs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/8 - Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/9 - About.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/template/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics/main/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/utils/ensure_a_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/utils/favicon_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/utils/is_nics_initialized.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 20:25:23.000000 nics-3.0.0b5/nics/main/utils/page404_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 20:25:29.000000 nics-3.0.0b5/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 20:25:23.000000 nics-3.0.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 20:25:23.000000 nics-3.0.0b5/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 20:25:29.000000 nics-3.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 20:25:23.000000 nics-3.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 20:31:49.000000 nics-3.0.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-18 20:31:49.000000 nics-3.0.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 20:31:56.000000 nics-3.0.0b6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/cmd_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/ensure_nics_env_can_be_installed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/get_user_details.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/cmd_init/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/loading/copy_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/loading/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/loading/workflow_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_init/print_outro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/cmd_upgrade/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_upgrade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_upgrade/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_upgrade/gather_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/cmd_upgrade/where_is_the_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/404.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/settings.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/template/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/1 - Page1.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/template/tree/2 - Pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    25360 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/2 - Pages/logo200.png
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/2 - Pages/page.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/template/tree/7 - FAQs/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/7 - FAQs/1 - Question1.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/7 - FAQs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/8 - Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/9 - About.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/template/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics/main/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/utils/ensure_a_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/utils/favicon_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/utils/is_nics_initialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-18 20:31:49.000000 nics-3.0.0b6/nics/main/utils/page404_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 20:31:56.000000 nics-3.0.0b6/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 20:31:49.000000 nics-3.0.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 20:31:49.000000 nics-3.0.0b6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 20:31:56.000000 nics-3.0.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 20:31:49.000000 nics-3.0.0b6/setup.py
```

### Comparing `nics-3.0.0b5/LICENSE` & `nics-3.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/PKG-INFO` & `nics-3.0.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-3.0.0b5/nics/main/__init__.py` & `nics-3.0.0b6/nics/main/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/__init__.py` & `nics-3.0.0b6/nics/main/cmd_init/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/ensure_nics_env_can_be_installed.py` & `nics-3.0.0b6/nics/main/cmd_init/ensure_nics_env_can_be_installed.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/get_user_details.py` & `nics-3.0.0b6/nics/main/cmd_init/get_user_details.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/loading/__init__.py` & `nics-3.0.0b6/nics/main/cmd_init/loading/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/loading/settings_writer.py` & `nics-3.0.0b6/nics/main/cmd_init/loading/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/loading/workflow_writer.py` & `nics-3.0.0b6/nics/main/cmd_init/loading/workflow_writer.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_init/print_outro.py` & `nics-3.0.0b6/nics/main/cmd_init/print_outro.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_upgrade/__init__.py` & `nics-3.0.0b6/nics/main/cmd_upgrade/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_upgrade/checks.py` & `nics-3.0.0b6/nics/main/cmd_upgrade/checks.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_upgrade/gather_settings.py` & `nics-3.0.0b6/nics/main/cmd_upgrade/gather_settings.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/cmd_upgrade/where_is_the_container.py` & `nics-3.0.0b6/nics/main/cmd_upgrade/where_is_the_container.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/constants.py` & `nics-3.0.0b6/nics/main/constants.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/template/tree/2 - Pages/logo200.png` & `nics-3.0.0b6/nics/main/template/tree/2 - Pages/logo200.png`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/utils/favicon_maker.py` & `nics-3.0.0b6/nics/main/utils/favicon_maker.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/utils/is_nics_initialized.py` & `nics-3.0.0b6/nics/main/utils/is_nics_initialized.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics/main/utils/page404_maker.py` & `nics-3.0.0b6/nics/main/utils/page404_maker.py`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/nics.egg-info/PKG-INFO` & `nics-3.0.0b6/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 3.0.0b5
+Version: 3.0.0b6
 Summary: Automated markdown-based documentation page workflow
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: Documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: Report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-3.0.0b5/nics.egg-info/SOURCES.txt` & `nics-3.0.0b6/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-3.0.0b5/pyproject.toml` & `nics-3.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "3.0.0b5"
+version = "3.0.0b6"
 description = "Automated markdown-based documentation page workflow"
 readme = "readme.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

### Comparing `nics-3.0.0b5/readme.md` & `nics-3.0.0b6/readme.md`

 * *Files identical despite different names*

