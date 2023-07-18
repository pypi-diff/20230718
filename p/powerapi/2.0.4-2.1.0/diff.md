# Comparing `tmp/powerapi-2.0.4.tar.gz` & `tmp/powerapi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerapi-2.0.4.tar", last modified: Wed Jun 14 09:43:35 2023, max compression
+gzip compressed data, was "powerapi-2.1.0.tar", last modified: Tue Jul 18 11:53:38 2023, max compression
```

## Comparing `powerapi-2.0.4.tar` & `powerapi-2.1.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-14 09:43:24.000000 powerapi-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-14 09:43:35.955064 powerapi-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-14 09:43:24.000000 powerapi-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.939064 powerapi-2.0.4/powerapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/actor/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/backend_supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/backend_supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/backend_supervisor/backend_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/common_cli_parsing_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18482 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/cli/parsing_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.943064 powerapi-2.0.4/powerapi/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/base_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/csvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/direct_prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/file_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/socket_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/database/virtiofs_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatch_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/hwpc_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/power_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/procfs_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatch_rule/simple_dispatch_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/blocking_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/route_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/dispatcher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.947064 powerapi-2.0.4/powerapi/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/abstract_cpu_dram_formula.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/formula/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/simple_formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/formula/simple/simple_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/poison_pill_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/handler/start_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/puller/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/puller_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/puller/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/simple_puller_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/puller/simple/simple_puller_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.951064 powerapi-2.0.4/powerapi/pusher/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/pusher_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/pusher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/control_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/formula_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/hwpc_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/power_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/procfs_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/report_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/libvirt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/report_modifier/report_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.955064 powerapi-2.0.4/powerapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/stat_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-14 09:43:24.000000 powerapi-2.0.4/powerapi/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:43:35.939064 powerapi-2.0.4/powerapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 09:43:35.000000 powerapi-2.0.4/powerapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-14 09:43:24.000000 powerapi-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:43:35.955064 powerapi-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.030722 powerapi-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-18 11:53:26.000000 powerapi-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-18 11:53:38.030722 powerapi-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-07-18 11:53:26.000000 powerapi-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.014722 powerapi-2.1.0/powerapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.018722 powerapi-2.1.0/powerapi/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/actor/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/actor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/actor/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.018722 powerapi-2.1.0/powerapi/backend_supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/backend_supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/backend_supervisor/backend_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.018722 powerapi-2.1.0/powerapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/common_cli_parsing_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33313 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/cli/parsing_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/base_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/csvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/direct_prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/socket_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/database/virtiofs_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/dispatch_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/hwpc_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/power_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/procfs_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatch_rule/simple_dispatch_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/blocking_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/route_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/dispatcher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/simple/simple_dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/abstract_cpu_dram_formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.022722 powerapi-2.1.0/powerapi/formula/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/simple/simple_formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/formula/simple/simple_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/handler/poison_pill_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/handler/start_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/puller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/puller_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/puller/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/simple/simple_puller_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/puller/simple/simple_puller_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/pusher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/pusher_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/pusher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/simple/simple_pusher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/pusher/simple/simple_pusher_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/control_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/formula_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/hwpc_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/power_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/procfs_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.026723 powerapi-2.1.0/powerapi/report_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report_modifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report_modifier/libvirt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/report_modifier/report_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.030722 powerapi-2.1.0/powerapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/stat_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-18 11:53:26.000000 powerapi-2.1.0/powerapi/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:38.018722 powerapi-2.1.0/powerapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-18 11:53:38.000000 powerapi-2.1.0/powerapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-18 11:53:38.000000 powerapi-2.1.0/powerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:53:38.000000 powerapi-2.1.0/powerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-18 11:53:38.000000 powerapi-2.1.0/powerapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 11:53:38.000000 powerapi-2.1.0/powerapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-18 11:53:26.000000 powerapi-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:53:38.030722 powerapi-2.1.0/setup.cfg
```

### Comparing `powerapi-2.0.4/LICENSE` & `powerapi-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/PKG-INFO` & `powerapi-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.4
+Version: 2.1.0
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.4 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.1.0 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.4/README.md` & `powerapi-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/__init__.py` & `powerapi-2.1.0/powerapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.4"
+__version__ = "2.1.0"
```

### Comparing `powerapi-2.0.4/powerapi/actor/__init__.py` & `powerapi-2.1.0/powerapi/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/actor/actor.py` & `powerapi-2.1.0/powerapi/actor/actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/actor/socket_interface.py` & `powerapi-2.1.0/powerapi/actor/socket_interface.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/actor/state.py` & `powerapi-2.1.0/powerapi/actor/state.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/actor/supervisor.py` & `powerapi-2.1.0/powerapi/actor/supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/backend_supervisor/__init__.py` & `powerapi-2.1.0/powerapi/backend_supervisor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/backend_supervisor/backend_supervisor.py` & `powerapi-2.1.0/powerapi/backend_supervisor/backend_supervisor.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,27 +79,18 @@
         When end raise (for exemple by CRTL+C)
         -> Kill all actor in the following order (Puller - Dispatcher/Formula - Pusher)
         1. Send SIGTERM
         2. Join X seconds
         3. If still alive, send SIGKILL
         4. Join
         """
-        def kill_behaviour(the_actor):
-            the_actor.terminate()
-            the_actor.join(5)
-            if the_actor.is_alive():
-                the_actor.kill()
-                the_actor.join()
-
         for actor in self.supervised_actors:
             if not actor.is_alive():
                 self.kill_actors()
                 return
-            else:
-                kill_behaviour(actor)
 
         actor_sentinels = [actor.sentinel for actor in self.supervised_actors]
 
         select.select(actor_sentinels, actor_sentinels, actor_sentinels)
         self.kill_actors()
 
     def join_stream_mode_off(self):
```

### Comparing `powerapi-2.0.4/powerapi/cli/__init__.py` & `powerapi-2.1.0/powerapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/cli/config_validator.py` & `powerapi-2.1.0/powerapi/cli/config_validator.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/cli/generator.py` & `powerapi-2.1.0/powerapi/cli/generator.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/cli/parsing_manager.py` & `powerapi-2.1.0/powerapi/cli/parsing_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,40 +22,42 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
 import sys
 import json
 import logging
 
 from typing import Callable, Any
 from powerapi.cli.config_parser import RootConfigParser, SubgroupConfigParser, store_val
 from powerapi.exception import MissingArgumentException, BadTypeException, \
-    AlreadyAddedSubparserException, UnknownArgException, MissingValueException, BadContextException
+    AlreadyAddedSubparserException, UnknownArgException, MissingValueException, BadContextException, \
+    RepeatedArgumentException, AlreadyAddedSubgroupException
+from powerapi.utils.cli import merge_dictionaries
 
 
 class BaseConfigParsingManager:
     """ Abstract class for dealing with parsing of configurations. """
 
     def __init__(self):
         self.cli_parser = None
 
-    def add_argument_to_cli_parser(self, *names, is_flag: bool = False, action: Callable = store_val,
-                                   default_value: Any = None, help_text: str = '', argument_type: type = str,
-                                   is_mandatory: bool = False):
+    def add_argument(self, *names, is_flag: bool = False, action: Callable = store_val,
+                     default_value: Any = None, help_text: str = '', argument_type: type = str,
+                     is_mandatory: bool = False):
         """
         Add an argument to the parser and its specification
 
         """
         self.cli_parser.add_argument(*names, is_flag=is_flag, action=action, default_value=default_value,
-                                     help_text=help_text, argument_type=argument_type, is_mandatory=is_mandatory)
+                                     help_text=help_text, argument_type=bool if is_flag else argument_type,
+                                     is_mandatory=is_mandatory)
 
     def validate(self, conf: dict) -> dict:
         """ Check the parsed configuration"""
         raise NotImplementedError
 
 
 class SubgroupConfigParsingManager(BaseConfigParsingManager):
@@ -92,40 +94,71 @@
     """
 
     def __init__(self):
         BaseConfigParsingManager.__init__(self)
         self.subparser = {}
         self.cli_parser = RootConfigParser()
 
