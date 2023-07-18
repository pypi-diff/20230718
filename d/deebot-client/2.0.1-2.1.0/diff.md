# Comparing `tmp/deebot-client-2.0.1.tar.gz` & `tmp/deebot-client-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-2.0.1.tar", last modified: Fri Jul  7 09:12:15 2023, max compression
+gzip compressed data, was "deebot-client-2.1.0.tar", last modified: Tue Jul 18 20:37:57 2023, max compression
```

## Comparing `deebot-client-2.0.1.tar` & `deebot-client-2.1.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-07 09:12:10.000000 deebot-client-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-07 09:12:15.670465 deebot-client-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-07 09:12:10.000000 deebot-client-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.666464 deebot-client-2.0.1/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.666464 deebot-client-2.0.1/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-07 09:12:10.000000 deebot-client-2.0.1/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.666464 deebot-client-2.0.1/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-07 09:12:15.000000 deebot-client-2.0.1/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-07 09:12:15.000000 deebot-client-2.0.1/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:12:15.000000 deebot-client-2.0.1/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 09:12:15.000000 deebot-client-2.0.1/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 09:12:15.000000 deebot-client-2.0.1/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 09:12:10.000000 deebot-client-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-07 09:12:15.670465 deebot-client-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-07 09:12:11.000000 deebot-client-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.662464 deebot-client-2.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/commands/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/events/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:12:15.670465 deebot-client-2.0.1/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-07 09:12:10.000000 deebot-client-2.0.1/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-18 20:37:50.000000 deebot-client-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-18 20:37:57.565588 deebot-client-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-18 20:37:50.000000 deebot-client-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.557587 deebot-client-2.1.0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.561588 deebot-client-2.1.0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-18 20:37:50.000000 deebot-client-2.1.0/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.557587 deebot-client-2.1.0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 20:37:57.000000 deebot-client-2.1.0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-18 20:37:50.000000 deebot-client-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 20:37:57.569588 deebot-client-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-18 20:37:50.000000 deebot-client-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.553587 deebot-client-2.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 20:37:57.565588 deebot-client-2.1.0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-18 20:37:50.000000 deebot-client-2.1.0/tests/messages/test_stats.py
```

### Comparing `deebot-client-2.0.1/LICENSE.txt` & `deebot-client-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/PKG-INFO` & `deebot-client-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.1
+Version: 2.1.0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Client Library for Deebot Vacuums
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/deebot-client?style=for-the-badge)](https://pypi.org/project/deebot-client)
 <a href="https://www.buymeacoffee.com/edenhaus" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" width="150px" height="35px" alt="Buy Me A Coffee" style="height: 35px !important;width: 150px !important;" ></a>
```

### Comparing `deebot-client-2.0.1/README.md` & `deebot-client-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/api_client.py` & `deebot-client-2.1.0/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/authentication.py` & `deebot-client-2.1.0/deebot_client/authentication.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/command.py` & `deebot-client-2.1.0/deebot_client/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,25 +58,21 @@
             bot_reached (bool): True if the command was targeting the bot and it responded in time. False otherwise.
                                 This value is not indicating if the command was executed successfully.
         """
         try:
             result = await self._execute(authenticator, device_info, event_bus)
             if result.state == HandlingState.SUCCESS:
                 # Execute command which are requested by the handler
-                tasks = []
-                for requested_command in result.requested_commands:
-                    tasks.append(
-                        asyncio.create_task(
+                async with asyncio.TaskGroup() as tg:
+                    for requested_command in result.requested_commands:
+                        tg.create_task(
                             requested_command.execute(
                                 authenticator, device_info, event_bus
                             )
                         )
-                    )
-
-                await asyncio.gather(*tasks)
 
                 return self._targets_bot
         except Exception:  # pylint: disable=broad-except
             _LOGGER.warning(
                 "Could not execute command %s",
                 self.name,
                 exc_info=True,
```

### Comparing `deebot-client-2.0.1/deebot_client/commands/__init__.py` & `deebot-client-2.1.0/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/charge.py` & `deebot-client-2.1.0/deebot_client/commands/charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/charge_state.py` & `deebot-client-2.1.0/deebot_client/commands/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/clean.py` & `deebot-client-2.1.0/deebot_client/commands/clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/clean_count.py` & `deebot-client-2.1.0/deebot_client/commands/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/clean_logs.py` & `deebot-client-2.1.0/deebot_client/commands/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/common.py` & `deebot-client-2.1.0/deebot_client/commands/common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/custom.py` & `deebot-client-2.1.0/deebot_client/commands/custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/error.py` & `deebot-client-2.1.0/deebot_client/commands/error.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/fan_speed.py` & `deebot-client-2.1.0/deebot_client/commands/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/life_span.py` & `deebot-client-2.1.0/deebot_client/commands/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/map.py` & `deebot-client-2.1.0/deebot_client/commands/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/pos.py` & `deebot-client-2.1.0/deebot_client/commands/pos.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/stats.py` & `deebot-client-2.1.0/deebot_client/commands/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/volume.py` & `deebot-client-2.1.0/deebot_client/commands/volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/commands/water_info.py` & `deebot-client-2.1.0/deebot_client/commands/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/events/__init__.py` & `deebot-client-2.1.0/deebot_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/events/const.py` & `deebot-client-2.1.0/deebot_client/events/const.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/events/event_bus.py` & `deebot-client-2.1.0/deebot_client/events/event_bus.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,50 +13,26 @@
     from ..command import Command
 
 _LOGGER = get_logger(__name__)
 
 T = TypeVar("T", bound=Event)
 
 
-class EventListener(Generic[T]):
-    """Object that allows event consumers to easily unsubscribe from event bus."""
-
-    def __init__(
-        self,
-        event_processing_data: "_EventProcessingData",
-        callback: Callable[[T], Coroutine[Any, Any, None]],
-    ) -> None:
-        self._event_processing_data: Final = event_processing_data
-        self.callback: Final = callback
-
-    def unsubscribe(self) -> None:
-        """Unsubscribe from event bus."""
-        self._event_processing_data.subscribers.remove(self)
-
-
 class _EventProcessingData(Generic[T]):
     """Data class, which holds all needed data per EventDto."""
 
     def __init__(self) -> None:
         super().__init__()
 
-        self._subscribers: Final[list[EventListener[T]]] = []
-        self._semaphore: Final = asyncio.Semaphore(1)
+        self.subscriber_callbacks: Final[
+            list[Callable[[T], Coroutine[Any, Any, None]]]
+        ] = []
+        self.semaphore: Final = asyncio.Semaphore(1)
         self.last_event: T | None = None
 
-    @property
-    def subscribers(self) -> list[EventListener[T]]:
-        """Return subscribers."""
-        return self._subscribers
-
-    @property
-    def semaphore(self) -> asyncio.Semaphore:
-        """Return semaphore."""
-        return self._semaphore
-
 
 class EventBus:
     """A very simple event bus system."""
 
     def __init__(
         self,
         execute_command: Callable[["Command"], Coroutine[Any, Any, None]],
@@ -66,40 +42,40 @@
         self._tasks: set[asyncio.Future[Any]] = set()
 
         self._execute_command: Final = execute_command
 
     def has_subscribers(self, event: type[T]) -> bool:
         """Return True, if emitter has subscribers."""
         return (
-            len(self._event_processing_dict[event].subscribers) > 0
+            len(self._event_processing_dict[event].subscriber_callbacks) > 0
             if event in self._event_processing_dict
             else False
         )
 
     def subscribe(
         self,
         event_type: type[T],
         callback: Callable[[T], Coroutine[Any, Any, None]],
-    ) -> EventListener[T]:
+    ) -> Callable[[], None]:
         """Subscribe to event."""
         event_processing_data = self._get_or_create_event_processing_data(event_type)
 
-        listener = EventListener(event_processing_data, callback)
-        event_processing_data.subscribers.append(listener)
+        def unsubscribe() -> None:
+            event_processing_data.subscriber_callbacks.remove(callback)
+
+        event_processing_data.subscriber_callbacks.append(callback)
 
         if event_processing_data.last_event:
             # Notify subscriber directly with the last event
-            create_task(
-                self._tasks, listener.callback(event_processing_data.last_event)
-            )
-        elif len(event_processing_data.subscribers) == 1:
+            create_task(self._tasks, callback(event_processing_data.last_event))
+        elif len(event_processing_data.subscriber_callbacks) == 1:
             # first subscriber therefore do refresh
             self.request_refresh(event_type)
 
-        return listener
+        return unsubscribe
 
     def notify(self, event: T) -> bool:
         """Notify subscriber with given event representation."""
         event_processing_data = self._get_or_create_event_processing_data(type(event))
 
         if (
             isinstance(event, StateEvent)
@@ -122,18 +98,18 @@
                     self.request_refresh(event_type)
 
         if event == event_processing_data.last_event:
             _LOGGER.debug("Event is the same! Skipping (%s)", event)
             return False
 
         event_processing_data.last_event = event
-        if event_processing_data.subscribers:
+        if event_processing_data.subscriber_callbacks:
             _LOGGER.debug("Notify subscribers with %s", event)
-            for subscriber in event_processing_data.subscribers:
-                create_task(self._tasks, subscriber.callback(event))
+            for callback in event_processing_data.subscriber_callbacks:
+                create_task(self._tasks, callback(event))
             return True
 
         _LOGGER.debug("No subscribers... Discharging %s", event)
         return False
 
     def request_refresh(self, event_class: type[T]) -> None:
         """Request manual refresh."""
@@ -158,19 +134,17 @@
             commands = EVENT_DTO_REFRESH_COMMANDS.get(event_class, [])
             if not commands:
                 return
 
             if len(commands) == 1:
                 await self._execute_command(commands[0])
             else:
-                tasks = []
-                for command in commands:
-                    tasks.append(asyncio.create_task(self._execute_command(command)))
-
-                await asyncio.gather(*tasks)
+                async with asyncio.TaskGroup() as tg:
+                    for command in commands:
+                        tg.create_task(self._execute_command(command))
 
     def _get_or_create_event_processing_data(
         self, event_class: type[T]
     ) -> _EventProcessingData[T]:
         with self._lock:
             event_processing_data = self._event_processing_dict.get(event_class, None)
```

### Comparing `deebot-client-2.0.1/deebot_client/events/map.py` & `deebot-client-2.1.0/deebot_client/events/map.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Map event module."""
 from dataclasses import dataclass
+from datetime import datetime
 from enum import Enum, unique
 from typing import Any
 
 from ..events import Event
 
 
 @unique
@@ -91,7 +92,14 @@
 
 @dataclass(frozen=True)
 class CachedMapInfoEvent(Event):
     """Cached map info event."""
 
     name: str
     active: bool
+
+
+@dataclass(frozen=True)
+class MapChangedEvent(Event):
+    """Map changed event."""
+
+    when: datetime = datetime.utcnow()
```

### Comparing `deebot-client-2.0.1/deebot_client/logging_filter.py` & `deebot-client-2.1.0/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/map.py` & `deebot-client-2.1.0/deebot_client/map.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,38 @@
 import base64
 import dataclasses
 import lzma
 import math
 import struct
 import zlib
 from collections.abc import Callable, Coroutine
+from datetime import datetime, timedelta
 from io import BytesIO
 from typing import Any, Final
 
 from numpy import ndarray, reshape, zeros
 from PIL import Image, ImageDraw, ImageOps
 
+from deebot_client.events.map import MapChangedEvent
+
 from .command import Command
 from .commands import GetCachedMapInfo, GetMinorMap
 from .events import (
     MajorMapEvent,
     MapSetEvent,
     MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
     Position,
     PositionsEvent,
     PositionType,
     RoomsEvent,
 )
-from .events.event_bus import EventBus, EventListener
+from .events.event_bus import EventBus
 from .exceptions import MapError
 from .logging_filter import get_logger
 from .models import Room
 from .util import OnChangedDict, OnChangedList, cancel, create_task
 
 _LOGGER = get_logger(__name__)
 _PIXEL_WIDTH = 50
@@ -136,49 +139,20 @@
         self,
         execute_command: Callable[[Command], Coroutine[Any, Any, None]],
         event_bus: EventBus,
     ):
         self._execute_command = execute_command
         self._event_bus = event_bus
 
