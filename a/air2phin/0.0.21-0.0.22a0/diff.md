# Comparing `tmp/air2phin-0.0.21.tar.gz` & `tmp/air2phin-0.0.22a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air2phin-0.0.21.tar", last modified: Wed Mar 22 04:29:11 2023, max compression
+gzip compressed data, was "air2phin-0.0.22a0.tar", last modified: Tue Jul 18 11:06:33 2023, max compression
```

## Comparing `air2phin-0.0.21.tar` & `air2phin-0.0.22a0.tar`

### file list

```diff
@@ -1,68 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-03-22 04:29:11.039381 air2phin-0.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-03-22 04:28:58.000000 air2phin-0.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-22 04:29:11.043381 air2phin-0.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-22 04:28:58.000000 air2phin-0.0.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/air2phin/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/air2phin/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/air2phin/core/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/core/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/rules/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/rules/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/core/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/transformer/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/transformer/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/core/transformer/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/fake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/fake/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/core/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/core/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/fake/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/hooks/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/hooks/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/fake/models/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/models/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/fake/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/fake/utils/trigger_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/air2phin/rules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/rules/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/core/dagContext.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/rules/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/hooks/MySqlHook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/hooks/PostgresHook.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/rules/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/models/Variable.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/rules/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/operators/BashOperator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/operators/DummyOperator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/operators/PostgreOperator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/operators/PythonOperator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/operators/SparkSqlOperator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/rules/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/rules/utils/TriggerRule.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.039381 air2phin-0.0.21/src/air2phin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-22 04:28:58.000000 air2phin-0.0.21/src/air2phin/utils/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 04:29:11.035381 air2phin-0.0.21/src/air2phin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-22 04:29:11.000000 air2phin-0.0.21/src/air2phin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 04:29:10.000000 air2phin-0.0.21/src/air2phin.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.356608 air2phin-0.0.22a0/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-18 11:06:33.356712 air2phin-0.0.22a0/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-18 11:06:33.357114 air2phin-0.0.22a0/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.343706 air2phin-0.0.22a0/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.346038 air2phin-0.0.22a0/src/air2phin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-18 11:06:16.000000 air2phin-0.0.22a0/src/air2phin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.347539 air2phin-0.0.22a0/src/air2phin/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-17 08:44:50.000000 air2phin-0.0.22a0/src/air2phin/cli/command.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 03:54:45.000000 air2phin-0.0.22a0/src/air2phin/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.347699 air2phin-0.0.22a0/src/air2phin/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/core/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.348353 air2phin-0.0.22a0/src/air2phin/core/rules/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/core/rules/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    10532 2023-07-17 08:45:31.000000 air2phin-0.0.22a0/src/air2phin/core/rules/config.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/core/rules/loader.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.348902 air2phin-0.0.22a0/src/air2phin/core/transformer/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/core/transformer/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/core/transformer/imports.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-17 08:44:50.000000 air2phin-0.0.22a0/src/air2phin/core/transformer/operators.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 06:01:46.000000 air2phin-0.0.22a0/src/air2phin/core/transformer/route.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.349056 air2phin-0.0.22a0/src/air2phin/fake/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/fake/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.349408 air2phin-0.0.22a0/src/air2phin/fake/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/fake/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/fake/core/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9292 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/fake/core/hook.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.349787 air2phin-0.0.22a0/src/air2phin/fake/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/fake/hooks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/fake/hooks/mysql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/fake/hooks/postgres.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.350059 air2phin-0.0.22a0/src/air2phin/fake/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/src/air2phin/fake/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a0/src/air2phin/fake/models/variable.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.350279 air2phin-0.0.22a0/src/air2phin/fake/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/src/air2phin/fake/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/src/air2phin/fake/utils/trigger_rule.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.350536 air2phin-0.0.22a0/src/air2phin/patch/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-17 08:28:03.000000 air2phin-0.0.22a0/src/air2phin/patch/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1157 2023-07-18 09:46:40.000000 air2phin-0.0.22a0/src/air2phin/patch/marco_path.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.344901 air2phin-0.0.22a0/src/air2phin/rules/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.351123 air2phin-0.0.22a0/src/air2phin/rules/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 09:38:49.000000 air2phin-0.0.22a0/src/air2phin/rules/core/dagContext.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 09:38:16.000000 air2phin-0.0.22a0/src/air2phin/rules/core/removeModule.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.351718 air2phin-0.0.22a0/src/air2phin/rules/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/rules/hooks/MySqlHook.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/rules/hooks/PostgresHook.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.352043 air2phin-0.0.22a0/src/air2phin/rules/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/src/air2phin/rules/models/Variable.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.354968 air2phin-0.0.22a0/src/air2phin/rules/operators/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/BashOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/CheckOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/CommonSensor.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/DataSyncOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/DummyOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/FbiRefreshOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 09:43:32.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/PostgreOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 06:25:26.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/PythonOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 09:41:50.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/RedshiftOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a0/src/air2phin/rules/operators/SparkSqlOperator.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.355178 air2phin-0.0.22a0/src/air2phin/rules/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a0/src/air2phin/rules/utils/TriggerRule.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/runner.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.355828 air2phin-0.0.22a0/src/air2phin/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a0/src/air2phin/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-17 08:27:58.000000 air2phin-0.0.22a0/src/air2phin/utils/file.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.356095 air2phin-0.0.22a0/src/air2phin/utils/marco/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-17 09:02:06.000000 air2phin-0.0.22a0/src/air2phin/utils/marco/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.356486 air2phin-0.0.22a0/src/air2phin/utils/marco/convertor/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-17 09:04:59.000000 air2phin-0.0.22a0/src/air2phin/utils/marco/convertor/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1677 2023-07-18 09:46:39.000000 air2phin-0.0.22a0/src/air2phin/utils/marco/convertor/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 09:46:39.000000 air2phin-0.0.22a0/src/air2phin/utils/marco/convertor/calculate.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3636 2023-07-18 09:46:39.000000 air2phin-0.0.22a0/src/air2phin/utils/marco/helper.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 11:01:27.000000 air2phin-0.0.22a0/src/air2phin/utils/reshape.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 09:46:39.000000 air2phin-0.0.22a0/src/air2phin/utils/string.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 11:06:33.347030 air2phin-0.0.22a0/src/air2phin.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-18 11:06:33.000000 air2phin-0.0.22a0/src/air2phin.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a0/src/air2phin.egg-info/zip-safe
```

### Comparing `air2phin-0.0.21/PKG-INFO` & `air2phin-0.0.22a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.21
+Version: 0.0.22a0
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.21/README.md` & `air2phin-0.0.22a0/README.md`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/setup.cfg` & `air2phin-0.0.22a0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 	=src
 packages = 
 	find_namespace:
 install_requires = 
 	libcst
 	PyYaml
 	tqdm
+	croniter
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 air2phin = 
 	rules/**/*.yaml
```