-    def add_subgroup_parser(self, name: str, subgroup_parser: SubgroupConfigParsingManager, help_text: str = ''):
+    def add_argument_prefix(self, argument_prefix: str):
+        """
+        Add a simple argument prefix to the cli_parser
+        :param argument_prefix: a new argument prefix to be added
+        """
+        self.cli_parser.add_argument_prefix(argument_prefix=argument_prefix)
+
+    def add_subgroup(self, name: str, help_text: str = '', prefix: str = ''):
+        """
+        Add a group to the cli_parser
+        :param name: the group's name
+        :param help_text: a help text for the subgroup
+        :param prefix: a prefix related to the subgroup
+        """
+        try:
+            self.cli_parser.add_subgroup(subgroup_type=name, help_text=help_text, prefix=prefix)
+        except AlreadyAddedSubgroupException as exn:
+            msg = "Configuration error: " + exn.msg
+            logging.error(msg)
+            sys.exit(-1)
+
+    def add_subgroup_parser(self, subgroup_name: str, subgroup_parser: SubgroupConfigParsingManager):
 
         """
         Add a Subgroup Parser to call when <name> is encountered
         When name is encountered, the subgroup parser such as subgroup_parser.name match conf[name].type
 
         """
-        if name in self.subparser:
-            if subgroup_parser.name in list(self.subparser[name]):
-                raise AlreadyAddedSubparserException(name)
+        if subgroup_name in self.subparser:
+            if subgroup_parser.name in list(self.subparser[subgroup_name]):
+                raise AlreadyAddedSubparserException(subgroup_name)
         else:
