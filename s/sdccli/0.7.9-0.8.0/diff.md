# Comparing `tmp/sdccli-0.7.9.tar.gz` & `tmp/sdccli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdccli-0.7.9.tar", max compression
+gzip compressed data, was "sdccli-0.8.0.tar", max compression
```

## Comparing `sdccli-0.7.9.tar` & `sdccli-0.8.0.tar`

### file list

```diff
@@ -1,74 +1,73 @@
--rw-r--r--   0        0        0     1067 2021-04-14 09:50:37.618261 sdccli-0.7.9/LICENSE.txt
--rw-r--r--   0        0        0      937 2021-04-14 09:50:48.366396 sdccli-0.7.9/pyproject.toml
--rw-r--r--   0        0        0       21 2021-04-14 09:50:48.366396 sdccli-0.7.9/sdccli/__init__.py
--rw-r--r--   0        0        0     2127 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/__init__.py
--rw-r--r--   0        0        0     5291 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/alert.py
--rw-r--r--   0        0        0     9160 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/backup.py
--rw-r--r--   0        0        0     5549 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/capture.py
--rw-r--r--   0        0        0     3924 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/command.py
--rw-r--r--   0        0        0     8177 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/compliance.py
--rw-r--r--   0        0        0     7144 2021-04-14 09:50:37.618261 sdccli-0.7.9/sdccli/cli/dashboard/__init__.py
--rw-r--r--   0        0        0     5036 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/dashboard/panel.py
--rw-r--r--   0        0        0     7872 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/dashboardv2.py
--rw-r--r--   0        0        0     4617 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/event.py
--rw-r--r--   0        0        0     4406 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/eventv1.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/__init__.py
--rw-r--r--   0        0        0      139 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/json_formatter/__init__.py
--rw-r--r--   0        0        0      841 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/__init__.py
--rw-r--r--   0        0        0      464 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/alert.py
--rw-r--r--   0        0        0      887 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/dashboard.py
--rw-r--r--   0        0        0     1017 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/panel.py
--rw-r--r--   0        0        0     1962 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/policy_events.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/__init__.py
--rw-r--r--   0        0        0      537 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/alert.py
--rw-r--r--   0        0        0     4497 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/image.py
--rw-r--r--   0        0        0     3583 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
--rw-r--r--   0        0        0    18732 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/__init__.py
--rw-r--r--   0        0        0     3528 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/falco_list.py
--rw-r--r--   0        0        0     3548 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/falco_macro.py
--rw-r--r--   0        0        0    10159 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/policy/rule.py
--rw-r--r--   0        0        0     6687 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/profile.py
--rw-r--r--   0        0        0      884 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/__init__.py
--rw-r--r--   0        0        0     3788 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/alert.py
--rw-r--r--   0        0        0     7778 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/cve_report.py
--rw-r--r--   0        0        0     8439 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/image.py
--rw-r--r--   0        0        0     3925 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/policy.py
--rw-r--r--   0        0        0     3702 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/query.py
--rw-r--r--   0        0        0     4148 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/registry.py
--rw-r--r--   0        0        0     3419 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/repo.py
--rw-r--r--   0        0        0     1470 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/runtime.py
--rw-r--r--   0        0        0     2484 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/subscription.py
--rw-r--r--   0        0        0     4079 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/vulnerability/__init__.py
--rw-r--r--   0        0        0     1848 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/scanning/vulnerability/bundle.py
--rw-r--r--   0        0        0      587 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/__init__.py
--rw-r--r--   0        0        0     1893 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/access_key.py
--rw-r--r--   0        0        0     3071 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/notification.py
--rw-r--r--   0        0        0     7376 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/team.py
--rw-r--r--   0        0        0     3749 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/cli/settings/user.py
--rw-r--r--   0        0        0     5394 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/config.py
--rw-r--r--   0        0        0     8316 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/drop.py
--rw-r--r--   0        0        0     2804 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/falco_macro.py
--rw-r--r--   0        0        0      639 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/helpers.py
--rw-r--r--   0        0        0      796 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/printer.py
--rw-r--r--   0        0        0    20309 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/restore.py
--rw-r--r--   0        0        0     1493 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/time.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/__init__.py
--rw-r--r--   0        0        0     2379 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/alert.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/Pipfile
--rw-r--r--   0        0        0       42 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/__init__.py
--rw-r--r--   0        0        0    12512 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/dump.py
--rw-r--r--   0        0        0    13838 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/backup/restore.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/__init__.py
--rw-r--r--   0        0        0     5161 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v2.py
--rw-r--r--   0        0        0     6105 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v3.py
--rw-r--r--   0        0        0     6903 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/dashboard/panel.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/policy/__init__.py
--rw-r--r--   0        0        0     2247 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/policy/events.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/__init__.py
--rw-r--r--   0        0        0     1137 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/alert.py
--rw-r--r--   0        0        0     4084 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/image.py
--rw-r--r--   0        0        0     3781 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/scanning/vulnerability.py
--rw-r--r--   0        0        0        0 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/settings/__init__.py
--rw-r--r--   0        0        0      530 2021-04-14 09:50:37.622262 sdccli-0.7.9/sdccli/usecases/settings/team.py
--rw-r--r--   0        0        0     1341 2021-04-14 09:50:48.895765 sdccli-0.7.9/setup.py
--rw-r--r--   0        0        0      872 2021-04-14 09:50:48.896160 sdccli-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-18 06:41:23.873646 sdccli-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      952 2023-07-18 06:41:41.566273 sdccli-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-07-18 06:41:41.566273 sdccli-0.8.0/sdccli/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/__init__.py
+-rw-r--r--   0        0        0     5291 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/alert.py
+-rw-r--r--   0        0        0     9586 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/backup.py
+-rw-r--r--   0        0        0     5549 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/capture.py
+-rw-r--r--   0        0        0     3924 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/command.py
+-rw-r--r--   0        0        0     8177 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/compliance.py
+-rw-r--r--   0        0        0     8388 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/dashboard/__init__.py
+-rw-r--r--   0        0        0     5036 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/dashboard/panel.py
+-rw-r--r--   0        0        0     7875 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/dashboardv2.py
+-rw-r--r--   0        0        0     4617 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/event.py
+-rw-r--r--   0        0        0     4406 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/eventv1.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/__init__.py
+-rw-r--r--   0        0        0      139 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/json_formatter/__init__.py
+-rw-r--r--   0        0        0      841 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/__init__.py
+-rw-r--r--   0        0        0      464 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/alert.py
+-rw-r--r--   0        0        0      887 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/dashboard.py
+-rw-r--r--   0        0        0     1017 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/panel.py
+-rw-r--r--   0        0        0     1992 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/policy_events.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/__init__.py
+-rw-r--r--   0        0        0      537 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/alert.py
+-rw-r--r--   0        0        0     4553 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/image.py
+-rw-r--r--   0        0        0     3583 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py
+-rw-r--r--   0        0        0    18732 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/policy/__init__.py
+-rw-r--r--   0        0        0     3528 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/policy/falco_list.py
+-rw-r--r--   0        0        0     3548 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/policy/falco_macro.py
+-rw-r--r--   0        0        0    10159 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/policy/rule.py
+-rw-r--r--   0        0        0     6687 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/profile.py
+-rw-r--r--   0        0        0      884 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/__init__.py
+-rw-r--r--   0        0        0     3788 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/alert.py
+-rw-r--r--   0        0        0     7778 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/cve_report.py
+-rw-r--r--   0        0        0     8444 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/image.py
+-rw-r--r--   0        0        0     3925 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/policy.py
+-rw-r--r--   0        0        0     3702 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/query.py
+-rw-r--r--   0        0        0     4148 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/registry.py
+-rw-r--r--   0        0        0     3419 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/repo.py
+-rw-r--r--   0        0        0     1470 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/runtime.py
+-rw-r--r--   0        0        0     2484 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/subscription.py
+-rw-r--r--   0        0        0     4079 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/vulnerability/__init__.py
+-rw-r--r--   0        0        0     1848 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/scanning/vulnerability/bundle.py
+-rw-r--r--   0        0        0      587 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/settings/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/settings/access_key.py
+-rw-r--r--   0        0        0     3071 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/settings/notification.py
+-rw-r--r--   0        0        0     7376 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/settings/team.py
+-rw-r--r--   0        0        0     3749 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/cli/settings/user.py
+-rw-r--r--   0        0        0     7450 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/config.py
+-rw-r--r--   0        0        0     9102 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/drop.py
+-rw-r--r--   0        0        0     2804 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/falco_macro.py
+-rw-r--r--   0        0        0      769 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/helpers.py
+-rw-r--r--   0        0        0      796 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/printer.py
+-rw-r--r--   0        0        0    23837 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/restore.py
+-rw-r--r--   0        0        0     1493 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/time.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/usecases/__init__.py
+-rw-r--r--   0        0        0     2379 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/usecases/alert.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/usecases/backup/Pipfile
+-rw-r--r--   0        0        0       42 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/usecases/backup/__init__.py
+-rw-r--r--   0        0        0    13890 2023-07-18 06:41:23.881646 sdccli-0.8.0/sdccli/usecases/backup/dump.py
+-rw-r--r--   0        0        0    15088 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/backup/restore.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/dashboard/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/dashboard/dashboard_v2.py
+-rw-r--r--   0        0        0     7644 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/dashboard/dashboard_v3.py
+-rw-r--r--   0        0        0     6903 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/dashboard/panel.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/policy/__init__.py
+-rw-r--r--   0        0        0     2247 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/policy/events.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/scanning/__init__.py
+-rw-r--r--   0        0        0     1137 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/scanning/alert.py
+-rw-r--r--   0        0        0     4084 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/scanning/image.py
+-rw-r--r--   0        0        0     3781 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/scanning/vulnerability.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/settings/__init__.py
+-rw-r--r--   0        0        0      530 2023-07-18 06:41:23.885647 sdccli-0.8.0/sdccli/usecases/settings/team.py
+-rw-r--r--   0        0        0     1006 1970-01-01 00:00:00.000000 sdccli-0.8.0/PKG-INFO
```

### Comparing `sdccli-0.7.9/LICENSE.txt` & `sdccli-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/pyproject.toml` & `sdccli-0.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "sdccli"
-version = "0.7.9"
+version = "0.8.0"
 description = "CLI client for Sysdig Cloud"
 authors = ["Sysdig Inc. <info@sysdig.com>"]
 license = "MIT"
 maintainers = [
     "Nestor Salceda <nestor.salceda@sysdig.com>",
     "Federico Barcelona <fede.barcelona@sysdig.com>"
 ]
 documentation = "https://sysdiglabs.github.io/sysdig-platform-cli/"
 
 [tool.poetry.scripts]
 sdc-cli = 'sdccli.cli:cli'
 
 [tool.poetry.dependencies]
 python = "^3.6"
