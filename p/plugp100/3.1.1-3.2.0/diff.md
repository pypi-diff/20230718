# Comparing `tmp/plugp100-3.1.1.tar.gz` & `tmp/plugp100-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugp100-3.1.1.tar", last modified: Sat Jul 15 10:37:05 2023, max compression
+gzip compressed data, was "plugp100-3.2.0.tar", last modified: Tue Jul 18 16:39:01 2023, max compression
```

## Comparing `plugp100-3.1.1.tar` & `plugp100-3.2.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.200684 plugp100-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 10:36:51.000000 plugp100-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-15 10:36:51.000000 plugp100-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-15 10:37:05.200684 plugp100-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-15 10:36:51.000000 plugp100-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/api/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/hub_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/hub_device_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/s200b_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/t100_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/t110_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/hub/t31x_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/ledstrip_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/light_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/light_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/light_effect_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/plug_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/api/tapo_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/common/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/functional/either.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/common/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/discover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/encryption/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/encryption/key_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/encryption/tp_link_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/handshake_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/login_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/secure_passthrough_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/requests/set_device_info/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/set_device_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/set_device_info/play_alarm_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/set_device_info/set_light_color_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/set_device_info/set_light_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/set_device_info/set_plug_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/tapo_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/requests/trigger_logs_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/child_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/energy_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.200684 plugp100-3.1.1/plugp100/responses/hub_childs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/s200b_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/t100_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/t110_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/t31x_device_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/hub_childs/trigger_log_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/power_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/tapo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-15 10:36:51.000000 plugp100-3.1.1/plugp100/responses/tapo_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:05.196684 plugp100-3.1.1/plugp100.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-15 10:37:05.000000 plugp100-3.1.1/plugp100.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-15 10:37:05.000000 plugp100-3.1.1/plugp100.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:37:05.000000 plugp100-3.1.1/plugp100.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 10:37:05.000000 plugp100-3.1.1/plugp100.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 10:37:05.000000 plugp100-3.1.1/plugp100.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 10:36:51.000000 plugp100-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-15 10:37:05.200684 plugp100-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-15 10:36:51.000000 plugp100-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.568038 plugp100-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 16:38:47.000000 plugp100-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 16:38:47.000000 plugp100-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 16:39:01.568038 plugp100-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-18 16:38:47.000000 plugp100-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.560038 plugp100-3.2.0/plugp100/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/api/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/hub_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/hub_device_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/s200b_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/t100_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/t110_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/hub/t31x_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/ledstrip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/light_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/light_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/light_effect_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/plug_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/power_strip_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/api/tapo_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/common/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/functional/either.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/state_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/common/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/discover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.564038 plugp100-3.2.0/plugp100/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/encryption/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/encryption/key_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/encryption/tp_link_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.568038 plugp100-3.2.0/plugp100/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/handshake_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/login_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/secure_passthrough_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.568038 plugp100-3.2.0/plugp100/requests/set_device_info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/set_device_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/set_device_info/play_alarm_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/set_device_info/set_light_color_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/set_device_info/set_light_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/set_device_info/set_plug_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/tapo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/requests/trigger_logs_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.568038 plugp100-3.2.0/plugp100/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/alarm_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/child_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/energy_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.568038 plugp100-3.2.0/plugp100/responses/hub_childs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/s200b_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/t100_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/t110_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/t31x_device_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/hub_childs/trigger_log_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/power_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/tapo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 16:38:47.000000 plugp100-3.2.0/plugp100/responses/tapo_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:39:01.560038 plugp100-3.2.0/plugp100.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 16:39:01.000000 plugp100-3.2.0/plugp100.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-18 16:39:01.000000 plugp100-3.2.0/plugp100.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:39:01.000000 plugp100-3.2.0/plugp100.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 16:39:01.000000 plugp100-3.2.0/plugp100.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 16:39:01.000000 plugp100-3.2.0/plugp100.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 16:38:47.000000 plugp100-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 16:39:01.568038 plugp100-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-18 16:38:47.000000 plugp100-3.2.0/setup.py
```

### Comparing `plugp100-3.1.1/LICENSE` & `plugp100-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/PKG-INFO` & `plugp100-3.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.1.1
+Version: 3.2.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.1.1/README.md` & `plugp100-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/__init__.py` & `plugp100-3.2.0/plugp100/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         sys.path.append(os.path.join(vendor_dir, vendor_path))
 
 from plugp100.responses import *
 from plugp100.requests import *
 from plugp100.api import *
 from plugp100.common import *
 
-__version__ = "3.1.1"
+__version__ = "3.2.0"
```

### Comparing `plugp100-3.1.1/plugp100/api/hub/hub_device.py` & `plugp100-3.2.0/plugp100/api/hub/hub_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from plugp100.api.hub.hub_device_tracker import HubConnectedDeviceTracker, HubDeviceEvent
 from plugp100.api.tapo_client import TapoClient, Json
 from plugp100.common.functional.either import Either, Right, Left
 from plugp100.common.utils.json_utils import dataclass_encode_json
 from plugp100.requests.set_device_info.play_alarm_params import PlayAlarmParams
 from plugp100.requests.tapo_request import TapoRequest
+from plugp100.responses.alarm_type_list import AlarmTypeList
 from plugp100.responses.child_device_list import ChildDeviceList
 from plugp100.responses.device_state import HubDeviceState
 
 HubSubscription = Callable[[], Any]
 
 
 # The HubDevice class is a blueprint for creating hub devices.