-            self.subparser[name] = {}
+            self.subparser[subgroup_name] = {}
 
-        self.subparser[name][subgroup_parser.name] = subgroup_parser
+        self.subparser[subgroup_name][subgroup_parser.name] = subgroup_parser
 
-        self.cli_parser.add_subgroup_parser(name, subgroup_parser.cli_parser, help_text)
+        self.cli_parser.add_subgroup_parser(subgroup_type=subgroup_name, subgroup_parser=subgroup_parser.cli_parser)
 
-    def _parse_cli(self, cli_line):
+    def _parse_cli(self, cli_line: list) -> dict:
         return self.cli_parser.parse(cli_line)
 
-    def _parse_config_from_json_file(self, filename):
-        config_file = open(filename, 'r')
-        conf = json.load(config_file)
+    def _parse_config_from_json_file(self, file_name: str, current_conf: dict) -> dict:
+
+        # Select for each argument, le long version name
+        conf = self.cli_parser.parse_config_dict(file_name=file_name)
+
+        conf = merge_dictionaries(source=current_conf, destination=conf)
+
+        return conf
+
+    def _parse_config_from_environment_variables(self, current_conf: dict) -> dict:
+
+        conf = self.cli_parser.parse_config_environment_variables()
 
-        # Select for each argument, le long version
-        return self.cli_parser.parse_config_dict(conf)
+        conf = merge_dictionaries(source=current_conf, destination=conf)
+
+        return conf
 
     def validate(self, conf: dict) -> dict:
         """ Check the parsed configuration"""
 
         # check types
         for current_argument_name, current_argument_value in conf.items():
             is_an_arg = False
@@ -135,50 +168,65 @@
                     is_an_arg = True
 
             if not is_an_arg:
                 for _, argument_definition in self.cli_parser.get_arguments().items():
                     if current_argument_name in argument_definition.names:
                         is_an_arg = True
                         # check type
-                        if not isinstance(current_argument_value, argument_definition.type) and not argument_definition.is_flag:
-                            print('args:', current_argument_name, current_argument_value, argument_definition.type, argument_definition.names)
+                        if not isinstance(current_argument_value,
+                                          argument_definition.type) and not argument_definition.is_flag:
                             raise BadTypeException(current_argument_name, argument_definition.type)
 
             if not is_an_arg:
                 raise UnknownArgException(current_argument_name)
 
         # Check that all the mandatory arguments are present
         conf = self.cli_parser.validate(conf)
 
         return conf
 
     def parse(self, args: list = None) -> dict:
         """
-        Find the configuration method (CLI or config file)
+        Parse the configurations defined via le CLI, Environment Variables and configuration file.
+        The priority of defined values is the following:
+        1. CLI
+        2. Environment Variables
+        3. Configuration File
+
         Call the method to produce a configuration dictionary
         check the configuration
         """
 
         if not args:
             args = sys.argv