-click = "^7.1.2"
-prettytable = "^0.7.2"
+click = "^8.0.1"
+prettytable = "^2"
 pyyaml = "^5.3.1"
 requests = "^2"
 python-dateutil = "^2.8.1"
-sdcclient = "^0.15.1"
+sdcclient = "^0.17.0"
+httmock = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
-mamba = "^0.11.1"
+mamba = "^0.11.2"
 expects = "^0.9.0"
 flake8 = "^3.8.4"
 doublex = "^1.9.2"
 doublex-expects = "^0.7.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `sdccli-0.7.9/sdccli/cli/__init__.py` & `sdccli-0.8.0/sdccli/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,9 +52,9 @@
 cli.add_command(event)
 cli.add_command(policy)
 cli.add_command(scanning)
 cli.add_command(profile)
 cli.add_command(settings)
 cli.add_command(dashboard_v2)
 
-if getattr(sys, 'frozen', False):
+if getattr(sys, 'frozen', False) or __name__ == '__main__':
     cli(sys.argv[1:])
```

### Comparing `sdccli-0.7.9/sdccli/cli/alert.py` & `sdccli-0.8.0/sdccli/cli/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/backup.py` & `sdccli-0.8.0/sdccli/cli/backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from pathlib import Path
-
-import click
-import yaml
 import os
 import os.path
 import sys
-from sdccli import drop
-from sdccli import restore
+from pathlib import Path
+
+import click
+
 from sdccli.usecases.backup import *
 
 
 @click.group(name='backup', short_help="Backup operations")
 def backup():
     pass
 
@@ -20,66 +18,66 @@
 @click.argument('backup-file', nargs=1)
 @click.argument('section', nargs=-1)
 @click.pass_obj
 def dump(cnf, overwrite, backup_file, section):
     """
     BACKUP_FILE: File where the data must be saved to.
 
-    SECTION: Restore only the specified section. Valid values: dashboards, notification_channels, alerts, users, teams_monitor, teams_secure, policies, falco_rules, falco_lists, falco_macros
+    SECTION: Backup only the specified section. Valid values: dashboards, notification_channels, alerts, users, teams_monitor, teams_secure, policies, falco_rules, falco_lists, falco_macros, scanning_alerts
     """
     backup_file_path = Path(backup_file)
     if backup_file_path.exists() and not overwrite:
         print("Error: file {} already exists. Use -f if you want to overwrite it.".format(backup_file))
         sys.exit(1)
 
     if not backup_file_path.parent.exists():
         backup_file_path.parent.mkdir(parents=True)
 
     if backup_file_path.exists() and not backup_file_path.is_file():
         print("Error: {} is not file".format(backup_file))
         sys.exit(1)
 
-    sdmonitor = cnf.sdmonitor
-    sdsecure = cnf.sdsecure
-
     repository = open(backup_file, mode='w')
     use_cases_to_execute = []
 
     if not section or 'dashboards' in section:
-        use_cases_to_execute.append(DumpDashboardsUseCase(sdmonitor, repository))
+        use_cases_to_execute.append(DumpDashboardsUseCase(cnf.sdmonitor, repository))
 
     if not section or 'notification_channels' in section:
-        use_cases_to_execute.append(DumpNotificationChannelsUseCase(sdmonitor, repository))
+        use_cases_to_execute.append(DumpNotificationChannelsUseCase(cnf.sdmonitor, repository))
 
     if not section or 'alerts' in section:
-        use_cases_to_execute.append(DumpAlertsUseCase(sdmonitor, repository))
+        use_cases_to_execute.append(DumpAlertsUseCase(cnf.sdmonitor, repository))
 
     if not section or 'users' in section:
-        use_cases_to_execute.append(DumpUsersUseCase(sdmonitor, repository))
+        use_cases_to_execute.append(DumpUsersUseCase(cnf.sdmonitor, repository))
 
     if not section or 'teams_monitor' in section:
-        use_cases_to_execute.append(DumpTeamsMonitorUseCase(sdmonitor, repository))
+        use_cases_to_execute.append(DumpTeamsMonitorUseCase(cnf.sdmonitor, repository))
 
     if not section or 'teams_secure' in section:
-        use_cases_to_execute.append(DumpTeamsSecureUseCase(sdsecure, repository))
+        use_cases_to_execute.append(DumpTeamsSecureUseCase(cnf.sdsecure, repository))
 
     if not section or 'policies' in section:
         if cnf.sdsecure.policy_v2:
