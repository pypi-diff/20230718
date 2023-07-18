# Comparing `tmp/systembridgeconnector-3.8.0.dev4.tar.gz` & `tmp/systembridgeconnector-3.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-3.8.0.dev4.tar", last modified: Tue Jul 18 09:42:21 2023, max compression
+gzip compressed data, was "systembridgeconnector-3.8.0.dev5.tar", last modified: Tue Jul 18 09:46:11 2023, max compression
```

## Comparing `systembridgeconnector-3.8.0.dev4.tar` & `systembridgeconnector-3.8.0.dev5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:42:21.986350 systembridgeconnector-3.8.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 09:42:21.986350 systembridgeconnector-3.8.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:42:21.986350 systembridgeconnector-3.8.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:42:21.982349 systembridgeconnector-3.8.0.dev4/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 09:42:19.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:42:21.986350 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data_remote_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/open_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/register_data_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/update_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17270 2023-07-18 09:42:04.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:42:21.982349 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 09:42:21.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-18 09:42:21.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:42:21.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 09:42:21.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 09:42:21.000000 systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:11.386659 systembridgeconnector-3.8.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 09:46:11.386659 systembridgeconnector-3.8.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:46:11.386659 systembridgeconnector-3.8.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:11.382659 systembridgeconnector-3.8.0.dev5/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 09:46:09.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:11.386659 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data_remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/register_data_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/update_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17270 2023-07-18 09:45:51.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:46:11.382659 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-18 09:46:11.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-18 09:46:11.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:46:11.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 09:46:11.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 09:46:11.000000 systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/top_level.txt
```

### Comparing `systembridgeconnector-3.8.0.dev4/pyproject.toml` & `systembridgeconnector-3.8.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/setup.py` & `systembridgeconnector-3.8.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/const.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/const.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/http_client.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/battery.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/cpu.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/data.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/data.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data_bridge.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/database_data_remote_bridge.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/database_data_remote_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/disk.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/disk.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/media_files.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/memory.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/network.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/network.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/notification.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/response.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/response.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/models/system.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/models/system.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/version.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector/websocket_client.py` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector/websocket_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-3.8.0.dev4/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-3.8.0.dev5/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