+
         current_position = 0
         filename = None
         for current_arg in args:
             if current_arg == '--config-file':
                 if current_position + 1 == len(args):
                     logging.error("CLI Error: config file path needed with argument --config-file")
                     sys.exit(-1)
                 filename = args[current_position + 1]
+                args.pop(current_position + 1)
+                args.pop(current_position)
+                break
             current_position += 1
 
         try:
-            if filename:
-                conf = self._parse_config_from_json_file(filename)
-            else:
+
+            if len(args) > 1:
                 conf = self._parse_cli(args[1:])
+            else:
+                conf = {}
+            conf = self._parse_config_from_environment_variables(current_conf=conf)
+            if filename:
+                conf = self._parse_config_from_json_file(file_name=filename, current_conf=conf)
+
+            # We validate the conf
             conf = self.validate(conf)
 
         except MissingValueException as exn:
             msg = 'CLI error: argument ' + exn.argument_name + ': expect a value'
             logging.error(msg)
             sys.exit(-1)
 
@@ -210,8 +258,12 @@
                 str(exn.colno))
             sys.exit(-1)
 
         except MissingArgumentException as exn:
             logging.error("Configuration Error: " + exn.msg)
             sys.exit(-1)
 
+        except RepeatedArgumentException as exn:
+            logging.error("Configuration Error: " + exn.msg)
+            sys.exit(-1)
+
         return conf
```

### Comparing `powerapi-2.0.4/powerapi/database/__init__.py` & `powerapi-2.1.0/powerapi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/base_db.py` & `powerapi-2.1.0/powerapi/database/base_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/csvdb.py` & `powerapi-2.1.0/powerapi/database/csvdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/direct_prometheus_db.py` & `powerapi-2.1.0/powerapi/database/direct_prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/file_db.py` & `powerapi-2.1.0/powerapi/database/file_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/influxdb.py` & `powerapi-2.1.0/powerapi/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/influxdb2.py` & `powerapi-2.1.0/powerapi/database/influxdb2.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/mongodb.py` & `powerapi-2.1.0/powerapi/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/opentsdb.py` & `powerapi-2.1.0/powerapi/database/opentsdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/prometheus_db.py` & `powerapi-2.1.0/powerapi/database/prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/socket_db.py` & `powerapi-2.1.0/powerapi/database/socket_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/database/virtiofs_db.py` & `powerapi-2.1.0/powerapi/database/virtiofs_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/__init__.py` & `powerapi-2.1.0/powerapi/dispatch_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/dispatch_rule.py` & `powerapi-2.1.0/powerapi/dispatch_rule/dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/hwpc_dispatch_rule.py` & `powerapi-2.1.0/powerapi/dispatch_rule/hwpc_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/power_dispatch_rule.py` & `powerapi-2.1.0/powerapi/dispatch_rule/power_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/procfs_dispatch_rule.py` & `powerapi-2.1.0/powerapi/dispatch_rule/procfs_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatch_rule/simple_dispatch_rule.py` & `powerapi-2.1.0/powerapi/dispatch_rule/simple_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/__init__.py` & `powerapi-2.1.0/powerapi/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/blocking_detector.py` & `powerapi-2.1.0/powerapi/dispatcher/blocking_detector.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/dispatcher_actor.py` & `powerapi-2.1.0/powerapi/dispatcher/dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/handlers.py` & `powerapi-2.1.0/powerapi/dispatcher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/route_table.py` & `powerapi-2.1.0/powerapi/dispatcher/route_table.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/simple/__init__.py` & `powerapi-2.1.0/powerapi/dispatcher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_actor.py` & `powerapi-2.1.0/powerapi/dispatcher/simple/simple_dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/dispatcher/simple/simple_dispatcher_handlers.py` & `powerapi-2.1.0/powerapi/dispatcher/simple/simple_dispatcher_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/exception.py` & `powerapi-2.1.0/powerapi/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 class PowerAPIException(Exception):
     """
     PowerAPIException base class
     """
+
     def __init__(self, *args: object):
         Exception.__init__(self, args)
 
 
 class PowerAPIExceptionWithMessage(PowerAPIException):
     """
     PowerAPIException base class
@@ -53,15 +54,16 @@
     """
 
 
 class ParserException(PowerAPIException):
     """
     Base Exception for parser error
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         PowerAPIException.__init__(self)
         self.argument_name = argument_name
 
 
 class NoNameSpecifiedForSubgroupException(ParserException):
     """
     Exception raised when attempting to parse substring thant describe a component which not contains the component name