-        self._map_data: Final[MapData] = MapData()
+        self._map_data: Final[MapData] = MapData(event_bus)
         self._amount_rooms: int = 0
         self._last_image: LastImage | None = None
-        self._listeners: list[EventListener] = []
+        self._unsubscribers: list[Callable[[], None]] = []
         self._tasks: set[asyncio.Future[Any]] = set()
 
-        async def on_map_set(event: MapSetEvent) -> None:
-            if event.type == MapSetType.ROOMS:
-                self._amount_rooms = len(event.subsets)
-                for room_id, _ in self._map_data.rooms.copy().items():
-                    if room_id not in event.subsets:
-                        self._map_data.rooms.pop(room_id, None)
-            else:
-                for subset_id, subset in self._map_data.map_subsets.copy().items():
-                    if subset.type == event.type and subset_id not in event.subsets:
-                        self._map_data.map_subsets.pop(subset_id, None)
-
-        self._event_bus.subscribe(MapSetEvent, on_map_set)
-
-        async def on_map_subset(event: MapSubsetEvent) -> None:
-            if event.type == MapSetType.ROOMS and event.name:
-                room = Room(event.name, event.id, event.coordinates)
-                if self._map_data.rooms.get(event.id, None) != room:
-                    self._map_data.rooms[room.id] = room
-
-                    if len(self._map_data.rooms) == self._amount_rooms:
-                        self._event_bus.notify(
-                            RoomsEvent(list(self._map_data.rooms.values()))
-                        )
-
-            elif self._map_data.map_subsets.get(event.id, None) != event:
-                self._map_data.map_subsets[event.id] = event
-
-        self._event_bus.subscribe(MapSubsetEvent, on_map_subset)
-
     # ---------------------------- METHODS ----------------------------
 
     def _update_trace_points(self, data: str) -> None:
         _LOGGER.debug("[_update_trace_points] Begin")
         trace_points = _decompress_7z_base64_data(data)
 
         for i in range(0, len(trace_points), 5):
