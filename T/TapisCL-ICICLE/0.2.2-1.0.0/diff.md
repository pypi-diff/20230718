# Comparing `tmp/TapisCL-ICICLE-0.2.2.tar.gz` & `tmp/TapisCL-ICICLE-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.2.2.tar", last modified: Tue Jul 11 23:32:52 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-1.0.0.tar", last modified: Tue Jul 18 18:12:53 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.2.2.tar` & `TapisCL-ICICLE-1.0.0.tar`

### file list

```diff
@@ -1,59 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.474839 TapisCL-ICICLE-0.2.2/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    44898 2023-07-11 23:32:52.474336 TapisCL-ICICLE-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3015 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/README.md
--rw-rw-rw-   0        0        0     1222 2023-07-11 23:32:32.000000 TapisCL-ICICLE-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 23:32:52.474839 TapisCL-ICICLE-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.445412 TapisCL-ICICLE-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.446807 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.449804 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10294 2023-07-11 22:01:19.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    13905 2023-07-11 23:10:26.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.458433 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0    14439 2023-07-11 22:55:10.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/appCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.460425 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     7310 2023-07-11 22:55:48.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0    20538 2023-07-11 22:05:10.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10475 2023-07-11 17:43:00.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2190 2023-06-21 21:26:22.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1757 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    11359 2023-07-06 00:05:20.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     6692 2023-07-11 21:52:39.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0    10586 2023-07-11 20:26:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.462418 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4414 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0    25444 2023-07-11 23:15:25.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/systemCommands.py
--rw-rw-rw-   0        0        0     8018 2023-07-05 23:06:02.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.464411 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10250 2023-07-11 21:49:02.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.465585 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4404 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.468850 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.471840 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44898 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1692 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-11 23:32:52.000000 TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-0.2.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:32:52.472837 TapisCL-ICICLE-0.2.2/tests/
--rw-rw-rw-   0        0        0      191 2023-07-10 17:51:41.000000 TapisCL-ICICLE-0.2.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    50383 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8502 2023-07-12 23:36:44.000000 TapisCL-ICICLE-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1227 2023-07-18 18:09:08.000000 TapisCL-ICICLE-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.727013 TapisCL-ICICLE-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.729007 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.731078 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10788 2023-07-18 17:46:54.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.737564 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.740555 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/__init__.py
+-rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appCommands.py
+-rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+-rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appForms.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.742548 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/__init__.py
+-rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemCommands.py
+-rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemForms.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.745058 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     9283 2023-07-18 16:53:44.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argumentValidators.py
+-rw-rw-rw-   0        0        0    20827 2023-07-18 17:33:56.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10791 2023-07-18 16:22:47.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1828 2023-07-18 17:57:50.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    11399 2023-07-17 16:26:08.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7191 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.747413 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.749406 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.751400 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.754909 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.759110 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    50383 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.759110 TapisCL-ICICLE-1.0.0/tests/
+-rw-rw-rw-   0        0        0       81 2023-07-17 16:51:58.000000 TapisCL-ICICLE-1.0.0/tests/test.py
```

### Comparing `TapisCL-ICICLE-0.2.2/LICENSE` & `TapisCL-ICICLE-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/PKG-INFO` & `TapisCL-ICICLE-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.2.2
+Version: 1.0.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,31 +695,109 @@
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
 1. `pip install TapisCL-ICICLE`. Current version 0.0.24
-2. `python -m TapisCLICICLE`
+2. run using `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
-3. `python cli.py`
-### Operations
-#### **Full Terminal Interface:**
-1. run ``python -m TapisCLICICLE``
-2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be icicle.tapis.io
-3. the application will then prompt you to choose your authentication method, password, federated, or device code. Which ones are avaiable depends on the tenant in question. If you choose either the 2nd or 3rd option, you will be asked to create a session password to authenticate secure operations.
-4. if all went well the console should open. You can run `help` to see command options
-5. to exit the application, run `exit`. To shut it down, run `shutdown`. The server automatically shuts down after 25 minutes of inactivity
+3. from the src folder, run using `python -m TapisCLICICLE`
 
-#### **Bash Command Line:**
+### Known Issues
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
 
-Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
+## Usage
+### Interfaces
+TapisCLICICLE supports two interface types:
+#### Full Terminal Interface:
+If you want a full fledged command line environment to interact with your Tapis services, run the app using `python -m TapisCLICICLE` with no additional arguments. This will spawn the environment where you can enter commands.
+#### Bash Command Line:
+Alternatively, if you want to enter commands directly into your bash terminal, you can run the app with arguments. For example, `python -m TapisCLICICLE create_pod (pod_name) (pod_template)` will create a pod without opening the app environment. The same goes for all commands.
 
-`python -m TapisCLICICLE help -v`
+### Authentication
+TapisCLICICLE supports 3 authentication methods, password, federated, and device code grants. Authentication has a timeout of 5000 seconds of inactivity.
+For each method of authentication, you will be asked to submit a tenant URI. This determines what resources you will have access to. 
+For both federated and device code grants, you will be prompted to create a session password for secure operations (like obtaining pod credentials)
+#### Password
+You can log in to the app using an account username and password for the TACC portal. You must obtain an account directly from TACC to use this login method.
+
+#### Federated
+Requires a valid CILogon account through your university, with google, or with ORCID. Upon selecting this method, a webpage will open requesting login with one of these methods. Once you are authenticated you will receive an access token on the webpage. Dont show this token to anyone. Simultaneously you will be prompted to enter this token on the TapisCLICICLE app. Once you do, you will be authenticated and can use the app.
+
+#### Device Code
+This is functionally the same as the federated authentication, except you are prompted to enter an app generated user code to generate your token after logging in using CILogon. Once you generate your token you must confirm completion on the app and you will be authenticated
+
+#### Notes on Authentication
+Both federated and device code grants are experiemental at the current state in development, and work on only a few tenants
+
+### Help
+TapisCLICICLE supports several Tapis services for interfacing with HPC systems. Basic information on these services can be obtained using the `help` command.
+If you want to get a list of commands which fall under a certain service, enter the service name into the command line. For example, running `Systems` will show all commands under the systems service
+To get information about an individual command, you can run `(command) -h`. This will list all command syntax. Running `(command) -h -v`, specifying verbose with -v will give detailed description of each argument associated with the command
+When running help commands, arguments marked with an (f) do not receive values directly, but send a request for a form back to the client.
+
+### Commands
+Commands in TapisCLICICLE can be divided into 2 classifications: creational and managerial
+
+#### General Commands
+General commands are for managing and viewing information on your current application session.
+
+General Commands:
+* whoami: return information about the current logged in user
+* whereami: return the current tenant URI
+* switch_tenant_to --tenant_uri (tenant_uri) --auth (auth type): log in to a different tenant without shutting down the app. Tenant URI is the base URL of the tenant you want to connect to. For example, icicle.tapis.io, or smartfoods.tapis.io. The auth parameter must be one of the 3 authentication methods previously mentioned, password, federated, or device_code grant.
+* exit: exit the current instance of the application client without deactivating the app entirely. The app continues to run in the background until timeout, or a new user session starts. Starting the client again after
+* shutdown: completely shut down the application client and background. If you want to run the application again you will have to re-authenticate
+* user (username): gets information about the user connected to the specified username
+* get_tenants: gets a list of available tenants to connect to
+* get_tenant (tenant_id): get more detailed information about a specific tenant specified by the tenant id.
+* manpages: brings you to this page
+
+#### Creational
+These commands are for creating and updating Tapis services like pods and systems. These commands generally have lots of optional arguments for configuration, and forms to fill out. If you choose, in lieu of writing your configurations in the command line you can write and upload your own service config file from an application generated config file template. For all creational commands, you can do this by adding the argument `-f (path to your config file)`
+In the event that you do make a mistake while writing your config in the command line, your work is saved to a config file (the application will tell you where when this happens). When you fix the errors in the config file you can immediately re-upload it to try again.
+
+Creational commands include:
+* create_system
+* update_system
+* create_pod
+* update_pod
+* create_volume
+* update_volume
+* create_snapshot
+* update_snapshot
+* create_app
+* update_app
+* submit_job
+
+##### Generating Config Files
+WIP
+
+#### Managerial
+Managerial commands are generally for getting information about the Tapis services you have access to, managing permissions, state, and sharing for those services. These wont usually have more than 3 arguments. 
+
+### Services
+Each Tapis service has their own command group which allows you to interface with that service. Currently, TapisCLICICLE supports 7 services:
+* Systems
+* Files
+* Apps
+* Jobs
+* Pods
+* Volumes
+* Query
+
+#### Systems
+Systems lie at the core of most workflows in Tapis, and TapisCLICICLE. They are representations of your account on an HPC system, and interface with HPC resources using SSH. You can read more specifics about Tapis systems [here](https://tapis.readthedocs.io/en/latest/technical/systems.html). Systems enable the user to store and access files on as well as run jobs on that resource. 
+Each system has 4 key characteristics:
+* id: the identifier for the system
+* systemType: What type of system are you interfacing with? LINUX, IRODS, or GLOBUS
+* host: What is the hostname of the system you are trying to connect to? This can be anything that supports Tapis systems, whether it be a url or IP address. SOmething like stampede2.tacc.utexas.edu
+* defaultAuthnMethod: What authentication method will you use on this system?
+
+##### S3 Bucket Systems
+Tapis also supports interfacing with AWS S3 Bucket systems
 
-this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
-### Known Issues
-Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
-The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
```

### Comparing `TapisCL-ICICLE-0.2.2/pyproject.toml` & `TapisCL-ICICLE-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.2.2"
+version = "1.0.0"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
 pyperclip = "*"
 py2neo = "*"
 psycopg2-binary = "*"
 blessed = "*"
 prompt_toolkit = "*"
 TapisFederatedAuthClientAPI = "*"
 requests = "*"
-pyreadline3 = "*"
+questionary = "1.10.0"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
 Homepage = "https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE"
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,30 +83,31 @@
     def configure_parser(self, arguments):
         parser = argparse.ArgumentParser(description="Command Line Argument Parser", exit_on_error=False, usage=argparse.SUPPRESS, add_help=False, conflict_handler='resolve')
         parser.add_argument('command_selection')
         parser.add_argument('positionals', nargs='*')
         parser.error = self.parser_error
         
         for arg_name, arg in arguments.items():
-            if arg['action'] == 'store_true':
+            if (arg['action'] == 'store_true' and arg['arg_type'] == 'standard') or (arg['arg_type'] == 'form' and arg['flattening_type'] == 'FLATTEN'):
                 default = False