@@ -48,14 +49,18 @@
         The function `get_state` asynchronously retrieves device information and returns either the device state or an
         exception.
         @return: an instance of the `Either` class, which can hold either a `HubDeviceState` object or an `Exception`
         object.
         """
         return (await self._api.get_device_info()) | HubDeviceState.try_from_json
 
+    async def get_supported_alarm_tones(self) -> Either[AlarmTypeList, Exception]:
+        return (await self._api.execute_raw_request(
+            TapoRequest(method="get_support_alarm_type_list", params=None))) | AlarmTypeList.try_from_json
+
     async def get_state_as_json(self) -> Either[Json, Exception]:
         return await self._api.get_device_info()
 
     async def get_children(self) -> Either[ChildDeviceList, Exception]:
         return await self._api.get_child_device_list()
 
     async def control_child(self, device_id: str, request: TapoRequest) -> Either[Json, Exception]:
```

### Comparing `plugp100-3.1.1/plugp100/api/hub/hub_device_tracker.py` & `plugp100-3.2.0/plugp100/api/hub/hub_device_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/hub/s200b_device.py` & `plugp100-3.2.0/plugp100/api/hub/s200b_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/hub/t100_device.py` & `plugp100-3.2.0/plugp100/api/hub/t100_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/hub/t110_device.py` & `plugp100-3.2.0/plugp100/api/hub/t110_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/hub/t31x_device.py` & `plugp100-3.2.0/plugp100/api/hub/t31x_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/ledstrip_device.py` & `plugp100-3.2.0/plugp100/api/ledstrip_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/light_device.py` & `plugp100-3.2.0/plugp100/api/light_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/light_effect.py` & `plugp100-3.2.0/plugp100/api/light_effect.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/light_effect_preset.py` & `plugp100-3.2.0/plugp100/api/light_effect_preset.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/plug_device.py` & `plugp100-3.2.0/plugp100/api/plug_device.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/api/tapo_client.py` & `plugp100-3.2.0/plugp100/api/tapo_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/common/functional/either.py` & `plugp100-3.2.0/plugp100/common/functional/either.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/common/state_tracker.py` & `plugp100-3.2.0/plugp100/common/state_tracker.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/common/utils/http_client.py` & `plugp100-3.2.0/plugp100/common/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/encryption/key_pair.py` & `plugp100-3.2.0/plugp100/encryption/key_pair.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/encryption/tp_link_cipher.py` & `plugp100-3.2.0/plugp100/encryption/tp_link_cipher.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/example.py` & `plugp100-3.2.0/plugp100/example.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/requests/tapo_request.py` & `plugp100-3.2.0/plugp100/requests/tapo_request.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/device_state.py` & `plugp100-3.2.0/plugp100/responses/device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/energy_info.py` & `plugp100-3.2.0/plugp100/responses/energy_info.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/hub_childs/s200b_device_state.py` & `plugp100-3.2.0/plugp100/responses/hub_childs/s200b_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/hub_childs/t100_device_state.py` & `plugp100-3.2.0/plugp100/responses/hub_childs/t100_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/hub_childs/t110_device_state.py` & `plugp100-3.2.0/plugp100/responses/hub_childs/t110_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/hub_childs/t31x_device_state.py` & `plugp100-3.2.0/plugp100/responses/hub_childs/t31x_device_state.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/hub_childs/trigger_log_response.py` & `plugp100-3.2.0/plugp100/responses/hub_childs/trigger_log_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/tapo_exception.py` & `plugp100-3.2.0/plugp100/responses/tapo_exception.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100/responses/tapo_response.py` & `plugp100-3.2.0/plugp100/responses/tapo_response.py`

 * *Files identical despite different names*

### Comparing `plugp100-3.1.1/plugp100.egg-info/PKG-INFO` & `plugp100-3.2.0/plugp100.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugp100
-Version: 3.1.1
+Version: 3.2.0
 Summary: Controller for TP-Link Tapo P100 and other devices
 Home-page: https://github.com/petretiandrea/plugp100
 Download-URL: https://github.com/petretiandrea/plugp100
 Author: @petretiandrea
 Author-email: petretiandrea@gmail.com
 License: GPL3
 Keywords: Tapo,P100
```

### Comparing `plugp100-3.1.1/plugp100.egg-info/SOURCES.txt` & `plugp100-3.2.0/plugp100.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 plugp100.egg-info/top_level.txt
 plugp100/api/__init__.py
 plugp100/api/ledstrip_device.py
 plugp100/api/light_device.py
 plugp100/api/light_effect.py
 plugp100/api/light_effect_preset.py
 plugp100/api/plug_device.py
+plugp100/api/power_strip_device.py
 plugp100/api/tapo_client.py
 plugp100/api/hub/__init__.py
 plugp100/api/hub/hub_device.py
 plugp100/api/hub/hub_device_tracker.py
 plugp100/api/hub/s200b_device.py
 plugp100/api/hub/t100_device.py
 plugp100/api/hub/t110_device.py
@@ -45,14 +46,15 @@
 plugp100/requests/trigger_logs_params.py
 plugp100/requests/set_device_info/__init__.py
 plugp100/requests/set_device_info/play_alarm_params.py
 plugp100/requests/set_device_info/set_light_color_info_params.py
 plugp100/requests/set_device_info/set_light_info_params.py
 plugp100/requests/set_device_info/set_plug_info_params.py
 plugp100/responses/__init__.py
+plugp100/responses/alarm_type_list.py
 plugp100/responses/child_device_list.py
 plugp100/responses/device_state.py
 plugp100/responses/energy_info.py
 plugp100/responses/power_info.py
 plugp100/responses/tapo_exception.py
 plugp100/responses/tapo_response.py
 plugp100/responses/hub_childs/__init__.py
```

### Comparing `plugp100-3.1.1/setup.py` & `plugp100-3.2.0/setup.py`

 * *Files identical despite different names*

