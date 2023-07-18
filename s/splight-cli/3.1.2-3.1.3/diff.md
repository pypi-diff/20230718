# Comparing `tmp/splight-cli-3.1.2.tar.gz` & `tmp/splight-cli-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-3.1.2.tar", last modified: Mon Jul 17 12:08:27 2023, max compression
+gzip compressed data, was "splight-cli-3.1.3.tar", last modified: Tue Jul 18 13:13:33 2023, max compression
```

## Comparing `splight-cli-3.1.2.tar` & `splight-cli-3.1.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-17 12:08:27.381151 splight-cli-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-07-17 12:08:26.000000 splight-cli-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.377151 splight-cli-3.1.2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.377151 splight-cli-3.1.2/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/.splightignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/templates/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/tests/test_component_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/component/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16856 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-17 12:08:26.000000 splight-cli-3.1.2/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:08:27.381151 splight-cli-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-17 12:08:26.000000 splight-cli-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:08:27.381151 splight-cli-3.1.2/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 12:08:27.000000 splight-cli-3.1.2/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 13:13:33.071487 splight-cli-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16418 2023-07-18 13:13:32.000000 splight-cli-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/.splightignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/templates/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/tests/test_component_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/component/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.067487 splight-cli-3.1.3/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-18 13:13:32.000000 splight-cli-3.1.3/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:13:33.071487 splight-cli-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-18 13:13:32.000000 splight-cli-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:13:33.071487 splight-cli-3.1.3/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 13:13:33.000000 splight-cli-3.1.3/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-3.1.2/README.md` & `splight-cli-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/cli.py` & `splight-cli-3.1.3/cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/__init__.py` & `splight-cli-3.1.3/cli/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/component.py` & `splight-cli-3.1.3/cli/component/component.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/exceptions.py` & `splight-cli-3.1.3/cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/loaders.py` & `splight-cli-3.1.3/cli/component/loaders.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/templates/.splightignore` & `splight-cli-3.1.3/cli/component/templates/.splightignore`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/templates/auto_readme.md` & `splight-cli-3.1.3/cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/templates/main.py` & `splight-cli-3.1.3/cli/component/templates/main.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/templates/spec.json` & `splight-cli-3.1.3/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/templates/tests.py` & `splight-cli-3.1.3/cli/component/templates/tests.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/tests/test_component_manager.py` & `splight-cli-3.1.3/cli/component/tests/test_component_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/component/utils.py` & `splight-cli-3.1.3/cli/component/utils.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/config/__init__.py` & `splight-cli-3.1.3/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/constants.py` & `splight-cli-3.1.3/cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/context/__init__.py` & `splight-cli-3.1.3/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/context/workspace.py` & `splight-cli-3.1.3/cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/__init__.py` & `splight-cli-3.1.3/cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/alert/__init__.py` & `splight-cli-3.1.3/cli/engine/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/asset/__init__.py` & `splight-cli-3.1.3/cli/engine/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/attribute/__init__.py` & `splight-cli-3.1.3/cli/engine/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/component/__init__.py` & `splight-cli-3.1.3/cli/engine/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/datalake/__init__.py` & `splight-cli-3.1.3/cli/engine/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/file/__init__.py` & `splight-cli-3.1.3/cli/engine/file/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/manager/exceptions.py` & `splight-cli-3.1.3/cli/engine/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/manager/manager.py` & `splight-cli-3.1.3/cli/engine/manager/manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,15 +386,18 @@
         except Exception as exc:
             raise HubComponentNotFound(hub_component_name, version) from exc
         if not hub_component:
             raise HubComponentNotFound(hub_component_name, version)
         return hub_component[0]
 
     def _create_component_objects(
-        self, new_component: Component, hub_component: HubComponent
+        self,
+        new_component: Component,
+        hub_component: HubComponent,
+        create_new: bool = False,
     ):
         self._console.print(
             f"Creating component objects for {new_component.name}"
         )
         old_component_objects = ComponentObject.list(
             component_id=self.component_id
         )
@@ -408,16 +411,25 @@
                     ),
                     None,
                 )
                 if matching_hct:
                     new_object_data = self._create_objects(
                         obj.data, matching_hct.fields
                     )
-                    obj.data = new_object_data
-                    obj.save()
+                    if create_new:
+                        new_object = ComponentObject(
+                            name=obj.name,
+                            type=obj.type,
+                            data=new_object_data,
+                            component_id=new_component.id,
+                        )
+                        new_object.save()
+                    else:
+                        obj.data = new_object_data
+                        obj.save()
                     self._console.print(
                         f"Component Object {obj.name} saved succesfully"
                     )
             except Exception as e:
                 raise ComponentUpgradeManagerException(
                     f"Could not update component object {obj.name}"
                 ) from e
@@ -464,15 +476,17 @@
             new_inputs = self._update_input(
                 from_component.input, hub_component.input, True
             )
             from_component.input = new_inputs
             new_hub_version = f"{hub_component.name}-{hub_component.version}"
             from_component.version = new_hub_version
             from_component.save()
-            self._create_component_objects(from_component, hub_component)
+            self._create_component_objects(
+                from_component, hub_component, create_new=False
+            )
         except (
             InvalidComponentId,
             VersionUpdateError,
             ComponentCreateError,
             UpdateParametersError,
             HubComponentNotFound,
         ) as e:
@@ -490,15 +504,17 @@
             )
             new_inputs = self._update_input(
                 from_component.input, hub_component.input, True
             )
             new_component = self._create_new_component(
                 from_component, hub_component, new_inputs
             )
-            self._create_component_objects(new_component, hub_component)
+            self._create_component_objects(
+                new_component, hub_component, create_new=True
+            )
         except (
             InvalidComponentId,
             VersionUpdateError,
             ComponentCreateError,
             UpdateParametersError,
             HubComponentNotFound,
         ) as e:
```

### Comparing `splight-cli-3.1.2/cli/engine/secret/__init__.py` & `splight-cli-3.1.3/cli/engine/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/engine/setpoint/__init__.py` & `splight-cli-3.1.3/cli/engine/setpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/hub/component/__init__.py` & `splight-cli-3.1.3/cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/hub/component/exceptions.py` & `splight-cli-3.1.3/cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/hub/component/hub_manager.py` & `splight-cli-3.1.3/cli/hub/component/hub_manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/settings.py` & `splight-cli-3.1.3/cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/utils/input.py` & `splight-cli-3.1.3/cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/utils/loader.py` & `splight-cli-3.1.3/cli/utils/loader.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/utils/pprint.py` & `splight-cli-3.1.3/cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/utils/yaml.py` & `splight-cli-3.1.3/cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/cli/workspace/__init__.py` & `splight-cli-3.1.3/cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/setup.py` & `splight-cli-3.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `splight-cli-3.1.2/splight_cli.egg-info/SOURCES.txt` & `splight-cli-3.1.3/splight_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

