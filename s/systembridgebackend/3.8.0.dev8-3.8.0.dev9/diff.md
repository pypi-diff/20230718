# Comparing `tmp/systembridgebackend-3.8.0.dev8.tar.gz` & `tmp/systembridgebackend-3.8.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-3.8.0.dev8.tar", last modified: Tue Jul 18 10:18:03 2023, max compression
+gzip compressed data, was "systembridgebackend-3.8.0.dev9.tar", last modified: Tue Jul 18 14:36:15 2023, max compression
```

## Comparing `systembridgebackend-3.8.0.dev8.tar` & `systembridgebackend-3.8.0.dev9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.705515 systembridgebackend-3.8.0.dev8/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 10:18:00.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/battery/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/battery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/battery/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/cpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/cpu/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/disk/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/disk/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/display/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/display/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/gpu/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/media/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/media/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/memory/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/network/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/network/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/sensors/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/system/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/system/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/modules/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.709515 systembridgebackend-3.8.0.dev8/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/action.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/media.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/remote_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.713515 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 10:17:16.000000 systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:18:03.705515 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 10:18:03.000000 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-18 10:18:03.000000 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:18:03.000000 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 10:18:03.000000 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 10:18:03.000000 systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-18 14:36:12.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102485 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/modules/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/remote_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.938712 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 14:35:32.000000 systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:36:15.934712 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 14:36:15.000000 systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/top_level.txt
```

### Comparing `systembridgebackend-3.8.0.dev8/pyproject.toml` & `systembridgebackend-3.8.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/setup.py` & `systembridgebackend-3.8.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/__main__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/data.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/gui.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/gui.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/icon.ico` & `systembridgebackend-3.8.0.dev9/systembridgebackend/icon.ico`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/icon.png` & `systembridgebackend-3.8.0.dev9/systembridgebackend/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/battery/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/battery/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/battery/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/cpu/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/cpu/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/cpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/disk/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/disk/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/disk/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/display/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/display/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/display/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/gpu/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/gpu/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/gpu/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/listeners.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/media/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/media/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/media/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/memory/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/memory/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/network/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/network/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/network/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/sensors/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/sensors/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/sensors/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/system/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/system/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/system/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/modules/update.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/modules/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/server/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/server/api.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/server/mdns.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/server/websocket.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/action.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/__init__.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/linux.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/autostart/windows.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/autostart/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/keyboard.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/media.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/power.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/linux.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/linux.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend/utilities/shortcuts/windows.py` & `systembridgebackend-3.8.0.dev9/systembridgebackend/utilities/shortcuts/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-3.8.0.dev8/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-3.8.0.dev9/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