@@ -70,97 +72,126 @@
 
 class SubgroupAlreadyExistException(ParserException):
     """
     Exception raised when attempting to parse a substring to create a component with a name that already exist
     """
 
 
+class SubgroupDoesNotExistException(ParserException):
+    """
+    Exception raised when attempting to add arguments to a subgroup that does not exist
+    """
+
+
 class SubgroupParserWithoutNameArgumentException(PowerAPIException):
     """
     Exception raised when a subparser without argument name is added to a parser
     """
 
 
 class TooManyArgumentNamesException(ParserException):
     """
     Exception raised when attemtping to add an argument with too much names
 
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
 
 
 class AlreadyAddedArgumentException(ParserException):
     """
     Exception raised when attempting to add an argument to a parser that already
     have this argument
 
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
         self.msg = 'Parser already contain an argument ' + argument_name
 
 
 class AlreadyAddedSubparserException(ParserException):
     """
-    Exception raised when attempting to add an argument to a parser that already
-    have this argument
+    Exception raised when attempting to add a parser that already exists    """
+
+    def __init__(self, parser_name: str):
+        ParserException.__init__(self, parser_name)
+        self.msg = 'Parser already contain SubParser with name ' + parser_name
+
 
+class AlreadyAddedSubgroupException(ParserException):
     """
-    def __init__(self, argument_name):
-        ParserException.__init__(self, argument_name)
-        self.msg = 'Parser already contain SubParser with name ' + argument_name
+    Exception raised when attempting to add a subgroup that already exists    """
+
+    def __init__(self, subgroup_name: str):
+        ParserException.__init__(self, subgroup_name)
+        self.msg = 'Parser already contain Subgroup with name ' + subgroup_name
 
 
 class MissingArgumentException(ParserException):
     """
     Exception raised when a mandatory argument is missing
     """
 
-    def __init__(self, argument_name):
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
         self.msg = 'Argument with name(s) ' + argument_name + ' is missing'
 
 
+class RepeatedArgumentException(ParserException):
+    """
+    Exception raised when an argument is repeated several times in a configuration
+    """
+
+    def __init__(self, argument_name: str):
+        ParserException.__init__(self, argument_name)
+        self.msg = 'Argument with name(s) ' + argument_name + ' is repeated'
+
+
 class MissingValueException(ParserException):
     """
     Exception raised when an argument that require a value is caught without
     its value
 
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
         self.msg = 'Argument ' + argument_name + ' require a value'
 
 
 class UnknownArgException(ParserException):
     """
     Exception raised when the parser catch an argument that it can't handle
 
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
         self.msg = 'Unknown argument ' + argument_name
 
 
 class BadTypeException(ParserException):
     """
     Exception raised when an argument is parsed with a value of an incorrect type
     """
-    def __init__(self, argument_name, arg_type):
+
+    def __init__(self, argument_name: str, arg_type: type):
         ParserException.__init__(self, argument_name)
         self.msg = argument_name + " expect " + arg_type.__name__
 
 
 class BadContextException(ParserException):
     """
     Exception raised when the parser catch an argument that it can't handle in
     the current context
     """
-    def __init__(self, argument_name, context_list):
+
+    def __init__(self, argument_name: str, context_list: list):
         ParserException.__init__(self, argument_name)
         self.context_list = context_list
         self.msg = 'argument ' + argument_name + 'not used in the correct context\nUse it with the following arguments :'
         for main_arg_name, context_name in context_list:
             self.msg += '\n  --' + main_arg_name + ' ' + context_name
 
 
@@ -171,64 +202,80 @@
     """
 
 
 class FileDoesNotExistException(PowerAPIException):
     """
     This exception happens when the configuration define a input file that does not exist or is not accessible
     """
-    def __init__(self, file_name):
+
+    def __init__(self, file_name: str):
         PowerAPIException.__init__(self)
         self.file_name = file_name
         self.msg = "The File " + self.file_name + " does not exist or is not accessible"
 
 
 class SameLengthArgumentNamesException(ParserException):
     """
