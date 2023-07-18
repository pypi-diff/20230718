# Comparing `tmp/botocore-a-la-carte-cloudfront-1.31.3.tar.gz` & `tmp/botocore-a-la-carte-cloudfront-1.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cloudfront-1.31.3.tar", last modified: Fri Jul 14 01:45:51 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-cloudfront-1.31.4.tar", last modified: Tue Jul 18 01:54:55 2023, max compression
```

## Comparing `botocore-a-la-carte-cloudfront-1.31.3.tar` & `botocore-a-la-carte-cloudfront-1.31.4.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   144492 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147479 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.866469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147700 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   150842 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   154636 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   130784 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   133880 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   133424 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   148384 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.870468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   150982 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   151766 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   194806 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   197970 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   206093 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   264716 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.874468 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   267331 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   273141 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/
--rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   281937 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/
--rw-r--r--   0 runner    (1001) docker     (123)    52454 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 01:45:44.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   572390 2023-07-14 01:45:45.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 01:45:45.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:45:51.878469 botocore-a-la-carte-cloudfront-1.31.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-14 01:45:51.000000 botocore-a-la-carte-cloudfront-1.31.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.540150 botocore-a-la-carte-cloudfront-1.31.4/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.540150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.540150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   144492 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147479 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147700 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   150842 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:49.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   154636 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130784 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   133880 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.544150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   133424 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   148384 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   150982 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   151766 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   194806 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197970 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   206093 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.548150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   264716 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   267331 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   273141 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/
+-rw-r--r--   0 runner    (1001) docker     (123)    40823 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   281937 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    52454 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   572390 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-18 01:54:50.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:54:55.552150 botocore-a-la-carte-cloudfront-1.31.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-18 01:54:55.000000 botocore-a-la-carte-cloudfront-1.31.4/setup.py
```

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/LICENSE.txt` & `botocore-a-la-carte-cloudfront-1.31.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/PKG-INFO` & `botocore-a-la-carte-cloudfront-1.31.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudfront
-Version: 1.31.3
+Version: 1.31.4
 Summary: cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-05-31/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-05-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-10-21/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-10-21/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2014-11-06/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2014-11-06/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-04-17/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-04-17/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-07-27/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-07-27/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2015-09-17/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2015-09-17/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-13/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-13/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-01-28/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-01-28/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-01/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-08-20/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-08-20/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-07/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-07/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-09-29/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-09-29/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2016-11-25/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2016-11-25/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-03-25/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-03-25/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2017-10-30/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2017-10-30/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-06-18/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-06-18/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2018-11-05/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2018-11-05/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2019-03-26/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2019-03-26/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/paginators-1.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/service-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore/data/cloudfront/2020-05-31/waiters-2.json` & `botocore-a-la-carte-cloudfront-1.31.4/botocore/data/cloudfront/2020-05-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO` & `botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-cloudfront
-Version: 1.31.3
+Version: 1.31.4
 Summary: cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt` & `botocore-a-la-carte-cloudfront-1.31.4/botocore_a_la_carte_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-cloudfront-1.31.3/setup.py` & `botocore-a-la-carte-cloudfront-1.31.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-cloudfront',
-    version="1.31.3",
+    version="1.31.4",
     description='cloudfront data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/cloudfront/*/*.json'],
```

