# Comparing `tmp/botocore-a-la-carte-ec2-1.31.3.tar.gz` & `tmp/botocore-a-la-carte-ec2-1.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ec2-1.31.3.tar", last modified: Fri Jul 14 01:46:09 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ec2-1.31.4.tar", last modified: Tue Jul 18 01:55:09 2023, max compression
```

## Comparing `botocore-a-la-carte-ec2-1.31.3.tar` & `botocore-a-la-carte-ec2-1.31.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.242649 botocore-a-la-carte-ec2-1.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-14 01:46:09.242649 botocore-a-la-carte-ec2-1.31.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.226649 botocore-a-la-carte-ec2-1.31.3/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.226649 botocore-a-la-carte-ec2-1.31.3/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.226649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.230649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.230649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.230649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.230649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.234649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.234649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.238649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.242649 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)  2879802 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-14 01:45:45.000000 botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:46:09.242649 botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:46:09.242649 botocore-a-la-carte-ec2-1.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-14 01:46:09.000000 botocore-a-la-carte-ec2-1.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.928224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.932224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.932224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.932224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2880950 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-18 01:54:50.000000 botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:09.936224 botocore-a-la-carte-ec2-1.31.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-18 01:55:09.000000 botocore-a-la-carte-ec2-1.31.4/setup.py
```

### Comparing `botocore-a-la-carte-ec2-1.31.3/LICENSE.txt` & `botocore-a-la-carte-ec2-1.31.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.31.3
+Version: 1.31.4
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-09-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2014-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2014-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-03-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-04-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-04-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2015-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2015-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/examples-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-04-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-04-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-09-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-09-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998631155454106%*

 * *Differences: {"'shapes'": "{'AllowedInstanceType': {'pattern': '[a-zA-Z0-9\\\\.\\\\*\\\\-]+'}, "*

 * *             "'ExcludedInstanceType': {'pattern': '[a-zA-Z0-9\\\\.\\\\*\\\\-]+'}, "*

 * *             "'InstanceTypeInfo': {'members': {'NitroTpmSupport': OrderedDict([('shape', "*

 * *             "'NitroTpmSupport'), ('documentation', '<p>Indicates whether NitroTPM is "*

 * *             "supported.</p>'), ('locationName', 'nitroTpmSupport')]), 'NitroTpmInfo': "*

 * *             "OrderedDict([('shape', 'NitroTpmInfo'), ('documentation', '<p> […]*

```diff
@@ -9258,15 +9258,15 @@
                 "used"
             ],
             "type": "string"
         },
         "AllowedInstanceType": {
             "max": 30,
             "min": 1,
-            "pattern": "[a-zA-Z0-9\\.\\*]+",
+            "pattern": "[a-zA-Z0-9\\.\\*\\-]+",
             "type": "string"
         },
         "AllowedInstanceTypeSet": {
             "max": 400,
             "member": {
                 "locationName": "item",
                 "shape": "AllowedInstanceType"
@@ -29864,15 +29864,15 @@
                 "default"
             ],
             "type": "string"
         },
         "ExcludedInstanceType": {
             "max": 30,
             "min": 1,
-            "pattern": "[a-zA-Z0-9\\.\\*]+",
+            "pattern": "[a-zA-Z0-9\\.\\*\\-]+",
             "type": "string"
         },
         "ExcludedInstanceTypeSet": {
             "max": 400,
             "member": {
                 "locationName": "item",
                 "shape": "ExcludedInstanceType"
@@ -38246,14 +38246,24 @@
                     "shape": "NetworkInfo"
                 },
                 "NitroEnclavesSupport": {
                     "documentation": "<p>Indicates whether Nitro Enclaves is supported.</p>",
                     "locationName": "nitroEnclavesSupport",
                     "shape": "NitroEnclavesSupport"
                 },
+                "NitroTpmInfo": {
+                    "documentation": "<p>Describes the supported NitroTPM versions for the instance type.</p>",
+                    "locationName": "nitroTpmInfo",
+                    "shape": "NitroTpmInfo"
+                },
+                "NitroTpmSupport": {
+                    "documentation": "<p>Indicates whether NitroTPM is supported.</p>",
+                    "locationName": "nitroTpmSupport",
+                    "shape": "NitroTpmSupport"
+                },
                 "PlacementGroupInfo": {
                     "documentation": "<p>Describes the placement group settings for the instance type.</p>",
                     "locationName": "placementGroupInfo",
                     "shape": "PlacementGroupInfo"
                 },
                 "ProcessorInfo": {
                     "documentation": "<p>Describes the processor.</p>",
@@ -46744,14 +46754,42 @@
         "NitroEnclavesSupport": {
             "enum": [
                 "unsupported",
                 "supported"
             ],
             "type": "string"
         },
+        "NitroTpmInfo": {
+            "documentation": "<p>Describes the supported NitroTPM versions for the instance type.</p>",
+            "members": {
+                "SupportedVersions": {
+                    "documentation": "<p>Indicates the supported NitroTPM versions.</p>",
+                    "locationName": "supportedVersions",
+                    "shape": "NitroTpmSupportedVersionsList"
+                }
+            },
+            "type": "structure"
+        },
+        "NitroTpmSupport": {
+            "enum": [
+                "unsupported",
+                "supported"
+            ],
+            "type": "string"
+        },
+        "NitroTpmSupportedVersionType": {
+            "type": "string"
+        },
+        "NitroTpmSupportedVersionsList": {
+            "member": {
+                "locationName": "item",
+                "shape": "NitroTpmSupportedVersionType"
+            },
+            "type": "list"
+        },
         "OccurrenceDayRequestSet": {
             "member": {
                 "locationName": "OccurenceDay",
                 "shape": "Integer"
             },
             "type": "list"
         },
```

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore/data/ec2/2016-11-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.4/botocore/data/ec2/2016-11-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.31.3
+Version: 1.31.4
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.31.3/botocore_a_la_carte_ec2.egg-info/SOURCES.txt` & `botocore-a-la-carte-ec2-1.31.4/botocore_a_la_carte_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.3/setup.py` & `botocore-a-la-carte-ec2-1.31.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ec2',
-    version="1.31.3",
+    version="1.31.4",
     description='ec2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ec2/*/*.json'],
```