-    Exception raised when attemtping to add an argument with names that have the same length
+    Exception raised when attempting to add an argument with names that have the same length
 
     """
-    def __init__(self, argument_name):
+
+    def __init__(self, argument_name: str):
         ParserException.__init__(self, argument_name)
 
 
 class ModelNameAlreadyUsed(PowerAPIException):
     """
     Exception raised when attempting to add to a DBActorGenerator a model factory with a name already bound to another
     model factory in the DBActorGenerator
     """
 
-    def __init__(self, model_name):
+    def __init__(self, model_name: str):
         PowerAPIException.__init__(self)
         self.model_name = model_name
 
 
 class DatabaseNameDoesNotExist(PowerAPIException):
     """
     Exception raised when attempting to remove to a DBActorGenerator a database factory with a name that is not bound to
     another database factory in the DBActorGenerator
     """
 
-    def __init__(self, database_name):
+    def __init__(self, database_name: str):
         PowerAPIException.__init__(self)
         self.database_name = database_name
 
 
 class DatabaseNameAlreadyUsed(PowerAPIException):
     """
     Exception raised when attempting to add to a DBActorGenerator a database factory with a name already bound to
     another database factory in the DBActorGenerator
     """
 
-    def __init__(self, database_name):
+    def __init__(self, database_name: str):
         PowerAPIException.__init__(self)
         self.database_name = database_name
 
 
 class ModelNameDoesNotExist(PowerAPIException):
     """
     Exception raised when attempting to remove to a DBActorGenerator a model factory with a name that is not bound to
     another model factory in the DBActorGenerator
     """
 
-    def __init__(self, model_name):
+    def __init__(self, model_name: str):
         PowerAPIException.__init__(self)
         self.model_name = model_name
+
+
+class InvalidPrefixException(PowerAPIException):
+    """
+    Exception raised when attempting to add a new prefix that is a prefix of a existing one or
+    vice-versa
+    """
+
+    def __init__(self, existing_prefix: str, new_prefix: str):
+        PowerAPIException.__init__(self)
+        self.new_prefix = new_prefix
+        self.existing_prefix = existing_prefix
+        self.msg = "The new prefix " + self.new_prefix + " has a conflict with the existing prefix " \
+                   + self.existing_prefix
```

### Comparing `powerapi-2.0.4/powerapi/filter/__init__.py` & `powerapi-2.1.0/powerapi/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/filter/filter.py` & `powerapi-2.1.0/powerapi/filter/filter.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/__init__.py` & `powerapi-2.1.0/powerapi/formula/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/abstract_cpu_dram_formula.py` & `powerapi-2.1.0/powerapi/formula/abstract_cpu_dram_formula.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/formula_actor.py` & `powerapi-2.1.0/powerapi/formula/formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/handlers.py` & `powerapi-2.1.0/powerapi/formula/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/simple/__init__.py` & `powerapi-2.1.0/powerapi/formula/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/simple/simple_formula_actor.py` & `powerapi-2.1.0/powerapi/formula/simple/simple_formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/formula/simple/simple_handlers.py` & `powerapi-2.1.0/powerapi/formula/simple/simple_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/handler/__init__.py` & `powerapi-2.1.0/powerapi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/handler/handler.py` & `powerapi-2.1.0/powerapi/handler/handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/handler/poison_pill_message_handler.py` & `powerapi-2.1.0/powerapi/handler/poison_pill_message_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/handler/start_handler.py` & `powerapi-2.1.0/powerapi/handler/start_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/message.py` & `powerapi-2.1.0/powerapi/message.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/__init__.py` & `powerapi-2.1.0/powerapi/puller/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/handlers.py` & `powerapi-2.1.0/powerapi/puller/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/puller_actor.py` & `powerapi-2.1.0/powerapi/puller/puller_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/simple/__init__.py` & `powerapi-2.1.0/powerapi/puller/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/simple/simple_puller_actor.py` & `powerapi-2.1.0/powerapi/puller/simple/simple_puller_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/puller/simple/simple_puller_handlers.py` & `powerapi-2.1.0/powerapi/puller/simple/simple_puller_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/__init__.py` & `powerapi-2.1.0/powerapi/pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/handlers.py` & `powerapi-2.1.0/powerapi/pusher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/pusher_actor.py` & `powerapi-2.1.0/powerapi/pusher/pusher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/simple/__init__.py` & `powerapi-2.1.0/powerapi/pusher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_actor.py` & `powerapi-2.1.0/powerapi/pusher/simple/simple_pusher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/pusher/simple/simple_pusher_handlers.py` & `powerapi-2.1.0/powerapi/pusher/simple/simple_pusher_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/__init__.py` & `powerapi-2.1.0/powerapi/report/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/control_report.py` & `powerapi-2.1.0/powerapi/report/control_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/formula_report.py` & `powerapi-2.1.0/powerapi/report/formula_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/hwpc_report.py` & `powerapi-2.1.0/powerapi/report/hwpc_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/power_report.py` & `powerapi-2.1.0/powerapi/report/power_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/procfs_report.py` & `powerapi-2.1.0/powerapi/report/procfs_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report/report.py` & `powerapi-2.1.0/powerapi/report/report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report_modifier/__init__.py` & `powerapi-2.1.0/powerapi/report_modifier/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report_modifier/libvirt_mapper.py` & `powerapi-2.1.0/powerapi/report_modifier/libvirt_mapper.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/report_modifier/report_modifier.py` & `powerapi-2.1.0/powerapi/report_modifier/report_modifier.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/utils/__init__.py` & `powerapi-2.1.0/powerapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/utils/cli.py` & `powerapi-2.1.0/powerapi/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2023, INRIA
-# Copyright (c) 2023, University of Lille
+# Copyright (c) 2021, INRIA
+# Copyright (c) 2021, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,36 +23,45 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-def remove_first_characters(arg: str):
+import collections.abc as collections
+import datetime
+
+
+def timestamp_to_datetime(timestamp):
     """