### Comparing `air2phin-0.0.21/setup.py` & `air2phin-0.0.22a0/setup.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/__init__.py` & `air2phin-0.0.22a0/src/air2phin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 __project_name__ = "Air2phin"
-__version__ = "0.0.21"
+__version__ = "0.0.22a0"
```

### Comparing `air2phin-0.0.21/src/air2phin/cli/command.py` & `air2phin-0.0.22a0/src/air2phin/cli/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import difflib
 import logging
 import sys
 from pathlib import Path
 from typing import Dict, Sequence
 
 from air2phin import __project_name__, __version__
-from air2phin.constants import REGEXP, TOKEN
+from air2phin.constants import Regexp, Token
 from air2phin.core.rules.config import Config
 from air2phin.core.rules.loader import build_in_rules, path_rule
 from air2phin.runner import Runner
 from air2phin.utils.file import recurse_files
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger("air2phin")
@@ -26,14 +26,18 @@
         "exists migration.",
         "action": "store_true",
     },
     "verbose": {
         "action": "store_true",
         "help": "Show more verbose output.",
     },
+    "specific_arg": {
+        "help": "Whether to handle special variables.",
+        "action": "store_false",
+    },
 }
 
 
 def build_argparse() -> argparse.ArgumentParser:
     """Build argparse.ArgumentParser with specific configuration."""
     parser = argparse.ArgumentParser(
         prog="air2phin",
@@ -72,14 +76,19 @@
     )
     parser_test.add_argument(
         "-R",
         "--custom-only",
         **common_args["custom_only"],
     )
     parser_test.add_argument(
+        "-s",
+        "--specific-arg",
+        **common_args["specific_arg"],
+    )
+    parser_test.add_argument(
         "-d",
         "--diff",
         action="store_true",
         help=f"Prints diff of all the changes {__project_name__} would make.",
     )
     parser_test.add_argument(
         "stdin",
@@ -104,19 +113,24 @@
     )
     parser_migrate.add_argument(
         "-R",
         "--custom-only",
         **common_args["custom_only"],
     )
     parser_migrate.add_argument(
+        "-s",
+        "--specific-arg",
+        **common_args["specific_arg"],
+    )
+    parser_migrate.add_argument(
         "-I",
         "--include",
-        help=f"Include files based on conditions provided, default '{REGEXP.PATH_PYTHON}'",
+        help=f"Include files based on conditions provided, default '{Regexp.PATH_PYTHON}'",
         action="store",
-        default=REGEXP.PATH_PYTHON,
+        default=Regexp.PATH_PYTHON,
         type=str,
     )
     parser_migrate.add_argument(
         "-E",
         "--exclude",
         help="Exclude files based on conditions provided, without default value",
         action="store",
@@ -171,15 +185,15 @@
     customs_rules = []
     if hasattr(args, "custom_rules") and args.custom_rules:
         for rule in args.custom_rules:
             customs_rules.extend(recurse_files(rule))
     if logger.level <= logging.DEBUG and customs_rules:
         logger.debug(
             "This migration have custom rules:\n%s",
-            TOKEN.NEW_LINE.join((f"  {r}" for r in customs_rules)),
+            Token.NEW_LINE.join((f"  {r}" for r in customs_rules)),
         )
 
     if args.subcommand == "test":
         stdin = args.stdin
         config = Config(customs=customs_rules, customs_only=args.custom_only)
         runner = Runner(config)
```

### Comparing `air2phin-0.0.21/src/air2phin/constants.py` & `air2phin-0.0.22a0/src/air2phin/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-class TOKEN:
+class Token:
     """Constants token for air2phin."""
 
     QUESTION: str = "?"
     COMMA: str = ","
     POINT: str = "."
     SPACE: str = " "
     ZERO: str = "0"
     IMPORT: str = "import"
     STRING: str = "str"
     CODE: str = "code"
     NEW_LINE: str = "\n"
 
 
-class KEYWORD:
+class Keyword:
     """Constants keywords for air2phin."""
 
     MIGRATE_MARK: str = "-air2phin"
     WORKFLOW_SUBMIT: str = "submit"
+    WORKFLOW_MARCO_PATH_FMT: str = "PatchMarco({wf}).patch()"
     AIRFLOW_DAG_SCHEDULE: str = "schedule_interval"
     AIRFLOW_DAG: str = "airflow.DAG"
     AIRFLOW_DAG_SIMPLE: str = "DAG"
     DEFAULT_SCHEDULE: str = "0 0 0 * * ? *"
 
 
-class REGEXP:
+class Regexp:
     """Constants regular expression for air2phin."""
 
     PATH_YAML: str = "*.yaml"
     PATH_PYTHON: str = "*.py"
     PATH_ALL: str = "**/*"
 
 
-class CONFIG:
+class ConfigKey:
     """Constants config file for air2phin."""
 
     NAME: str = "name"
 
     EXAMPLE: str = "examples"
 
     MIGRATION: str = "migration"
@@ -52,12 +53,12 @@
 
     ARGUMENT: str = "arg"
     DEFAULT: str = "default"
     TYPE: str = "type"
     VALUE: str = "value"
 
 
-class NUMBER:
+class Number:
     """Constants number for air2phin."""
 
     SCHEDULE_TOTAL_NUM: int = 9
     SCHEDULE_SPACE_NUM: int = 4
```

### Comparing `air2phin-0.0.21/src/air2phin/core/__init__.py` & `air2phin-0.0.22a0/src/air2phin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/core/rules/config.py` & `air2phin-0.0.22a0/src/air2phin/core/rules/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List, NamedTuple, Optional
 
-from air2phin.constants import CONFIG, REGEXP, TOKEN
+from air2phin.constants import ConfigKey, Regexp, Token
 from air2phin.core.rules.loader import rule_calls, rule_imports
 from air2phin.utils.file import read_yaml, recurse_files
 
 logger = logging.getLogger("air2phin.config")
 
 
 class ParamDefaultConfig(NamedTuple):
@@ -30,15 +30,15 @@
 
 
 class ImportConfig(NamedTuple):
     """Import config."""
 
     replace: str
     add: List[str]
-    remove: List[str]
+    remove: bool
 
 
 class Config:
     """Configurations of air2phin, including all configs change behavior of air2phin.
 
     :param customs: User custom path of rules, will combine with build-in rules when :param:``customs_only``
         is False, will only use custom rules and ignore build-in rules when :param:``customs_only`` is True.
@@ -48,20 +48,22 @@
     :param calls: Build-in call rules path.
     """
 
     def __init__(
         self,
         customs: Optional[List[Path]] = None,
         customs_only: Optional[bool] = False,
+        handle_special_arg: Optional[bool] = False,
         inplace: Optional[bool] = False,
         imports: Optional[List[Path]] = rule_imports,
         calls: Optional[List[Path]] = rule_calls,
     ):
         self._customs = customs
         self.customs_only = customs_only
+        self.handle_special_arg = handle_special_arg
         if self.customs_only and not self._customs:
             raise ValueError(
                 "Argument `customs` not allow value None, when customs_only is True."
             )
         if self.customs_only:
             warnings.warn(
                 "Will only use customs rules to migration, will ignore built-in rules.",
@@ -122,58 +124,57 @@
         self._call_migrator = self.call_migrator()
         return self._call_migrator
 
     @staticmethod
     def _build_caller(
         src: str, dest: str, parameters: List[Dict[str, Any]]
     ) -> CallConfig:
+        replace = dict()
+        add = dict()
+        remove = []
+
+        if parameters:
+            for p in parameters:
+                if p[ConfigKey.ACTION] == ConfigKey.KW_REPLACE:
+                    replace[p[ConfigKey.SOURCE]] = p[ConfigKey.DESTINATION]
+                elif p[ConfigKey.ACTION] == ConfigKey.KW_ADD:
+                    add[p[ConfigKey.ARGUMENT]] = ParamDefaultConfig(
+                        type=p[ConfigKey.DEFAULT][ConfigKey.TYPE],
+                        value=p[ConfigKey.DEFAULT][ConfigKey.VALUE],
+                    )
+                elif p[ConfigKey.ACTION] == ConfigKey.KW_REMOVE:
+                    remove.append(p[ConfigKey.ARGUMENT])
+                else:
+                    raise ValueError(
+                        f"Unknown action type {p[ConfigKey.ACTION]} in {p}"
+                    )
+
         return CallConfig(
             long=dest,
-            short=dest.split(TOKEN.POINT)[-1],
+            short=dest.split(Token.POINT)[-1],
             src_long=src,
-            src_short=src.split(TOKEN.POINT)[-1],
-            replace={
-                p[CONFIG.SOURCE]: p[CONFIG.DESTINATION]
-                for p in parameters
-                if p[CONFIG.ACTION] == CONFIG.KW_REPLACE
-            }
-            if parameters
-            else dict(),
-            add={
-                p[CONFIG.ARGUMENT]: ParamDefaultConfig(
-                    type=p[CONFIG.DEFAULT][CONFIG.TYPE],
-                    value=p[CONFIG.DEFAULT][CONFIG.VALUE],
-                )
-                for p in parameters
-                if p[CONFIG.ACTION] == CONFIG.KW_ADD
-            }
-            if parameters
-            else dict(),
-            remove=[
-                p[CONFIG.ARGUMENT]
-                for p in parameters
-                if p[CONFIG.ACTION] == CONFIG.KW_REMOVE
-            ]
-            if parameters
-            else [],
+            src_short=src.split(Token.POINT)[-1],
+            replace=replace,
+            add=add,
+            remove=remove,
         )
 
     @staticmethod
     def get_module_action(
         migration: Dict[str, Any], action_type: str
     ) -> Optional[Dict[str, Any]]:
         """Get specific action type from rules.
 
         :param migration: Config Migration node.
         :param action_type: Action type, can be `add`, `remove`, `replace`.
         """
         actions = [
             action
-            for action in migration[CONFIG.MODULE]
-            if action[CONFIG.ACTION] == action_type
+            for action in migration[ConfigKey.MODULE]
+            if action[ConfigKey.ACTION] == action_type
         ]
         if len(actions) > 1:
             raise ValueError("Each type of action can only have one.")
         return actions[0] if actions else None
 
     @staticmethod
     def rules_override(rule_paths: List[Path]) -> List[Dict]:
@@ -182,95 +183,111 @@
         Use dict comprehension to overwrite built-in rules, if custom rules also have the same name rules,
         will use the latest rules pass to :class:`Config`.
         """
         rules_map = {}
 
         rule_files = []
         for path in rule_paths:
-            rule_files.extend(recurse_files(path, include=REGEXP.PATH_YAML))
+            rule_files.extend(recurse_files(path, include=Regexp.PATH_YAML))
 
         for filename in rule_files:
             content = read_yaml(filename)
-            rule_name = content.get(CONFIG.NAME)
+            rule_name = content.get(ConfigKey.NAME)
             if rule_name in rules_map:
                 logger.info(
                     "Rule name with %s will be override by file %s", rule_name, filename
                 )
             rules_map[rule_name] = content
         return list(rules_map.values())
 
     def call_migrator(self) -> Dict[str, CallConfig]:
         """Get all call migrator from rules."""
         migrator = {}
 
         for rule in self.rules_override(self.calls_path):
-            migration = rule[CONFIG.MIGRATION]
-            parameters = migration.get(CONFIG.PARAMETER, None)
-            replace = self.get_module_action(migration, CONFIG.KW_REPLACE)
-            src = replace[CONFIG.SOURCE]
-            dest = replace[CONFIG.DESTINATION]
+            migration = rule[ConfigKey.MIGRATION]
+            parameters = migration.get(ConfigKey.PARAMETER, None)
+            replace = self.get_module_action(migration, ConfigKey.KW_REPLACE)
+            if replace is None:
+                continue
+            src = replace[ConfigKey.SOURCE]
+            dest = replace[ConfigKey.DESTINATION]
 
             if isinstance(src, str):
                 migrator[src] = self._build_caller(src, dest, parameters)
             elif isinstance(src, list):
                 for inner_src in src:
                     migrator[inner_src] = self._build_caller(
                         inner_src, dest, parameters
                     )
             else:
                 raise RuntimeError("Invalid migration.module.src type: %s" % type(src))
         return migrator
 
     @staticmethod
-    def _build_replace_importer(action: Dict[str, Any]) -> str:
-        dest = action[CONFIG.DESTINATION]
-        module, asname = dest.rsplit(TOKEN.POINT, 1)
+    def _build_replace_importer(action: Dict[str, Any]) -> Optional[str]:
+        if action is None:
+            return None
+        dest = action[ConfigKey.DESTINATION]
+        module, asname = dest.rsplit(Token.POINT, 1)
         return f"from {module} import {asname}"
 
     @staticmethod
-    def _get_rp_add_action(action: Dict[str, Any]) -> Optional[List[str]]:
+    def _get_rp_add_action(action: Dict[str, Any]) -> List[str]:
         """Get replace and add action list from rules.
 
         :param action: Config migration module action.
         """
 
         def _build_import_statement(mod: str) -> str:
-            spec = mod.rsplit(TOKEN.POINT, 1)
+            spec = mod.rsplit(Token.POINT, 1)
             return f"from {spec[0]} import {spec[1]}"
 
         if action is None:
             return []
-        module = action[CONFIG.MODULE]
+        module = action[ConfigKey.MODULE]
         if isinstance(module, str):
             return [_build_import_statement(module)]
         elif isinstance(module, list):
             return [_build_import_statement(mod) for mod in module]
         else:
             raise RuntimeError(
                 "Invalid migration.module.action.module type: %s" % type(module)
             )
 
+    @staticmethod
+    def _build_remove_importer(action: Dict[str, Any]) -> bool:
+        if action is None or ConfigKey.MODULE not in action:
+            return False
+        return True
+
     def imp_migrator(self) -> Dict[str, ImportConfig]:
         """Get all import migrator from rules."""
         imps = {}
 
         for rule in self.rules_override(self.imports_path):
-            replace = self.get_module_action(rule[CONFIG.MIGRATION], CONFIG.KW_REPLACE)
-            add = self.get_module_action(rule[CONFIG.MIGRATION], CONFIG.KW_ADD)
-            remove = self.get_module_action(rule[CONFIG.MIGRATION], CONFIG.KW_REMOVE)
+            replace = self.get_module_action(
+                rule[ConfigKey.MIGRATION], ConfigKey.KW_REPLACE
+            )
+            add = self.get_module_action(rule[ConfigKey.MIGRATION], ConfigKey.KW_ADD)
+            remove = self.get_module_action(
+                rule[ConfigKey.MIGRATION], ConfigKey.KW_REMOVE
+            )
 
-            src = replace[CONFIG.SOURCE]
-            if isinstance(src, str):
-                imps[src] = ImportConfig(
+            qualname = (
+                replace[ConfigKey.SOURCE] if replace else remove[ConfigKey.MODULE]
+            )
+            if isinstance(qualname, str):
+                imps[qualname] = ImportConfig(
                     replace=self._build_replace_importer(replace),
                     add=self._get_rp_add_action(add),
-                    remove=self._get_rp_add_action(remove),
+                    remove=self._build_remove_importer(remove),
                 )
-            elif isinstance(src, list):
-                for inner_src in src:
+            elif isinstance(qualname, list):
+                for inner_src in qualname:
                     imps[inner_src] = ImportConfig(
                         replace=self._build_replace_importer(replace),
                         add=self._get_rp_add_action(add),
-                        remove=self._get_rp_add_action(remove),
+                        remove=self._build_remove_importer(remove),
                     )
 
         return imps
```

### Comparing `air2phin-0.0.21/src/air2phin/core/rules/loader.py` & `air2phin-0.0.22a0/src/air2phin/core/rules/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 project = Path(__file__).parent.parent.parent
 
 path_rule = project.joinpath("rules")
 path_operators = path_rule.joinpath("operators")
 path_hooks = path_rule.joinpath("hooks")
 path_models = path_rule.joinpath("models")
 path_utils = path_rule.joinpath("utils")
-path_dag_cnx = path_rule.joinpath("core", "dagContext.yaml")
+path_dag_cnx = path_rule.joinpath("core")
 
 rule_imports = [path_dag_cnx, path_operators, path_hooks, path_models, path_utils]
 
 rule_calls = [path_dag_cnx, path_operators, path_hooks, path_models]
 
 
 def build_in_rules() -> List[Path]:
```

### Comparing `air2phin-0.0.21/src/air2phin/core/transformer/imports.py` & `air2phin-0.0.22a0/src/air2phin/core/transformer/imports.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # under the License.
 from typing import Optional, Sequence, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import FlattenSentinel, RemovalSentinel
 
-from air2phin.constants import TOKEN
+from air2phin.constants import Token
 from air2phin.core.rules.config import Config, ImportConfig
 
 
 class ImportTransformer(cst.CSTTransformer):
     """CST Transformer for airflow operators."""
 
     def __init__(self, config: Config):
@@ -67,30 +67,37 @@
         if self.mod_ref is not None:
             src_full_refs = [
                 f"{self.mod_ref}.{class_name}" for class_name in self.class_names
             ]
 
             replaces = []
             adds = set()
+            remove = set()
             for full_ref in src_full_refs:
                 if full_ref in self.config.imports:
                     dest: ImportConfig = self.config.imports[full_ref]
+                    if dest.remove:
+                        remove.update(full_ref)
                     replaces.append(dest.replace)
                     adds.update(dest.add)
 
+            # remove remove statement
+            if remove:
+                return cst.RemoveFromParent()
+
             # get replace statement
             if len(replaces) == 0:
                 return updated_node
             elif len(replaces) == 1:
                 statement = replaces[0]
             else:
                 class_name_only = [
-                    stat.split(f" {TOKEN.IMPORT} ")[1] for stat in replaces[1:]
+                    stat.split(f" {Token.IMPORT} ")[1] for stat in replaces[1:]
                 ]
-                statement = f"{TOKEN.COMMA} ".join(replaces[:1] + class_name_only)
+                statement = f"{Token.COMMA} ".join(replaces[:1] + class_name_only)
 
             # Return replace and add statement
             # TODO, will use ; as separator of multiple statements, we should better use \n in the future
             return FlattenSentinel(
                 [
                     *[cst.parse_statement(add).body[0] for add in adds],
                     cst.parse_statement(statement).body[0],
```

### Comparing `air2phin-0.0.21/src/air2phin/core/transformer/operators.py` & `air2phin-0.0.22a0/src/air2phin/core/transformer/operators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from typing import Optional, Sequence, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import Arg, BaseExpression, FlattenSentinel, RemovalSentinel
 
-from air2phin.constants import KEYWORD, TOKEN
+from air2phin.constants import Keyword, Token
 from air2phin.core.rules.config import CallConfig, Config, ParamDefaultConfig
 from air2phin.utils import string
 
 
 class OpTransformer(cst.CSTTransformer):
     """CST Transformer for airflow operators.
 
@@ -54,33 +54,35 @@
     def match_call_name(self, node: cst.Call) -> bool:
         if m.matches(node.func, m.TypeOf(m.Name)):
             val = cst.ensure_type(node.func, cst.Name).value
         elif m.matches(node.func, m.TypeOf(m.Attribute)):
             val = cst.ensure_type(node.func, cst.Attribute).attr.value
         else:
             return True
-        return val in self.qualified_name.split(TOKEN.POINT)
+        return val in self.qualified_name.split(Token.POINT)
 
     def _handle_specific_args(self, node: cst.Arg) -> cst.Arg:
         """Handle specific args for custom rule.
 
         Including:
         * airflow.DAG.schedule_interval: migrate schedule value
         """
+        if self._config.handle_special_arg is False:
+            return node
         name = node.keyword.value
         if (
-            KEYWORD.AIRFLOW_DAG in self.qualified_name
-            and name == KEYWORD.AIRFLOW_DAG_SCHEDULE
+            Keyword.AIRFLOW_DAG in self.qualified_name
+            and name == Keyword.AIRFLOW_DAG_SCHEDULE
         ):
             if not m.matches(
                 node,
                 m.Arg(value=m.SimpleString()),
             ):
                 return node.with_changes(
-                    value=cst.SimpleString(f"'{KEYWORD.DEFAULT_SCHEDULE}'")
+                    value=cst.SimpleString(f"'{Keyword.DEFAULT_SCHEDULE}'")
                 )
 
             orig_value = cst.ensure_type(node.value, cst.SimpleString).value
             value = string.convert_schedule(orig_value.strip("'").strip('"'))
             return node.with_changes(value=cst.SimpleString(value=f"'{value}'"))
         return node
 
@@ -125,17 +127,17 @@
 
     def _handle_missing_default(self, nodes: Sequence[cst.Arg]) -> Sequence[cst.Arg]:
         mutable = list(nodes)
         one_of = copy.deepcopy(mutable[-1])
         for arg in self.config.add.keys():
             default: ParamDefaultConfig = self.config.add.get(arg)
 
-            if default.type == TOKEN.STRING:
+            if default.type == Token.STRING:
                 value = cst.SimpleString(value=f'"{default.value}"')
-            elif default.type == TOKEN.CODE:
+            elif default.type == Token.CODE:
                 value = cst.parse_expression(default.value)
             else:
                 raise NotImplementedError
             mutable.append(
                 one_of.with_changes(
                     value=value,
                     keyword=cst.Name(value=arg),
```

### Comparing `air2phin-0.0.21/src/air2phin/core/transformer/route.py` & `air2phin-0.0.22a0/src/air2phin/core/transformer/route.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from typing import List, Set, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst import BaseExpression, FlattenSentinel, RemovalSentinel, SimpleStatementLine
 from libcst.metadata import PositionProvider, QualifiedName, QualifiedNameProvider
 
-from air2phin.constants import KEYWORD
+from air2phin.constants import Keyword
 from air2phin.core.rules.config import Config
 from air2phin.core.transformer.imports import ImportTransformer
 from air2phin.core.transformer.operators import OpTransformer
 
 
 class Transformer(cst.CSTTransformer):
     """CST Transformer route class from airflow to dolphinscheduler-sdk-python.
@@ -86,15 +86,15 @@
         """Migrate from import statement."""
         return updated_node.visit(ImportTransformer(self.config))
 
     def leave_WithItem_asname(self, node: cst.WithItem) -> None:
         """Get airflow Dags alias names."""
         if m.matches(node.item, m.Call()) and m.matches(
             cst.ensure_type(node.item, cst.Call).func,
-            m.Name(value=KEYWORD.AIRFLOW_DAG_SIMPLE),
+            m.Name(value=Keyword.AIRFLOW_DAG_SIMPLE),
         ):
             self.workflow_alias.add(node.asname.name.value)
 
     def leave_Expr(
         self, original_node: cst.Expr, updated_node: cst.Expr
     ) -> Union[
         cst.BaseSmallStatement,
@@ -103,31 +103,38 @@
     ]:
         """Update workflow ``alias.submit()`` expr exits or not statement."""
         if m.matches(
             original_node.value,
             m.Call(
                 func=m.Attribute(
                     value=m.OneOf(*[m.Name(a) for a in self.workflow_alias]),
-                    attr=m.Name(KEYWORD.WORKFLOW_SUBMIT),
+                    attr=m.Name(Keyword.WORKFLOW_SUBMIT),
                 )
             ),
         ):
             self.have_submit_expr.add(original_node.value.func.value.value)
         return updated_node
 
     def _build_submit_exprs(self) -> List[SimpleStatementLine]:
         miss_alias = self.workflow_alias.difference(self.have_submit_expr)
         return [
-            cst.parse_statement(f"{alias}.{KEYWORD.WORKFLOW_SUBMIT}()")
+            cst.parse_statement(f"{alias}.{Keyword.WORKFLOW_SUBMIT}()")
             for alias in miss_alias
         ]
 
+    def _build_marco_path_exprs(self) -> List[SimpleStatementLine]:
+        return [
+            cst.parse_statement(Keyword.WORKFLOW_MARCO_PATH_FMT.format(wf=alias))
+            for alias in self.workflow_alias
+        ]
+
     def leave_Module(
         self, original_node: cst.Module, updated_node: cst.Module
     ) -> cst.Module:
         if self.have_submit_expr == self.workflow_alias:
             return updated_node
 
         # add submit expr when do not have
         body_with_submit = list(updated_node.body)
+        body_with_submit.extend(self._build_marco_path_exprs())
         body_with_submit.extend(self._build_submit_exprs())
         return updated_node.with_changes(body=body_with_submit)
```

### Comparing `air2phin-0.0.21/src/air2phin/fake/core/hook.py` & `air2phin-0.0.22a0/src/air2phin/fake/core/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from contextlib import closing
 from typing import Any, Callable, Iterable, Mapping, Optional, Tuple, Union
 
 import sqlparse
 from sqlalchemy import create_engine, text
 
-from air2phin.constants import TOKEN
+from air2phin.constants import Token
 from air2phin.fake.core.connection import Connection
 
 
 def fetch_all_handler(cursor) -> list[tuple] | None:
     """Handler for DbApiHook.run() to return results."""
     if cursor.description is not None:
         return cursor.fetchall()
@@ -78,16 +78,16 @@
             schema=pattern_match.get("database", None),
             login=data.get("user", None),
             password=data.get("password", None),
         )
 
     @staticmethod
     def _get_type_name(conn_id) -> Tuple[Any, str]:
-        if TOKEN.POINT in conn_id:
-            return conn_id.strip().split(TOKEN.POINT)
+        if Token.POINT in conn_id:
+            return conn_id.strip().split(Token.POINT)
         return None, conn_id.strip()
 
     @classmethod
     def _get_connection_params_from_env(
         cls, metadata_conn: str, conn_id: str
     ) -> Connection:
         sql_qry_type_name = (
@@ -115,15 +115,15 @@
         )
 
         datasource_type, datasource_name = cls._get_type_name(conn_id)
         engine = create_engine(metadata_conn, echo=True)
 
         with engine.connect() as conn:
             # conn_id not in format of datasource_type.datasource_name
-            if TOKEN.POINT not in conn_id:
+            if Token.POINT not in conn_id:
                 result_name = conn.execute(
                     text(sql_qry_name.format(name=datasource_name))
                 )
                 if result_name.rowcount == 0:
                     raise ValueError(
                         f"Connection {conn_id} not found in dolphinscheduler metadata database."
                     )
```

### Comparing `air2phin-0.0.21/src/air2phin/fake/hooks/mysql.py` & `air2phin-0.0.22a0/src/air2phin/fake/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/fake/hooks/postgres.py` & `air2phin-0.0.22a0/src/air2phin/fake/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/fake/models/variable.py` & `air2phin-0.0.22a0/src/air2phin/fake/models/variable.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/fake/utils/trigger_rule.py` & `air2phin-0.0.22a0/src/air2phin/fake/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/core/dagContext.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/core/dagContext.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -2,48 +2,53 @@
 description: The configuration for migrating airflow.DAG context to pydolphinscheduler workflow context.
 
 migration:
   module:
     - action: replace
       src: airflow.DAG
       dest: pydolphinscheduler.core.process_definition.ProcessDefinition
+    - action: add
+      module: air2phin.patch.marco_path.PatchMarco
   parameter:
     - action: replace
       src: dag_id
       dest: name
     - action: replace
       src: start_date
       dest: start_time
-    - action: replace
-      src: schedule_interval
-      dest: schedule
+    - action: add
+      arg: release_state
+      default: 
+        type: str
+        value: 'offline'
 
 examples:
   assign:
     description: |
       The example of migrating `airflow.DAG` declaration with assigned.
     src: |
       from airflow import DAG
       from datetime import datetime
   
       dag = DAG(
           dag_id='dag',
           description='DAG description',
           start_date=datetime(2020, 1, 1),
-          schedule_interval='5 4 * * *',
+          schedule_interval='0 5 4 * * ? *',
       )
     dest: |
-      from pydolphinscheduler.core.process_definition import ProcessDefinition
+      from air2phin.patch.marco_path import PatchMarco; from pydolphinscheduler.core.process_definition import ProcessDefinition
       from datetime import datetime
   
       dag = ProcessDefinition(
           name='dag',
           description='DAG description',
           start_time=datetime(2020, 1, 1),
-          schedule='0 5 4 * * ? *',
+          schedule_interval='0 5 4 * * ? *',
+      release_state="offline",
       )
   context:
     description: |
       The example of migrating `airflow.DAG` in context mode.
     src: |
       from airflow import DAG
       from datetime import datetime
@@ -52,18 +57,20 @@
           dag_id='dag',
           description='DAG description',
           start_date=datetime(2020, 1, 1),
           schedule_interval='@once',
       ) as dag:
           pass
     dest: |
-      from pydolphinscheduler.core.process_definition import ProcessDefinition
+      from air2phin.patch.marco_path import PatchMarco; from pydolphinscheduler.core.process_definition import ProcessDefinition
       from datetime import datetime
   
       with ProcessDefinition(
           name='dag',
           description='DAG description',
           start_time=datetime(2020, 1, 1),
-          schedule='0 0 0 * * ? *',
+          schedule_interval='@once',
+      release_state="offline",
       ) as dag:
           pass
+      PatchMarco(dag).patch()
       dag.submit()
```

### Comparing `air2phin-0.0.21/src/air2phin/rules/hooks/MySqlHook.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/hooks/MySqlHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/hooks/PostgresHook.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/hooks/PostgresHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/models/Variable.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/models/Variable.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/operators/BashOperator.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/operators/BashOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/operators/DummyOperator.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/operators/DummyOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/operators/PostgreOperator.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/operators/PostgreOperator.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 description: The configuration for migrating Airflow PostgresOperator to DolphinScheduler SQL task.
 
 migration:
   module:
     - action: replace
       src: airflow.providers.postgres.operators.postgres.PostgresOperator
       dest: pydolphinscheduler.tasks.sql.Sql
+    - action: add
+      module: pydolphinscheduler.resources_plugin.Local
   parameter:
     - action: replace
       src: task_id
       dest: name
     - action: replace
       src: postgres_conn_id
       dest: datasource_name
+    - action: add
+      arg: resource_plugin
+      default:
+        type: code
+        value: Local(prefix="/path/to/dir/")
 
 examples:
   bare_sql:
     description: |
       The example of migrating `airflow.providers.postgres.operators.postgres.PostgresOperator` with
       bare sql statement as parameter ``sql``.
     src: |
@@ -24,34 +31,36 @@
 
       task = PostgresOperator(
           task_id='postgres-sql',
           postgres_conn_id='postgres_default_conn',
           sql='select * from table',
       )
     dest: |
-      from pydolphinscheduler.tasks.sql import Sql
+      from pydolphinscheduler.resources_plugin import Local; from pydolphinscheduler.tasks.sql import Sql
 
       task = Sql(
           name='postgres-sql',
           datasource_name='postgres_default_conn',
           sql='select * from table',
+      resource_plugin=Local(prefix="/path/to/dir/"),
       )
   sql_file:
     description: |
       The example of migrating `airflow.operators.spark_sql_operator.SparkSqlOperator` with sql file as
       parameter ``sql``.
     src: |
       from airflow.providers.postgres.operators.postgres import PostgresOperator
 
       task = PostgresOperator(
           task_id='postgres-sql',
           postgres_conn_id='postgres_default_conn',
           sql='test.sql',
       )
     dest: |
-      from pydolphinscheduler.tasks.sql import Sql
+      from pydolphinscheduler.resources_plugin import Local; from pydolphinscheduler.tasks.sql import Sql
 
       task = Sql(
           name='postgres-sql',
           datasource_name='postgres_default_conn',
           sql='test.sql',
+      resource_plugin=Local(prefix="/path/to/dir/"),
       )
```

### Comparing `air2phin-0.0.21/src/air2phin/rules/operators/PythonOperator.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/operators/PythonOperator.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,24 @@
   parameter:
     - action: replace
       src: task_id
       dest: name
     - action: replace
       src: python_callable
       dest: definition
+    - action: add
+      arg: environment_name
+      default: 
+        type: str
+        value: airflow_migrate
+    - action: add
+      arg: resource_list
+      default: 
+        type: code
+        value: '["airflow"]'
 
 examples:
   python_operator:
     description: The example of migrating `airflow.operators.python_operator.PythonOperator`.
     src: |
       from airflow.operators.python_operator import PythonOperator
 
@@ -34,14 +44,16 @@
 
       def foo():
           print('Hello World!')
 
       task = Python(
           name='python',
           definition=foo,
+      environment_name="airflow_migrate",
+      resource_list=["airflow"],
       )
   nested_python:
     description: |
       The example of migrating `airflow.operators.python_operator.PythonOperator` with nested function in
       `python_callable`.
     src: |
       from airflow.operators.python_operator import PythonOperator
@@ -64,8 +76,10 @@
 
       def foo():
           bar()
 
       task = Python(
           name='python',
           definition=foo,
+      environment_name="airflow_migrate",
+      resource_list=["airflow"],
       )
```

### Comparing `air2phin-0.0.21/src/air2phin/rules/operators/SparkSqlOperator.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/operators/SparkSqlOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/rules/utils/TriggerRule.yaml` & `air2phin-0.0.22a0/src/air2phin/rules/utils/TriggerRule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.21/src/air2phin/runner.py` & `air2phin-0.0.22a0/src/air2phin/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from timeit import default_timer as timer
 from typing import List, Optional
 
 import libcst as cst
 from tqdm import tqdm
 
-from air2phin.constants import KEYWORD, TOKEN
+from air2phin.constants import Keyword, Token
 from air2phin.core.rules.config import Config
 from air2phin.core.transformer.route import Transformer
 from air2phin.utils.file import add_stem_suffix, read, write
 
 logger = logging.getLogger("air2phin.runner")
 
 
@@ -47,28 +47,28 @@
         start = timer()
         content = read(path)
         migrated = self.with_str(content)
 
         if self.config.inplace:
             write(path, migrated)
         else:
-            new_path = add_stem_suffix(path, KEYWORD.MIGRATE_MARK)
+            new_path = add_stem_suffix(path, Keyword.MIGRATE_MARK)
             write(new_path, migrated)
 
         logger.debug("End migrate file %s, elapsed time %.5fs", path, timer() - start)
 
     def with_files(self, paths: List[Path]) -> None:
         """Run air2phin with multiple files to dolphinscheduler python sdk definition.
 
         :param paths: Path of file you want to migrate.
         """
         logger.info("Start migrate files, total %d files scan.", len(paths))
         logger.debug(
             "Start migrate files, files contain:\n%s",
-            TOKEN.NEW_LINE.join((f"  {p}" for p in paths)),
+            Token.NEW_LINE.join((f"  {p}" for p in paths)),
         )
 
         start = timer()
         for file in tqdm(paths):
             self.with_file(file)
 
         logger.info(
@@ -85,15 +85,15 @@
         """
         logger.info(
             "Start multiple processing migrate files, total %d files scan.", len(paths)
         )
         logger.debug(
             "Start migrate files with processes number %d, files contain:\n%s",
             processes,
-            TOKEN.NEW_LINE.join((f"  {p}" for p in paths)),
+            Token.NEW_LINE.join((f"  {p}" for p in paths)),
         )
 
         start = timer()
         with Pool(processes) as pool:
             list(tqdm(pool.imap(self.with_file, paths), total=len(paths)))
 
         logger.debug(
```

### Comparing `air2phin-0.0.21/src/air2phin/utils/file.py` & `air2phin-0.0.22a0/src/air2phin/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import yaml
 
-from air2phin.constants import REGEXP
+from air2phin.constants import Regexp
 
 
 def read(path: Path) -> str:
     """Read content from path.
 
     :param path: Path to read content.
     """
@@ -50,15 +50,15 @@
     """
     stem, suffix = path.stem, path.suffix
     new_name = f"{stem}{suf}{suffix}"
     return path.with_name(new_name)
 
 
 def recurse_files(
-    path: Path, include: Optional[str] = REGEXP.PATH_ALL, exclude: Optional[str] = None
+    path: Path, include: Optional[str] = Regexp.PATH_ALL, exclude: Optional[str] = None
 ) -> List[Path]:
     """Recurse all match pattern files in path.
 
     :param path: file or directory path want to recurse.
     :param include: include match pattern in given path, default include all file in directory.
     :param exclude: include match pattern in given path, default None.
     """
```

### Comparing `air2phin-0.0.21/src/air2phin.egg-info/PKG-INFO` & `air2phin-0.0.22a0/src/air2phin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.21
+Version: 0.0.22a0
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.21/src/air2phin.egg-info/SOURCES.txt` & `air2phin-0.0.22a0/src/air2phin.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -28,20 +28,34 @@
 src/air2phin/fake/hooks/__init__.py
 src/air2phin/fake/hooks/mysql.py
 src/air2phin/fake/hooks/postgres.py
 src/air2phin/fake/models/__init__.py
 src/air2phin/fake/models/variable.py
 src/air2phin/fake/utils/__init__.py
 src/air2phin/fake/utils/trigger_rule.py
+src/air2phin/patch/__init__.py
+src/air2phin/patch/marco_path.py
 src/air2phin/rules/core/dagContext.yaml
+src/air2phin/rules/core/removeModule.yaml
 src/air2phin/rules/hooks/MySqlHook.yaml
 src/air2phin/rules/hooks/PostgresHook.yaml
 src/air2phin/rules/models/Variable.yaml
 src/air2phin/rules/operators/BashOperator.yaml
+src/air2phin/rules/operators/CheckOperator.yaml
+src/air2phin/rules/operators/CommonSensor.yaml
+src/air2phin/rules/operators/DataSyncOperator.yaml
 src/air2phin/rules/operators/DummyOperator.yaml
+src/air2phin/rules/operators/FbiRefreshOperator.yaml
 src/air2phin/rules/operators/PostgreOperator.yaml
 src/air2phin/rules/operators/PythonOperator.yaml
+src/air2phin/rules/operators/RedshiftOperator.yaml
 src/air2phin/rules/operators/SparkSqlOperator.yaml
 src/air2phin/rules/utils/TriggerRule.yaml
 src/air2phin/utils/__init__.py
 src/air2phin/utils/file.py
-src/air2phin/utils/string.py
+src/air2phin/utils/reshape.py
+src/air2phin/utils/string.py
+src/air2phin/utils/marco/__init__.py
+src/air2phin/utils/marco/helper.py
+src/air2phin/utils/marco/convertor/__init__.py
+src/air2phin/utils/marco/convertor/base.py
+src/air2phin/utils/marco/convertor/calculate.py
```

