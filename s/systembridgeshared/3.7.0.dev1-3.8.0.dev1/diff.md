# Comparing `tmp/systembridgeshared-3.7.0.dev1.tar.gz` & `tmp/systembridgeshared-3.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeshared-3.7.0.dev1.tar", last modified: Mon Jul  3 08:33:15 2023, max compression
+gzip compressed data, was "systembridgeshared-3.8.0.dev1.tar", last modified: Tue Jul 18 08:30:42 2023, max compression
```

## Comparing `systembridgeshared-3.7.0.dev1.tar` & `systembridgeshared-3.8.0.dev1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:33:15.401466 systembridgeshared-3.7.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.393466 systembridgeshared-3.7.0.dev1/systembridgeshared/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 08:33:13.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.397466 systembridgeshared-3.7.0.dev1/systembridgeshared/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_remote_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/display.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/get_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/open_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/open_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/register_data_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/models/update_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-07-03 08:32:55.000000 systembridgeshared-3.7.0.dev1/systembridgeshared/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:33:15.393466 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 08:33:15.000000 systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:30:42.041765 systembridgeshared-3.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-18 08:30:42.041765 systembridgeshared-3.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:30:42.041765 systembridgeshared-3.8.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:30:42.033765 systembridgeshared-3.8.0.dev1/systembridgeshared/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 08:30:39.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:30:42.041765 systembridgeshared-3.8.0.dev1/systembridgeshared/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/database_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/database_data_remote_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/database_data_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/get_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/register_data_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/models/update_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17315 2023-07-18 08:30:17.000000 systembridgeshared-3.8.0.dev1/systembridgeshared/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:30:42.033765 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-18 08:30:41.000000 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-18 08:30:41.000000 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:30:41.000000 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 08:30:41.000000 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 08:30:41.000000 systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/top_level.txt
```

### Comparing `systembridgeshared-3.7.0.dev1/pyproject.toml` & `systembridgeshared-3.8.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/setup.py` & `systembridgeshared-3.8.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/common.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/common.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/const.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/const.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/database.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/database.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/exceptions.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/http_client.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/logger.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/logger.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/battery.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/cpu.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/data.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/data.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/database_data.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/database_data_remote_bridge.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/database_data_remote_bridge.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/disk.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/disk.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/media.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/media.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/media_files.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/memory.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/network.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/network.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/notification.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/response.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/response.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/models/system.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/models/system.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/settings.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/settings.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/update.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,19 @@
         """Update each package."""
         for package, version in packages.items():
             self._logger.info("Updating %s to version %s", package, version)
             if version:
                 self._install_package(f"{package}=={version}")
 
         asyncio_get_loop().call_later(
-            5, os.execl, sys.executable, sys.executable, *sys.argv
+            5,
+            os.execl,
+            sys.executable,
+            sys.executable,
+            *sys.argv,
         )
 
     def update(
         self,
         version: Optional[str],
         wait: bool = False,
     ) -> dict[str, Optional[str]]:
```

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared/websocket_client.py` & `systembridgeshared-3.8.0.dev1/systembridgeshared/websocket_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeshared-3.7.0.dev1/systembridgeshared.egg-info/SOURCES.txt` & `systembridgeshared-3.8.0.dev1/systembridgeshared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