-            elif arg['action'] == 'store_false':
+            elif (arg['action'] == 'store_false' and arg['arg_type'] == 'standard') or (arg['arg_type'] != 'standard' and arg['required']):
                 default = True
             else:
                 default = None
             parser.add_argument(f"-{arg['truncated_arg']}", arg['full_arg'],
                                 action=arg['action'], default=default)
         return parser
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
-            os.system(rf"pythonw {server_path}")
+            os.system(rf"pythonw {server_path} 1>stdout.txt 2>stderr.txt")
+            #os.system(rf"python {server_path}")
         else: # unix based
             subprocess.Popen(['nohup', 'python3', server_path, '&'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     #@decorators.AnimatedLoading
     def connection_initialization(self):
         """
         start the local server through the client
@@ -185,15 +186,20 @@
             kwargs = vars(kwargs)
             self.interface(kwargs)
             kwargs = vars(self.parser.parse_args(['exit']))
             response_message = schemas.CommandData(request_content=kwargs)
             self.connection.send(response_message)
             self.connection.close()
         except Exception as e:
+            error_str = traceback.format_exc()
+            #if self.debug:
+            print(error_str)
             print(e)
+            error_message = schemas.ResponseData(error=str(e))
+            self.connection.send(error_message)
         finally:
             sys.exit(0)
 
     def cli_window(self):
         title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
         print(title)
         print(r"""Enter 'exit' to exit the client
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from getpass import getpass
 import os
 import json
 import pprint
 import time
-import pyreadline3
 
 from prompt_toolkit.validation import Validator, ValidationError
 from prompt_toolkit.completion import word_completer, WordCompleter
+from prompt_toolkit.shortcuts import checkboxlist_dialog
 from prompt_toolkit import prompt
+
 from blessed import Terminal
 
 
 if __name__ != "__main__":
     from ..socketopts import schemas
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
 saved_command = os.path.join(__location__, r'entered_command.json')
 
 
-LINE_READER = base_read_line = pyreadline3.BaseReadline()
-
-
 class Formatters:
     """
     Format received dictionaries in the client code
     """
     def print_response(self, input_data, depth: int=0):
         if isinstance(input_data, (list, set, tuple)):
             for data in input_data:
@@ -43,43 +41,43 @@
         elif isinstance(input_data, (int, str)):
             print(f"{depth * '  '}{input_data}")
         if depth == 0:
             print("\n")
 
 
 class ParserTypeLenEnforcer:
-        def __init__(self, name: str=str(), size: tuple=(0, 0), data_type: str='string', choices: list=list()):
-            self.arg_name = name
-            self.data_type = data_type
-            self.lower_size_limit, self.upper_size_limit = size
-            self.choices = choices
-
-        def update_constraints(self, name=None, data_type=None, choices=None, size_limit=None, **kwargs):
-            self.arg_name = name
-            self.data_type = data_type
-            self.choices = choices
-            self.lower_size_limit, self.upper_size_limit = size_limit
-
-        def __call__(self, data):
-            if self.data_type:
-                try:
-                    if self.data_type == 'string':
-                        str(data)
-                    elif self.data_type == 'int':
-                        int(data)
-                except Exception as e:
-                    raise ValidationError(message=str(e) + self.data_type, cursor_position=0)
-            if self.data_type == int:
-                if not data >= self.lower_size_limit or not data < self.upper_size_limit:
-                    raise ValidationError(message=f"The input for the argument {self.arg_name} must be in the range ({self.lower_size_limit}, {self.upper_size_limit}). Got value {data}", cursor_position=0)
-            elif self.data_type == str:
-                if not len(data) >= self.lower_size_limit or not len(data) < self.upper_size_limit:
-                    raise ValidationError(message=f"The input length for the argument {self.arg_name} must be in the range ({self.lower_size_limit}, {self.upper_size_limit}). Got length {len(data)}", cursor_position=0)
-            if self.choices and data not in self.choices:
-                raise ValidationError(message=f"The input for the argument {self.arg_name} must be one of the following: {self.choices}", cursor_position=0)
+    def __init__(self, name: str=str(), size: tuple=(0, 0), data_type: str='string', choices: list=list()):
+        self.arg_name = name
+        self.data_type = data_type
+        self.lower_size_limit, self.upper_size_limit = size
+        self.choices = choices
+
+    def update_constraints(self, name=None, data_type=None, choices=None, size_limit=None, **kwargs):
+        self.arg_name = name
+        self.data_type = data_type
+        self.choices = choices
+        self.lower_size_limit, self.upper_size_limit = size_limit
+
+    def __call__(self, data):
+        if self.data_type:
+            try:
+                if self.data_type == 'string':
+                    data = str(data)
+                elif self.data_type == 'int':
+                    data = int(data)
+            except Exception as e:
+                raise ValidationError(message=str(e) + self.data_type, cursor_position=0)
+        if self.data_type == int:
+            if not data >= self.lower_size_limit or not data < self.upper_size_limit:
+                raise ValidationError(message=f"The input for the argument {self.arg_name} must be in the range ({self.lower_size_limit}, {self.upper_size_limit}). Got value {data}", cursor_position=0)
+        elif self.data_type == str:
+            if not len(data) >= self.lower_size_limit or not len(data) < self.upper_size_limit:
+                raise ValidationError(message=f"The input length for the argument {self.arg_name} must be in the range ({self.lower_size_limit}, {self.upper_size_limit}). Got length {len(data)}", cursor_position=0)
+        if self.choices and data not in self.choices:
+            raise ValidationError(message=f"The input for the argument {self.arg_name} must be one of the following: {self.choices}", cursor_position=0)
 
 
 class ResponseValidator(Validator):
     def __init__(self):
         super().__init__()
         self.enforcer = ParserTypeLenEnforcer()
 
@@ -88,43 +86,74 @@
         self.enforcer(text)
 
         
 class Handlers(Formatters):
     def __init__(self):
         self.validator = ResponseValidator()
 
+    def __labelled_form(self, form_options, form_filled):
+        labelled_dict = dict()
+        for field_name, field_metadata in form_options.items():
+            if field_metadata['required']:
+                requirement_str = 'R'
+            else:
+                requirement_str = 'O'
+            labelled_dict[f"({requirement_str}) {field_name}"] = form_filled[field_name]
+        return json.dumps(labelled_dict, indent=3)
+
+
     def __expression_input(self) -> str: 
         """
         Input an expression as requested by the server for something like cypher queries
         """
         print("Enter 'exit' to submit") 
         expression = ''
         line = ''
         while line != 'exit': 
             line = str(input("> "))
             if line != 'exit':
                 expression += line
         return expression
     
-    def confirmation_handler(self, argument):
+    def confirm_form_exit(self, message: str=None):
+        print(message)
+        while True:
+            decision = str(input("(y/n)"))
+            if decision == 'y':
+                return True
+            elif decision == 'n':
+                return False
+            else:
+                print("Enter valid response")
+        
+    def confirmation_handler(self, argument: dict=None):
+        print(argument['name'])
         if 'description' in argument and argument['description']:
             print(argument['description'])
-        print(argument['name'])
         while True:
             decision = str(input("(y/n)"))
             if decision == 'y':
-                decision = True
-                break
+                return True
             elif decision == 'n':
-                decision = False
-                break
+                if not argument['required']:
+                    return False
+                raise KeyboardInterrupt('User negative reply on confirmation, cancelling')
             else:
                 print("Enter valid response")
-        return decision
     
+    def selection_list_handler(self, term: Terminal, attrs: dict):
+        with term.fullscreen():
+            results_array = checkboxlist_dialog(
+                title="CheckboxList dialog",
+                text="What would you like in your breakfast ?",
+                values=[(True, field) for field in attrs['option_list']]
+            ).run()
+            results = dict(zip(attrs['option_list'], results_array))
+            return results
+        
     def input_dict_handler(self, term: Terminal, attrs: dict, default=None):
         mode = 'create'
         if not default:
             default = dict()
         answer = default
         default_name = attrs['data_type']['name']
         with term.fullscreen():
@@ -139,20 +168,20 @@
                     continue
                 if name.lower() == 'exit':
                     return answer
                 if mode == 'create':
                     mode = 'create'
                     attrs['data_type']['name'] = name
                     if name in answer:
-                        default_value = answer#[name]
+                        default_value = answer
                     else:
                         default_value = None
-                    pprint.pprint({name:attrs['data_type']})
                     sub_answer = self.advanced_input_handler({name:attrs['data_type']}, term, default=default_value)
-                    answer.update(**sub_answer)
+                    if sub_answer[name]:
+                        answer.update(**sub_answer)
                 elif mode == 'delete':
                     mode = 'delete'
                     try:
                         answer.pop(name)
                     except KeyError:
                         pass
 
@@ -185,66 +214,81 @@
                     try:
                         answer.pop(int(decision)-1)
                     except IndexError:
                         continue
                     continue
                 elif decision.isdigit() and mode == 'modify':
                     try:
-                        print({f"{attrs['name']}_{str(decision)}":answer[int(decision)-1]})
-                        time.sleep(5)
                         sub_answer = self.advanced_input_handler({f"{attrs['name']}_{str(decision)}":attrs['data_type']}, term, default={f"{attrs['name']}_{str(decision)}":answer[int(decision)-1]})
-                        answer[int(decision)-1] = sub_answer[f"{attrs['name']}_{str(decision)}"]
+                        if sub_answer:
+                            answer[int(decision)-1] = sub_answer[f"{attrs['name']}_{str(decision)}"]
                     except IndexError:
                         continue
                     continue
                 else:
                     continue
                 sub_answer = self.advanced_input_handler({f"{attrs['name']}_{str(len(answer)+1)}":attrs['data_type']}, term)
                 index, value = list(sub_answer.items())[0]
-                answer.append(value)
+                if value:
+                    answer.append(value)
 
     def form_handler(self, term: Terminal, attrs: dict, form_name, default=None):
         form_options = attrs['arguments_list']
         completer = WordCompleter(list(form_options.keys()))
         if not default:
             form_input = dict()
             for name, command_metadata in form_options.items():
                 if command_metadata['default_value']:
                     form_input[name] = command_metadata['default_value']
                     continue
                 form_input[name] = ''
         else:
             form_input = {arg_name:arg_default_value for arg_name, arg_default_value in default.items() if arg_name in form_options}
-        while True:
-            print(f"{term.clear}now editing the form: {form_name}")
-            print(json.dumps(form_input, indent=3))
-            field = prompt('Enter the field you want to modify. Enter exit to complete: ', completer=completer)
-            if field.lower() == 'exit':
-                return form_input
-            elif field not in form_options:
-                continue
-            result = self.advanced_input_handler({field:form_options[field]}, term, default=form_input)
-            form_input[field] = result[field]
+        with term.fullscreen():
+            while True:
+                print(f"{term.clear}now editing the form: {form_name}")
+                print(self.__labelled_form(form_options, form_input))
+                field = prompt('Enter the field you want to modify. Enter exit to complete: ', completer=completer)
+                if field.lower() == 'exit':
+                    unfulfilled_requirements = []
+                    for field_name, field_metadata in form_options.items():
+                        if field_metadata['required'] and not form_input[field_name] and form_input[field_name] != False:
+                            unfulfilled_requirements.append(field_name)
+                    if unfulfilled_requirements:
+                        decision = self.confirm_form_exit(f'The fields {unfulfilled_requirements} are required but did not receive any input. If you exit this form will not be submitted.\nSubmit form?')
+                        if decision:
+                            return None
+                        else:
+                            continue
+                    return form_input
+                elif field not in form_options:
+                    continue
+                result = self.advanced_input_handler({field:form_options[field]}, term, default=form_input)
+                form_input[field] = result[field]
             
     def str_input(self, attrs):
         completer = None
         if 'choices' in attrs and attrs['choices']:
             completer = WordCompleter(attrs['choices'])
         answer = prompt(f"{attrs['name']}: ", validator=self.validator, wrap_lines=True, completer=completer)
+        if attrs['data_type'] == 'str':
+            answer = str(answer)
+        elif attrs['data_type'] == 'int':
+            answer = int(answer)
+        elif attrs['data_type'] == 'bool':
+            answer = bool(answer)
         return answer
     
     def advanced_input_handler(self, form_request: dict, term: Terminal, default=None):
         response = dict()
         for field, attrs in form_request.items():
             arg_type = attrs['arg_type']
             self.validator.enforcer.update_constraints(**attrs)
             if 'description' in attrs and attrs['description']:
                 print(attrs['description'])
-            # pprint.pprint(form_request)
-            # print(field)
             if default:
                 default_selection = default[field]
             else:
                 default_selection = None
             try:
                 match arg_type:
                     case 'secure':
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/appCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appCommands.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 import json
+import pprint
 
 
 if __name__ != "__main__":
-    from . import baseCommand, decorators
-    from .arguments import argument
+    from .. import baseCommand, decorators
+    from ..arguments import argument
+    from . import appForms
     Argument = argument.Argument
 
 
 def get_latest_version(t, kwargs):
-    if 'appVersion' not in kwargs:
+    if 'appVersion' not in kwargs or not kwargs['appVersion']:
         version = t.apps.getAppLatestVersion(**kwargs).version
         kwargs['appVersion'] = version
     return kwargs
 
 
 class create_app(baseCommand.BaseCommand):
     """
     @help: create an app. You must have a properly configured app config file. 
     See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/app-config.json
     """
     supports_config_file=True
     required_arguments = [
         Argument('id', positional=True, description='This can be the same as another app as long as the version number is different'),
         Argument('version', positional=True),
-        Argument('containerImage')
+        Argument('containerImage'),
+        Argument('execSystemId', size_limit=(1, 80), description='what system id will this be run on?')
     ]
     optional_arguments = [
         Argument('description', arg_type='str_input'),
         Argument('owner', default_value=r"${apiUserId}"),
         Argument('enabled', action='store_true'),
-        Argument('runtime', choices=['SINGULARITY', 'DOCKER']),
-        Argument('runtimeVersion'),
-        Argument('runtimeOptions', choices=['NONE', 'SINGULARITY_START', 'SINGULARITY_RUN']),
-        Argument('jobType', choices=['BATCH', 'FORK']),
-        Argument('maxJobs', data_type='int'),
-        Argument('maxJobsPerUser', data_type='int'),
-        Argument("strictFileInputs", action='store_true'),
+        appForms.CONFIGURE_RUNTIME,
+        appForms.JOB_CONSTRAINTS,
+        Argument("strictFileInputs", action='store_true', description='indicates if you want your jobs to be able to accept unnamed file inputs'),
         Argument('tags', arg_type='input_list', data_type=Argument('tag', size_limit=(1, 128))),
     ]
     async def run(self, *args, **kwargs) -> str: # create a tapis app taking a json descriptor file path
         url = self.t.apps.createAppVersion(**kwargs)
         return f"App created successfully\nID: {kwargs['id']}\nVersion: {kwargs['version']}\nURL: {url}\n"
     
 
@@ -56,25 +55,20 @@
     """
     updateable_form_retriever = AppUpdatingRetriever()
     supports_config_file = True
     required_arguments = [
         Argument('appId', size_limit=(1, 80), positional=True),
     ]
     optional_arguments = [
+        Argument('execSystemId', size_limit=(1, 80), description='what system id will this be run on?'),
         Argument('appVersion', size_limit=(1, 64)),
         Argument('description', arg_type='str_input'),
-        Argument('owner', default_value=r"${apiUserId}"),
-        Argument('enabled', action='store_true'),
-        Argument('runtime', choices=['SINGULARITY', 'DOCKER']),
-        Argument('runtimeVersion'),
-        Argument('runtimeOptions', choices=['NONE', 'SINGULARITY_START', 'SINGULARITY_RUN']),
-        Argument('jobType', choices=['BATCH', 'FORK']),
-        Argument('maxJobs', data_type='int'),
-        Argument('maxJobsPerUser', data_type='int'),
-        Argument("strictFileInputs", action='store_true'),
+        appForms.CONFIGURE_RUNTIME,
+        appForms.JOB_CONSTRAINTS,
+        Argument("strictFileInputs", action='store_true', description='indicates if you want your jobs to be able to accept unnamed file inputs'),
         Argument('tags', arg_type='input_list', data_type=Argument('tag', size_limit=(1, 128))),
     ]
     async def run(self, *args, **kwargs):
         kwargs = get_latest_version(self.t, kwargs)
         self.t.apps.patchApp(**kwargs)
         return f'updated app {kwargs["appId"]} successfully'
     
@@ -92,99 +86,70 @@
     """
     updateable_form_retriever = JobUpdatingRetriever()
     supports_config_file=True
     required_arguments = [
         Argument('appId', size_limit=(1, 80), positional=True)
     ]
     optional_arguments = [
+        Argument('execSystemId', size_limit=(1, 80), description='what system id will this be run on?'),
+        appForms.SYSTEM_CONFIG,
+        appForms.ARCHIVE_ON_APP_ERROR,
+        appForms.APP_ARGUMENTS,
+        appForms.CONTAINER_ARGUMENTS,
+        appForms.SCHEDULER_OPTIONS,
+        appForms.JOB_ENVIRONMENT_VARIABLES,
+        appForms.JOB_ALLOCATION_CONFIGURATION,
         Argument('appVersion', size_limit=(1, 64)),
         Argument('description', arg_type='str_input'),
-        Argument('dynamicExecSystem', arg_type='confirmation', description="System is dynamic?"),
-        Argument('execSystemConstraints', arg_type='input_list', data_type=Argument('constraint', size_limit=(3, 4096))),
-        Argument('execSystemId', size_limit=(1, 80), description='what system id will this be run on?'),
-        Argument('execSystemExecDir', size_limit=(1, 4096), description='based on the system job working dir? automatically generated if not specified'),
-        Argument('execSystemInputDir', size_limit=(1, 4096), description='what system path will be used to stage input files? automatically generated if not specified'),
-        Argument('execSystemOutputDir', size_limit=(1, 4096), description='Where will tapis put job output files? automatically generated if not specified'),
-        Argument('execSystemLogicalQueue', size_limit=(1, 128), description='What batch logical queue on the system will be used for execution?'),
-        Argument('archiveSystemId', size_limit=(1, 80), description='What system will be used when archiving outputs?'),
-        Argument('archivesystemDir', size_limit=(1, 4096), description='What system directory will be used for archiving?'),
-        Argument('archiveOnAppError', arg_type='confirmation', description='archive on error?'),
         Argument("isMpi", arg_type='confirmation', description="is mpi?"),
-        Argument('mpiCmd', size_limit=(1, 126), arg_type='str_input', description='command to launch MPI jobs. Conflicts with cmdPrefix if isMpi is set'),
+        Argument('mpiCmd', size_limit=(1, 126), arg_type='str_input', description='command to launch MPI jobs. Conflicts with cmdPrefix if isMpi is set', mutually_exclusive_with=['cmdPrefix']),
         Argument('cmdPrefix', size_limit=(1, 126), description='string put in front of app run command to run with mpi command'),
-        argument.Form('parameterSet', arguments_list=[
-            Argument('appArgs', arg_type='input_list', data_type=argument.Form('appArg', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"]),
-                Argument('arg')]
-            ), description='command line arguments to be passed to the application'),
-            Argument('containerArgs', arg_type='input_list', data_type=argument.Form('containerArg', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"], description='How will this argument be treated when processing jobs? EG should the job require it?'),
-                Argument('arg', description='value for the argument')
-            ]), description='command line arguments to be passed to the container at runtime, whether singularity or container'),
-            Argument('schedulerOptions', arg_type='input_list', data_type=argument.Form('schedulerOption', arguments_list=[
-                Argument('name', size_limit=(1, 80)),
-                Argument('description', size_limit=(1, 8096)),
-                Argument('inputMode', choices=['REQUIRED', "FIXED", "INCLUDE_ON_DEMAND", "INCLUDE_BY_DEFAULT"]),
-                Argument('arg')
-            ]), description='options to pass to hpc batch scheduler'),
-            Argument('envVariables', arg_type='input_list', data_type=argument.Form('environment_variable', arguments_list=[
-                Argument('key'),
-                Argument('value'),
-                Argument('description', size_limit=(1, 2048))
-            ]), description='environment variables placed into the runtime environment')
-        ], description='collections used during job execution. Specify app args, container args, scheduler options, evnironment variables, and archive filter for job execution'),
-        Argument('fileInputs', arg_type='input_list', data_type=argument.Form('fileInput', arguments_list=[
+        Argument('fileInputs', arg_type='input_list', data_type=argument.Form('fileInput', optional_arguments=[
             Argument('name', size_limit=(1, 80)),
             Argument('description', size_limit=(1, 8096)),
             Argument('inputMode', choices=['REQUIRED', 'OPTIONAL', 'FIXED'], description='indicates how input should be treeated when processing job request'),
             Argument('autoMountLocal', arg_type='confirmation', description='should the service automatically mount file paths to the containers?'),
             Argument('sourceUrl', description='source used by jobs service when staging file inputs'),
             Argument('targetPath', description='where in the container will the files go when staging the inputs')
         ]), description='selection of file inputs that must be staged to run application'),
-        Argument('fileInputArrays', arg_type='input_list', data_type=argument.Form('fileInput', arguments_list=[
+        Argument('fileInputArrays', arg_type='input_list', data_type=argument.Form('fileInput', optional_arguments=[
             Argument('name', size_limit=(1, 80)),
             Argument('description', size_limit=(1, 8096)),
             Argument('inputMode', choices=['REQUIRED', 'OPTIONAL', 'FIXED']),
             Argument('sourceUrls', arg_type='input_list', data_type=Argument('sourceUrl')),
             Argument('targetPath')
         ]), description='collection of arrays of inputs to be staged to the application'),
-        Argument('nodeCount', data_type='int', description='how many nodes do you want to request in your job?'),
-        Argument('coresPerNode', data_type='int', description='how many cores per node?'),
-        Argument('memoryMB', data_type='int'),
-        Argument('maxMinutes', data_type='int', description='max job runtime'),
-        Argument('subscriptions', arg_type='input_list', data_type=argument.Form('subscription', arguments_list=[
+        Argument('subscriptions', arg_type='input_list', data_type=argument.Form('subscription', optional_arguments=[
             Argument('description'),
             Argument('enabled', arg_type='confirmation', description='enable subscription?'),
             Argument('jobEventCategoryFilter', choices=['ALL', 'JOB_NEW_STATUS', 'JOB_INPUT_TRANSACTION_ID', 'JOB_ARCHIVE_TRANSACTION_ID', 'JOB_ERROR_MESSAGE', 'JOB_SUBSCRIPTION']),
             Argument('ttlMinutes', data_type='int'),
-            Argument('deliveryTargets', arg_type='input_list', data_type=argument.Form('deliveryTarget', arguments_list=[
+            Argument('deliveryTargets', arg_type='input_list', data_type=argument.Form('deliveryTarget', required_arguments=[
                 Argument('deliveryMethod', choices=['WEBHOOK', 'EMAIL']),
                 Argument('deliveryAddress')
             ]))
         ]))
     ]
     async def run(self, *args, **kwargs):
+        for default_arg in self.default_arguments:
+            if default_arg.argument in kwargs:
+                kwargs.pop(default_arg.argument)
         kwargs = get_latest_version(self.t, kwargs)
         appId = kwargs.pop('appId')
         appVersion = kwargs.pop('appVersion')
-        kwargs.pop('connection')
         jobAttributes = {'jobAttributes':kwargs}
         self.t.apps.patchApp(appId=appId, appVersion=appVersion, **jobAttributes)
         return 'updated job attributes successfully'
     
 
 class get_apps(baseCommand.BaseCommand):
     """
     @help: get a list of all available apps
     """
-    return_fields = ['id', 'version']
+    return_fields = ['id', 'version', 'status']
     optional_arguments = [
         Argument('listType', choices=[
             'OWNED',
             'SHARED_PUBLIC',
             'SHARED_DIRECT',
             'READ_PERM', 
             'MINE',
@@ -234,19 +199,22 @@
     """
     @help: disable the app
     """
     async def run(self, *args, **kwargs):
         return self.t.apps.disableApp(**kwargs)
     
 
-class delete_app(is_app_enabled):
+class delete_app(baseCommand.BaseCommand):
     """
     @help: delete the app
     """
-    decorator=decorators.NeedsConfirmation()
+    required_arguments = [
+        Argument('appId', size_limit=(1, 80), positional=True),
+        Argument('confirm', arg_type='confirmation')
+    ]
     async def run(self, *args, **kwargs):
         return self.t.apps.disableApp(**kwargs)
     
 
 class undelete_app(is_app_enabled):
     """
     @help: undo a deletion of an app
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,110 @@
 import typing
 import abc
+import pprint
 
+from . import argumentValidators
 
-ALLOWED_ARG_TYPES = typing.Literal['silent', 'secure', 'expression', 'input_list', 'input_dict', 'form', 'str_input', 'confirmation']
+
+ALLOWED_ARG_TYPES = typing.Literal['silent', 'secure', 'expression', 'input_list', 'input_dict', 'form', 'str_input', 'confirmation', 'selection_list']
 ALLOWED_DATA_TYPES = typing.Literal['string', 'int', 'bool']
 ALLOWED_ACTIONS = typing.Literal['store', 'store_true', 'store_false']
 
 
-class DynamicChoiceList(abc.ABC):
-    @abc.abstractmethod
-    def __call__(self, tapis_instance):
-        pass
-
-
 class AbstractArgument(abc.ABC):
     @abc.abstractmethod
     def json(self):
         pass
+    
 
-
-def cast_int(data):
-    return int(data)
-
-def cast_string(data):
-    return str(data)
-
-def cast_bool(data):
-    return bool(data)
-
-
-class Argument(AbstractArgument):
-    type_map = {
-        'int':cast_int,
-        'string':cast_string,
-        'bool':cast_bool
-    }
+class Argument(argumentValidators.Validators, AbstractArgument):
     def __init__(self, argument: str,
                  data_type: ALLOWED_DATA_TYPES | typing.Type[AbstractArgument] = 'string',
                  arg_type: ALLOWED_ARG_TYPES | typing.Literal['standard']='standard',
-                 choices: list | typing.Type[DynamicChoiceList] | None=None, 
+                 choices: list | None=None, 
                  action: typing.Literal['store', 'store_true', 'store_false']="store", 
                  description: str="",
                  positional: bool=False,
                  default_value=None,
                  depends_on: list = [],
-                 size_limit: tuple=(0,4096)):
+                 mutually_exclusive_with: list = [],
+                 part_of: str = "",
+                 size_limit: tuple=(-1,-1)):
         if arg_type not in typing.get_args(ALLOWED_ARG_TYPES) and arg_type != 'standard':
             raise ValueError(f"The arg type parameter in the argument {self.__class__.__name__} must be in the list {ALLOWED_ARG_TYPES}. Got arg type {arg_type}")
         if data_type not in typing.get_args(ALLOWED_DATA_TYPES) and not issubclass(data_type.__class__, AbstractArgument):
             raise ValueError(f"The data type argument provided to the argument {self.__class__.__name__} must be in the list {ALLOWED_DATA_TYPES}, or must be a subclass of AbstractArgument")
         if action not in typing.get_args(ALLOWED_ACTIONS):
             raise ValueError(f"Action {action} not in the list {ALLOWED_ACTIONS}, in argument {self.__class__.__name__}")
         if arg_type in ('input_list', 'input_dict') and isinstance(data_type, Argument) and data_type.arg_type == 'standard':
             data_type.arg_type = 'str_input'
         if action != 'store':
             data_type = 'bool'
+        super().__init__(arg_type)
+        if action in ('store_true', 'store_false'):
+            data_type = 'bool'
+        if arg_type != 'standard':
+            action = 'store_true'
         self.argument = argument
         self.arg_type = arg_type
         self.data_type = data_type
         self.choices = choices
-        if self.arg_type != 'standard':
-            action = 'store_true'
         self.action = action
         self.description = description
         self.positional = positional
         self.default_value = default_value
         self.size_limit=size_limit
         self.depends_on = depends_on
+        self.mutually_exclusive_with = mutually_exclusive_with
+        self.required = None
+        self.part_of = part_of
 
         self.truncated_arg = None
         self.full_arg = f"--{self.argument}"
 
-    def verify_standard_value(self, value):
-        if self.arg_type == "standard":
-            #print(f"ARGUMENT NAME: {self.argument}\nARGUMENT VALUE: {value}\n")
-            if value == None and self.default_value:
-                value = self.default_value
-                return value
-            elif not value:
-                return value
-            min_, max_ = self.size_limit
-            try:
-                value = self.type_map[self.data_type](value)
-            except:
-                raise ValueError(f"The argument {self.argument} requires a datatype {self.data_type}")
-            if type(value) == int:
-                if value >= max_ or value < min_:
-                    raise ValueError(f"The argument {self.argument} must be a value in the range {self.size_limit}")
-            elif type(value) == str and (len(value) >= max_ or len(value) < min_):
-                raise ValueError(f"The argument {self.argument} must be between the sizes {self.size_limit}")
-            elif self.choices and value not in self.choices:
-                raise ValueError(f"The value for argument {self.argument} must be in the list {self.choices}")
-            elif value == None and self.default_value:
-                value = self.default_value
-        return value
+    def is_required(self, is_required: bool):
+        """
+        setter for the required attribute
+        """
+        self.required = is_required
+
+    def verify_rules_followed(self, value):
+        """
+        check to make sure the value assigned to the argument follows all existing rules
+        """
+        if self.required and not value and value != False and self.arg_type != 'silent':
+            raise ValueError(f'The argument {self.argument} is required')
+        return_value = self.validator_map[self.arg_type](value)
+        if isinstance(return_value, bool) and self.data_type != 'bool' and self.action != 'store_true' and not return_value:
+            print(f"{self.argument} RETURNING NONE")
+            return None
+        return return_value
 
     def json(self):
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
             'data_type':self.data_type,
             'choices':self.choices,
             'action':self.action,
             'description':self.description,
             'positional':self.positional,
             'default_value':self.default_value,
             'size_limit':self.size_limit,
             'truncated_arg':self.truncated_arg,
             'full_arg':self.full_arg,
-            'depends_on':self.depends_on
+            'depends_on':self.depends_on,
+            'mutually_exclusive_with':self.mutually_exclusive_with,
+            'part_of':self.part_of,
+            'required':self.required
         }
         if self.data_type in ('string', 'int', 'bool'):
             json['data_type'] = self.data_type
         else:
-            json['data_type'] = self.data_type.json()
+            json['data_type'] = self.data_type.json() 
         return json
     
     def help_message(self):
         help = {"name":self.argument,
                 "description":f"{self.description}"}
         if self.choices and isinstance(self.choices, list):
             help['choices'] = self.choices
@@ -140,25 +127,49 @@
     def str(self):
         help_str = f"{self.truncated_arg}/{self.full_arg} "
         if self.positional:
             help_str = f"<{self.argument}> "
         elif self.action == 'store':
             help_str += f"<{self.argument}> "
         if self.arg_type != 'standard':
-            help_str += ' (f)\t'
+            help_str += ' (f) '
         return help_str
 
 
 class Form(Argument):
-    def __init__(self, form_name, arguments_list, description=None):
-        super().__init__(form_name, arg_type='form', description=description)
+    def __init__(self, form_name, required_arguments=None, optional_arguments=None, description=None, depends_on=None, flattening_type: typing.Literal['NONE', 'FLATTEN', 'RETRIEVE']='NONE'):
+        super().__init__(form_name, arg_type='form', description=description, depends_on=depends_on)
+        arguments_list = list()
+        if required_arguments:
+            for argument in required_arguments:
+                argument.is_required(True)
+            arguments_list += required_arguments
+        if optional_arguments:
+            for argument in optional_arguments:
+                argument.is_required(False)
+            arguments_list += optional_arguments
         for argument in arguments_list:
+            if not issubclass(argument.__class__, Argument):
+                raise TypeError(f'The argument {argument.argument} must be an Argument type')
             if argument.arg_type == 'standard':
                 argument.arg_type = 'str_input'
         self.arguments_list = {argument.argument:argument for argument in arguments_list}
+        self.flattening_type = flattening_type
+    
+    def flatten_form_data(self, value): 
+        if value and not isinstance(value, bool):
+            if self.flattening_type == 'FLATTEN':
+                flattened_form_info = {self.argument:True}
+                flattened_form_info.update(**{arg_name:arg_value for arg_name, arg_value in value[self.argument].items()})
+                return flattened_form_info
+            if self.flattening_type == 'RETRIEVE':
+                exctracted_form_data = {arg_name:arg for arg_name, arg in value[self.argument].items()}
+                return exctracted_form_data
+            else:
+                return value
 
     def json(self):
         fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
             'data_type':self.data_type,
@@ -166,15 +177,42 @@
             'action':self.action,
             'description':self.description,
             'positional':self.positional,
             'default_value':self.default_value,
             'size_limit':self.size_limit,
             'truncated_arg':self.truncated_arg,
             'full_arg':self.full_arg,
-            'arguments_list':fields
+            'arguments_list':fields,
+            'required':self.required,
+            'flattening_type':self.flattening_type
+        }
+        return json
+    
+
+class SelectionList(Argument):
+    def __init__(self, argument, option_dict):
+        super().__init__(argument, data_type='selection_list')
+        self.option_dict = option_dict
+        self.option_list = list(option_dict.keys())
+
+    def json(self):
+        json = {
+            'name':self.argument,
+            'arg_type':self.arg_type,
+            'data_type':self.data_type,
+            'choices':self.choices,
+            'action':self.action,
+            'description':self.description,
+            'positional':self.positional,
+            'default_value':self.default_value,
+            'size_limit':self.size_limit,
+            'truncated_arg':self.truncated_arg,
+            'full_arg':self.full_arg,
+            'option_list':self.option_list,
+            'required':self.required
         }
         return json
     
 
 class RequestHandler:
     def handle_requests(self, request):
         pass
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import abc
 import ast
 import json
 from typing import Type
 import typing
 from abc import abstractmethod, ABC
 import os
-from pprint import pprint
+from pprint import pprint, pformat
 from datetime import datetime
 
-from commands import decorators # I finally understand. Imported at the top level by serverRun, so it can only see packages from that vantage point
+# I finally understand. Imported at the top level by serverRun, so it can only see packages from that vantage point
 from utilities import exceptions
-from commands.arguments.argument import Argument, DynamicChoiceList, ALLOWED_ARG_TYPES
+from commands.arguments.argument import Argument, ALLOWED_ARG_TYPES
 from socketopts import schemas
 from commands import dataFormatters
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(f"{__file__}")))
 saved_command_root_dir = os.path.join(__location__, r'..\user_files')
@@ -48,15 +48,14 @@
 
 class CommandMetaClass(abc.ABCMeta):
     def __new__(cls, name, bases, attrs):
         instance = super().__new__(cls, name, bases, attrs)
         if name not in ('BaseQuery', 'BaseCommand'):
             instance.__check_run(name, attrs)
             instance.__check_command_args(name, attrs)
-            instance.__check_decorator(name, attrs)
             instance.__check_command_opt(name, attrs)
         return instance
     
     def __check_run(self, name, attrs):
         if 'run' not in list(attrs.keys()):
             raise AttributeError(f"The command {name} requires a 'run()' method")
         elif not inspect.iscoroutinefunction(attrs['run']):
@@ -68,156 +67,157 @@
         if 'required_arguments' in list(attrs.keys()): 
             args += attrs['required_arguments']
         if 'optional_arguments' in list(attrs.keys()): 
             args += attrs['optional_arguments']
         if args:
             for argument in args:
                 if not issubclass(argument.__class__, Argument) and not isinstance(argument, Argument):
-                    raise AttributeError(f"The argument {argument.argument} of the command '{name}' must be of type 'Argument'")
+                    raise AttributeError(f"The argument {argument} of the command '{name}' must be of type 'Argument'. Currently {type(argument)}")
                 if 'optional_arguments' in list(attrs.keys()) and argument in attrs['optional_arguments'] and argument.positional:
                     raise AttributeError(f"The optional argument {argument.argument} of the command {name} cannot be positional. All positional arguments must be required")
         if 'kwargs' not in run_params or 'args' not in run_params:
             raise AttributeError(f"The run() method of the {name} class must have a **kwargs and *args as parameters")
         
-    def __check_decorator(self, name, attrs):
-        if 'decorator' in list(attrs.keys()) and type(attrs['decorator']) not in decorators.DECORATOR_LIST:
-            raise TypeError(f"The decorator parameter of the command {name} is invalid. Must be set to None or to a decorator type. Currently is {type(attrs['decorator'])}")
-        
     def __check_command_opt(self, name, attrs):
         if 'command_opt' in list(attrs.keys()) and type((attrs['command_opt'])) != list:
             raise TypeError(f"The command opt attribute of the command {name} must be a list!")
         
 
 class UpdatableFormRetriever(abc.ABC):
     @abc.abstractmethod
     def __call__(self, tapis_instance, **kwargs):
         pass
 
 
-class HelpMenu:
-    def __init__(self, required_arguments: dict[str, Argument], optional_arguments: dict[str, Argument]):
-        self.required_arguments = required_arguments
-        self.optional_arguments = optional_arguments
-        self.arguments = {**required_arguments, **optional_arguments}
-        self.help = self.create_help_menu()
-
-    def create_help_menu(self):
-        help_dict = {'required':dict(), 'optional':dict()}
-        for arg_name, argument in self.required_arguments.items():
-            help_dict['required'][arg_name] = argument.help_message()
-        for arg_name, argument in self.optional_arguments.items():
-            help_dict['optional'][arg_name] = argument.help_message()
-        return help_dict
-    
-    def dict(self):
-        return self.arguments
-
-
 class BaseCommand(ABC, HelpStringRetriever, metaclass=CommandMetaClass):
-    decorator = None
     return_fields: list = []
     command_opt: list = None
     supports_config_file: bool = False
     required_arguments: list[Argument] | dict = list()
     optional_arguments: list[Argument] | dict = list()
+    default_arguments = [Argument('connection', arg_type='silent'),
+                            Argument('verbose', action='store_true', arg_type='silent'),
+                            Argument('help', action='store_true', arg_type='silent'),
+                            Argument('positionals', arg_type='silent')]
     updateable_form_retriever: UpdatableFormRetriever = None
     def __init__(self):
         self.t = None
         self.username = None
         self.password = None
         self.server = None
         self.arguments = dict()
         self.return_formatter: dataFormatters.BaseDataFormatter = dataFormatters.BaseDataFormatter(self.return_fields)
-        self.default_arguments()
+        self.required_arguments += self.default_arguments
         if self.supports_config_file:
             self.optional_arguments.append(Argument('file'))
+        if self.required_arguments:
+            for argument in self.required_arguments:
+                argument.is_required(True)
+        if self.optional_arguments:
+            for argument in self.optional_arguments:
+                argument.is_required(False)
         if isinstance(self.required_arguments, list):
             self.required_arguments = {argument.argument:argument for argument in self.required_arguments}
             self.arguments.update(**self.required_arguments)
-        if isinstance(self.optional_arguments, list):  
-            self.optional_arguments = {argument.argument:argument for argument in self.optional_arguments}
+        if isinstance(self.optional_arguments, list): 
+            self.optional_arguments = {argument.argument:argument for argument in self.optional_arguments} 
             self.arguments.update(**self.optional_arguments)
         self.positional_arguments = [arg_name for arg_name, arg in self.required_arguments.items() if arg.positional]
         self.form_arguments = [arg_name for arg_name, arg in self.arguments.items() if arg.arg_type not in  ('standard', 'silent')]
         self.help: dict[dict[str, list[dict[str, str]]]] = dict()
 
         self.command_execution_sequence = []
         if self.positional_arguments:
             self.command_execution_sequence.append(self.check_for_positionals)
         if self.command_opt:
             self.command_execution_sequence.append(self.handle_arg_opts)
         self.command_execution_sequence.append(self.verify_argument_rules_followed)
         if self.form_arguments:
             self.command_execution_sequence.append(self.handle_form_input)
-        self.command_execution_sequence.append(self.verify_argument_rules_followed)
         self.command_execution_sequence.append(self.filter_kwargs)
 
-    def default_arguments(self):
-        """
-        these are pseudarguments that allow some non-argument data to be passed to the command. This is a bit hacky, but its programatically necessary in the context of this framework
-        """
-        default_arguments = [Argument('connection', arg_type='silent'),
-                            Argument('verbose', arg_type='silent'),
-                            Argument('help', arg_type='silent'),
-                            Argument('positionals', arg_type='silent')]
-        
-        for command in default_arguments:
-            self.required_arguments.append(command)
-
     async def verify_argument_rules_followed(self, kwargs):
         """
         verify that the rules for each argument are followed, this is the argument validation
         """
         for name, value in self.arguments.items():
-            if name in self.required_arguments and kwargs[name] == None:
-                raise Exception(f"The argument {name} is required by the command {self.__class__.__name__}")
-            elif name in kwargs and name in self.required_arguments and name not in self.form_arguments:
-                kwargs[name] = self.required_arguments[name].verify_standard_value(kwargs[name])
-            elif name in kwargs and name in self.optional_arguments and name not in self.form_arguments:
-                kwargs[name] = self.optional_arguments[name].verify_standard_value(kwargs[name])
+            kwargs[name] = self.arguments[name].verify_rules_followed(kwargs[name])
             if kwargs[name] and value.depends_on:
                 for dependency in value.depends_on:
                     if not kwargs[dependency]:
                         raise Exception(f"The argument {name} requires the arguments {value.depends_on}")
+            if kwargs[name] and value.mutually_exclusive_with and kwargs[value.mutually_exclusive_with]:
+                raise Exception(f'The argument {name} is mutually exclusive with {value.mutually_exclusive_with}. Only one can be specified!')
         return kwargs
 
     async def filter_kwargs(self, kwargs):
         """
-        filters out kwargs that have None value, Tapis breaks if I dont do this
+        filters out kwargs that have None value, Tapis breaks if I dont do this, especially with form arguments
         """
         filtered_kwargs = dict()
-        for arg, value in kwargs.items():
-            if arg in self.arguments and value or arg in self.required_arguments or (value == False and arg in self.arguments and self.arguments[arg].arg_type == 'standard'):
-                filtered_kwargs[arg] = value
+        for arg_name, value in kwargs.items():
+            if value != None:
+                filtered_kwargs[arg_name] = value
+        #kwargs['connection'].logger.info(f"Running the command {self.__class__.__name__} with the kwargs {pformat(filtered_kwargs)}")
         return filtered_kwargs
 
     async def handle_config_file(self, kwargs):
         """
         when there is a config file submitted, that config file overrides all the other received kwargs
         """
         if kwargs['file']:
             with open(kwargs['file'], 'r') as f:
                 kwargs = json.load(f)
             if 'error' in kwargs:
                 kwargs.pop('error')
         return kwargs
     
-    async def handle_form_input(self, kwargs, complex_args_flag=True):
+    async def handle_form_input(self, kwargs):
         """
         handles forms when the user selects to fill them out
         """
-        existing_values = dict()
+        existing_values = dict() # If it aint broke, dont fix it. This code sucks but I cant meet the deadline if I try fixing this abomination
         if self.updateable_form_retriever:
             existing_values = self.return_formatter.obj_to_dict(self.updateable_form_retriever(self.t, **kwargs))
-        for arg_name in self.form_arguments:
-            if kwargs[arg_name] or arg_name in self.required_arguments:
-                request = schemas.FormRequest(request_content={arg_name:self.arguments[arg_name]}, existing_data=existing_values)
+            to_pop = []
+            reformatted_default_values = dict()
+            for argument in self.form_arguments:
+                argument = self.arguments[argument]
+                if argument.arg_type == 'form' and argument.flattening_type in ('FLATTEN', 'RETRIEVE') and set(argument.arguments_list.keys()).issubset(set(existing_values.keys())):
+                    reformatted_default_values[argument.argument] = {sub_arg_name:sub_arg_value for sub_arg_name, sub_arg_value in existing_values.items() if sub_arg_name in argument.arguments_list}
+                    to_pop += list(argument.arguments_list.keys()) + [argument.argument]
+                elif argument.arg_type == 'form' and argument.part_of and argument.argument in existing_values[argument.part_of]:
+                    reformatted_default_values[argument.argument] = existing_values[argument.part_of][argument.argument]
+                    if argument.part_of not in to_pop:
+                        to_pop.append(argument.part_of)
+            for argument, value in existing_values.items():
+                if argument not in to_pop:
+                    reformatted_default_values[argument] = value
+            if reformatted_default_values:
+                existing_values = reformatted_default_values
+
+        for arg_name in self.form_arguments: 
+            argument = self.arguments[arg_name]
+            if kwargs[arg_name] or argument.required:
+                pprint(f"NAME: {arg_name}\nVALUE: {kwargs[arg_name]}\n REQUIRED: {self.arguments[arg_name].required}")
+                request = schemas.FormRequest(request_content={arg_name:argument}, existing_data=existing_values)
                 await kwargs['connection'].send(request)
                 response: schemas.FormResponse = await kwargs['connection'].receive()
-                kwargs.update(**response.request_content)
+                response_value = response.request_content
+                if response_value == None:
+                    raise ValueError(f"No value was received for the argument {arg_name}")
+                response_value = argument.verify_rules_followed(response_value)
+                if argument.arg_type == 'form' and argument.flattening_type in ('FLATTEN', 'RETRIEVE'):
+                    kwargs.pop(arg_name)
+                if argument.part_of:
+                    if argument.part_of not in kwargs:
+                        kwargs[argument.part_of] = dict()
+                    kwargs[argument.part_of][argument.argument] = response_value
+                else:
+                    kwargs.update(**response_value)
         return kwargs
 
     async def handle_arg_opts(self, kwargs):
         """
         arg opts handle special operations, like supporting relative file paths, and system entry
         """
         for opt in self.command_opt:
@@ -236,51 +236,46 @@
         """
         whenever the tenant or user changes, the new tapis object with the new credentials must be passed to each command to ensure they are operating on the currect user
         """
         self.t = t
         self.username = username
         self.password = password
         self.server = server
-        for key, arg in self.optional_arguments.items():
-            if issubclass(arg.choices.__class__, DynamicChoiceList):
-                arg.choices = arg.choices(self.t)
 
     def update_args_with_truncated(self, truncated_args_dict):
         """
         when the command group finishes processing all the truncated arguments, they get passed back here to be processed and assigned
         """
         try:
-            for key in self.required_arguments:
-                self.required_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
-            for key in self.optional_arguments:
-                self.optional_arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
+            for key in self.arguments:
+                self.arguments[key].truncated_arg = f"-{truncated_args_dict[key]}"
             self.help['required'] = self.__argument_help_compiler(self.required_arguments)
             self.help['optional'] = self.__argument_help_compiler(self.optional_arguments)
         except Exception as e:
-            print(self.__class__.__name__)
             raise e
         
     def __argument_help_compiler(self, arg_dict: dict[str, Argument]):
         """
         compile the help menus based on stored command metadata
         """
         verbose_dict = dict()
         standard_str = str()
         for name, argument in arg_dict.items():
-            if not (name in self.required_arguments and name in self.form_arguments) and argument.arg_type != 'silent':
+            if argument.arg_type != 'silent' and not (argument.arg_type != 'standard' and argument.required):
                 verbose_dict[name] = argument.help_message()
                 standard_str += argument.str()
         return {'verbose':verbose_dict, 'standard':standard_str}
 
     def __get_help(self, verbose):
         """
         return the compiled help menus
         """
         help_dict = {"Command":self.__class__.__name__,
-                    "Description":self.help_string_retriever()}
+                    "Description":self.help_string_retriever(),
+                    "Support Config File":self.supports_config_file}
         if not verbose:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__} {self.help['required']['standard']}\n(Optional Arguments) {self.help['optional']['standard']}"})
         else:
             help_dict.update(**{
                 "Syntax":f"{self.__class__.__name__}",
                 "Required Arguments":self.help['required']['verbose'],
@@ -301,36 +296,31 @@
         """
         pass
 
     async def __call__(self, **kwargs):
         """
         runs all command meta-operations
         """
-        if self.supports_config_file and kwargs['file']:
+        kwargs['connection'].logger.info(f"Attempting to execute the command {self.__class__.__name__}")
+        if self.supports_config_file and kwargs['file']: # if there is a config file input, skip all the other steps and take kwargs from that file
             new_kwargs = await self.handle_config_file(kwargs)
             for arg_name, arg in kwargs.items():
                 if arg_name in ('connection', 'positionals', 'verbose', 'help'):
                     new_kwargs[arg_name] = arg
             kwargs = new_kwargs
         else:
-            if self.decorator:
-                try:
-                    return_value = await self.decorator(input_command=self, **kwargs)
-                except (ValueError, exceptions.NoConfirmationError) as e:
-                    return f"Command execution failed due to {e}"
-
             if kwargs['help']:
                 return self.__get_help(verbose=kwargs['verbose'])
             for handler in self.command_execution_sequence:
                 kwargs = await handler(kwargs)
         try:
             return_value = await self.run(**kwargs)
         except (exceptions.Shutdown, exceptions.Exit) as e:
             raise e
-        except Exception as e:
+        except Exception as e: # this whole part writes command input to a file in the event a form command fails
             if self.supports_config_file:
                 current_date = datetime.now()
                 formatted_date = current_date.strftime("%m-%d-%y")
                 main_save_path = f"{saved_command_root_dir}\\{formatted_date}"
                 try:
                     os.listdir(main_save_path)
                 except:
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandMap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,36 @@
+from .Apps import appCommands
+from .Systems import systemCommands
+import pprint
+
+
 if __name__ != "__main__":
-    from . import systemCommands, volumeCommands, serverCommands, appCommands, podCommands, fileCommands, dataFormatters, baseCommand, jobCommands
+    from . import volumeCommands, serverCommands, podCommands, fileCommands, dataFormatters, baseCommand, jobCommands
     from .query import postgres, neo4j
     from utilities import exceptions
     from commands.arguments.argument import Argument
     from commands.commandOpts import CHECK_EXPLICIT_ID
 
 
 class Systems(baseCommand.BaseCommandMap):
     """
     @help: run operations on Tapis systems
     """
     command_map = {
         'get_systems':systemCommands.get_systems(), # since initialization of commands is separate from __init__, you dont need to specify these as classes anymore
-        'get_system_info':systemCommands.get_system_info(),
+        'get_system':systemCommands.get_system(),
         'get_scheduler_profiles':systemCommands.get_scheduler_profiles(),
+        'create_scheduler_profile':systemCommands.create_scheduler_profile(),
+        'delete_scheduler_profile':systemCommands.delete_scheduler_profile(),
         'submit_system_credentials':systemCommands.submit_system_credentials(),
         'verify_pki_keys':systemCommands.verify_pki_keys(),
         'create_system':systemCommands.create_system(),
+        'create_s3_system':systemCommands.create_s3_system(),
         'update_system':systemCommands.update_system(),
+        'update_s3_system':systemCommands.update_s3_system(),
         'is_system_enabled':systemCommands.is_system_enabled(),
         'enable_system':systemCommands.enable_system(),
         'disable_system':systemCommands.disable_system(),
         'system':systemCommands.system(),
         'exit_system':systemCommands.exit_system(),
         'delete_system':systemCommands.delete_system(),
         'undelete_system':systemCommands.undelete_system(),
@@ -42,16 +51,15 @@
         'get_tenants':serverCommands.get_tenants(),
         'get_tenant':serverCommands.get_tenant(),
         'whoami':serverCommands.whoami(),
         'user':serverCommands.user(),
         'whereami':serverCommands.whereami(),
         'exit':serverCommands.exit(),
         'shutdown':serverCommands.shutdown(),
-        "get_args":serverCommands.get_args(),
-        'switch_service_to':serverCommands.switch_service_to(),
+        'switch_tenant_to':serverCommands.switch_tenant_to(),
         'manpages':serverCommands.manpages()
     }
 
 
 class Pods(baseCommand.BaseCommandMap):
     """
     @help: run operations on tapis pods
@@ -232,22 +240,22 @@
             command.set_t_and_creds(t, username, password, self)
 
     async def run_command(self, connection, command_data: dict):
         """
         process and run command based on received kwargs
         """
         command_name = command_data['command_selection']
-
         if command_name in self.aggregate_command_map:
             command = self.aggregate_command_map[command_name]
             command_data['connection'] = connection
             kwargs = dict()
             for argument, value in command_data.items():
                 if argument in command.arguments:
                     kwargs[argument] = value
+            pprint.pprint(kwargs)
             return await command(**kwargs)
         elif command_name in self.groups:
             return self.groups[command_name]()
         elif command_name == "help":
             return self.help
         else:
             raise exceptions.CommandNotFoundError(command_name)
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class CHECK_EXPLICIT_ID:
     def __init__(self, arg_name: str):
         self.arg_name = arg_name
     
     def __call__(self, kwargs):
-        if not kwargs[self.arg_name]:
+        if self.arg_name not in kwargs or not kwargs[self.arg_name]:
             kwargs[self.arg_name] = kwargs['connection'].system
         return kwargs
 
 
 class CHECK_PWD:
     """
     support the invocation of relative paths for tapis systems
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     
     def non_verbose_formatter(self, serialized_data):
         formatted = dict()
         if self.non_verbose_fields:
             for field in self.non_verbose_fields:
                 if isinstance(field, str):
                     formatted[field] = serialized_data[field]
-                    print(serialized_data[field])
                 elif isinstance(field, list):
                     formatted[field] = self.non_verbose_formatter(serialized_data[field])
             return formatted
         else:
             return serialized_data
     
     def __call__(self, data, verbose):
         serialized = self.obj_to_dict(data)
-        if verbose:
-            return serialized
-        if isinstance(serialized, list) and self.non_verbose_fields:
-            return_data = list()
-            for fragment in serialized:
-                non_verbose_fragment = self.non_verbose_formatter(fragment)
-                return_data.append(non_verbose_fragment)
-            return return_data
-        return self.non_verbose_formatter(serialized)
+        if not isinstance(data, (str, int)):
+            if verbose:
+                return serialized
+            if isinstance(serialized, list) and self.non_verbose_fields:
+                return_data = list()
+                for fragment in serialized:
+                    non_verbose_fragment = self.non_verbose_formatter(fragment)
+                    return_data.append(non_verbose_fragment)
+                return return_data
+            return self.non_verbose_formatter(serialized)
+        else:
+            return data
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('file_path', positional=True),
         Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         size = self.t.files.getStatInfo(systemId=kwargs['systemId'], path=kwargs['file_path']).size
-        if size <= 4000:
+        if size <= 4096:
             file_info = self.t.files.getContents(systemId=kwargs['systemId'],
                                 path=kwargs['file_path'])
         else:
             file_info = "file too large to print"
         return file_info
     
 
@@ -121,15 +121,14 @@
         return f"File copied successfully to {kwargs['destination_file']}"
     
 
 class rm(baseCommand.BaseCommand):
     """
     @help: delete a selected file
     """
-    decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('file_path', positional=True),
         Argument('systemId', size_limit=(1, 80), positional=True)
     ]
     async def run(self, *args, **kwargs):
         self.t.delete(systemId=kwargs['systemId'], path=kwargs['file_path'])
@@ -232,15 +231,15 @@
 class upload(baseCommand.BaseCommand):
     """
     @help: upload a file to the system 
     the source and destination files must both be in the file argument, respectively, separated by a comma
     @todo: make it so that this doesnt need to take both source and destination files, but have it so it retrieves the current file location on the tapis system
     and sets that file location to be the upload point. Do the same for downloads but in reverse
     """
-    command_opt = [commandOpts.CHECK_PWD(('destination_file',))]
+    command_opt = [commandOpts.CHECK_PWD(('destination_file',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('source_file', positional=True),
         Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('destination_file'),
     ]
     async def run(self, *args, **kwargs) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         if not kwargs['destination_file']:
@@ -252,15 +251,15 @@
 
 
 class download(baseCommand.BaseCommand):
     """
     @help: download a file from the system
     the source and destination files must both be in the file argument, respectively, separated by a comma
     """
-    command_opt = [commandOpts.CHECK_PWD(('source_file',))]
+    command_opt = [commandOpts.CHECK_PWD(('source_file',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('source_file', positional=True),
         Argument('systemId', size_limit=(1, 80), positional=True),
         Argument('destination_file'),
         Argument('connection', arg_type='silent')
     ]
     async def run(self, *args, **kwargs) -> str: # download a remote file using tapis, operates basically the same as upload
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from .arguments import argument
-    from . import appCommands
+    from .Apps import appCommands
     from commands import commandOpts
     Argument = argument.Argument
 
 
 class hide_job(baseCommand.BaseCommand):
     """
     @help: hide a job if its already completed
     """
     required_arguments = [
-        Argument('jobUuid')
+        Argument('jobUuid', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.hideJob(**kwargs)
     
 
 class unhide_job(hide_job):
     """
@@ -25,15 +25,18 @@
         return self.t.jobs.unhideJob(**kwargs)
     
 
 class cancel_job(hide_job):
     """
     @help: cancel a job as it executes
     """
-    deceorator = decorators.NeedsConfirmation()
+    required_arguments = [
+        Argument('jobUuid', positional=True),
+        Argument('confirm', arg_type='confirmation')
+    ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.cancelJob(**kwargs)
     
 
 class get_job(hide_job):
     """
     @help: get a job and its information
@@ -109,18 +112,18 @@
     """
     @help: submit a job to be run on the select system based on a pre-existing app
     """
     return_fields = ['name', 'status', 'uuid', 'appId', 'execSystemId']
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('execSystemId')]
     required_arguments = [
         Argument('appId', size_limit=(1, 80), positional=True),
-        Argument('appVersion', size_limit=(1, 64)),
         Argument('name', positional=True)
     ]
     async def run(self, *args, **kwargs):
+        kwargs = appCommands.get_latest_version(self.t, kwargs)
         return self.t.jobs.submitJob(**kwargs)
     
 
 class share_job(baseCommand.BaseCommand):
     """
     @help: share a job with the select grantee user
     """
@@ -174,15 +177,15 @@
             'JOB_ARCHIVE_TRANSACTION_ID',
             'JOB_SUBSCRIPTION',
             'JOB_SHARE_EVENT',
             'JOB_ERROR_MESSAGE',
             'JOB_USER_EVENT',
             'ALL'
             ]),
-        Argument('deliveryTargets', arg_type='input_list', data_type=argument.Form('deliveryTarget', arguments_list=[
+        Argument('deliveryTargets', arg_type='input_list', data_type=argument.Form('deliveryTarget', required_arguments=[
             Argument('deliveryMethod', choices=['WEBHOOK', 'EMAIL', 'QUEUE', 'ACTOR']),
             Argument('deliveryAddress')
         ]))
     ]
     optional_arguments = [
         Argument('description', arg_type='str_input'),
     ]
@@ -203,14 +206,23 @@
         return self.t.jobs.getSubscriptions(**kwargs)
     
 
 class delete_subscriptions(baseCommand.BaseCommand):
     """
     @help: delete a subscription if you no longer want to receive its notifications
     """
-    decorator = decorators.NeedsConfirmation()
     required_arguments = [
-        Argument('uuid')
+        Argument('confirm', arg_type='confirmation')
+    ]
+    optional_arguments = [
+        Argument('jobUuid'),
+        Argument('subscriptionUuid', mutually_exclusive_with=['jobUuid'])
     ]
     async def run(self, *args, **kwargs):
-        self.t.jobs.deleteSubscriptions(**kwargs)
+        if kwargs['jobUuid']:
+            uuid = kwargs['jobUuid']
+        elif kwargs['subscriptionUuid']:
+            uuid = kwargs['subscriptionUuid']
+        else:
+            raise ValueError('Must either specify jobUuid or subscriptionUuid')
+        self.t.jobs.deleteSubscriptions(uuid=uuid)
         return f"subscription {kwargs['uuid']} deleted"
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/podCommands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pyperclip
+import pprint
 from tapipy.tapis import errors as TapisErrors
 
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from .arguments import argument
     Argument = argument.Argument
@@ -29,50 +30,51 @@
     async def run(self, *args, **kwargs) -> str: 
         pod_data = self.t.pods.get_pod(pod_id=kwargs["pod_id"])
         return pod_data
 
 
 class create_pod(baseCommand.BaseCommand):
     """
-    @help: create a new pod on the selected Tapis service
-    @doc: fix the pod updating, make sure non selected optional vaiables do not overwrite. Why description appending???
+    @help: create a new pod. Pods are non persistent and have limited lives by default. You can either set them to live forever by setting time to stop to -1, or have them backup to a volume mount
     """
     return_fields = ['pod_id', 'pod_template', 'status']
     supports_config_file=True
     required_arguments=[
         Argument('pod_id', positional=True),
-        Argument('pod_template', positional=True)
+        Argument('pod_template', positional=True),
     ]
     optional_arguments=[
-        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
-        Argument('command', arg_type='input_list', data_type=argument.Argument('command', arg_type='str_input'), description="Command to run in the pod"),
-        Argument('environment_variables', arg_type='input_dict', data_type=argument.Argument('environment_variable', arg_type='str_input')),
-        Argument('roles_required', arg_type='input_list', data_type=argument.Argument('required_role', arg_type='str_input'), description='what role is required by the user to access this pod?'),
-        Argument('time_to_stop_default', data_type='int'),
-        Argument('time_to_stop_instance', data_type='int'),
         Argument('volume_mounts', arg_type='input_dict', data_type=argument.Form(
-            'volume_mount', arguments_list = [
+            'volume_mount', required_arguments = [
                 Argument('type', choices=['tapisvolume', 'tapissnapshot', 'pvc']),
-                Argument("mount_path", description='This is top level path you want to mount the volume on inside the pod. This is something like <neo4j-home>\data for a neo4j pod. Data from that path will load to the mount and become persistent'),
+                Argument("mount_path", description='This is top level path you want to mount the volume on inside the pod. This is something like <neo4j-home>\data for a neo4j pod. Data from that path will load to the mount and become persistent')
+            ],
+            optional_arguments = [
                 Argument('sub_path', description='If you want to only load a single file, like file.txt (which is inside the parent mount path) you can specify here')
             ]
         ), description="Used to attach the pod to an existing kubernetes volume to provide pod persistence (in case of crash). Each key is the volume_id"),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('command', arg_type='input_list', data_type=argument.Argument('command', arg_type='str_input'), description="Command to run in the pod"),
+        Argument('environment_variables', arg_type='input_dict', data_type=argument.Argument('environment_variable', arg_type='str_input')),
+        Argument('roles_required', arg_type='input_list', data_type=argument.Argument('required_role', arg_type='str_input'), description='what role is required by the user to access this pod?'),
+        Argument('time_to_stop_default', data_type='int', description='set to -1 to run forever'),
+        Argument('time_to_stop_instance', data_type='int', description='set to -1 to run forever'),
         Argument('networking', arg_type='input_dict', data_type=argument.Form(
-            'network', arguments_list = [
-                Argument('protocol', description='Something like https'),
-                Argument('port', data_type='int'),
+            'network', required_arguments = [
+                Argument('protocol', default_value='http', description='Something like https'),
+                Argument('port', data_type='int', default_value=5000),
                 Argument('url')
             ]
         ), description='Important networking configuration. You probably shouldnt touch this, but I wont stop you'),
         argument.Form(
-            'resources', arguments_list = [
-                Argument('cpu_request', data_type='int'),
-                Argument('cpu_limit', data_type='int'),
-                Argument('mem_request', data_type='int'),
-                Argument('mem_limit', data_type='int'),
+            'resources', required_arguments = [
+                Argument('cpu_request', data_type='int', default_value=250),
+                Argument('cpu_limit', data_type='int', default_value=2000),
+                Argument('mem_request', data_type='int', default_value=256),
+                Argument('mem_limit', data_type='int', default_value=3072),
             ]
         )
     ]
     async def run(self, *args, **kwargs) -> str:
         template_name = kwargs['pod_template']
         template_formats = (f"template/{template_name}", f"{self.username}/{template_name}", template_name)
         if 'volume_mounts' in kwargs and kwargs['volume_mounts']:
@@ -110,16 +112,48 @@
     @help: update a pod. Must be restarted to stage changes
     """
     updateable_form_retriever=PodUpdatingRetriever()
     return_fields = ['pod_id', 'pod_template', 'status']
     required_arguments=[
         Argument('pod_id', positional=True),
     ]
+    optional_arguments=[
+        Argument('volume_mounts', arg_type='input_dict', data_type=argument.Form(
+            'volume_mount', required_arguments = [
+                Argument('type', choices=['tapisvolume', 'tapissnapshot', 'pvc']),
+                Argument("mount_path", description='This is top level path you want to mount the volume on inside the pod. This is something like <neo4j-home>\data for a neo4j pod. Data from that path will load to the mount and become persistent')
+            ],
+            optional_arguments = [
+                Argument('sub_path', description='If you want to only load a single file, like file.txt (which is inside the parent mount path) you can specify here')
+            ]
+        ), description="Used to attach the pod to an existing kubernetes volume to provide pod persistence (in case of crash). Each key is the volume_id"),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('command', arg_type='input_list', data_type=argument.Argument('command', arg_type='str_input'), description="Command to run in the pod"),
+        Argument('environment_variables', arg_type='input_dict', data_type=argument.Argument('environment_variable', arg_type='str_input')),
+        Argument('roles_required', arg_type='input_list', data_type=argument.Argument('required_role', arg_type='str_input'), description='what role is required by the user to access this pod?'),
+        Argument('time_to_stop_default', data_type='int'),
+        Argument('time_to_stop_instance', data_type='int'),
+        Argument('networking', arg_type='input_dict', data_type=argument.Form(
+            'network', required_arguments = [
+                Argument('protocol', default_value='http', description='Something like https'),
+                Argument('port', data_type='int', default_value=5000),
+                Argument('url')
+            ]
+        ), description='Important networking configuration. You probably shouldnt touch this, but I wont stop you'),
+        argument.Form(
+            'resources', required_arguments = [
+                Argument('cpu_request', data_type='int', default_value=250),
+                Argument('cpu_limit', data_type='int', default_value=2000),
+                Argument('mem_request', data_type='int', default_value=256),
+                Argument('mem_limit', data_type='int', default_value=3072),
+            ]
+        )
+    ]
     async def run(self, *args, **kwargs):
-        print(kwargs)
+        pprint.pprint(kwargs)
         pod_information = self.t.pods.update_pod(**kwargs)
         return pod_information
 
 
 class start_pod(baseCommand.BaseCommand):
     """
     @help: start the pod specified with pod_id
@@ -134,49 +168,48 @@
 
 
 class restart_pod(baseCommand.BaseCommand):
     """
     @help: initiate a pod restart
     """
     return_fields = ['pod_id', 'pod_template', 'status']
-    decorator=decorators.NeedsConfirmation()
     required_arguments=[
         Argument('pod_id', positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs) -> str:
         return_information = self.t.pods.restart_pod(pod_id=kwargs['pod_id'])
         return return_information
 
 
 class stop_pod(baseCommand.BaseCommand):
     """
     @help: stop a pod's operations
     """
     return_fields = ['pod_id', 'pod_template', 'status']
-    decorator=decorators.NeedsConfirmation()
     required_arguments=[
         Argument('pod_id', positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs):
         return_information = self.t.pods.stop_pod(pod_id=kwargs['pod_id'])
         return str(return_information)
 
 
 class delete_pod(baseCommand.BaseCommand):
     """
     @help: delete select pod
     """
-    return_fields = ['pod_id', 'pod_template', 'status']
-    decorator=decorators.NeedsConfirmation()
     required_arguments=[
         Argument('pod_id', positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs) -> str: 
         return_information = self.t.pods.delete_pod(pod_id=kwargs['pod_id'])
-        return str(return_information)
+        return return_information
     
 
 class set_pod_perms(baseCommand.BaseCommand):
     """
     @help: set the permissions for the pod selected
     """
     return_fields = ['permissions']
@@ -191,21 +224,20 @@
 
 
 class delete_pod_perms(baseCommand.BaseCommand):
     """
     @help: delete the selected pod from the pods service you are connected to
     """
     return_fields = ['permissions']
-    decorator=decorators.NeedsConfirmation()
     required_arguments=[
         Argument('pod_id', positional=True),
         Argument('username')
     ]
     async def run(self, *args, **kwargs) -> str: # take away someones perms if they are being malicious, or something
-        return_information = self.t.pods.delete_pod_perms(pod_id=kwargs['pod_id'], user=kwargs['username'])
+        return_information = self.t.pods.delete_pod_permission(pod_id=kwargs['pod_id'], user=kwargs['username'])
         return return_information
 
 
 class get_pod_perms(baseCommand.BaseCommand):
     """
     @help: get the permissions list for the selected pod
     """
@@ -218,15 +250,14 @@
         return return_information
 
 
 class copy_pod_password(baseCommand.BaseCommand):
     """
     @help: copy the pod password to the clipboard
     """
-    decorator=decorators.Auth()
     required_arguments=[
         Argument('pod_id', positional=True),
     ]
     async def run(self, *args, **kwargs) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
         password = self.t.pods.get_pod_credentials(pod_id=kwargs['pod_id']).user_password
         pyperclip.copy(password)
         password = None
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+import webbrowser
 
 from tapipy.tapis import Tapis
 
 
 if __name__ != "__main__":
     from . import baseCommand, decorators
     from utilities import exceptions
@@ -17,39 +18,40 @@
         tenant = t.tenants.get_tenant(tenant_id=t.tenant_id)
         site_id = tenant.site_id
         supported_services = t.tenants.get_site(site_id=site_id).services
         filtered_supported_services = [service for service in supported_services if service in self.available_services]
         return filtered_supported_services
 
 
-class get_tenants(baseCommand.BaseCommand):
+class get_tenants(baseCommand.BaseCommand): # give this return fields
     """
     @help: get a list of available tenants to authenticate with
     """
     async def run(self, *args, **kwargs):
         return_data = dict()
         tenants = self.t.tenants.list_tenants()
         for tenant in tenants:
             return_data[tenant.tenant_id] = {'uri':tenant.base_url.split('//')[1], 'owner':tenant.owner, 'description':tenant.description}
         return return_data
+
     
 
 class get_tenant(baseCommand.BaseCommand):
     """
     @help: get a specific tenant
     """
     required_arguments = [
         Argument('tenant_id', positional=True)
     ]
     async def run(self, *args, **kwargs):
         tenant = self.t.tenants.get_tenant(**kwargs)
         return {'uri':tenant.base_url.split('//')[1], 'owner':tenant.owner, 'description':tenant.description}
     
     
-class switch_service_to(baseCommand.BaseCommand):
+class switch_tenant_to(baseCommand.BaseCommand):
     """
     @help: switch the connected tapis service
     @todo: upgrade to federated auth
     """
     required_arguments=[
         Argument('tenant_uri', size_limit=(0, 80), positional=True),
         Argument('auth', choices=['password', 'device_code', 'federated']),
@@ -101,21 +103,14 @@
     @help: returns the username of the selected user
     """
     required_arguments = [
         Argument('username', positional=True)
     ]
     async def run(self, *args, **kwargs):
         return self.t.authenticator.get_profile(**kwargs)
-
-class get_args(baseCommand.BaseCommand):
-    """
-    @help: get the list of possible arguments 
-    """
-    async def run(self, *args, **kwargs):
-        return self.server.arguments
     
 
 class whereami(baseCommand.BaseCommand):
     """
     @help: get the URI of current tapis tenant
     """
     async def run(self, *args, **kwargs):
@@ -123,8 +118,9 @@
     
 
 class manpages(baseCommand.BaseCommand):
     """
     @help: get a link to the application manpages
     """
     async def run(self, *args, **kwargs):
+        webbrowser.open('https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE')
         return "Please see https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE for manpages (will add actual manpages later)"
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/systemCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemCommands.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 Add a way to set a default system to be accessed. You must be able to override this by explicitly specifying system id in command
 add intuitive file access and manipulation using this default system. 
 """
 
 
 import json
 import os
+import pprint
 import webbrowser
 
 
 if __name__ != "__main__":
-    from . import baseCommand, decorators
-    from .arguments import argument
-    from . import commandOpts
+    from .. import baseCommand, decorators
+    from ..arguments import argument
+    from .. import commandOpts
     from socketopts import schemas
+    from . import systemForms
     Argument = argument.Argument
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 base_config_path = os.path.join(__location__, '..\\..\\..\\tapis-config-files\\system-config.json')
 
@@ -53,19 +55,20 @@
     @doc: this is an example of the doc segment of the docstring. not included in help message
     """
     return_fields = ['id', 'systemType', 'host']
     optional_arguments = [
         Argument('listType', choices=['OWNED', 'SHARED_PUBLIC', 'ALL'])
     ]
     async def run(self, *args, **kwargs):
+        pprint.pprint(kwargs)
         systems = self.t.systems.getSystems(**kwargs)
         return systems
     
 
-class get_system_info(baseCommand.BaseCommand):
+class get_system(baseCommand.BaseCommand):
     """
     @help: get information on a selected system
     """
     return_fields = ['id', 'systemType', 'host', 'enabled']
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments=[
         Argument('systemId', size_limit=(1, 80), positional=True)
@@ -103,123 +106,58 @@
 
 class get_scheduler_profiles(baseCommand.BaseCommand):
     """
     @help: get list of scheduler profiles in order to use while creating system
     """
     async def run(self, *args, **kwargs):
         return [{"name":scheduler.name, "description":scheduler.description, "tenant":scheduler.tenant} for scheduler in self.t.systems.getSchedulerProfiles()]
-
-
-class get_scheduler_profiles_choices(argument.DynamicChoiceList):
-    def __call__(self, tapis_instance):
-        profiles_unfiltered = tapis_instance.systems.getSchedulerProfiles()
-        return [profile.name for profile in profiles_unfiltered]
     
 
-class create_system(baseCommand.BaseCommand):
+class create_scheduler_profile(baseCommand.BaseCommand):
     """
-    @help: create a system. Must have a properly configured system file.
-    see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
-    this command will automatically create and upload the ssh keys
+    @help: create a new Tapis scheduler profile with which to run batch jobs on a system
     """
-    supports_config_file=True
-    required_arguments=[
-        Argument('id', size_limit=(1, 80), positional=True),
-        Argument('systemType', choices=["LINUX", "S3", "IRODS", "GLOBUS"], description=
-                                    """LINUX is a standard linux kernel
-S3 refers to an AWS S3 Bucket
-IRODS refers to an IRODS data management system
-GLOBUS refers to a GLOBUS file system"""),
-        Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. For S3, this is the AWS bucket URL"),
-        Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "ACCESS_KEY", "TOKEN", "CERT"], description=
-                                    """Depending on your systemType, you will be restricted to certain options.
-Linux: PASSWORD, PKI_KEYS
-S3: ACCESS_KEY
-GLOBUS: TOKEN
-IRODS: TOKEN
-In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
+    required_arguments = [
+        Argument('name')
     ]
-    optional_arguments=[
-        Argument('canExec', action='store_true', default_value=False, depends_on=['jobRuntimes']),
-        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
-        Argument('owner'),
-        Argument('enabled', action='store_true'),
-        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
-        Argument('bucketName'),
-        Argument('rootDir', default_value='/', size_limit=(0, 4096)),
-        Argument('port', data_type='int'),
-        Argument('useProxy', action='store_true'),
-        Argument('proxyHost', size_limit=(0, 256)),
-        Argument('proxyPort', data_type='int'),
-        Argument('isDtn', action='store_true', depends_on=['rootDir']),
-        Argument('dtnSystemId', size_limit=(0, 80)),
-        Argument('dtnMountPoint'),
-        Argument('canRunBatch', action='store_true', depends_on=['batchScheduler', 'batchLogicalQueues', 'batchLogicalDefaultQueue']),
-        Argument('enableCmdPrefix', action='store_true'),
-        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
-        Argument('jobRuntimes', arg_type='input_list', data_type=argument.Form(
-            'jobRuntime', arguments_list = [
-                Argument('runtimeType', choices=['DOCKER', 'SINGULARITY']), 
-                Argument('version')
-                ]
-            )),
-        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096), description='Where on this hpc system are jobs run?'),
-        Argument('jobEnvVariables', arg_type='input_list', data_type=argument.Form(
-            'jobEnvironmentVariable', arguments_list = [
-                Argument('key'),
-                Argument('value', default_value=''),
-                Argument('description', size_limit=(0, 2048), arg_type='str_input')
-            ]
-        )),
-        Argument('jobMaxJobs', data_type='int'),
-        Argument('jobMaxJobsPerUser', data_type='int'),
-        Argument('batchScheduler', choices=['SLURM', "CONDOR", "PBS", "SGE", "UGE", "TORQUE"]),
-        Argument('batchLogicalQueues', arg_type='input_list', data_type=argument.Form(
-            'batchLogicalQueue', arguments_list = [
-                Argument('name', size_limit=(1, 128)),
-                Argument('hpcQueueName', size_limit=(1, 128)),
-                Argument('maxJobs', data_type='int'),
-                Argument('maxJobsPerUser', data_type='int'),
-                Argument('minNodeCount', data_type='int'),
-                Argument('maxNodeCount', data_type='int'),
-                Argument('minCoresPerNode', data_type='int'),
-                Argument('maxCoresPerNode', data_type='int'),
-                Argument('minMemoryMB', data_type='int'),
-                Argument('maxMemoryMB', data_type='int'),
-                Argument('minMinutes', data_type='int'),
-                Argument('maxMinutes', data_type='int')
-            ]
-        )),
-        Argument('batchDefaultLoginQueue', size_limit=(1, 128)),
-        Argument('batchSchedulerProfile', choices=get_scheduler_profiles_choices()),
-        Argument('jobCapabilities', arg_type='input_list', data_type=argument.Form(
-            'jobCapability', arguments_list=[
-                Argument('category', choices=['SCHEUDLER', 
-                                              'OS', 'HARDWARE', 
-                                              'SOFTWARE', 'JOB', 
-                                              'CONTAINER', 'MISC', 
-                                              'CUSTOM']),
-                Argument('name', size_limit=(1, 128)),
-                Argument('datatype', choices=['STRING', 'INTEGER', 
-                                              'BOOLEAN', 'NUMBER', 
-                                              'TIMESTAMP']),
-                Argument('precedence', data_type='int'),
-                Argument('value')
-            ]
-        )),
-        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
-        Argument('notes', arg_type='str_input'),
-        Argument('importRefId')
+    optional_arguments = [
+        Argument('description', arg_type='str_input'),
+        Argument('owner', default_value=r"${apiUserId}"),
+        Argument('moduleLoads', arg_type='input_list',
+                  data_type=argument.Form('moduleLoad',
+                    required_arguments = [
+                        Argument('moduleLoadCommand')
+                    ],
+                    optional_arguments = [
+                        Argument('modulesToLoad', arg_type='input_list', data_type=Argument('module'))
+                    ]))
     ]
-    def __init__(self):
-        super().__init__()
+    async def run(self, *args, **kwargs):
+        return self.t.systems.createSchedulerProfile(**kwargs)
+
+
+class delete_scheduler_profile(baseCommand.BaseCommand):
+    """
+    @help: delete a scheduler profile
+    """
+    required_arguments = [
+        Argument('name'),
+        Argument('confirm', arg_type='confirmation')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.systems.deleteSchedulerProfile(**kwargs)
+    
+
+class SystemAuth:
+    sys_auth_map = None
+    def config_auth_map(self):
         self.sys_auth_map = {"LINUX":{"PASSWORD":self.password_auth, "PKI_KEYS":self.pki_keys_auth}, 
                              "S3":{"ACCESS_KEY":self.access_key_auth}, "GLOBUS":{"TOKEN":self.token_auth}, 
-                             "IRODS":{"TOKEN":self.token_auth}}
-
+                             "IRODS":{"TOKEN":self.password_auth}}
+        
     async def password_auth(self, **kwargs):
         request = schemas.FormRequest(request_content={'username':Argument('username', arg_type='str_input'), "password":Argument('password', arg_type='secure')},
                                         message={'message':f"Enter your credentials to the select host specified in the system creation"})
         await kwargs['connection'].send(request)
         response = await kwargs['connection'].receive()
         response_content = response.request_content
         password = response_content['password']
@@ -267,141 +205,206 @@
                                       6. run the verify_pki_keys command and submit the system id {kwargs['id']} and the file path of the public and private keys
                                       7. you should be able to access the system now"""},
                                       request_content={"continue":Argument("continue", arg_type='confirmation')})
         await kwargs['connection'].send(request)
         await kwargs['connection'].receive()
         return None        
     
+    async def base_system_auth(self, kwargs):
+        if kwargs['defaultAuthnMethod'] not in self.sys_auth_map[kwargs['systemType']]:
+            raise ValueError(f"The system type {kwargs['systemType']} does not support {kwargs['defaultAuthnMethod']} authentication.")
+        else:
+            try:
+                auth_result = await self.sys_auth_map[kwargs['systemType']][kwargs['defaultAuthnMethod']](**kwargs)
+                return auth_result
+            except Exception as e:
+                raise Exception(f"System creation for {kwargs['id']} succeeded, but Authentication for the system failed, maybe you entered something wrong? run the submit_system_credentials command")
+    
     async def authenticate(self, kwargs):
         return await self.sys_auth_map[kwargs['systemType']][kwargs['defaultAuthnMethod']](**kwargs)
 
+
+class create_system(baseCommand.BaseCommand, SystemAuth):
+    """
+    @help: create a system. Must have a properly configured system file.
+    see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
+    this command will automatically create and upload the ssh keys
+    """
+    supports_config_file=True
+    required_arguments=[
+        Argument('id', size_limit=(1, 80), positional=True),
+        Argument('systemType', choices=["LINUX", "S3", "IRODS", "GLOBUS"], description=
+                                    """LINUX is a standard linux system
+IRODS refers to an IRODS data management system
+GLOBUS refers to a GLOBUS file system"""),
+        Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. In the case of Globus, this is a Globus ID"),
+        Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "TOKEN"], description=
+                                    """Depending on your systemType, you will be restricted to certain options.
+LINUX: PASSWORD, PKI_KEYS
+GLOBUS: TOKEN
+IRODS: PASSWORD
+In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
+    ]
+    optional_arguments=[
+        systemForms.CAN_EXEC,
+        systemForms.USE_PROXY,
+        systemForms.CAN_RUN_BATCH,
+        systemForms.MOUNT_DATA_TRANSFER_NODE,
+        systemForms.JOB_CONSTRAINTS,
+        systemForms.JOB_CAPABILITIES,
+        systemForms.JOB_ENVIRONMENT_VARIABLES,
+        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
+        Argument('owner', default_value=r"${apiUserId}"),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('enabled', action='store_true'),
+        Argument('rootDir', default_value='/', size_limit=(0, 4096)),
+        Argument('port', data_type='int', default_value=22),
+        Argument('isDtn', action='store_true', depends_on=['rootDir'], mutually_exclusive_with=['mountDataTransferNode', 'canExec']),
+        Argument('enableCmdPrefix', action='store_true'),
+        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
+        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
+        Argument('notes', arg_type='str_input'),
+        Argument('importRefId')
+    ]
+    def __init__(self):
+        super().__init__()
+        self.config_auth_map()
+
     async def run(self, *args, **kwargs) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
         return_info = dict()
         return_info['system_creation_info'] = self.t.systems.createSystem(**kwargs)
-        if kwargs['defaultAuthnMethod'] not in self.sys_auth_map[kwargs['systemType']]:
-            raise ValueError(f"The system type {kwargs['systemType']} does not support {kwargs['defaultAuthnMethod']} authentication.")
-        else:
-            try:
-                return_info['auth_result'] = await self.sys_auth_map[kwargs['systemType']][kwargs['defaultAuthnMethod']](**kwargs)
-            except Exception as e:
-                return_info['auth_result'] = f"Authentication for the system {kwargs['id']} failed, maybe you entered something wrong? run the submit_system_credentials command"
+        return_info['auth_result'] = await self.base_system_auth(kwargs)
         return return_info
     
 
+class create_s3_system(create_system):
+    """
+    @help: create a system specially configured to support AWS s3 buckets
+    """
+    required_arguments = [
+        Argument('id', size_limit=(1, 80), positional=True),
+        Argument('host', size_limit=(1, 256), description="AWS S3 bucket url"),
+        Argument('bucketName')
+    ]
+    optional_arguments = [
+        systemForms.USE_PROXY,
+        systemForms.CAN_RUN_BATCH,
+        systemForms.MOUNT_DATA_TRANSFER_NODE,
+        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
+        Argument('owner', default_value=r"${apiUserId}"),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('enabled', action='store_true'),
+        Argument('rootDir', default_value='/', size_limit=(0, 4096)),
+        Argument('port', data_type='int', default_value=22),
+        Argument('enableCmdPrefix', action='store_true'),
+        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
+        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
+        Argument('notes', arg_type='str_input'),
+        Argument('importRefId')
+    ]
+    async def run(self, *args, **kwargs):
+        kwargs['defaultAuthnMethod'] = 'ACCESS_KEY'
+        kwargs['systemType'] = 'S3', 
+        return_info = dict()
+        return_info['system_creation_info'] = self.t.systems.createSystem(**kwargs)
+        return_info['auth_result'] = await self.base_system_auth(kwargs)
+        return return_info
+
+
 class submit_system_credentials(create_system):
     """
     @help: manually submit system credentials
     """
     supports_config_file = False
     required_arguments = [
         Argument('id', positional=True)
     ]
     optional_arguments = []
     async def run(self, *args, **kwargs):
         system_info = self.t.systems.getSystem(systemId=kwargs['id'])
         kwargs['systemType'] = system_info.systemType
         kwargs['defaultAuthnMethod'] = system_info.defaultAuthnMethod
+        kwargs['host'] = system_info.host
         return_info = await self.authenticate(kwargs)
         return return_info
     
 
 class SystemUpdatingRetriever(baseCommand.UpdatableFormRetriever):
     def __call__(self, tapis_instance, **kwargs):
         system_data = tapis_instance.systems.getSystem(systemId=kwargs["systemId"])
         return system_data
     
 
-class update_system(create_system):
+class update_system(baseCommand.BaseCommand):
     """
     @help: update a system with new information
     """
     updateable_form_retriever = SystemUpdatingRetriever()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments=[
         Argument('systemId', size_limit=(1, 80), positional=True),
     ]
     optional_arguments=[
-        Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "ACCESS_KEY", "TOKEN", "CERT"], description=
+        systemForms.USE_PROXY,
+        systemForms.CAN_RUN_BATCH,
+        systemForms.MOUNT_DATA_TRANSFER_NODE,
+        systemForms.JOB_CONSTRAINTS,
+        systemForms.JOB_CAPABILITIES,
+        systemForms.JOB_ENVIRONMENT_VARIABLES,
+        Argument('defaultAuthnMethod', choices=['PASSWORD', "PKI_KEYS", "TOKEN"], description=
                                     """Depending on your systemType, you will be restricted to certain options.
-                                    Linux: PASSWORD, PKI_KEYS
-                                    S3: ACCESS_KEY
-                                    GLOBUS: TOKEN
-                                    IRODS: TOKEN
-                                    In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
-        Argument('host', size_limit=(1, 256), description="In the case of Linux this is the hostname or IP of the HPC system you want to connect to. For S3, this is the AWS bucket URL"),
-        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
-        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
-        Argument('port', data_type='int'),
-        Argument('useProxy', action='store_true'),
-        Argument('proxyHost', size_limit=(0, 256)),
-        Argument('proxyPort', data_type='int'),
-        Argument('dtnSystemId', size_limit=(0, 80)),
-        Argument('dtnMountPoint'),
-        Argument('canRunBatch', action='store_true'),
-        Argument('enableCmdPrefix', action='store_true'),
-        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
+LINUX: PASSWORD, PKI_KEYS
+GLOBUS: TOKEN
+IRODS: PASSWORD
+In the case you choose password, your username and password will either be your TACC account info, or the login info you used with federated/device_code grant"""),
         Argument('jobRuntimes', arg_type='input_list', data_type=argument.Form(
-            'jobRuntime', arguments_list = [
-                Argument('runtimeType', choices=['DOCKER', 'SINGULARITY']), 
-                Argument('version')
+            'jobRuntime', required_arguments = [
+                    Argument('runtimeType', choices=['DOCKER', 'SINGULARITY']), 
+                ],
+                optional_arguments=[
+                    Argument('version')
                 ]
             )),
-        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096)),
-        Argument('jobEnvVariables', arg_type='input_list', data_type=argument.Form(
-            'jobEnvironmentVariable', arguments_list = [
-                Argument('key'),
-                Argument('value', default_value=''),
-                Argument('description', size_limit=(0, 2048), arg_type='str_input')
-            ]
-        )),
-        Argument('jobMaxJobs', data_type='int'),
-        Argument('jobMaxJobsPerUser', data_type='int'),
-        Argument('batchScheduler', choices=['SLURM', "CONDOR", "PBS", "SGE", "UGE", "TORQUE"]),
-        Argument('batchLogicalQueues', arg_type='input_list', data_type=argument.Form(
-            'batchLogicalQueue', arguments_list = [
-                Argument('name', size_limit=(1, 128)),
-                Argument('hpcQueueName', size_limit=(1, 128)),
-                Argument('maxJobs', data_type='int'),
-                Argument('maxJobsPerUser', data_type='int'),
-                Argument('minNodeCount', data_type='int'),
-                Argument('maxNodeCount', data_type='int'),
-                Argument('minCoresPerNode', data_type='int'),
-                Argument('maxCoresPerNode', data_type='int'),
-                Argument('minMemoryMB', data_type='int'),
-                Argument('maxMemoryMB', data_type='int'),
-                Argument('minMinutes', data_type='int'),
-                Argument('maxMinutes', data_type='int')
-            ]
-        )),
-        Argument('batchDefaultLoginQueue', size_limit=(1, 128)),
-        Argument('batchSchedulerProfile', choices=get_scheduler_profiles_choices()),
-        Argument('jobCapabilities', arg_type='input_list', data_type=argument.Form(
-            'jobCapability', arguments_list=[
-                Argument('category', choices=['SCHEUDLER', 
-                                              'OS', 'HARDWARE', 
-                                              'SOFTWARE', 'JOB', 
-                                              'CONTAINER', 'MISC', 
-                                              'CUSTOM']),
-                Argument('name', size_limit=(1, 128)),
-                Argument('datatype', choices=['STRING', 'INTEGER', 
-                                              'BOOLEAN', 'NUMBER', 
-                                              'TIMESTAMP']),
-                Argument('precedence', data_type='int'),
-                Argument('value')
-            ]
-        )),
+        Argument('jobWorkingDir', default_value=r"HOST_EVAL($WORK2)", size_limit=(0, 4096), description='Where on this hpc system are jobs run?'),
+        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('port', data_type='int', default_value=22),
+        Argument('enableCmdPrefix', action='store_true'),
+        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
         Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
         Argument('notes', arg_type='str_input'),
         Argument('importRefId')
     ]
     async def run(self, *args, **kwargs):
         result = self.t.systems.patchSystem(**kwargs)
         return result
     
 
+class update_s3_system(update_system):
+    """
+    @help: update an s3 system
+    """
+    optional_arguments = [
+        systemForms.USE_PROXY,
+        systemForms.CAN_RUN_BATCH,
+        systemForms.MOUNT_DATA_TRANSFER_NODE,
+        Argument('effectiveUserId', default_value=r"${apiUserId}", size_limit=(0, 60)),
+        Argument('description', arg_type='str_input', size_limit=(0, 2048)),
+        Argument('port', data_type='int', default_value=22),
+        Argument('enableCmdPrefix', action='store_true'),
+        Argument('mpiCmd', size_limit=(0, 126), arg_type='str_input'),
+        Argument('tags', arg_type='input_list', data_type=Argument('tag', arg_type='str_input')),
+        Argument('notes', arg_type='str_input'),
+        Argument('importRefId')
+    ]
+    async def run(self, *args, **kwargs):
+        result = self.t.systems.patchSystem(**kwargs)
+        return result
+
+
 class is_system_enabled(baseCommand.BaseCommand):
     """
     @help: check to see if a system is enabled
     """
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
         Argument('systemId', positional=True)
@@ -418,27 +421,26 @@
         return self.t.systems.enableSystem(**kwargs)
     
 
 class disable_system(is_system_enabled):
     """
     @help: disable a system
     """
-    decorator=decorators.NeedsConfirmation()
     async def run(self, *args, **kwargs):
         return self.t.systems.disableSystem(**kwargs)
     
 
 class delete_system(baseCommand.BaseCommand):
     """
     @help: delete the selected system
     """
-    decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments=[
         Argument('systemId', size_limit=(1, 80), positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs) -> str:
         kwargs['connection'].system = ''
         kwargs['connection'].pwd = ''
         return_value = self.t.systems.deleteSystem(systemId=kwargs['systemId'])
         return return_value
     
@@ -447,15 +449,15 @@
     """
     @help: undo deletion
     """
     required_arguments=[
         Argument('systemId', size_limit=(1, 80), positional=True),
     ]
     async def run(self, *args, **kwargs):
-        return self.t.systems.undelete(**kwargs)
+        return self.t.systems.undeleteSystem(**kwargs)
 
 class create_child_system(baseCommand.BaseCommand):
     """
     @help: create a child system which inherits majority attributes from parent
     """
     required_arguments = [
         Argument('parentId', positional=True),
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,18 +83,18 @@
         return self.t.pods.update_volume(**kwargs)
     
 
 class delete_volume(baseCommand.BaseCommand):
     """
     @help: delete a volume
     """
-    decorator=decorators.NeedsConfirmation()
     command_opt = [commandOpts.CHECK_EXPLICIT_ID('volume_id')]
     required_arguments = [
-        Argument('volume_id', positional=True)
+        Argument('volume_id', positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.delete_volume_files(**kwargs)
 
 
 class dir(baseCommand.BaseCommand):
     """
@@ -150,15 +150,14 @@
         return self.t.pods.get_volume_permission(**kwargs)
     
 
 class delete_volume_permission(baseCommand.BaseCommand):
     """
     @help: delete the persmission for a user on a volume
     """
-    decorator=decorators.NeedsConfirmation()
     required_arguments = [
         Argument('volume_id', positional=True),
         Argument('username'),
         Argument('level')
     ]
     async def run(self, *args, **kwargs):
         user = kwargs.pop('username')
@@ -225,17 +224,17 @@
         return self.t.pods.update_snapshot(**kwargs)
     
 
 class delete_snapshot(baseCommand.BaseCommand):
     """
     @help: delete snapshot information
     """
-    decorator=decorators.NeedsConfirmation()
     required_arguments = [
-        Argument('snapshot_id', positional=True)
+        Argument('snapshot_id', positional=True),
+        Argument('confirm', arg_type='confirmation')
     ]
     async def run(self, *args, **kwargs):
         return self.t.pods.delete_snapshot(**kwargs)
     
 
 class list_snapshot_files(baseCommand.BaseCommand):
     """
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,27 +23,29 @@
         self.name = name
         self.connection_list: list = connection_list
         self.reader: asyncio.StreamReader = reader
         self.writer: asyncio.StreamWriter = writer
         self.task: asyncio.Task = None
         self.status = "CLOSED"
         self.shutdown_message = schemas.ResponseData(message={'message':'Shutdown initiated, closing'}, exit_status=1)
+        self.logger.info('Connection successfully initiated, beginning handshake')
 
     def set_status_device_authenticating(self):
         self.status = 'DEVICE_CODE_AUTH'
 
     def set_status_closed(self):
         self.status = 'CLOSED'
 
     def set_status_exiting(self):
         self.status = 'EXITING'
 
     def set_task(self, task: asyncio.Task):
         self.task = task
         self.status = 'OPEN'
+        self.logger.info('Asyncio task for socket operations was received, and is now active')
 
     async def close(self, connection_list_lock: asyncio.Lock):
         self.logger.info('ATTEMPTING TO CLOSE')
         if self.status in ('OPEN', 'EXITING'):
             result = self.task.cancel()
             self.logger.info("successfully cancelled task")
             await self.send(self.shutdown_message)
@@ -54,15 +56,18 @@
             await self.send(schemas.AuthRequest(error='cancelled authentication during device_code grant', auth_request_type='device_code'))
             self.writer.close()
             await self.writer.wait_closed()
         else:
             self.writer.close()
             await self.writer.wait_closed()
         async with connection_list_lock:
-            self.connection_list.remove(self)
+            try:
+                self.connection_list.remove(self)
+            except Exception as e:
+                self.logger.info("Connection was not in the command list, closure ocurred during connection setup")
         print(self.connection_list)
         self.logger.info('SUCCESSFULLY CLOSED')
 
 
 class Server(commandMap.AggregateCommandMap, logger.ServerLogger, decorators.DecoratorSetup, auth.ServerSideAuth):
     """
     Receives commands from the client and executes Tapis operations
@@ -144,84 +149,79 @@
         """
         accept connection request and initialize communication with the client
         """  
         self.num_connections += 1
         self.end_time = time.time() + self.SESSION_TIME
         connection = ServerConnection(f"CON-{self.num_connections}", reader=reader, writer=writer, connection_list=self.connections_list, debug=self.debug)
         ip, port = writer.transport.get_extra_info('socket').getsockname()
-        self.logger.info("Received connection request")
         try:
             await self.handshake(connection)
+            connection.logger.info('Handshake complete')
         except exceptions.InvalidCredentialsReceived as e:
-            self.logger.warning("invalid credentials entered too many times. Cancelling request")
+            connection.logger.warning("invalid credentials entered too many times. Cancelling request")
             await connection.close(self.connection_list_lock)
             return
         except exceptions.ClientSideError as e:
-            self.logger.warning(f"Encountered client side error during startup handshake. {e}")
+            connection.logger.warning(f"Encountered client side error during startup handshake. {e}")
             await connection.close(self.connection_list_lock)
             return
         except Exception as e:
-            self.logger.warning(e)
+            connection.logger.warning(e)
             await connection.close(self.connection_list_lock)
             return
-        self.logger.info("connection is running now")
+        connection.logger.info('Sending command arguments now')
         await connection.send(schemas.ResponseData(request_content={name:argument.json() for name, argument in self.arguments.items()}))
-        
         setup_response: schemas.ResponseData = await connection.receive()
         if not setup_response.request_content['setup_success']:
-            self.logger.warning(f"The setup of the connection {connection.name} failed")
+            connection.logger.warning(f"The setup of the connection upon sending argument information failed")
             return
-
+        connection.logger.info(f"Argument setup succeeded on the client side")
         loop = asyncio.get_event_loop()
         task: asyncio.Task = loop.create_task(self.receive_and_execute(connection))
         connection.set_task(task)
         self.connections_list.append(connection)
-        print([connection.status for connection in self.connections_list])
+        connection.logger.info('All connection setup complete, beginning normal operations')
 
     async def receive_and_execute(self, connection: ServerConnection):
         """
         receive and process commands
         """
-        self.logger.info(f"{connection.name} is now running")
         while self.running:
             try:
                 message = await connection.receive()
                 if not self.running:
                     raise exceptions.Shutdown
                 kwargs = message.request_content
                 result = await self.run_command(connection, kwargs)
                 response = schemas.ResponseData(message={"message":result}, url=self.url, active_username=self.username)
                 self.end_time = time.time() + self.SESSION_TIME 
                 await connection.send(response)
-                self.logger.info(message.schema_type)
             except exceptions.ClientSideError as e:
                 self.logger.warning(e)
                 continue
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
-                #error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username, exit_status=1)
-                #await connection.send(error_response)
-                self.logger.warning(str(e))
+                connection.logger.warning(str(e))
                 self.running = False
                 return
             except exceptions.Exit as e:
-                self.logger.info("user exit initiated")
-                # error_response = schemas.ResponseData(error=str(e), exit_status=1, url=self.url, active_username=self.username)
-                # await connection.send(error_response)
+                connection.logger.info("user exit initiated")
                 connection.set_status_exiting()
                 return
-            except OSError:
-                self.logger.info("connection was lost, waiting to reconnect")
-                await connection.close(self.connection_list_lock)
             except asyncio.CancelledError:
                 return 'task was cancelled'
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
+                if isinstance(e, OSError) and 'The specified network name is no longer available' in str(e):
+                    print(e)
+                    connection.logger.info("connection was lost, waiting to reconnect")
+                    connection.set_status_closed()
+                    return
                 error_str = traceback.format_exc()
                 error_response = schemas.ResponseData(error=str(e), url=self.url, active_username=self.username)
                 await connection.send(error_response)
-                self.logger.warning(f"{error_str}")
+                connection.logger.warning(f"{error_str}")
     
     async def main(self):
         self.server = await asyncio.start_server(self.accept, sock=self.sock)
         try:
             async with self.server:
                 result = await asyncio.gather(self.server.serve_forever(), self.check_timeout(), self.check_shutdown(), return_exceptions=True)#, self.check_timeout(), return_exceptions=True)
                 self.logger.info(str(result))
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,22 +28,28 @@
     """
     behind the scenes, low level functions to handle the socket operations asynchronoously on the server
     """
     def __init__(self, name, debug=False):
         self.initialize_logger(f"{name} LOGGER")
         self.debug_state = debug
 
-    def debug(self, operation: typing.Literal["SENDING", "RECEIVED", "WAITING"], message: str | typing.Type[schemas.BaseSchema]):
+    def debug(self, operation: typing.Literal["SENDING", "RECEIVED", "WAITING"], data: str | typing.Type[schemas.BaseSchema], message: str | None = None):
         if self.debug_state:
-            if not isinstance(message, str):
-                self.logger.info(f"""{operation}: {message.schema_type}
-                                    MESSAGE: {pformat(message.message)}
-                                    ERROR: {pformat(message.error)}""") # MESSAGE CONTENT:{pformat(message.request_content)}
+            if not isinstance(data, str):
+                self.logger.info(f"""{operation}: {data.schema_type}
+                                    MESSAGE: {pformat(data.data)}
+                                    ERROR: {pformat(data.error)}
+                                    MESSAGE CONTENT:{pformat(data.request_content)}""")
             else:
-                self.logger.info(message)
+                self.logger.info(data)
+            return
+        if self.__class__.__name__ == 'ClientSocketOpts':
+            return
+        elif message:
+            self.logger.info(message)
 
 
 class ClientSocketOpts(BaseSocketOpts):
     """
     synchronous sockets to be used by clients
     """
     def __json_receive_explicit(self, connection):
@@ -62,15 +68,15 @@
         connection.send(json_data.encode())
 
     def send(self, data: typing.Type[schemas.BaseSchema]):
         self.debug('SENDING', data)
         self.__json_send_explicit(self.connection, data.dict())
 
     def receive(self) -> typing.Type[schemas.BaseSchema]:
-        self.debug("WAITING", "Awaiting message receive")
+        self.debug("WAITING", "Awaiting data receive")
         data = self.__json_receive_explicit(self.connection)
         schema_type = schema_types[data['schema_type']]
         self.debug('RECEIVED', schema_type(**data))
         return schema_type(**data)
 
 
 class ServerSocketOpts(BaseSocketOpts):
@@ -95,24 +101,24 @@
                 continue
 
     async def send(self, data: typing.Type[schemas.BaseSchema]):
         if data.request_content:
             for key, value in data.request_content.items():
                 if not isinstance(value, (str, list, tuple, bool, int, dict, set)) and value != None:
                     data.request_content[key] = value.json()
-        self.debug('SENDING', data)
+        self.debug('SENDING', data, message=f'Sending data of type {data.schema_type} to the client')
         data.pwd = self.pwd
         data.system = self.system
         json_data = json.dumps(data.dict())
         self.writer.write(json_data.encode())
         await self.writer.drain()
 
     async def receive(self):
-        self.debug("WAITING", "Awaiting message receive")
+        self.debug("WAITING", "Awaiting data receive", message='Waiting to receive data from the client on this connection')
         data = await self.__json_receive_explicit_async()
         schema_type = schema_types[data['schema_type']]
         formatted_data = schema_type(**data)
-        self.debug('RECEIVED', formatted_data)
+        self.debug('RECEIVED', formatted_data, message=f'Successfully received data of type {formatted_data.schema_type}')
         if formatted_data.error:
             raise exceptions.ClientSideError(formatted_data.error)
         return formatted_data
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.2.2
+Version: 1.0.0
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -695,31 +695,109 @@
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
 
 ### Installation
 #### Using PyPi
 1. `pip install TapisCL-ICICLE`. Current version 0.0.24
-2. `python -m TapisCLICICLE`
+2. run using `python -m TapisCLICICLE`
 #### Running Python Code Directly
 1. Clone the repository to local machine.
 2. `python -m pip install -r requirements.txt`
-3. `python cli.py`
-### Operations
-#### **Full Terminal Interface:**
-1. run ``python -m TapisCLICICLE``
-2. You will be promted to enter a Tapis service link. You can find this on the Tapis service provider's wesbite usually. If you are working with icicle, this should be icicle.tapis.io
-3. the application will then prompt you to choose your authentication method, password, federated, or device code. Which ones are avaiable depends on the tenant in question. If you choose either the 2nd or 3rd option, you will be asked to create a session password to authenticate secure operations.
-4. if all went well the console should open. You can run `help` to see command options
-5. to exit the application, run `exit`. To shut it down, run `shutdown`. The server automatically shuts down after 25 minutes of inactivity
+3. from the src folder, run using `python -m TapisCLICICLE`
 
-#### **Bash Command Line:**
+### Known Issues
+Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
+The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
 
-Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
+## Usage
+### Interfaces
+TapisCLICICLE supports two interface types:
+#### Full Terminal Interface:
+If you want a full fledged command line environment to interact with your Tapis services, run the app using `python -m TapisCLICICLE` with no additional arguments. This will spawn the environment where you can enter commands.
+#### Bash Command Line:
+Alternatively, if you want to enter commands directly into your bash terminal, you can run the app with arguments. For example, `python -m TapisCLICICLE create_pod (pod_name) (pod_template)` will create a pod without opening the app environment. The same goes for all commands.
 
-`python -m TapisCLICICLE help -v`
+### Authentication
+TapisCLICICLE supports 3 authentication methods, password, federated, and device code grants. Authentication has a timeout of 5000 seconds of inactivity.
+For each method of authentication, you will be asked to submit a tenant URI. This determines what resources you will have access to. 
+For both federated and device code grants, you will be prompted to create a session password for secure operations (like obtaining pod credentials)
+#### Password
+You can log in to the app using an account username and password for the TACC portal. You must obtain an account directly from TACC to use this login method.
+
+#### Federated
+Requires a valid CILogon account through your university, with google, or with ORCID. Upon selecting this method, a webpage will open requesting login with one of these methods. Once you are authenticated you will receive an access token on the webpage. Dont show this token to anyone. Simultaneously you will be prompted to enter this token on the TapisCLICICLE app. Once you do, you will be authenticated and can use the app.
+
+#### Device Code
+This is functionally the same as the federated authentication, except you are prompted to enter an app generated user code to generate your token after logging in using CILogon. Once you generate your token you must confirm completion on the app and you will be authenticated
+
+#### Notes on Authentication
+Both federated and device code grants are experiemental at the current state in development, and work on only a few tenants
+
+### Help
+TapisCLICICLE supports several Tapis services for interfacing with HPC systems. Basic information on these services can be obtained using the `help` command.
+If you want to get a list of commands which fall under a certain service, enter the service name into the command line. For example, running `Systems` will show all commands under the systems service
+To get information about an individual command, you can run `(command) -h`. This will list all command syntax. Running `(command) -h -v`, specifying verbose with -v will give detailed description of each argument associated with the command
+When running help commands, arguments marked with an (f) do not receive values directly, but send a request for a form back to the client.
+
+### Commands
+Commands in TapisCLICICLE can be divided into 2 classifications: creational and managerial
+
+#### General Commands
+General commands are for managing and viewing information on your current application session.
+
+General Commands:
+* whoami: return information about the current logged in user
+* whereami: return the current tenant URI
+* switch_tenant_to --tenant_uri (tenant_uri) --auth (auth type): log in to a different tenant without shutting down the app. Tenant URI is the base URL of the tenant you want to connect to. For example, icicle.tapis.io, or smartfoods.tapis.io. The auth parameter must be one of the 3 authentication methods previously mentioned, password, federated, or device_code grant.
+* exit: exit the current instance of the application client without deactivating the app entirely. The app continues to run in the background until timeout, or a new user session starts. Starting the client again after
+* shutdown: completely shut down the application client and background. If you want to run the application again you will have to re-authenticate
+* user (username): gets information about the user connected to the specified username
+* get_tenants: gets a list of available tenants to connect to
+* get_tenant (tenant_id): get more detailed information about a specific tenant specified by the tenant id.
+* manpages: brings you to this page
+
+#### Creational
+These commands are for creating and updating Tapis services like pods and systems. These commands generally have lots of optional arguments for configuration, and forms to fill out. If you choose, in lieu of writing your configurations in the command line you can write and upload your own service config file from an application generated config file template. For all creational commands, you can do this by adding the argument `-f (path to your config file)`
+In the event that you do make a mistake while writing your config in the command line, your work is saved to a config file (the application will tell you where when this happens). When you fix the errors in the config file you can immediately re-upload it to try again.
+
+Creational commands include:
+* create_system
+* update_system
+* create_pod
+* update_pod
+* create_volume
+* update_volume
+* create_snapshot
+* update_snapshot
+* create_app
+* update_app
+* submit_job
+
+##### Generating Config Files
+WIP
+
+#### Managerial
+Managerial commands are generally for getting information about the Tapis services you have access to, managing permissions, state, and sharing for those services. These wont usually have more than 3 arguments. 
+
+### Services
+Each Tapis service has their own command group which allows you to interface with that service. Currently, TapisCLICICLE supports 7 services:
+* Systems
+* Files
+* Apps
+* Jobs
+* Pods
+* Volumes
+* Query
+
+#### Systems
+Systems lie at the core of most workflows in Tapis, and TapisCLICICLE. They are representations of your account on an HPC system, and interface with HPC resources using SSH. You can read more specifics about Tapis systems [here](https://tapis.readthedocs.io/en/latest/technical/systems.html). Systems enable the user to store and access files on as well as run jobs on that resource. 
+Each system has 4 key characteristics:
+* id: the identifier for the system
+* systemType: What type of system are you interfacing with? LINUX, IRODS, or GLOBUS
+* host: What is the hostname of the system you are trying to connect to? This can be anything that supports Tapis systems, whether it be a url or IP address. SOmething like stampede2.tacc.utexas.edu
+* defaultAuthnMethod: What authentication method will you use on this system?
+
+##### S3 Bucket Systems
+Tapis also supports interfacing with AWS S3 Bucket systems
 
-this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
-### Known Issues
-Since the application relies heavily on sockets to run properly, when they fail so does the application. If the application crashes frequently, or doesnt start, you should restart your computer, this should fix the issue. If it doesnt however, check the logs.log file, and create an issue on the github repo.
-The application has known compatibility issues with the WSL vpn due to its reliance on sockets. If you intend to use the application with WSL turn off your VPN. If the application doesnt work and you have a VPN on, turn it off just to make sure.
```

### Comparing `TapisCL-ICICLE-0.2.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,34 @@
 src/TapisCLICICLE/__init__.py
 src/TapisCLICICLE/__main__.py
 src/TapisCLICICLE/serverRun.py
 src/TapisCLICICLE/client/__init__.py
 src/TapisCLICICLE/client/cli.py
 src/TapisCLICICLE/client/handlers.py
 src/TapisCLICICLE/commands/__init__.py
-src/TapisCLICICLE/commands/appCommands.py
 src/TapisCLICICLE/commands/baseCommand.py
 src/TapisCLICICLE/commands/commandMap.py
 src/TapisCLICICLE/commands/commandOpts.py
 src/TapisCLICICLE/commands/dataFormatters.py
 src/TapisCLICICLE/commands/decorators.py
 src/TapisCLICICLE/commands/fileCommands.py
 src/TapisCLICICLE/commands/jobCommands.py
 src/TapisCLICICLE/commands/podCommands.py
 src/TapisCLICICLE/commands/serverCommands.py
-src/TapisCLICICLE/commands/systemCommands.py
 src/TapisCLICICLE/commands/volumeCommands.py
+src/TapisCLICICLE/commands/Apps/__init__.py
+src/TapisCLICICLE/commands/Apps/appCommands.py
+src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+src/TapisCLICICLE/commands/Apps/appForms.py
+src/TapisCLICICLE/commands/Systems/__init__.py
+src/TapisCLICICLE/commands/Systems/systemCommands.py
+src/TapisCLICICLE/commands/Systems/systemForms.py
 src/TapisCLICICLE/commands/arguments/__init__.py
 src/TapisCLICICLE/commands/arguments/argument.py
+src/TapisCLICICLE/commands/arguments/argumentValidators.py
 src/TapisCLICICLE/commands/query/__init__.py
 src/TapisCLICICLE/commands/query/neo4j.py
 src/TapisCLICICLE/commands/query/postgres.py
 src/TapisCLICICLE/server/__init__.py
 src/TapisCLICICLE/server/auth.py
 src/TapisCLICICLE/server/server.py
 src/TapisCLICICLE/socketopts/__init__.py
```