@@ -223,77 +197,111 @@
                             )
                             raise MapError("Map Limit reached!")
                         if pixel_type in [0x01, 0x02, 0x03]:
                             draw.point((point_x, point_y), fill=_COLORS[pixel_type])
 
     def enable(self) -> None:
         """Enable map."""
-        if self._listeners:
+        if self._unsubscribers:
             return
 
         create_task(self._tasks, self._execute_command(GetCachedMapInfo()))
 
+        async def on_map_set(event: MapSetEvent) -> None:
+            if event.type == MapSetType.ROOMS:
+                self._amount_rooms = len(event.subsets)
+                for room_id, _ in self._map_data.rooms.copy().items():
+                    if room_id not in event.subsets:
+                        self._map_data.rooms.pop(room_id, None)
+            else:
+                for subset_id, subset in self._map_data.map_subsets.copy().items():
+                    if subset.type == event.type and subset_id not in event.subsets:
+                        self._map_data.map_subsets.pop(subset_id, None)
+
+        self._unsubscribers.append(self._event_bus.subscribe(MapSetEvent, on_map_set))
+
+        async def on_map_subset(event: MapSubsetEvent) -> None:
+            if event.type == MapSetType.ROOMS and event.name:
+                room = Room(event.name, event.id, event.coordinates)
+                if self._map_data.rooms.get(event.id, None) != room:
+                    self._map_data.rooms[room.id] = room
+
+                    if len(self._map_data.rooms) == self._amount_rooms:
+                        self._event_bus.notify(
+                            RoomsEvent(list(self._map_data.rooms.values()))
+                        )
+
+            elif self._map_data.map_subsets.get(event.id, None) != event:
+                self._map_data.map_subsets[event.id] = event
+
+        self._unsubscribers.append(
+            self._event_bus.subscribe(MapSubsetEvent, on_map_subset)
+        )
+
         async def on_position(event: PositionsEvent) -> None:
             self._map_data.positions = event.positions
 