-    Remove the two first characters of arg if it has more than 2 characters, otherwise, it removes only the first one.
-    :param str arg: The string to remove the first characters
+    Create datetime from a timestamp value
+
+    :param int timestamp:
+    :rtype: datetime.datetime
     """
-    if len(arg) > 2:
-        return arg[2:]
-    return arg[1]
+    return datetime.datetime.fromtimestamp(timestamp / 1000)
 
 
-def find_longest_string_in_list(string_list: list):
+def datetime_to_timestamp(date):
     """
-    Find the largest string contained in the given list
-    :param list string_list: List of strings
+    Cast a datetime object to a simple timestamp
+
+    :param datetime.datetime date:
+    :rtype: int
     """
-    max_len = 0
-    longest_string = ''
-    for name in string_list:
-        if len(name) > max_len:
-            longest_string = name
-            max_len = len(name)
-    return longest_string
+    return int(datetime.datetime.timestamp(date) * 1000)
 
 
-def string_to_bool(bool_value: str):
+def dict_merge(dict1, dict2):
     """
-    Transforms a str to bool according to their content
+    Recursive dict merge, act like dict.update() but update
+    all level and not only top-level.
+
+    :param dict dict1:
+    :param dict dict2:
+
     """
-    return bool_value.lower() in ("yes", "true", "t", "1")
+    for key, value in dict2.items():
+        if (key in dict1 and isinstance(dict1[key], dict) and isinstance(dict2[key], collections.Mapping)):
+            dict_merge(dict1[key], dict2[key])
+        else:
+            dict1[key] = value
```

### Comparing `powerapi-2.0.4/powerapi/utils/json_stream.py` & `powerapi-2.1.0/powerapi/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/utils/stat_buffer.py` & `powerapi-2.1.0/powerapi/utils/stat_buffer.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/utils/sync.py` & `powerapi-2.1.0/powerapi/utils/sync.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi/utils/tree.py` & `powerapi-2.1.0/powerapi/utils/tree.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi.egg-info/PKG-INFO` & `powerapi-2.1.0/powerapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.4
+Version: 2.1.0
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.4 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.1.0 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.4/powerapi.egg-info/SOURCES.txt` & `powerapi-2.1.0/powerapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/powerapi.egg-info/requires.txt` & `powerapi-2.1.0/powerapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.4/pyproject.toml` & `powerapi-2.1.0/pyproject.toml`

 * *Files identical despite different names*