-            use_cases_to_execute.append(DumpPoliciesUseCase(sdsecure, repository))
+            use_cases_to_execute.append(DumpPoliciesUseCase(cnf.sdsecure, repository))
         else:
             use_cases_to_execute.append(DumpPoliciesUseCase(cnf.sdsecure_v1, repository))
 
     if not section or 'falco_rules' in section:
-        use_cases_to_execute.append(DumpUserCreatedRulesUseCase(sdsecure, repository))
+        use_cases_to_execute.append(DumpUserCreatedRulesUseCase(cnf.sdsecure, repository))
 
     if not section or 'falco_lists' in section:
-        use_cases_to_execute.append(DumpUserCreatedFalcoListsUseCase(sdsecure, repository))
+        use_cases_to_execute.append(DumpUserCreatedFalcoListsUseCase(cnf.sdsecure, repository))
 
     if not section or 'falco_macros' in section:
-        use_cases_to_execute.append(DumpUserCreatedFalcoMacrosUseCase(sdsecure, repository))
+        use_cases_to_execute.append(DumpUserCreatedFalcoMacrosUseCase(cnf.sdsecure, repository))
+
+    if not section or 'scanning_alerts' in section:
+        use_cases_to_execute.append(DumpScanningAlertsUseCase(cnf.sdsecure, cnf.sdscanning, repository))
 
     errors = []
     for use_case in use_cases_to_execute:
         ok, res = use_case.execute()
         if not ok:
             errors.append(res)
 
@@ -124,85 +122,88 @@
 @click.option('--all-users', is_flag=True, help="Restore dashboards even if you are not the owner "
                                                 "(may duplicate the dashboards if they already exist in the environment)")
 @click.pass_obj
 def restore_from_backup(cnf, backup_file, section, full, all_users):
     """
     BACKUP_PATH: File where the data must be restored from.
 
-    SECTION: Restore only the specified section. Valid values: dashboards, notification_channels, alerts, users, teams_monitor, teams_secure, policies, falco_rules, falco_lists, falco_macros.
+    SECTION: Restore only the specified section. Valid values: dashboards, notification_channels, alerts, users, teams_monitor, teams_secure, policies, falco_rules, falco_lists, falco_macros, scanning_alerts.
     """
     if not os.path.isfile(backup_file):
         print("Error: {} is not a correct backup file".format(backup_file))
         sys.exit(1)
 
-    sdmonitor = cnf.sdmonitor
-    sdsecure = cnf.sdsecure
-
     use_cases_to_execute = []
 
     if not section or 'dashboards' in section:
         if full:
             if all_users:
-                use_cases_to_execute.append(
-                    RemoveAllAndRestoreAllDashboardsUseCase(sdmonitor, open(backup_file, mode='r')))
+                use_cases_to_execute.append(RemoveAllAndRestoreAllDashboardsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
             else:
-                use_cases_to_execute.append(
-                    RemoveOwnedAndRestoreOwnedDashboardsUseCase(sdmonitor, open(backup_file, mode='r')))
+                use_cases_to_execute.append(RemoveOwnedAndRestoreOwnedDashboardsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
         else:
             if all_users:
-                use_cases_to_execute.append(RestoreAllDashboardsUseCase(sdmonitor, open(backup_file, mode='r')))
+                use_cases_to_execute.append(RestoreAllDashboardsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
             else:
-                use_cases_to_execute.append(RestoreOwnedDashboardsUseCase(sdmonitor, open(backup_file, mode='r')))
+                use_cases_to_execute.append(RestoreOwnedDashboardsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
 
     if not section or 'notification_channels' in section:
         if full:
-            use_cases_to_execute.append(
-                RemoveAndRestoreNotificationChannelsUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RemoveAndRestoreNotificationChannelsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
         else:
-            use_cases_to_execute.append(RestoreNotificationChannelsUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RestoreNotificationChannelsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
 
     if not section or 'alerts' in section:
         if full:
-            use_cases_to_execute.append(RemoveAndRestoreAlertsUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RemoveAndRestoreAlertsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
         else:
-            use_cases_to_execute.append(RestoreAlertsUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RestoreAlertsUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
 
     if not section or 'users' in section:
-        use_cases_to_execute.append(RestoreUsersUseCase(sdmonitor, open(backup_file, mode='r')))
+        use_cases_to_execute.append(RestoreUsersUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
 
     if not section or 'teams_monitor' in section:
         if full:
-            use_cases_to_execute.append(RemoveAndRestoreTeamsMonitorUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RemoveAndRestoreTeamsMonitorUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
         else:
-            use_cases_to_execute.append(RestoreTeamsMonitorUseCase(sdmonitor, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RestoreTeamsMonitorUseCase(cnf.sdmonitor, open(backup_file, mode='r')))
 
     if not section or 'teams_secure' in section:
         if full:
-            use_cases_to_execute.append(RemoveAndRestoreTeamsSecureUseCase(sdsecure, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RemoveAndRestoreTeamsSecureUseCase(cnf.sdsecure, open(backup_file, mode='r')))
         else:
-            use_cases_to_execute.append(RestoreTeamsSecureUseCase(sdsecure, open(backup_file, mode='r')))
+            use_cases_to_execute.append(RestoreTeamsSecureUseCase(cnf.sdsecure, open(backup_file, mode='r')))
 
     if full:
         if not section or 'policies' in section:
-            use_cases_to_execute.append(RemovePoliciesUseCase(sdsecure))
+            use_cases_to_execute.append(RemovePoliciesUseCase(cnf.sdsecure))
         if not section or 'falco_rules' in section:
-            use_cases_to_execute.append(RemoveFalcoRulesUseCase(sdsecure))
+            use_cases_to_execute.append(RemoveFalcoRulesUseCase(cnf.sdsecure))
         if not section or 'falco_macros' in section:
-            use_cases_to_execute.append(RemoveFalcoMacrosUseCase(sdsecure))
+            use_cases_to_execute.append(RemoveFalcoMacrosUseCase(cnf.sdsecure))
         if not section or 'falco_lists' in section:
-            use_cases_to_execute.append(RemoveFalcoListsUseCase(sdsecure))
+            use_cases_to_execute.append(RemoveFalcoListsUseCase(cnf.sdsecure))
 
     if not section or 'falco_lists' in section:
-        use_cases_to_execute.append(RestoreFalcoListsUseCase(sdsecure, open(backup_file, mode='r')))
+        use_cases_to_execute.append(RestoreFalcoListsUseCase(cnf.sdsecure, open(backup_file, mode='r')))
     if not section or 'falco_macros' in section:
-        use_cases_to_execute.append(RestoreFalcoMacrosUseCase(sdsecure, open(backup_file, mode='r')))
+        use_cases_to_execute.append(RestoreFalcoMacrosUseCase(cnf.sdsecure, open(backup_file, mode='r')))
     if not section or 'falco_rules' in section:
-        use_cases_to_execute.append(RestoreFalcoRulesUseCase(sdsecure, open(backup_file, mode='r')))
+        use_cases_to_execute.append(RestoreFalcoRulesUseCase(cnf.sdsecure, open(backup_file, mode='r')))
     if not section or 'policies' in section:
-        use_cases_to_execute.append(RestorePoliciesUseCase(sdsecure, open(backup_file, mode='r')))
+        use_cases_to_execute.append(RestorePoliciesUseCase(cnf.sdsecure, open(backup_file, mode='r')))
+
+    if not section or 'scanning_alerts' in section:
+        if full:
+            use_cases_to_execute.append(RemoveScanningAlertsUseCase(cnf.sdscanning_alerts_v1))
+        use_cases_to_execute.append(RestoreScanningAlertsUseCase(
+            cnf.sdsecure_v1,
+            cnf.sdscanning_alerts_v1,
+            open(backup_file, mode='r'),
+        ))
 
     errors = []
     for use_case in use_cases_to_execute:
         ok, res = use_case.execute()
         if not ok:
             errors.append(res)
```

### Comparing `sdccli-0.7.9/sdccli/cli/capture.py` & `sdccli-0.8.0/sdccli/cli/capture.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/command.py` & `sdccli-0.8.0/sdccli/cli/command.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/compliance.py` & `sdccli-0.8.0/sdccli/cli/compliance.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/dashboard/__init__.py` & `sdccli-0.8.0/sdccli/cli/dashboard/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,33 +43,57 @@
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
 
 
 @dashboard.command(name='add-json', short_help="Add dashboards from a json file")
 @click.argument('jsonfile', nargs=1, type=click.Path(exists=True))
+@click.option('--ignore-sharing-settings', is_flag=True, help="Ignores the sharing settings configured in the JSON, "
+                                                              "not sending them to the API")
 @click.pass_obj
-def add_json(cnf, jsonfile):
+def add_json(cnf, jsonfile, ignore_sharing_settings):
     """
     JSONFILE: A file with a json description of one or multiple dashboards
     """
     try:
         with open(jsonfile) as f:
             dashboard_json = json.load(f)
     except Exception as error:
         print("Error parsing rules file (%s): %s" % (jsonfile, str(error)))
         sys.exit(1)
 
     try:
-        res = use_case.add_json_dashboard(cnf.sdmonitor, dashboard_json)
+        res = use_case.add_json_dashboard(cnf.sdmonitor, dashboard_json, ignore_sharing_settings)
         cnf.formatter.format(res, "dashboard")
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
 
+@dashboard.command(name='update-json', short_help="Update dashboards from a json file")
+@click.argument('jsonfile', nargs=1, type=click.Path(exists=True))
+@click.option('--ignore-sharing-settings', is_flag=True, help="Ignores the sharing settings configured in the JSON, "
+                                                              "not sending them to the API")
+@click.pass_obj
+def update_json(cnf, jsonfile, ignore_sharing_settings):
+    """
+    JSONFILE: A file with a json description of one or multiple dashboards
+    """
+    try:
+        with open(jsonfile) as f:
+            dashboard_json = json.load(f)
+    except Exception as error:
+        print("Error parsing rules file (%s): %s" % (jsonfile, str(error)))
+        sys.exit(1)
+
+    try:
+        res = use_case.update_json_dashboard(cnf.sdmonitor, dashboard_json, ignore_sharing_settings)
+        cnf.formatter.format(res, "dashboard")
+    except Exception as ex:
+        print(f"Error: {str(ex)}")
+        sys.exit(1)
 
 @dashboard.command(name='list', short_help="List all dashboards")
 @click.pass_obj
 def list_dashboards(cnf):
     try:
         res = use_case.list_dashboards(cnf.sdmonitor)
         cnf.formatter.format(res, "dashboardList")
```

### Comparing `sdccli-0.7.9/sdccli/cli/dashboard/panel.py` & `sdccli-0.8.0/sdccli/cli/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/dashboardv2.py` & `sdccli-0.8.0/sdccli/cli/dashboardv2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import sys
 
 import click
 
-import sdccli.usecases.dashboard.dashboard_v2 as use_case
 import sdccli.helpers as helpers
+import sdccli.usecases.dashboard.dashboard_v2 as use_case
 
 
 @click.group(name='dashboard_v2', short_help='Sysdig Monitor dashboard operations')
 def dashboard_v2():
     pass
 
 
@@ -41,15 +41,15 @@
         cnf.formatter.format(res, "dashboard")
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
 
 
 @dashboard_v2.command(name='add-panel',
-                   short_help="Adds a panel to the dashboard. A panel can be a time series, or a top chart (i.e. bar chart), or a number panel.")
+                      short_help="Adds a panel to the dashboard. A panel can be a time series, or a top chart (i.e. bar chart), or a number panel.")
 @click.argument('dashboard', nargs=1)
 @click.argument('name', nargs=1)
 @click.option('--type', nargs=1, default="timeSeries",
               help="type of the new panel. Valid values are: 'timeSeries', 'top', 'number'")
 @click.option('--metric', nargs=1, multiple=True, required=True,
               help="Specify a metric to show in the panel. A metric comes in the form of 'metricId:aggregation:groupKey'. A metricId is any of the entries that can "
                    "be found in the Metrics section of the Explore page in Sysdig Monitor. A grouping key is any of the entries that can be found in the Show or "
```

### Comparing `sdccli-0.7.9/sdccli/cli/event.py` & `sdccli-0.8.0/sdccli/cli/event.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/eventv1.py` & `sdccli-0.8.0/sdccli/cli/eventv1.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/__init__.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/dashboard.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/dashboard.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/panel.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/policy_events.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/policy_events.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     }
 
 
 def print_policy_event_v1(event):
     event["date"] = datetime.strftime(parser.parse(event["timestamp"]), "%Y-%m-%d %H:%M:%S %Z")
     event["type"] = event["originator"]
     event["severity"] = _severity_mapping[event["severity"]]
-    event["tags"] = ", ".join(event["content"].get("ruleTags", []))
+    ruleTags = event["content"].get("ruleTags", []) or []
+    event["tags"] = ", ".join(ruleTags)
     event["output"] = event["content"].get("output", "")
     print_item(event, ["id", "name", "description", "date", "type", "severity", "output", "tags"])
 
     if "fields" in event["content"]:
         print("fields:")
         max_size = max(len(k) for k in event["content"]["fields"].keys())
         for key, value in event["content"]["fields"].items():
```

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/alert.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/image.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,43 @@
 
 from sdccli.printer import print_item, print_list
 
 
 def formats():
     return {
         "scanningImage": _print_image,
+        "scanningImageAdded": _print_image_added,
         "scanningImageList": _print_images,
         "scanningQueryImage": _print_query,
         "scanningVulnImage": _print_vuln,
         "scanningEvaluationImage": _print_evaluation,
     }
 
 
-def _print_image(images):
+def _print_image_added(images):
     for image in images:
-        image["fulltag"] = [d["fulltag"] for d in image['image_detail']]
-        if 'image_content' in image and image['image_content']:
-            image_content = image['image_content']
-            if 'metadata' in image_content and image_content['metadata']:
-                image_content_metadata = image_content['metadata']
-                image['dockerfile_mode'] = str(image_content_metadata['dockerfile_mode'])
-                image['distro'] = str(image_content_metadata['distro'])
-                image['distro_version'] = str(image_content_metadata['distro_version'])
-                image['size'] = str(image_content_metadata['image_size'])
-                image['arch'] = str(image_content_metadata['arch'])
-                image['layer_count'] = str(image_content_metadata['layer_count'])
-
-        keys = ["imageDigest", "imageId", "parentDigest", "analysis_status", "image_type", "fulltag",
-                "dockerfile_mode", "distro", "distro_version", "size", "arch", "layer_count", "annotations"]
-        print_item(image, keys)
+        _print_image(image)
+
+
+def _print_image(image):
+    image["fulltag"] = [d["fulltag"] for d in image['image_detail']]
+    if 'image_content' in image and image['image_content']:
+        image_content = image['image_content']
+        if 'metadata' in image_content and image_content['metadata']:
+            image_content_metadata = image_content['metadata']
+            image['dockerfile_mode'] = str(image_content_metadata['dockerfile_mode'])
+            image['distro'] = str(image_content_metadata['distro'])
+            image['distro_version'] = str(image_content_metadata['distro_version'])
+            image['size'] = str(image_content_metadata['image_size'])
+            image['arch'] = str(image_content_metadata['arch'])
+            image['layer_count'] = str(image_content_metadata['layer_count'])
+
+    keys = ["imageDigest", "imageId", "parentDigest", "analysis_status", "image_type", "fulltag",
+            "dockerfile_mode", "distro", "distro_version", "size", "arch", "layer_count", "annotations"]
+    print_item(image, keys)
 
 
 def _print_query(res):
     res, query_type = res
     if not query_type:
         for t in res:
             print("%s: available" % (t,))
@@ -116,8 +121,8 @@
         print("Warn results:")
         for warn_result in scan_info["warn_results"]:
             print(f"  - {warn_result}")
 
     if scan_info["stop_results"]:
         print("Stop results:")
         for stop_result in scan_info["stop_results"]:
-            print(f"  x {stop_result}")
+            print(f"  x {stop_result}")
```

### Comparing `sdccli-0.7.9/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py` & `sdccli-0.8.0/sdccli/cli/formatter/text_formatter/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/policy/__init__.py` & `sdccli-0.8.0/sdccli/cli/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/policy/falco_list.py` & `sdccli-0.8.0/sdccli/cli/policy/falco_list.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/policy/falco_macro.py` & `sdccli-0.8.0/sdccli/cli/policy/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/policy/rule.py` & `sdccli-0.8.0/sdccli/cli/policy/rule.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/profile.py` & `sdccli-0.8.0/sdccli/cli/profile.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/__init__.py` & `sdccli-0.8.0/sdccli/cli/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/alert.py` & `sdccli-0.8.0/sdccli/cli/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/cve_report.py` & `sdccli-0.8.0/sdccli/cli/scanning/cve_report.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/image.py` & `sdccli-0.8.0/sdccli/cli/scanning/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     try:
         res = use_case.add_scanning_image(cnf.sdscanning,
                                           input_image,
                                           force=force,
                                           dockerfile=dockerfile_contents,
                                           annotations=annotations,
                                           autosubscribe=not noautosubscribe)
-        cnf.formatter.format(res, "scanningImage")
+        cnf.formatter.format(res, "scanningImageAdded")
     except Exception as ex:
         print(f"Error: {str(ex)}")
         sys.exit(1)
 
 
 @image.command(name='list', short_help="List all images")
 @click.option('--full', is_flag=True, help="Show full row output for each image")
```

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/policy.py` & `sdccli-0.8.0/sdccli/cli/scanning/policy.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/query.py` & `sdccli-0.8.0/sdccli/cli/scanning/query.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/registry.py` & `sdccli-0.8.0/sdccli/cli/scanning/registry.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/repo.py` & `sdccli-0.8.0/sdccli/cli/scanning/repo.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/runtime.py` & `sdccli-0.8.0/sdccli/cli/scanning/runtime.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/subscription.py` & `sdccli-0.8.0/sdccli/cli/scanning/subscription.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/vulnerability/__init__.py` & `sdccli-0.8.0/sdccli/cli/scanning/vulnerability/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/scanning/vulnerability/bundle.py` & `sdccli-0.8.0/sdccli/cli/scanning/vulnerability/bundle.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/settings/__init__.py` & `sdccli-0.8.0/sdccli/cli/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/settings/access_key.py` & `sdccli-0.8.0/sdccli/cli/settings/access_key.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/settings/notification.py` & `sdccli-0.8.0/sdccli/cli/settings/notification.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/settings/team.py` & `sdccli-0.8.0/sdccli/cli/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/cli/settings/user.py` & `sdccli-0.8.0/sdccli/cli/settings/user.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/config.py` & `sdccli-0.8.0/sdccli/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import os.path
 
 import yaml
-from sdcclient import SdMonitorClient
-from sdcclient import SdMonitorClient as SdMonitorClientV2
-from sdcclient import SdSecureClient, SdScanningClient, SdSecureClientV1
+from sdcclient import SdMonitorClient, SdMonitorClient as SdMonitorClientV2, SdSecureClient, SdScanningClient, \
+    SdSecureClientV1
 from sdcclient.monitor import EventsClientV1
-from sdcclient.secure import PolicyEventsClientOld
+from sdcclient.secure import PolicyEventsClientOld, ScanningAlertsClientV1
 
 from sdccli.cli.formatter.json_formatter import JsonFormatter
 from sdccli.cli.formatter.text_formatter import NormalFormatter
 
 
 class Config(object):
     __default_config_paths = [
@@ -23,14 +22,29 @@
 
     def __init__(self, json=False):
         self.json = json
         self.formatter = JsonFormatter() if json else NormalFormatter()
         self.monitor = {}
         self.secure = {}
 
+    def load_from_text(self, text, env=None):
+        try:
+            config = yaml.load(text, Loader=yaml.SafeLoader)
+        except yaml.YAMLError as exc:
+            raise Exception("error in configuration file:", exc)
+
+        if "envs" not in config:
+            raise Exception("config file does not have a envs parent")
+
+        if env not in config["envs"]:
+            raise Exception("environment provided '{}' not found in the configuration file, "
+                            "envs found: {}".format(env, list(config['envs'].keys())))
+
+        self.__config_with_defaults(config["envs"][env])
+
     def load(self, path=None, env=None):
         env = env if env is not None else os.getenv("SDC_ENV", "main")
 
         if path is None or path == "":
             found = False
             for file_path in self.__default_config_paths:
                 if os.path.isfile(file_path):
@@ -40,27 +54,15 @@
                 self.__config_with_defaults()
                 return
         else:
             if not os.path.isfile(path):
                 raise EnvironmentError("couldn't find the provided config file: {}".format(path))
 
         with open(path, "r") as f:
-            try:
-                config = yaml.load(f, Loader=yaml.SafeLoader)
-            except yaml.YAMLError as exc:
-                raise Exception("error in configuration file:", exc)
-
-            if "envs" not in config:
-                raise Exception("config file does not have a envs parent")
-
-            if env not in config["envs"]:
-                raise Exception("environment provided '{}' not found in the configuration file, "
-                                "envs found: {}".format(env, list(config['envs'].keys())))
-
-            self.__config_with_defaults(config["envs"][env])
+            self.load_from_text(f.read(), env)
 
     def __config_with_defaults(self, config=None):
         if config is None:
             config = {}
 
         monitor_token = os.environ.get('SDC_TOKEN')
         if os.environ.get('SDC_MONITOR_TOKEN'):
@@ -98,54 +100,92 @@
         if not (self.monitor['ssl_verify'] and self.secure['ssl_verify']):
             # suppress the InsecureRequestWarning when non tls connections are created
             import urllib3
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     @property
     def events_client_v1(self):
+        if "token" not in self.monitor:
+            raise PermissionError("attempt to execute a Monitor operation without providing a Monitor token")
         return EventsClientV1(
             token=self.monitor["token"],
             sdc_url=self.monitor["url"],
-            ssl_verify=self.monitor["ssl_verify"]
+            ssl_verify=self.monitor["ssl_verify"],
+            custom_headers=self.monitor.get("extra_headers", {})
         )
 
     @property
     def sdmonitor(self):
+        if "token" not in self.monitor:
+            raise PermissionError("attempt to execute a Monitor operation without providing a Monitor token")
         return SdMonitorClient(
             token=self.monitor["token"],
             sdc_url=self.monitor["url"],
-            ssl_verify=self.monitor["ssl_verify"])
+            ssl_verify=self.monitor["ssl_verify"],
+            custom_headers=self.monitor.get("extra_headers", {})
+        )
 
     @property
     def sdmonitor_v2(self):
+        if "token" not in self.monitor:
+            raise PermissionError("attempt to execute a Monitor operation without providing a Monitor token")
         return SdMonitorClientV2(
             token=self.monitor["token"],
             sdc_url=self.monitor["url"],
-            ssl_verify=self.monitor["ssl_verify"])
+            ssl_verify=self.monitor["ssl_verify"],
+            custom_headers=self.monitor.get("extra_headers", {})
+        )
 
     @property
     def policy_events_client_old(self):
+        if "token" not in self.monitor:
+            raise PermissionError("attempt to execute a Monitor operation without providing a Monitor token")
         return PolicyEventsClientOld(
             token=self.monitor["token"],
             sdc_url=self.monitor["url"],
-            ssl_verify=self.monitor["ssl_verify"])
+            ssl_verify=self.monitor["ssl_verify"],
+            custom_headers=self.monitor.get("extra_headers", {})
+        )
 
     @property
     def sdsecure(self):
+        if "token" not in self.secure:
+            raise PermissionError("attempt to execute a Secure operation without providing a Secure token")
         return SdSecureClient(
             token=self.secure["token"],
             sdc_url=self.secure["url"],
-            ssl_verify=self.secure["ssl_verify"])
+            ssl_verify=self.secure["ssl_verify"],
+            custom_headers=self.secure.get("extra_headers", {})
+        )
 
     @property
     def sdsecure_v1(self):
+        if "token" not in self.secure:
+            raise PermissionError("attempt to execute a Secure operation without providing a Secure token")
         return SdSecureClientV1(
             token=self.secure["token"],
             sdc_url=self.secure["url"],
-            ssl_verify=self.secure["ssl_verify"])
+            ssl_verify=self.secure["ssl_verify"],
+            custom_headers=self.secure.get("extra_headers", {})
+        )
 
     @property
     def sdscanning(self):
+        if "token" not in self.secure:
+            raise PermissionError("attempt to execute a Secure operation without providing a Secure token")
         return SdScanningClient(
             token=self.secure["token"],
             sdc_url=self.secure["url"],
-            ssl_verify=self.secure["ssl_verify"])
+            ssl_verify=self.secure["ssl_verify"],
+            custom_headers=self.secure.get("extra_headers", {})
+        )
+
+    @property
+    def sdscanning_alerts_v1(self):
+        if "token" not in self.secure:
+            raise PermissionError("attempt to execute a Secure operation without providing a Secure token")
+        return ScanningAlertsClientV1(
+                token=self.secure["token"],
+                sdc_url=self.secure["url"],
+                ssl_verify=self.secure["ssl_verify"],
+                custom_headers=self.secure.get("extra_headers", {})
+        )
```

### Comparing `sdccli-0.7.9/sdccli/drop.py` & `sdccli-0.8.0/sdccli/drop.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from multiprocessing.pool import ThreadPool
 
 from sdcclient import SdSecureClient
+from sdcclient.secure import ScanningAlertsClientV1
 
 from sdccli.falco_macro import SortMacrosByDepedency
+from sdccli.helpers import is_managed_policy
 
 ORIGIN_SECURE_UI = 'Secure UI'
 ORIGIN_SYSDIG = 'Sysdig'
 
 
 def dashboards(sdmonitor, remove_unowned=False):
     ok, data = sdmonitor.get_dashboards()
@@ -216,17 +218,22 @@
     return True, sorted_macros_by_dependency
 
 
 def policies(sdsecure: SdSecureClient):
     ok, data = sdsecure.list_policies()
     if not ok:
         return False, data
+
     # Policies are the only resource that can be removed with an origin different from "Secure UI".
     # Policies from "Sysdig" can also be removed. This does not happen with rules, lists, etc.
-    removable_policies = [policy for policy in data if policy['origin'] in [ORIGIN_SECURE_UI, ORIGIN_SYSDIG]]
+    removable_policies = [
+            policy
+            for policy in data
+            if policy['origin'] in [ORIGIN_SECURE_UI, ORIGIN_SYSDIG] and not is_managed_policy(policy)
+    ]
 
     errors = []
     res = []
     total = len(removable_policies)
 
     for i, policy in enumerate(removable_policies, start=1):
         print(f"[{i}/{total}] Removing policy {policy['name'].strip()}... ")
@@ -276,7 +283,33 @@
         removed, err = sdmonitor.delete_notification_channel(channel)
         if removed:
             res.append(channel)
         else:
             print("Error: " + err)
 
     return True, res
+
+
+def scanning_alerts(client: ScanningAlertsClientV1):
+    ok, data = client.list_alerts()
+    if not ok:
+        return False, data
+
+    res = []
+    errors = []
+    total = len(data['alerts'])
+    for i, alert in enumerate(data['alerts']):
+        print("[{}/{}] Removing scanning alert {}... ".format(
+            i + 1,
+            total,
+            alert['name']
+        ))
+        removed, err = client.delete_alert(alert['alertId'])
+        if removed:
+            res.append(alert)
+        else:
+            errors.append(err)
+
+    if len(errors) > 0:
+        return False, errors
+
+    return True, res
```

### Comparing `sdccli-0.7.9/sdccli/falco_macro.py` & `sdccli-0.8.0/sdccli/falco_macro.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/printer.py` & `sdccli-0.8.0/sdccli/printer.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/restore.py` & `sdccli-0.8.0/sdccli/restore.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
+import typing
 
 import requests
-from sdcclient import SdSecureClient, SdMonitorClient
+from sdcclient import SdSecureClient, SdMonitorClient, SdSecureClientV1
 from sdcclient._common import _SdcCommon
+from sdcclient.secure import ScanningAlertsClientV1
 
 from sdccli.falco_macro import SortMacrosByDepedency
 
 ORIGIN_SECURE_UI = "Secure UI"
 
 
 def dashboards(file_data, sdmonitor, existing_dashboards, restore_unowned):
@@ -510,15 +512,14 @@
                          ['id']):
                 print("      already exists, skip")
                 ids_changed[str(id)] = str(existing_channels[name]['id'])
                 continue
             else:
                 sdmonitor.delete_notification_channel(existing_channels[name])
 
-        del channel["teamId"]
         ok, result = sdmonitor.create_notification_channel(channel)
         if not ok:
             errors.append("couldn't recreate team " + channel['name'] + ': ' + result)
         else:
             ids_changed[str(id)] = str(result["notificationChannel"]["id"])
 
     if errors:
@@ -532,14 +533,122 @@
         print('Restoring user falco rules...')
         ok, result = sdsecure.set_user_falco_rules(file_data["userRulesFile"]["content"])
         if not ok:
             return False, result
         return True, None
 
 
+def scanning_alerts(alerts: typing.List[dict],
+                    notif_channels: typing.Dict[str, dict],
+                    secure: SdSecureClientV1,
+                    scanning: ScanningAlertsClientV1):
+
+    def unique_name(name: str, names: typing.Set[str]) -> str:
+        new_name = name
+        i = 1
+
+        while new_name in names:
+            new_name = f'{name} ({i})'
+            i += 1
+
+        return new_name
+
+    errors = []
+
+    ok, res = scanning.list_alerts()
+    if not ok:
+        return False, res
+
+    existing_alerts = {alert['name']: alert for alert in res['alerts']}
+
+    ok, nc_res = secure.list_notification_channels()
+    if not ok:
+        return False, nc_res
+
+    existing_nc = {nc['name']: nc for nc in nc_res['notificationChannels']}
+
+    restored = []
+    total = len(alerts)
+    for i, alert in enumerate(alerts):
+        print("[{}/{}] Creating scanning alert {}... ".format(i + 1, total, alert['name']))
+
+        if alert['name'] in existing_alerts:
+            if equal_scanning_alerts(alert, existing_alerts[alert['name']]):
+                print("      already exists, skip")
+                continue
+            alert['name'] = unique_name(alert['name'], set(existing_alerts.keys()))
+
+        alert_nc_names = {notif_channels[nc_id]['name'] for nc_id in alert['notificationChannelIds']}
+
+        new_alert_nc_ids = []
+        for nc_name in alert_nc_names:
+            if nc_name not in existing_nc:
+                print(f"  Warning: The Notification Channel '{nc_name}' does not exist in the environment, "
+                      f"the restored scanning alert won't be assigned to this NC.")
+                continue
+            new_alert_nc_ids.append(existing_nc[nc_name]['id'])
+
+        alert['notificationChannelIds'] = new_alert_nc_ids
+        del alert['alertId']
+        del alert['createdAt']
+        del alert['customerId']
+        del alert['teamId']
+        del alert['updatedAt']
+
+        ok, res = scanning.add_alert_object(alert)
+        if not ok:
+            errors.append(res)
+            continue
+        restored.append(res)
+
+    if errors:
+        return False, errors
+
+    return True, restored
+
+
+def equal_scanning_alerts(a1: dict, a2: dict) -> bool:
+    if a1.get('enabled', False) != a2.get('enabled', False):
+        return False
+    if a1['type'] != a2['type']:
+        return False
+    if a1['name'] != a2['name']:
+        return False
+    if a1.get('description', '') != a2.get('description', ''):
+        return False
+    if a1.get('scope', '') != a2.get('scope', ''):
+        return False
+    if a1['triggers'] != a2['triggers']:
+        return False
+    if a1['autoscan'] != a2['autoscan']:
+        return False
+    if a1['onlyPassFail'] != a2['onlyPassFail']:
+        return False
+    if a1['skipEventSend'] != a2['skipEventSend']:
+        return False
+
+    def repo_to_str(r): return f'{r["registry"]}/{r["repository"]}:{r["tag"]}'
+    a1_repo_dict = {repo_to_str(r): r for r in a1.get('repositories', [])}
+    a2_repo_dict = {repo_to_str(r): r for r in a2.get('repositories', [])}
+    if len(a1_repo_dict) != len(a2_repo_dict):
+        return False
+    for k, v in a1_repo_dict.items():
+        if k not in a2_repo_dict:
+            return False
+        if a2_repo_dict[k] != v:
+            return False
+
+    a1_notif = sorted(a1.get('notificationChannelIds', []))
+    a2_notif = sorted(a2.get('notificationChannelIds', []))
+    if a1_notif != a2_notif:
+        return False
+
+    return True
+
+
 def same_dict(d1, d2, skip_keys):
     if (d1.keys() - skip_keys) != (d2.keys() - skip_keys):
         return False
 
     for k in d1.keys():
         if k in skip_keys:
             continue
```

### Comparing `sdccli-0.7.9/sdccli/time.py` & `sdccli-0.8.0/sdccli/time.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/alert.py` & `sdccli-0.8.0/sdccli/usecases/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/backup/dump.py` & `sdccli-0.8.0/sdccli/usecases/backup/dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 
 class DumpTeamsMonitorUseCase(DumpMonitorUseCase):
     def __init__(self, monitor, repository):
         super().__init__(monitor, repository)
 
     def execute(self):
-        ok, res = self._monitor.get_teams()
+        ok, res = self._monitor.get_teams(product_filter='SDC')
         if not ok:
             return ok, res
         self._sort_res(res)
 
         res = [{"kind": "monitor_teams", "version": 1, "spec": res}]
 
         self._repository.write(self._formatter(res))
@@ -145,15 +145,15 @@
 
 
 class DumpTeamsSecureUseCase(DumpSecureUseCase):
     def __init__(self, secure, repository):
         super().__init__(secure, repository)
 
     def execute(self):
-        ok, res = self._secure.get_teams()
+        ok, res = self._secure.get_teams(product_filter='SDS')
         if not ok:
             return ok, res
         self._sort_res(res)
 
         res = [{"kind": "secure_teams", "version": 1, "spec": res}]
 
         self._repository.write(self._formatter(res))
@@ -343,29 +343,69 @@
 
         if len(errors) > 0:
             return False, errors
 
         return True, falco_lists
 
 
+class DumpScanningAlertsUseCase(DumpSecureUseCase):
+    def __init__(self, secure, scanning, repository):
+        super().__init__(secure, repository)
+        self.scanning = scanning
+
+    def execute(self):
+        ok, res_alerts = self.scanning.list_alerts()
+        if not ok:
+            return ok, res_alerts
+        self._sort_res(res_alerts)
+
+        ok, res_nc = self._secure.list_notification_channels()
+        if not ok:
+            return ok, res_nc
+        self._sort_res(res_nc)
+
+        used_nc = {
+            nc
+            for alert in res_alerts.get('alerts')
+            for nc in alert['notificationChannelIds']
+        }
+
+        res = [{
+            "kind": "scanning_alerts",
+            "version": 1,
+            "spec": {
+                'alerts_response': res_alerts,
+                'notification_channels': {
+                    nc['id']: nc
+                    for nc in res_nc['notificationChannels']
+                    if nc['id'] in used_nc
+                }
+            }
+        }]
+
+        self._repository.write(self._formatter(res))
+        return ok, res
+
+
 class DumpEverythingUseCase(object):
-    def __init__(self, monitor, secure, repository):
+    def __init__(self, monitor, secure, sdscanning, repository):
         # Monitor
         self._dump_users_to_repository = DumpUsersUseCase(monitor, repository)
         self._dump_dashboards_to_repository = DumpDashboardsUseCase(monitor, repository)
         self._dump_alerts_to_repository = DumpAlertsUseCase(monitor, repository)
         self._dump_teams_monitor_to_repository = DumpTeamsMonitorUseCase(monitor, repository)
         self._dump_notification_channels_to_repository = DumpNotificationChannelsUseCase(monitor,
                                                                                          repository)
         # Secure
         self._dump_teams_secure_to_repository = DumpTeamsSecureUseCase(secure, repository)
         self._dump_policies_to_repository = DumpPoliciesUseCase(secure, repository)
         self._dump_rules_to_repository = DumpUserCreatedRulesUseCase(secure, repository)
         self._dump_falco_macros_to_repository = DumpUserCreatedFalcoMacrosUseCase(secure, repository)
         self._dump_falco_lists_to_repository = DumpUserCreatedFalcoListsUseCase(secure, repository)
+        self._dump_scanning_alerts_to_repository = DumpScanningAlertsUseCase(secure, sdscanning, repository)
 
     def execute(self):
         errors = []
 
         # Monitor
         ok, res = self._dump_users_to_repository.execute()
         if not ok:
@@ -400,11 +440,15 @@
         if not ok:
             errors.append(res)
 
         ok, res = self._dump_falco_lists_to_repository.execute()
         if not ok:
             errors.append(res)
 
+        ok, res = self._dump_scanning_alerts_to_repository.execute()
+        if not ok:
+            errors.append(res)
+
         if len(errors) > 0:
             return False, errors
 
         return True, []
```

### Comparing `sdccli-0.7.9/sdccli/usecases/backup/restore.py` & `sdccli-0.8.0/sdccli/usecases/backup/restore.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 
 import yaml
 
 import sdccli.drop as drop
 import sdccli.restore as restore
+from sdccli.helpers import is_managed_policy
 
 
 def _same_dict(d1, d2, skip_keys):
     if (d1.keys() - skip_keys) != (d2.keys() - skip_keys):
         return False
 
     for k in d1.keys():
@@ -92,15 +93,14 @@
 
     def execute(self):
         file_data = self._load_data_from_repo("notification_channels")
         file_data = [item for sublist in file_data for item in sublist['notificationChannels']]  # Flatten lists
 
         _, res = self._monitor.list_notification_channels()
         existing_channels = {n['name']: n for n in res['notificationChannels']}
-
         return restore.notification_channels(file_data, self._monitor, existing_channels)
 
 
 class RemoveAndRestoreNotificationChannelsUseCase(RestoreMonitorUseCase):
     def __init__(self, monitor, repository, formatter=yaml.safe_load):
         super().__init__(monitor, repository, formatter)
 
@@ -330,31 +330,59 @@
 class RestorePoliciesUseCase(RestoreSecureUseCase):
     def __init__(self, secure, repository, formatter=yaml.safe_load):
         super().__init__(secure, repository, formatter)
 
     def execute(self):
         file_data = self._load_data_from_repo("policies")
         file_data = [item for sublist in file_data for item in sublist]  # Flatten lists
-
-        return restore.policies(file_data, self._secure)
+        restorable_policies = [
+            policy
+            for policy in file_data
+            if not is_managed_policy(policy)
+        ]
+        return restore.policies(restorable_policies, self._secure)
 
 
 class RemoveAndRestorePoliciesUseCase(RestoreSecureUseCase):
     def __init__(self, secure, repository, formatter=yaml.safe_load):
         super().__init__(secure, repository, formatter)
 
     def execute(self):
         file_data = self._load_data_from_repo("policies")
         file_data = [item for sublist in file_data for item in sublist]  # Flatten lists
-
+        restorable_policies = [
+                policy
+                for policy in file_data
+                if not is_managed_policy(policy)
+        ]
         ok, res = drop.policies(self._secure)
         if not ok:
             return False, res
+        return restore.policies(restorable_policies, self._secure)
+
 
-        return restore.policies(file_data, self._secure)
+class RestoreScanningAlertsUseCase(RestoreSecureUseCase):
+    def __init__(self, secure, scanning, repository, formatter=yaml.safe_load):
+        super().__init__(secure, repository, formatter)
+        self.scanning = scanning
+
+    def execute(self):
+        data = list(self._load_data_from_repo("scanning_alerts"))
+        alerts = [
+            alert
+            for kind in data
+            for alert in kind['alerts_response']['alerts']
+        ]
+
+        notif_channels = {
+            id: nc
+            for kind in data
+            for id, nc in kind['notification_channels'].items()
+        }
+        return restore.scanning_alerts(alerts, notif_channels, self._secure, self.scanning)
 
 
 class RemoveSecureUseCase(RemoveUseCase):
     def __init__(self, secure):
         self._secure = secure
 
 
@@ -384,7 +412,15 @@
 
 class RemoveFalcoMacrosUseCase(RemoveSecureUseCase):
     def __init__(self, secure):
         super().__init__(secure)
 
     def execute(self):
         return drop.falco_macros(self._secure)
+
+
+class RemoveScanningAlertsUseCase(RemoveSecureUseCase):
+    def __init__(self, secure):
+        super().__init__(secure)
+
+    def execute(self):
+        return drop.scanning_alerts(self._secure)
```

### Comparing `sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v2.py` & `sdccli-0.8.0/sdccli/usecases/dashboard/dashboard_v2.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/dashboard/dashboard_v3.py` & `sdccli-0.8.0/sdccli/usecases/dashboard/dashboard_v3.py`

 * *Files 20% similar despite different names*

```diff
@@ -145,21 +145,24 @@
         layout=panel.layout_dict)
     if not ok:
         raise Exception(res)
 
     return res["dashboard"]
 
 
-def add_json_dashboard(monitor, dashboard):
+def add_json_dashboard(monitor, dashboard, remove_sharing_settings=False):
     result = ""
 
     def add_json(monitor, dboard):
         if "dashboard" in dboard:
             dboard = dboard["dashboard"]
 
+        if remove_sharing_settings:
+            dboard['sharingSettings'] = []
+            dboard['shared'] = False
         dboard['timeMode'] = {'mode': 1}
         dboard['time'] = {'last': 2 * 60 * 60 * 1000000, 'sampling': 2 * 60 * 60 * 1000000}
         ok, res = monitor.create_dashboard_with_configuration(dboard)
         if ok:
             return "Created dashboard {}".format(dboard['name'])
         else:
             raise Exception("Error creating the dashboard {}: {}".format(dboard['name'], res))
@@ -171,14 +174,51 @@
         result = add_json(monitor, dashboard)
     else:
         raise Exception("Unsupported JSON format")
 
     return result
 
 
+def update_json_dashboard(monitor, dashboard, remove_sharing_settings=False):
+    result = ""
+
+    def update_json(monitor, dboard):
+        if "dashboard" in dboard:
+            dboard = dboard["dashboard"]
+        # If the dashboard exists, update it. If not, create it
+        try:
+            found = get_dashboard_by_id_or_name(monitor, dboard['id'])
+        except: 
+            return add_json_dashboard(monitor, dboard)
+        if remove_sharing_settings:
+            dboard['sharingSettings'] = []
+            dboard['shared'] = False
+        dboard['timeMode'] = {'mode': 1}
+        dboard['time'] = {'last': 2 * 60 * 60 * 1000000, 'sampling': 2 * 60 * 60 * 1000000}
+        ok, res = monitor.update_dashboard(dboard)
+        if ok:
+            return "Updated dashboard {}".format(dboard['name'])
+        if "status code 409" in res:            
+            raise Exception("Error updating for existing more recent version in dashboard {}: {}".format(dboard['name'], res))
+        else:
+            raise Exception("Error updating the dashboard {}: {}".format(dboard['name'], res))
+        
+
+
+    if isinstance(dashboard, list):
+        for db in dashboard:
+            result += update_json(monitor, db) + "\n"
+    elif isinstance(dashboard, dict):
+        result = update_json(monitor, dashboard)
+    else:
+        raise Exception("Unsupported JSON format")
+
+    return result
+
+
 def remove_panel_from_dashboard(monitor, dashboard, name):
     ok, res = monitor.remove_dashboard_panel(dashboard, name)
 
     if not ok:
         raise Exception("Error deleting dashboard ({}): {}".format(id, res))
```

### Comparing `sdccli-0.7.9/sdccli/usecases/dashboard/panel.py` & `sdccli-0.8.0/sdccli/usecases/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/policy/events.py` & `sdccli-0.8.0/sdccli/usecases/policy/events.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/scanning/alert.py` & `sdccli-0.8.0/sdccli/usecases/scanning/alert.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/scanning/image.py` & `sdccli-0.8.0/sdccli/usecases/scanning/image.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/scanning/vulnerability.py` & `sdccli-0.8.0/sdccli/usecases/scanning/vulnerability.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/sdccli/usecases/settings/team.py` & `sdccli-0.8.0/sdccli/usecases/settings/team.py`

 * *Files identical despite different names*

### Comparing `sdccli-0.7.9/PKG-INFO` & `sdccli-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: sdccli
-Version: 0.7.9
+Version: 0.8.0
 Summary: CLI client for Sysdig Cloud
 License: MIT
 Author: Sysdig Inc.
 Author-email: info@sysdig.com
 Maintainer: Nestor Salceda
 Maintainer-email: nestor.salceda@sysdig.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: prettytable (>=0.7.2,<0.8.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.1,<9.0.0)
+Requires-Dist: httmock (>=1.4.0,<2.0.0)
+Requires-Dist: prettytable (>=2,<3)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: sdcclient (>=0.15.1,<0.16.0)
+Requires-Dist: sdcclient (>=0.17.0,<0.18.0)
 Project-URL: Documentation, https://sysdiglabs.github.io/sysdig-platform-cli/
```