-        self._listeners.append(self._event_bus.subscribe(PositionsEvent, on_position))
+        self._unsubscribers.append(
+            self._event_bus.subscribe(PositionsEvent, on_position)
+        )
 
         async def on_map_trace(event: MapTraceEvent) -> None:
             if event.start == 0:
                 self._map_data.trace_values.clear()
 
             self._update_trace_points(event.data)
 
-        self._listeners.append(self._event_bus.subscribe(MapTraceEvent, on_map_trace))
+        self._unsubscribers.append(
+            self._event_bus.subscribe(MapTraceEvent, on_map_trace)
+        )
 
         async def on_major_map(event: MajorMapEvent) -> None:
-            tasks = []
-            for idx, value in enumerate(event.values):
-                if (
-                    self._map_data.map_pieces[idx].crc32_indicates_update(value)
-                    and event.requested
-                ):
-                    tasks.append(
-                        asyncio.create_task(
+            async with asyncio.TaskGroup() as tg:
+                for idx, value in enumerate(event.values):
+                    if (
+                        self._map_data.map_pieces[idx].crc32_indicates_update(value)
+                        and event.requested
+                    ):
+                        tg.create_task(
                             self._execute_command(
                                 GetMinorMap(map_id=event.map_id, piece_index=idx)
                             )
                         )
-                    )
 
-            if tasks:
-                await asyncio.gather(*tasks)
-
-        self._listeners.append(self._event_bus.subscribe(MajorMapEvent, on_major_map))
+        self._unsubscribers.append(
+            self._event_bus.subscribe(MajorMapEvent, on_major_map)
+        )
 
         async def on_minor_map(event: MinorMapEvent) -> None:
             self._map_data.map_pieces[event.index].update_points(event.value)
 
-        self._listeners.append(self._event_bus.subscribe(MinorMapEvent, on_minor_map))
+        self._unsubscribers.append(
+            self._event_bus.subscribe(MinorMapEvent, on_minor_map)
+        )
 
     def disable(self) -> None:
         """Disable map."""
-        listeners = self._listeners
-        self._listeners.clear()
-        for listener in listeners:
-            listener.unsubscribe()
+        unsubscribers = self._unsubscribers
+        self._unsubscribers.clear()
+        for unsubscribe in unsubscribers:
+            unsubscribe()
 
     def refresh(self) -> None:
         """Manually refresh map."""
-        if not self._listeners:
+        if not self._unsubscribers:
             raise MapError("Please enable the map first")
 
         # todo make it nice pylint: disable=fixme
         self._event_bus.request_refresh(PositionsEvent)
         self._event_bus.request_refresh(MapTraceEvent)
         self._event_bus.request_refresh(MajorMapEvent)
 
     def get_base64_map(self, width: int | None = None) -> bytes:
         """Return map as base64 image string."""
-        if not self._listeners:
+        if not self._unsubscribers:
             raise MapError("Please enable the map first")
 
         if (
             self._last_image is not None
             and width == self._last_image.width
             and not self._map_data.changed
         ):
@@ -338,27 +346,25 @@
             _LOGGER.debug(
                 "[get_base64_map] Resize based on the requested width: %d and calculated height %d",
                 width,
                 height,
             )
             new_size = (width, height)
         elif cropped.size[0] > 400 or cropped.size[1] > 400:
-            _LOGGER.debug(
-                "[get_base64_map] Resize disabled.. map over 400 and image width was passed"
-            )
+            _LOGGER.debug("[get_base64_map] Resize disabled.. map over 400")
         else:
             resize_factor = Map.RESIZE_FACTOR
             _LOGGER.debug("[get_base64_map] Resize factor: %d", resize_factor)
             new_size = (
                 cropped.size[0] * resize_factor,
                 cropped.size[1] * resize_factor,
             )
 
         if new_size is not None:
-            cropped = cropped.resize(new_size, Image.NEAREST)
+            cropped = cropped.resize(new_size, Image.Resampling.NEAREST)
 
         _LOGGER.debug("[get_base64_map] Saving to buffer")
         buffered = BytesIO()
         cropped.save(buffered, format="PNG")
         del cropped
 
         base64_image = base64.b64encode(buffered.getvalue())
@@ -489,15 +495,15 @@
             x1, y1 = xy[i]
             x2, y2 = xy[i + 1]
             x_length = x2 - x1
             y_length = y2 - y1
             length = math.sqrt(x_length**2 + y_length**2)
             dash_enabled = True
             position = 0
-            while position <= length:
+            while position < length:
                 for dash_step in dash:
                     if dash_enabled:
                         start = position / length
                         end = min((position + dash_step - 1) / length, 1)
                         self._thick_line(
                             [
                                 (
@@ -524,19 +530,24 @@
     base64_image: bytes
     width: int | None
 
 
 class MapData:
     """Map data."""
 
-    def __init__(self) -> None:
+    def __init__(self, event_bus: EventBus) -> None:
         self._changed: bool = False
 
         def on_change() -> None:
             self._changed = True
+            now = datetime.utcnow()
+            last_event = event_bus.get_last_event(MapChangedEvent)
+            if last_event is None or (now - last_event.when) > timedelta(seconds=1):
+                # throttle notify to ones a second
+                event_bus.notify(MapChangedEvent(now))
 
         self._on_change = on_change
         self._map_pieces: OnChangedList[MapPiece] = OnChangedList(
             on_change, [MapPiece(on_change, i) for i in range(64)]
         )
         self._map_subsets: OnChangedDict[int, MapSubsetEvent] = OnChangedDict(on_change)
         self._positions: OnChangedList[Position] = OnChangedList(on_change)
```

### Comparing `deebot-client-2.0.1/deebot_client/message.py` & `deebot-client-2.1.0/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/messages/__init__.py` & `deebot-client-2.1.0/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/messages/battery.py` & `deebot-client-2.1.0/deebot_client/messages/battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/messages/stats.py` & `deebot-client-2.1.0/deebot_client/messages/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/models.py` & `deebot-client-2.1.0/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client/mqtt_client.py` & `deebot-client-2.1.0/deebot_client/mqtt_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import json
 import ssl
 from collections.abc import Callable, MutableMapping
 from contextlib import suppress
 from dataclasses import _MISSING_TYPE, InitVar, dataclass, field, fields
 from datetime import datetime
 
-from asyncio_mqtt import Client, Message, MqttError
+from aiomqtt import Client, Message, MqttError
 from cachetools import TTLCache
 
 from deebot_client.events.event_bus import EventBus
 from deebot_client.exceptions import AuthenticationError
 
 from .authentication import Authenticator
 from .commands import COMMANDS_WITH_MQTT_P2P_HANDLING, CommandHandlingMqttP2P
 from .logging_filter import get_logger
 from .models import Configuration, Credentials, DeviceInfo
 
 RECONNECT_INTERVAL = 5  # seconds
 
 _LOGGER = get_logger(__name__)
+_CLIENT_LOGGER = get_logger(f"{__name__}.client")
 
 
 def _get_topics(device_info: DeviceInfo) -> list[str]:
     return [
         # iot/atr/[command]]/[did]]/[class]]/[resource]/j
         f"iot/atr/+/{device_info.did}/{device_info.get_class}/{device_info.resource}/j",
         # iot/p2p/[command]]/[sender did]/[sender class]]/[sender resource]
@@ -137,14 +138,15 @@
         credentials = await self._authenticator.authenticate()
         client_id = f"{credentials.user_id}@ecouser/{self._config.device_id}"
         return Client(
             hostname=self._config.hostname,
             port=self._config.port,
             username=credentials.user_id,
             password=credentials.token,
+            logger=_CLIENT_LOGGER,
             client_id=client_id,
             tls_context=self._config.ssl_context,
         )
 
     async def _cancel_mqtt_task(self) -> None:
         if self._mqtt_task is not None and self._mqtt_task.cancel():
             # Wait for the task to be cancelled
@@ -176,15 +178,14 @@
                             _LOGGER.debug("All mqtt tasks created")
                             await asyncio.wait(
                                 tasks, return_when=asyncio.FIRST_COMPLETED
                             )
                         finally:
                             for task in tasks:
                                 task.cancel()
-
                 except MqttError:
                     _LOGGER.warning(
                         "Connection lost; Reconnecting in %d seconds ...",
                         RECONNECT_INTERVAL,
                         exc_info=True,
                     )
                 except AuthenticationError:
```

### Comparing `deebot-client-2.0.1/deebot_client/vacuum_bot.py` & `deebot-client-2.1.0/deebot_client/vacuum_bot.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/deebot_client.egg-info/PKG-INFO` & `deebot-client-2.1.0/deebot_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.1
+Version: 2.1.0
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Client Library for Deebot Vacuums
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/deebot-client?style=for-the-badge)](https://pypi.org/project/deebot-client)
 <a href="https://www.buymeacoffee.com/edenhaus" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" width="150px" height="35px" alt="Buy Me A Coffee" style="height: 35px !important;width: 150px !important;" ></a>
```

### Comparing `deebot-client-2.0.1/deebot_client.egg-info/SOURCES.txt` & `deebot-client-2.1.0/deebot_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/setup.py` & `deebot-client-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="2.0.1",
+    version="2.1.0",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
@@ -25,14 +25,14 @@
         #   5 - Production/Stable
         "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Home Automation",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="home automation vacuum robot deebot ecovacs",
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
     package_data={"deebot_client": ["py.typed"]},
     install_requires=install_requires,
 )
```

### Comparing `deebot-client-2.0.1/tests/commands/__init__.py` & `deebot-client-2.1.0/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_advanced_mode.py` & `deebot-client-2.1.0/tests/commands/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_carpet.py` & `deebot-client-2.1.0/tests/commands/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_charge.py` & `deebot-client-2.1.0/tests/commands/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_clean.py` & `deebot-client-2.1.0/tests/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_clean_count.py` & `deebot-client-2.1.0/tests/commands/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_clean_log.py` & `deebot-client-2.1.0/tests/commands/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_clean_preference.py` & `deebot-client-2.1.0/tests/commands/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_common.py` & `deebot-client-2.1.0/tests/commands/test_common.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_continuous_cleaning.py` & `deebot-client-2.1.0/tests/commands/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_custom.py` & `deebot-client-2.1.0/tests/commands/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_fan_speed.py` & `deebot-client-2.1.0/tests/commands/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_life_span.py` & `deebot-client-2.1.0/tests/commands/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_map.py` & `deebot-client-2.1.0/tests/commands/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_mulitmap_state.py` & `deebot-client-2.1.0/tests/commands/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_true_detect.py` & `deebot-client-2.1.0/tests/commands/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/commands/test_water_info.py` & `deebot-client-2.1.0/tests/commands/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/messages/test_battery.py` & `deebot-client-2.1.0/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/messages/test_get_messages.py` & `deebot-client-2.1.0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.1/tests/messages/test_stats.py` & `deebot-client-2.1.0/tests/messages/test_stats.py`

 * *Files identical despite different names*

