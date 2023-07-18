# Comparing `tmp/torchqtm-0.2.0.tar.gz` & `tmp/torchqtm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchqtm-0.2.0.tar", last modified: Thu Jul 13 09:16:54 2023, max compression
+gzip compressed data, was "torchqtm-0.3.0.tar", last modified: Tue Jul 18 02:25:51 2023, max compression
```

## Comparing `torchqtm-0.2.0.tar` & `torchqtm-0.3.0.tar`

### file list

```diff
@@ -1,161 +1,165 @@
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.398827 torchqtm-0.2.0/
--rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-06-13 15:30:45.000000 torchqtm-0.2.0/LICENSE
--rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-13 09:16:54.398575 torchqtm-0.2.0/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     3547 2023-07-13 06:59:46.000000 torchqtm-0.2.0/README.md
--rw-r--r--   0 nymath     (501) staff       (20)       38 2023-07-13 09:16:54.398922 torchqtm-0.2.0/setup.cfg
--rw-r--r--   0 nymath     (501) staff       (20)     1418 2023-07-13 09:16:36.000000 torchqtm-0.2.0/setup.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.358359 torchqtm-0.2.0/test/
--rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testFunctional.py
--rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testRolling.py
--rw-r--r--   0 nymath     (501) staff       (20)        2 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/test_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testfunc_.py
--rw-r--r--   0 nymath     (501) staff       (20)     1865 2023-06-28 01:46:48.000000 torchqtm-0.2.0/test/testgplearn.py
--rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-13 15:30:46.000000 torchqtm-0.2.0/test/testop.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.359850 torchqtm-0.2.0/torchqtm/
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.362901 torchqtm-0.2.0/torchqtm/_C/
--rw-r--r--   0 nymath     (501) staff       (20)   108947 2023-07-13 02:19:26.000000 torchqtm-0.2.0/torchqtm/_C/__init__.c
--rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-27 12:01:02.000000 torchqtm-0.2.0/torchqtm/_C/__init__.cpp
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_C/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)   289603 2023-07-13 02:24:46.000000 torchqtm-0.2.0/torchqtm/_C/_functional.cpp
--rw-r--r--   0 nymath     (501) staff       (20)  1225596 2023-07-13 02:24:47.000000 torchqtm-0.2.0/torchqtm/_C/_rolling.cpp
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365194 torchqtm-0.2.0/torchqtm/_libs/
--rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365552 torchqtm-0.2.0/torchqtm/_libs/tslibs/
--rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/tslibs/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.365852 torchqtm-0.2.0/torchqtm/_libs/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/_libs/window/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368494 torchqtm-0.2.0/torchqtm/alphas/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    50043 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/alpha101.py
--rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/alphas.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368804 torchqtm-0.2.0/torchqtm/alphas/autoalpha/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.368910 torchqtm-0.2.0/torchqtm/alphas/autoalpha/boost/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/boost/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.369014 torchqtm-0.2.0/torchqtm/alphas/autoalpha/cnn/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/cnn/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371173 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/
--rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/_program.py
--rw-r--r--   0 nymath     (501) staff       (20)     6587 2023-06-26 08:02:51.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/fitness.py
--rw-r--r--   0 nymath     (501) staff       (20)     7231 2023-06-26 08:02:51.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/functions.py
--rw-r--r--   0 nymath     (501) staff       (20)    66960 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/genetic.py
--rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     1716 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/chatgpt.py
--rw-r--r--   0 nymath     (501) staff       (20)     1317 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/introduction.py
--rw-r--r--   0 nymath     (501) staff       (20)      700 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/ml.py
--rw-r--r--   0 nymath     (501) staff       (20)    28048 2023-06-19 13:01:39.000000 torchqtm-0.2.0/torchqtm/alphas/statistical.py
--rw-r--r--   0 nymath     (501) staff       (20)     9453 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/alphas/technical.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371553 torchqtm-0.2.0/torchqtm/assets/
--rw-r--r--   0 nymath     (501) staff       (20)       57 2023-07-04 07:03:05.000000 torchqtm-0.2.0/torchqtm/assets/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1430 2023-07-07 10:17:12.000000 torchqtm-0.2.0/torchqtm/assets/_assets.py
--rw-r--r--   0 nymath     (501) staff       (20)     6981 2023-06-19 12:57:55.000000 torchqtm-0.2.0/torchqtm/base.py
--rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/config.py
--rw-r--r--   0 nymath     (501) staff       (20)      337 2023-06-25 08:39:39.000000 torchqtm-0.2.0/torchqtm/configurator.py
--rw-r--r--   0 nymath     (501) staff       (20)     6957 2023-07-11 03:47:35.000000 torchqtm-0.2.0/torchqtm/constants.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.371783 torchqtm-0.2.0/torchqtm/core/
--rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/core/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.372036 torchqtm-0.2.0/torchqtm/core/window/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/core/window/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     6854 2023-07-11 09:25:38.000000 torchqtm-0.2.0/torchqtm/core/window/rolling.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.372842 torchqtm-0.2.0/torchqtm/data/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:11:51.000000 torchqtm-0.2.0/torchqtm/data/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     1477 2023-07-06 05:29:21.000000 torchqtm-0.2.0/torchqtm/data/bardata.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.373151 torchqtm-0.2.0/torchqtm/data/bundle/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-04 03:24:44.000000 torchqtm-0.2.0/torchqtm/data/bundle/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)       68 2023-07-04 03:26:41.000000 torchqtm-0.2.0/torchqtm/data/bundle/rqalpha.py
--rw-r--r--   0 nymath     (501) staff       (20)     7146 2023-07-13 06:47:38.000000 torchqtm-0.2.0/torchqtm/data/data_portal.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.374279 torchqtm-0.2.0/torchqtm/data/rq_data_source/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 10:32:43.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     3214 2023-07-04 09:31:26.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/adjust.py
--rw-r--r--   0 nymath     (501) staff       (20)    17792 2023-07-13 06:44:28.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/data_source.py
--rw-r--r--   0 nymath     (501) staff       (20)    13906 2023-07-04 09:22:00.000000 torchqtm-0.2.0/torchqtm/data/rq_data_source/readers.py
--rw-r--r--   0 nymath     (501) staff       (20)      885 2023-07-02 15:35:35.000000 torchqtm-0.2.0/torchqtm/data/sample.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.374540 torchqtm-0.2.0/torchqtm/derivatives/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:10:17.000000 torchqtm-0.2.0/torchqtm/derivatives/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.375073 torchqtm-0.2.0/torchqtm/derivatives/option/
--rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/Option.py
--rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.375426 torchqtm-0.2.0/torchqtm/derivatives/option/data/
--rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/data/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/data/load_data.py
--rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/derivatives/option/functional.py
--rw-r--r--   0 nymath     (501) staff       (20)      598 2023-06-19 14:11:23.000000 torchqtm-0.2.0/torchqtm/derivatives/option/main.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.376435 torchqtm-0.2.0/torchqtm/edbt/
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-27 14:16:32.000000 torchqtm-0.2.0/torchqtm/edbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    19847 2023-07-13 06:39:56.000000 torchqtm-0.2.0/torchqtm/edbt/algorithm.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.376771 torchqtm-0.2.0/torchqtm/edbt/gens/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:46:20.000000 torchqtm-0.2.0/torchqtm/edbt/gens/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2555 2023-07-11 09:33:34.000000 torchqtm-0.2.0/torchqtm/edbt/gens/sim_engine.py
--rw-r--r--   0 nymath     (501) staff       (20)     4761 2023-07-13 06:48:14.000000 torchqtm-0.2.0/torchqtm/edbt/run_algo.py
--rw-r--r--   0 nymath     (501) staff       (20)     3458 2023-07-11 05:26:20.000000 torchqtm-0.2.0/torchqtm/edbt/sim_params.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.378387 torchqtm-0.2.0/torchqtm/edbt/temp/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:29:06.000000 torchqtm-0.2.0/torchqtm/edbt/temp/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/account.py
--rw-r--r--   0 nymath     (501) staff       (20)     2269 2023-06-27 11:29:29.000000 torchqtm-0.2.0/torchqtm/edbt/temp/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/datahandler.py
--rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/setup.py
--rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-27 11:29:29.000000 torchqtm-0.2.0/torchqtm/edbt/temp/test.py
--rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/edbt/temp/testsearch.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.381879 torchqtm-0.2.0/torchqtm/finance/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 14:28:45.000000 torchqtm-0.2.0/torchqtm/finance/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)   381269 2023-07-13 03:01:39.000000 torchqtm-0.2.0/torchqtm/finance/_finance_ext.cpp
--rw-r--r--   0 nymath     (501) staff       (20)    14758 2023-07-13 05:54:26.000000 torchqtm-0.2.0/torchqtm/finance/account.py
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 02:21:33.000000 torchqtm-0.2.0/torchqtm/finance/finance_ext.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.382955 torchqtm-0.2.0/torchqtm/finance/metrics/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:15:11.000000 torchqtm-0.2.0/torchqtm/finance/metrics/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      143 2023-07-12 07:38:30.000000 torchqtm-0.2.0/torchqtm/finance/metrics/loader.py
--rw-r--r--   0 nymath     (501) staff       (20)     7566 2023-07-13 05:53:29.000000 torchqtm-0.2.0/torchqtm/finance/metrics/metric.py
--rw-r--r--   0 nymath     (501) staff       (20)     8929 2023-07-12 14:03:21.000000 torchqtm-0.2.0/torchqtm/finance/metrics/tracker.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.385124 torchqtm-0.2.0/torchqtm/finance/models/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:34.000000 torchqtm-0.2.0/torchqtm/finance/models/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      845 2023-07-12 01:43:27.000000 torchqtm-0.2.0/torchqtm/finance/models/cancel_policy.py
--rw-r--r--   0 nymath     (501) staff       (20)    11967 2023-07-11 02:59:21.000000 torchqtm-0.2.0/torchqtm/finance/models/commission.py
--rw-r--r--   0 nymath     (501) staff       (20)    20911 2023-07-13 06:01:13.000000 torchqtm-0.2.0/torchqtm/finance/models/slippage.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.388932 torchqtm-0.2.0/torchqtm/finance/orders/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:14:45.000000 torchqtm-0.2.0/torchqtm/finance/orders/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     8923 2023-07-12 08:40:39.000000 torchqtm-0.2.0/torchqtm/finance/orders/order.py
--rw-r--r--   0 nymath     (501) staff       (20)    15141 2023-07-13 06:13:29.000000 torchqtm-0.2.0/torchqtm/finance/orders/tracker.py
--rw-r--r--   0 nymath     (501) staff       (20)     2466 2023-07-06 10:00:32.000000 torchqtm-0.2.0/torchqtm/finance/portfolio.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.389870 torchqtm-0.2.0/torchqtm/finance/positions/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:19.000000 torchqtm-0.2.0/torchqtm/finance/positions/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)     3384 2023-07-12 06:15:32.000000 torchqtm-0.2.0/torchqtm/finance/positions/position.py
--rw-r--r--   0 nymath     (501) staff       (20)     7469 2023-07-13 05:14:10.000000 torchqtm-0.2.0/torchqtm/finance/positions/tracker.py
--rw-r--r--   0 nymath     (501) staff       (20)     1319 2023-07-06 07:02:43.000000 torchqtm-0.2.0/torchqtm/finance/transaction.py
--rw-r--r--   0 nymath     (501) staff       (20)     2566 2023-07-06 03:42:02.000000 torchqtm-0.2.0/torchqtm/finance/zp_math.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.392231 torchqtm-0.2.0/torchqtm/op/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/op/CrossSectionalOperators.py
--rw-r--r--   0 nymath     (501) staff       (20)      241 2023-06-19 12:58:39.000000 torchqtm-0.2.0/torchqtm/op/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/op/_numba.py
--rw-r--r--   0 nymath     (501) staff       (20)     1965 2023-06-19 12:23:32.000000 torchqtm-0.2.0/torchqtm/op/algos.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.392696 torchqtm-0.2.0/torchqtm/op/filters/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 13:07:06.000000 torchqtm-0.2.0/torchqtm/op/filters/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    21852 2023-07-07 03:49:36.000000 torchqtm-0.2.0/torchqtm/op/functional.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.393859 torchqtm-0.2.0/torchqtm/tdbt/
--rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/tdbt/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)    12045 2023-06-23 23:59:52.000000 torchqtm-0.2.0/torchqtm/tdbt/backtest.py
--rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/tdbt/dataset.py
--rw-r--r--   0 nymath     (501) staff       (20)     1779 2023-07-11 03:00:28.000000 torchqtm-0.2.0/torchqtm/types.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.394071 torchqtm-0.2.0/torchqtm/uniquant/
--rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/uniquant/__init__.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.398205 torchqtm-0.2.0/torchqtm/utils/
--rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/__init__.py
--rw-r--r--   0 nymath     (501) staff       (20)      431 2023-06-18 07:34:02.000000 torchqtm-0.2.0/torchqtm/utils/_decorators.py
--rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/benchmark.py
--rw-r--r--   0 nymath     (501) staff       (20)      219 2023-07-10 09:41:27.000000 torchqtm-0.2.0/torchqtm/utils/calendar_utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     1459 2023-07-12 02:05:09.000000 torchqtm-0.2.0/torchqtm/utils/datetime_utils.py
--rw-r--r--   0 nymath     (501) staff       (20)     9078 2023-07-11 05:35:03.000000 torchqtm-0.2.0/torchqtm/utils/exchange_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/rebalance.py
--rw-r--r--   0 nymath     (501) staff       (20)      114 2023-06-27 06:55:39.000000 torchqtm-0.2.0/torchqtm/utils/standards.py
--rw-r--r--   0 nymath     (501) staff       (20)     4248 2023-06-18 06:26:04.000000 torchqtm-0.2.0/torchqtm/utils/stats.py
--rw-r--r--   0 nymath     (501) staff       (20)      221 2023-07-04 05:59:26.000000 torchqtm-0.2.0/torchqtm/utils/trading_calendar.py
--rw-r--r--   0 nymath     (501) staff       (20)     1570 2023-07-06 16:31:56.000000 torchqtm-0.2.0/torchqtm/utils/universe.py
--rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/visualization.py
--rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-13 15:30:46.000000 torchqtm-0.2.0/torchqtm/utils/warnings.py
-drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-13 09:16:54.360611 torchqtm-0.2.0/torchqtm.egg-info/
--rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/PKG-INFO
--rw-r--r--   0 nymath     (501) staff       (20)     3794 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/SOURCES.txt
--rw-r--r--   0 nymath     (501) staff       (20)        1 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/dependency_links.txt
--rw-r--r--   0 nymath     (501) staff       (20)       44 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/requires.txt
--rw-r--r--   0 nymath     (501) staff       (20)        9 2023-07-13 09:16:54.000000 torchqtm-0.2.0/torchqtm.egg-info/top_level.txt
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.671337 torchqtm-0.3.0/
+-rw-r--r--   0 nymath     (501) staff       (20)     1063 2023-06-13 15:30:45.000000 torchqtm-0.3.0/LICENSE
+-rw-r--r--   0 nymath     (501) staff       (20)      107 2023-07-18 02:24:40.000000 torchqtm-0.3.0/MANIFEST.in
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-18 02:25:51.671124 torchqtm-0.3.0/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     3547 2023-07-13 06:59:46.000000 torchqtm-0.3.0/README.md
+-rw-r--r--   0 nymath     (501) staff       (20)       38 2023-07-18 02:25:51.671402 torchqtm-0.3.0/setup.cfg
+-rw-r--r--   0 nymath     (501) staff       (20)     1465 2023-07-18 02:25:28.000000 torchqtm-0.3.0/setup.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.614511 torchqtm-0.3.0/test/
+-rw-r--r--   0 nymath     (501) staff       (20)      505 2023-06-13 15:30:46.000000 torchqtm-0.3.0/test/testFunctional.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1216 2023-06-13 15:30:46.000000 torchqtm-0.3.0/test/testRolling.py
+-rw-r--r--   0 nymath     (501) staff       (20)        2 2023-06-13 15:30:46.000000 torchqtm-0.3.0/test/test_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)       93 2023-06-13 15:30:46.000000 torchqtm-0.3.0/test/testfunc_.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1865 2023-06-28 01:46:48.000000 torchqtm-0.3.0/test/testgplearn.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1660 2023-06-13 15:30:46.000000 torchqtm-0.3.0/test/testop.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.619202 torchqtm-0.3.0/torchqtm/
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.624333 torchqtm-0.3.0/torchqtm/_C/
+-rw-r--r--   0 nymath     (501) staff       (20)   108947 2023-07-13 02:19:26.000000 torchqtm-0.3.0/torchqtm/_C/__init__.c
+-rw-r--r--   0 nymath     (501) staff       (20)   109379 2023-06-27 12:01:02.000000 torchqtm-0.3.0/torchqtm/_C/__init__.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/_C/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   289603 2023-07-13 02:24:46.000000 torchqtm-0.3.0/torchqtm/_C/_functional.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)  1225596 2023-07-13 02:24:47.000000 torchqtm-0.3.0/torchqtm/_C/_rolling.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.626950 torchqtm-0.3.0/torchqtm/_libs/
+-rw-r--r--   0 nymath     (501) staff       (20)      323 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/_libs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.627351 torchqtm-0.3.0/torchqtm/_libs/tslibs/
+-rw-r--r--   0 nymath     (501) staff       (20)     1534 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/_libs/tslibs/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.627691 torchqtm-0.3.0/torchqtm/_libs/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/_libs/window/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.630638 torchqtm-0.3.0/torchqtm/alphas/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    50043 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/alpha101.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2093 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/alphas.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.631083 torchqtm-0.3.0/torchqtm/alphas/autoalpha/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.631194 torchqtm-0.3.0/torchqtm/alphas/autoalpha/boost/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/boost/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.631298 torchqtm-0.3.0/torchqtm/alphas/autoalpha/cnn/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/cnn/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.635191 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/
+-rw-r--r--   0 nymath     (501) staff       (20)      218 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    24986 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/_program.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6587 2023-06-26 08:02:51.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/fitness.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7231 2023-06-26 08:02:51.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/functions.py
+-rw-r--r--   0 nymath     (501) staff       (20)    66960 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/genetic.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2513 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1716 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/chatgpt.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1317 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/introduction.py
+-rw-r--r--   0 nymath     (501) staff       (20)      700 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/ml.py
+-rw-r--r--   0 nymath     (501) staff       (20)    28048 2023-06-19 13:01:39.000000 torchqtm-0.3.0/torchqtm/alphas/statistical.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9453 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/alphas/technical.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.635900 torchqtm-0.3.0/torchqtm/assets/
+-rw-r--r--   0 nymath     (501) staff       (20)       57 2023-07-04 07:03:05.000000 torchqtm-0.3.0/torchqtm/assets/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1430 2023-07-07 10:17:12.000000 torchqtm-0.3.0/torchqtm/assets/_assets.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6981 2023-06-19 12:57:55.000000 torchqtm-0.3.0/torchqtm/base.py
+-rw-r--r--   0 nymath     (501) staff       (20)      119 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/config.py
+-rw-r--r--   0 nymath     (501) staff       (20)      337 2023-06-25 08:39:39.000000 torchqtm-0.3.0/torchqtm/configurator.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6957 2023-07-11 03:47:35.000000 torchqtm-0.3.0/torchqtm/constants.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.636238 torchqtm-0.3.0/torchqtm/core/
+-rw-r--r--   0 nymath     (501) staff       (20)       47 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/core/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.636825 torchqtm-0.3.0/torchqtm/core/window/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/core/window/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     6854 2023-07-11 09:25:38.000000 torchqtm-0.3.0/torchqtm/core/window/rolling.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.638625 torchqtm-0.3.0/torchqtm/data/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:11:51.000000 torchqtm-0.3.0/torchqtm/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1477 2023-07-06 05:29:21.000000 torchqtm-0.3.0/torchqtm/data/bardata.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.639386 torchqtm-0.3.0/torchqtm/data/bundle/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-04 03:24:44.000000 torchqtm-0.3.0/torchqtm/data/bundle/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)       68 2023-07-04 03:26:41.000000 torchqtm-0.3.0/torchqtm/data/bundle/rqalpha.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7505 2023-07-14 10:02:40.000000 torchqtm-0.3.0/torchqtm/data/data_portal.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.640914 torchqtm-0.3.0/torchqtm/data/rq_data_source/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 10:32:43.000000 torchqtm-0.3.0/torchqtm/data/rq_data_source/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3214 2023-07-04 09:31:26.000000 torchqtm-0.3.0/torchqtm/data/rq_data_source/adjust.py
+-rw-r--r--   0 nymath     (501) staff       (20)    18443 2023-07-15 03:27:21.000000 torchqtm-0.3.0/torchqtm/data/rq_data_source/data_source.py
+-rw-r--r--   0 nymath     (501) staff       (20)    13906 2023-07-04 09:22:00.000000 torchqtm-0.3.0/torchqtm/data/rq_data_source/readers.py
+-rw-r--r--   0 nymath     (501) staff       (20)      885 2023-07-02 15:35:35.000000 torchqtm-0.3.0/torchqtm/data/sample.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.641638 torchqtm-0.3.0/torchqtm/derivatives/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 14:10:17.000000 torchqtm-0.3.0/torchqtm/derivatives/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.642800 torchqtm-0.3.0/torchqtm/derivatives/option/
+-rw-r--r--   0 nymath     (501) staff       (20)       45 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/derivatives/option/Option.py
+-rw-r--r--   0 nymath     (501) staff       (20)       97 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/derivatives/option/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.643373 torchqtm-0.3.0/torchqtm/derivatives/option/data/
+-rw-r--r--   0 nymath     (501) staff       (20)       40 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/derivatives/option/data/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      333 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/derivatives/option/data/load_data.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2698 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/derivatives/option/functional.py
+-rw-r--r--   0 nymath     (501) staff       (20)      598 2023-06-19 14:11:23.000000 torchqtm-0.3.0/torchqtm/derivatives/option/main.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.643821 torchqtm-0.3.0/torchqtm/dl/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-13 16:33:51.000000 torchqtm-0.3.0/torchqtm/dl/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2486 2023-07-13 16:56:24.000000 torchqtm-0.3.0/torchqtm/dl/data_loader.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.646113 torchqtm-0.3.0/torchqtm/edbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-06-27 14:16:32.000000 torchqtm-0.3.0/torchqtm/edbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    18994 2023-07-15 11:27:23.000000 torchqtm-0.3.0/torchqtm/edbt/algorithm.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.646982 torchqtm-0.3.0/torchqtm/edbt/gens/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:46:20.000000 torchqtm-0.3.0/torchqtm/edbt/gens/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2555 2023-07-11 09:33:34.000000 torchqtm-0.3.0/torchqtm/edbt/gens/sim_engine.py
+-rw-r--r--   0 nymath     (501) staff       (20)     5337 2023-07-15 18:05:12.000000 torchqtm-0.3.0/torchqtm/edbt/run_algo.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3458 2023-07-11 05:26:20.000000 torchqtm-0.3.0/torchqtm/edbt/sim_params.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.649453 torchqtm-0.3.0/torchqtm/edbt/temp/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 11:29:06.000000 torchqtm-0.3.0/torchqtm/edbt/temp/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2143 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/edbt/temp/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2269 2023-06-27 11:29:29.000000 torchqtm-0.3.0/torchqtm/edbt/temp/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7015 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/edbt/temp/datahandler.py
+-rw-r--r--   0 nymath     (501) staff       (20)      144 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/edbt/temp/setup.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3713 2023-06-27 11:29:29.000000 torchqtm-0.3.0/torchqtm/edbt/temp/test.py
+-rw-r--r--   0 nymath     (501) staff       (20)      187 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/edbt/temp/testsearch.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.655133 torchqtm-0.3.0/torchqtm/finance/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 14:28:45.000000 torchqtm-0.3.0/torchqtm/finance/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)   381269 2023-07-13 03:01:39.000000 torchqtm-0.3.0/torchqtm/finance/_finance_ext.cpp
+-rw-r--r--   0 nymath     (501) staff       (20)    14859 2023-07-15 09:27:50.000000 torchqtm-0.3.0/torchqtm/finance/account.py
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-07-02 02:21:33.000000 torchqtm-0.3.0/torchqtm/finance/finance_ext.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.657798 torchqtm-0.3.0/torchqtm/finance/metrics/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:15:11.000000 torchqtm-0.3.0/torchqtm/finance/metrics/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      143 2023-07-12 07:38:30.000000 torchqtm-0.3.0/torchqtm/finance/metrics/loader.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7566 2023-07-13 05:53:29.000000 torchqtm-0.3.0/torchqtm/finance/metrics/metric.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9674 2023-07-14 08:51:14.000000 torchqtm-0.3.0/torchqtm/finance/metrics/tracker.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.659840 torchqtm-0.3.0/torchqtm/finance/models/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:34.000000 torchqtm-0.3.0/torchqtm/finance/models/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      845 2023-07-12 01:43:27.000000 torchqtm-0.3.0/torchqtm/finance/models/cancel_policy.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11967 2023-07-11 02:59:21.000000 torchqtm-0.3.0/torchqtm/finance/models/commission.py
+-rw-r--r--   0 nymath     (501) staff       (20)    20911 2023-07-13 06:01:13.000000 torchqtm-0.3.0/torchqtm/finance/models/slippage.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.661386 torchqtm-0.3.0/torchqtm/finance/orders/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:14:45.000000 torchqtm-0.3.0/torchqtm/finance/orders/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     8923 2023-07-12 08:40:39.000000 torchqtm-0.3.0/torchqtm/finance/orders/order.py
+-rw-r--r--   0 nymath     (501) staff       (20)    15141 2023-07-13 06:13:29.000000 torchqtm-0.3.0/torchqtm/finance/orders/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2466 2023-07-06 10:00:32.000000 torchqtm-0.3.0/torchqtm/finance/portfolio.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.662458 torchqtm-0.3.0/torchqtm/finance/positions/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-27 18:16:19.000000 torchqtm-0.3.0/torchqtm/finance/positions/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)     3384 2023-07-12 06:15:32.000000 torchqtm-0.3.0/torchqtm/finance/positions/position.py
+-rw-r--r--   0 nymath     (501) staff       (20)     7633 2023-07-15 09:27:50.000000 torchqtm-0.3.0/torchqtm/finance/positions/tracker.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1319 2023-07-06 07:02:43.000000 torchqtm-0.3.0/torchqtm/finance/transaction.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2566 2023-07-06 03:42:02.000000 torchqtm-0.3.0/torchqtm/finance/zp_math.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.664370 torchqtm-0.3.0/torchqtm/op/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/op/CrossSectionalOperators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      241 2023-06-19 12:58:39.000000 torchqtm-0.3.0/torchqtm/op/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    11492 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/op/_numba.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1965 2023-06-19 12:23:32.000000 torchqtm-0.3.0/torchqtm/op/algos.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.664966 torchqtm-0.3.0/torchqtm/op/filters/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-19 13:07:06.000000 torchqtm-0.3.0/torchqtm/op/filters/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    21942 2023-07-13 13:31:23.000000 torchqtm-0.3.0/torchqtm/op/functional.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.665600 torchqtm-0.3.0/torchqtm/tdbt/
+-rw-r--r--   0 nymath     (501) staff       (20)        0 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/tdbt/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)    12045 2023-06-23 23:59:52.000000 torchqtm-0.3.0/torchqtm/tdbt/backtest.py
+-rw-r--r--   0 nymath     (501) staff       (20)      278 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/tdbt/dataset.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1779 2023-07-11 03:00:28.000000 torchqtm-0.3.0/torchqtm/types.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.665985 torchqtm-0.3.0/torchqtm/uniquant/
+-rw-r--r--   0 nymath     (501) staff       (20)       63 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/uniquant/__init__.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.670759 torchqtm-0.3.0/torchqtm/utils/
+-rw-r--r--   0 nymath     (501) staff       (20)      626 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/utils/__init__.py
+-rw-r--r--   0 nymath     (501) staff       (20)      431 2023-06-18 07:34:02.000000 torchqtm-0.3.0/torchqtm/utils/_decorators.py
+-rw-r--r--   0 nymath     (501) staff       (20)      997 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/utils/benchmark.py
+-rw-r--r--   0 nymath     (501) staff       (20)      219 2023-07-10 09:41:27.000000 torchqtm-0.3.0/torchqtm/utils/calendar_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1459 2023-07-12 02:05:09.000000 torchqtm-0.3.0/torchqtm/utils/datetime_utils.py
+-rw-r--r--   0 nymath     (501) staff       (20)     9078 2023-07-11 05:35:03.000000 torchqtm-0.3.0/torchqtm/utils/exchange_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2571 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/utils/rebalance.py
+-rw-r--r--   0 nymath     (501) staff       (20)      114 2023-06-27 06:55:39.000000 torchqtm-0.3.0/torchqtm/utils/standards.py
+-rw-r--r--   0 nymath     (501) staff       (20)     4248 2023-06-18 06:26:04.000000 torchqtm-0.3.0/torchqtm/utils/stats.py
+-rw-r--r--   0 nymath     (501) staff       (20)      221 2023-07-04 05:59:26.000000 torchqtm-0.3.0/torchqtm/utils/trading_calendar.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1570 2023-07-06 16:31:56.000000 torchqtm-0.3.0/torchqtm/utils/universe.py
+-rw-r--r--   0 nymath     (501) staff       (20)     1835 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/utils/visualization.py
+-rw-r--r--   0 nymath     (501) staff       (20)     2675 2023-06-13 15:30:46.000000 torchqtm-0.3.0/torchqtm/utils/warnings.py
+drwxr-xr-x   0 nymath     (501) staff       (20)        0 2023-07-18 02:25:51.620642 torchqtm-0.3.0/torchqtm.egg-info/
+-rw-r--r--   0 nymath     (501) staff       (20)     3984 2023-07-18 02:25:51.000000 torchqtm-0.3.0/torchqtm.egg-info/PKG-INFO
+-rw-r--r--   0 nymath     (501) staff       (20)     3857 2023-07-18 02:25:51.000000 torchqtm-0.3.0/torchqtm.egg-info/SOURCES.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        1 2023-07-18 02:25:51.000000 torchqtm-0.3.0/torchqtm.egg-info/dependency_links.txt
+-rw-r--r--   0 nymath     (501) staff       (20)       44 2023-07-18 02:25:51.000000 torchqtm-0.3.0/torchqtm.egg-info/requires.txt
+-rw-r--r--   0 nymath     (501) staff       (20)        9 2023-07-18 02:25:51.000000 torchqtm-0.3.0/torchqtm.egg-info/top_level.txt
```

### Comparing `torchqtm-0.2.0/LICENSE` & `torchqtm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/PKG-INFO` & `torchqtm-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.2.0
+Version: 0.3.0
 Summary: None
 Home-page: https://github.com/nymath/torchqtm
 Download-URL: https://github.com/nymath/torchqtm/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchqtm-0.2.0/README.md` & `torchqtm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/setup.py` & `torchqtm-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from distutils.core import setup
 from setuptools import find_packages
 from Cython.Build import cythonize
 import numpy
 import glob
+import platform
+
+PLATFORM = platform.system()
+
 
 extensions = glob.glob("torchqtm/_C/*.pyx")
 extensions.extend(glob.glob("torchqtm/window/*.pyx"))
 extensions.extend(glob.glob("torchqtm/finance/*.pyx"))
 
 install_requires = [
     'numpy',
@@ -17,15 +21,15 @@
 
 
 def main():
     setup(
         ext_modules=cythonize(extensions, annotate=True),
         include_dirs=[numpy.get_include()],
         name="torchqtm",
-        version="0.2.0",
+        version="0.3.0",
         author="ny",
         author_email="nymath@163.com",
         install_requires=install_requires,
         description="None",
         long_description=open('README.md', 'r').read(),
         long_description_content_type="text/markdown",
         url="https://github.com/nymath/torchqtm",
```

### Comparing `torchqtm-0.2.0/test/testRolling.py` & `torchqtm-0.3.0/test/testRolling.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/test/testgplearn.py` & `torchqtm-0.3.0/test/testgplearn.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/test/testop.py` & `torchqtm-0.3.0/test/testop.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/_C/__init__.c` & `torchqtm-0.3.0/torchqtm/_C/__init__.c`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/_C/__init__.cpp` & `torchqtm-0.3.0/torchqtm/_C/__init__.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/_C/_functional.cpp` & `torchqtm-0.3.0/torchqtm/_C/_functional.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/_C/_rolling.cpp` & `torchqtm-0.3.0/torchqtm/_C/_rolling.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/_libs/tslibs/__init__.py` & `torchqtm-0.3.0/torchqtm/_libs/tslibs/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/alpha101.py` & `torchqtm-0.3.0/torchqtm/alphas/alpha101.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/alphas.py` & `torchqtm-0.3.0/torchqtm/alphas/alphas.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/_program.py` & `torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/_program.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/fitness.py` & `torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/fitness.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/functions.py` & `torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/functions.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/genetic.py` & `torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/genetic.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/autoalpha/gplearn/utils.py` & `torchqtm-0.3.0/torchqtm/alphas/autoalpha/gplearn/utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/chatgpt.py` & `torchqtm-0.3.0/torchqtm/alphas/chatgpt.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/introduction.py` & `torchqtm-0.3.0/torchqtm/alphas/introduction.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/ml.py` & `torchqtm-0.3.0/torchqtm/alphas/ml.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/statistical.py` & `torchqtm-0.3.0/torchqtm/alphas/statistical.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/alphas/technical.py` & `torchqtm-0.3.0/torchqtm/alphas/technical.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/assets/_assets.py` & `torchqtm-0.3.0/torchqtm/assets/_assets.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/base.py` & `torchqtm-0.3.0/torchqtm/base.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/constants.py` & `torchqtm-0.3.0/torchqtm/constants.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/core/window/rolling.py` & `torchqtm-0.3.0/torchqtm/core/window/rolling.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/data/bardata.py` & `torchqtm-0.3.0/torchqtm/data/bardata.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/data/data_portal.py` & `torchqtm-0.3.0/torchqtm/data/data_portal.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,25 +212,34 @@
     ) -> pd.DataFrame:
         """
         不太明白
         """
     def history_bars(
             self,
             asset,
-            field,
+            fields,
             bar_count,
             frequency,
     ):
-        return self._data_source.history_true_bars(
-            asset=asset,
-            fields=field,
-            bar_count=bar_count,
-            frequency=frequency,
-            dt=self.current_dt,
-        )
+        if isinstance(fields, str):
+            return self._data_source._history_bars_single(
+                asset=asset,
+                field=fields,
+                bar_count=bar_count,
+                frequency=frequency,
+                dt=self.current_dt,
+            )
+        elif isinstance(fields, typing.Iterable):
+            return self._data_source._history_bars_many(
+                asset=asset,
+                fields=fields,
+                bar_count=bar_count,
+                frequency=frequency,
+                dt=self.current_dt,
+            )
 
     def _get_minute_window_data(self, assets, field, minutes_for_window):
         pass
 
     def _get_daily_window_data(self, assets, field, days_in_window, extra_slot=True):
         pass
```

### Comparing `torchqtm-0.2.0/torchqtm/data/rq_data_source/adjust.py` & `torchqtm-0.3.0/torchqtm/data/rq_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/data/rq_data_source/data_source.py` & `torchqtm-0.3.0/torchqtm/data/rq_data_source/data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,15 +191,16 @@
     #
     # def is_st_stock(self, order_book_id, dates):
     #     result = self._st_stock_days.contains(order_book_id, dates)
     #     return result if result is not None else [False] * len(dates)
 
     @lru_cache(None)
     def _all_day_bars_of(self, asset: Asset):
-        return self.daily_bar_readers[asset.type].ATTRIBUTES, self.daily_bar_readers[asset.type].load_data(asset.symbol)
+        return (self.daily_bar_readers[asset.type].ATTRIBUTES,
+                self.daily_bar_readers[asset.type].load_data(asset.symbol))
 
     @lru_cache(None)
     def _filtered_day_bars(self, asset: Asset):
         _, bars = self._all_day_bars_of(asset)
         return bars[bars['volume'] > 0]
 
     def get_bar(self, asset: Asset, dt: pd.Timestamp, frequency='1d') -> pd.DataFrame:
@@ -268,43 +269,65 @@
     #     df_bars = df_bars[-bar_count:]
     #     df_bars = df_bars.reset_index()
     #     df_bars['datetime'] = df_bars.apply(lambda x: np.uint64(convert_date_to_int(x['datetime'].date())), axis=1)
     #     df_bars = df_bars.set_index('datetime')
     #     bars = df_bars.to_records()
     #     return bars
 
-    def history_true_bars(
+    def _history_bars_single(
             self,
             asset,
-            fields,
+            field,
             bar_count,
             frequency,
             dt,
     ):
         if frequency != 'daily' and frequency != '1w':
             raise NotImplementedError
 
         else:
             attrs, bars = self._all_day_bars_of(asset)
 
         if len(bars) <= 0:
             return bars
 
         dt = np.uint64(convert_date_to_int(dt))
-        i = bars['datetime'].searchsorted(dt, side='right')
+        i = bars['datetime'].searchsorted(dt, side='right') - 1
         left = i - bar_count if i >= bar_count else 0
         bars = bars[left:i+1]
+        if isinstance(field, str) and field not in FIELDS_REQUIRE_ADJUSTMENT:
+            return bars if field is None else bars[field]
+        return bars[field]
+
+    def _history_bars_many(
+            self,
+            asset,
+            fields,
+            bar_count,
+            frequency,
+            dt,
+    ):
+        if frequency != 'daily' and frequency != '1w':
+            raise NotImplementedError
 
+        else:
+            attrs, bars = self._all_day_bars_of(asset)
+
+        if len(bars) <= 0:
+            return bars
+
+        dt = np.uint64(convert_date_to_int(dt))
+        i = bars['datetime'].searchsorted(dt, side='right') - 1
+        left = i + 1 - bar_count if i >= bar_count else 0
+        bars = bars[left:i+1]
+
+        pbars = pd.DataFrame(bars)
         if isinstance(fields, str) and fields not in FIELDS_REQUIRE_ADJUSTMENT:
             return bars if fields is None else bars[fields]
-
-        rlt = pd.DataFrame(bars)
-        rlt['datetime'] /= 1e6
-        rlt.index = pd.DatetimeIndex(rlt['datetime'].astype(int).astype(str))
-        return rlt[fields]
+        return bars[fields]
 
     def history_bars(
             self,
             asset: Asset,
             fields: List[str],
             bar_count: int,
             frequency: str,
```

### Comparing `torchqtm-0.2.0/torchqtm/data/rq_data_source/readers.py` & `torchqtm-0.3.0/torchqtm/data/rq_data_source/readers.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/data/sample.py` & `torchqtm-0.3.0/torchqtm/data/sample.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/derivatives/option/functional.py` & `torchqtm-0.3.0/torchqtm/derivatives/option/functional.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/derivatives/option/main.py` & `torchqtm-0.3.0/torchqtm/derivatives/option/main.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/algorithm.py` & `torchqtm-0.3.0/torchqtm/edbt/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from abc import ABCMeta, abstractmethod
 import datetime
 import logging
+import sys
 import pandas as pd
 import numpy as np
 
 from torchqtm.edbt.sim_params import SimulationParameters
 from torchqtm.finance.metrics.tracker import MetricsTracker
 from torchqtm.finance.orders.order import Order
 from torchqtm.finance.orders.tracker import OrdersTracker
 from torchqtm.assets import Asset, Equity, Future
 from torchqtm.data.data_portal import DataPortal
 from torchqtm.edbt.gens.sim_engine import DailySimulationClock, MinuteSimulationClock
 import typing
-from torchqtm.types import EVENT_TYPE, ASSET_TYPE
+from torchqtm.types import EVENT_TYPE, ASSET_TYPE, DATA_FREQUENCIES
 from torchqtm.finance.account import Account
 from torchqtm.utils.exchange_calendar import XSHGExchangeCalendar
 from torchqtm.utils.datetime_utils import DateTimeManager, DateTimeMixin
 
 
 class TradingAlgorithm(DateTimeMixin):
     _allow_setattr: bool = False
@@ -119,19 +120,19 @@
     def handle_data(self):
         pass
 
     def _handle_data(self):
         # self.rule.should_trigger(self.current_dt) # FIXME
         self.handle_data()
 
-    def analyze(self, perf):
+    def analyze(self):
         pass
 
-    def _analyze(self, perf):
-        self.analyze(perf)
+    def _analyze(self):
+        self.analyze()
 
     # def __repr__(self):
     #     pass
 
     def _create_sim_engine(self):
         self.on_dt_changed(self.sim_params.start_session)
 
@@ -379,16 +380,16 @@
         """
         order_id = order_param
         if isinstance(order_param, Order):
             order_id = order_param.id
         self.account.cancel(order_id)
 
     # the interface of data_portal
-    def history(self, symbol, field, bar_count, frequency):
-        self.data_portal.get_history_window(symbol, field, bar_count, frequency)
+    def history(self, asset, field, bar_count, frequency):
+        return self.data_portal.history_bars(asset, field, bar_count, frequency)
 
     def __repr__(self):
         template = """
 {class_name}(
 capital_base={capital_base},
 sim_params={sim_params},
 initialized={initialized},
@@ -430,18 +431,17 @@
         self.current_data = data_portal
         self.restrictions = restrictions
         self.sim_params = sim_params
         self.sim_engine = sim_engine
         self.benchmark_source = benchmark_source
 
     def on_bar(self, dt: pd.Timestamp):
-        # 调用的时间是15:00:00, 今晚下单, 明晚成交
+        # 15:00:00, order today, transact tomorrow
         self.set_dt(dt)
         self.algo.account.update_ledger()
-        # self.algo.on_dt_changed(dt)
 
         blotter = self.algo.account.orders_tracker
         new_transactions, new_commissions, closed_orders = blotter.get_transactions(self.current_data)
         blotter.prune_orders(closed_orders)
 
         for transaction in new_transactions:
             self.algo.account.handle_transaction(transaction)
@@ -459,17 +459,16 @@
         # 将new_order放入对应的数据结构中
         for new_order in new_orders:
             self.algo.account.handle_order(new_order)
 
     def on_session_start(self, dt: pd.Timestamp):
         """
         """
-        # 在半夜调用这个 00:00:00
+        # 00:00:00
         self.set_dt(dt)
-        # self.algo.on_dt_changed(dt)
 
         self.algo.metrics_tracker.handle_start_of_session(
             dt,
             self.algo.data_portal,
         )
 
     def on_session_end(self, dt):
@@ -492,14 +491,15 @@
         self.algo._before_trading_start()
 
     def on_exit(self):
         """
         Remove references to algo, data portal, et al to break cycles and ensure
         deterministic cleanup of these objects when the simulation finishes.
         """
+        self.algo.analyze()
         self.algo = None
         self.benchmark_source = None
         self.current_data = None
         self.data_portal = None
 
     def __iter__(self):
 
@@ -531,79 +531,56 @@
 
             def calculate_minute_capital_changes(dt):
                 return []
 
         event_bus = iter(self.sim_engine)
         while True:
             try:
-                dt, event = next(event_bus)  # 想想能不能改进为一个队列
-                if event == EVENT_TYPE.BAR:  # Bar event 产生于每天收盘, 也就是15:00:00
+                dt, event = next(event_bus)
+                if event == EVENT_TYPE.BAR:
                     self.on_bar(dt)
 
                 elif event == EVENT_TYPE.SESSION_START:
                     self.on_session_start(dt)
 
                 elif event == EVENT_TYPE.SESSION_END:
-                    positions = self.algo.account.positions
-                    execute_order_cancellation_policy()
-                    # TODO:
-                    # self.algo.validate_account_controls()
-                    yield self._get_daily_message(dt, self.algo, self.algo.metrics_tracker)
+                    yield self.on_session_end(dt)
 
                 elif event == EVENT_TYPE.MINUTE_START:
                     raise NotImplementedError
 
                 elif event == EVENT_TYPE.MINUTE_END:
                     raise NotImplementedError
 
                 elif event == EVENT_TYPE.BEFORE_TRADING_START:
                     self.on_before_trading_start(dt)
 
             except StopIteration:
                 break
 
+        print("\n")
+        self.on_exit()
+
     def _cleanup_expired_assets(self, dt, position_assets):
         """
         Clear out any assets that have expired before starting a new sim day.
 
         Performs two functions:
 
         1. Find all assets for which we have open get_orders and clears any get_orders whose aasets are
         on or after their auto_close_date.
 
         2. Find all assets for which we have positions and generates close_position events for any assets that have
         reached their auto_close_date.
         """
         pass
 
-    def _get_daily_message(self, dt, algo, metrics_tracker):
-        """
-        Get a perf message for the given datetime.
-        """
-        perf_message = metrics_tracker.handle_end_of_session(dt, self.data_portal)
-        perf_message["daily_perf"]["recorded_vars"] = algo.recorded_vars
-        return perf_message
-
-    def _get_minute_message(self, dt, algo, metrics_tracker):
-        """
-        Get a perf message for the given datetime
-        """
-        pass
-
-
-class TestAlgo(TradingAlgorithm):
-    def initialize(self):
-        pass
-
-    def before_trading_start(self):
-        pass
-
-    def handle_data(self):
-        self.history("000001.XSHE", "close", 10, "1d")
-
-    def analyze(self):
-        pass
-
+    def history(
+            self,
+            asset: Asset,
+            fields: typing.Union[str, typing.Iterable[str]],
+            bar_count: int,
+            frequency: DATA_FREQUENCIES,
+    ):
+        return self.data_portal.history_bars(asset, fields, bar_count, frequency)
 
-if __name__ == "__main__":
-    test = TestAlgo()
```

### Comparing `torchqtm-0.2.0/torchqtm/edbt/gens/sim_engine.py` & `torchqtm-0.3.0/torchqtm/edbt/gens/sim_engine.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/run_algo.py` & `torchqtm-0.3.0/torchqtm/edbt/run_algo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pandas as pd
 import typing
 
+import talib
+
 from torchqtm.edbt.algorithm import TradingAlgorithm
 from torchqtm.edbt.sim_params import SimulationParameters
 
 from torchqtm.finance.account import Account
 from torchqtm.finance.metrics.tracker import MetricsTracker
 from torchqtm.utils.calendar_utils import get_calendar
 from torchqtm.utils.datetime_utils import DateTimeManager
 from torchqtm.types import DATA_FREQUENCIES
 from torchqtm.data.data_portal import DataPortal
 from torchqtm.assets import Equity
 from torchqtm.finance.metrics.loader import DEFAULT_METRICS
+
+
 # Design a time machine
 
 
 class run_algo(object):
     def __init__(
             self,
             Algo: typing.Type[TradingAlgorithm],
@@ -87,51 +91,72 @@
         it = iter(algo.get_generator())
         while True:
             try:
                 next(it)
             except StopIteration:
                 break
 
-        print("Hello World")
-
 
 class TestAlgo(TradingAlgorithm):
     def initialize(self):
         self.safe_set_attr("sym", Equity("000001.XSHE"))
         self.safe_set_attr("count", 0)
 
     def before_trading_start(self):
         pass
 
     def handle_data(self):
-        if self.count == 0:
-            self.order(self.sym, 10000)
+        for i in range(300):
+            prices = self.history(self.sym, 'close', 21, "daily")
+
+        short_avg = talib.SMA(prices, 5)
+        long_avg = talib.SMA(prices, 20)
 
-        print("----------------------------------------------------")
-        print("current_dt", self.current_dt, self.data_portal.get_spot_value([self.sym], "close", self.current_dt, "daily"))
-        # print("orders", self.account.orders_tracker.data)
-        print("cash", self.account.ledger.cash)
-        self.data_portal.history_bars(self.sym, ["close"], 200, "daily")
-        print("portfolio_value", self.account.ledger.portfolio_value)
-        print("positions_value", self.account.ledger.positions_value)
-        print("returns", self.account.ledger.returns)
-        print(self.account.ledger.cash_flow)
-        self.count += 1
+        current_position = self.account.get_position(self.sym)
+        if short_avg[-1] - long_avg[-1] < 0 and short_avg[-2] - long_avg[-2] > 0 and current_position.amount > 0:
+            self.order(self.sym, -100)
+
+        if short_avg[-1] - long_avg[-1] > 0 and short_avg[-2] - long_avg[-2] < 0:
+            for i in range(100):
+                self.order(self.sym, 10)
 
     def analyze(self):
-        self.current_dt
+        print(self.account.ledger.cash)
+        print(self.account.ledger.portfolio_value)
+
+
+import sys
+
+
+def print_progress(progress):
+    '''
+    progress 是一个介于0和1之间的浮点数，代表当前进度
+    '''
+    bar_length = 50  # 进度条的长度，你可以根据自己的需求进行修改
+    assert 0 <= progress <= 1
+
+    # 计算已完成部分和未完成部分的长度
+    completed_length = int(bar_length * progress)
+    uncompleted_length = bar_length - completed_length
+
+    # 创建进度条字符串
+    progress_bar = '[' + '#' * completed_length + '-' * uncompleted_length + ']'
+
+    # 在同一行打印进度条和进度百分比
+    sys.stdout.write("\r" + progress_bar + ' {:.2f}%'.format(progress * 100))
+    sys.stdout.flush()
 
 
 if __name__ == "__main__":
     Algo = TestAlgo
     data_frequency: DATA_FREQUENCIES = "daily"
     capital_base = 1e6
     bundle = "rqalpha"
-    start = pd.Timestamp("20220101")
-    end = pd.Timestamp("20230101")
+    start = pd.Timestamp("20160101")
+    end = pd.Timestamp("20220101")
     output = None
     trading_calendar = None
     metrics_set = DEFAULT_METRICS
     local_namespace = None
     environ = None
     account_configs = None
     benchmark_spec = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torchqtm-0.2.0/torchqtm/edbt/sim_params.py` & `torchqtm-0.3.0/torchqtm/edbt/sim_params.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/temp/account.py` & `torchqtm-0.3.0/torchqtm/edbt/temp/account.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/temp/backtest.py` & `torchqtm-0.3.0/torchqtm/edbt/temp/backtest.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/temp/datahandler.py` & `torchqtm-0.3.0/torchqtm/edbt/temp/datahandler.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/edbt/temp/test.py` & `torchqtm-0.3.0/torchqtm/edbt/temp/test.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/_finance_ext.cpp` & `torchqtm-0.3.0/torchqtm/finance/_finance_ext.cpp`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/account.py` & `torchqtm-0.3.0/torchqtm/finance/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,7 +432,10 @@
     # def handle_end_of_session(
     #         self,
     #         dt: pd.Timestamp,
     #         data_portal: DataPortal,
     # ):
     #     self.sync_last_sale_price(dt, data_portal)
     #     self.end_of_session()
+
+    def get_position(self, asset: Asset):
+        return self.positions_tracker.get_position(asset)
```

### Comparing `torchqtm-0.2.0/torchqtm/finance/metrics/metric.py` & `torchqtm-0.3.0/torchqtm/finance/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/metrics/tracker.py` & `torchqtm-0.3.0/torchqtm/finance/metrics/tracker.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,40 @@
 
 from torchqtm.data.data_portal import DataPortal
 from torchqtm.finance.account import Account
 from torchqtm.finance.metrics.metric import Metric
 from torchqtm.utils.exchange_calendar import XSHGExchangeCalendar
 import numpy as np
 import pandas as pd
+import sys
 from torchqtm.types import DATA_FREQUENCIES
 
 log = logging.getLogger(__name__)
 import typing
 
 
+def print_progress(progress):
+    '''
+    progress 是一个介于0和1之间的浮点数，代表当前进度
+    '''
+    bar_length = 50  # 进度条的长度，你可以根据自己的需求进行修改
+    assert 0 <= progress <= 1
+
+    # 计算已完成部分和未完成部分的长度
+    completed_length = int(bar_length * progress)
+    uncompleted_length = bar_length - completed_length
+
+    # 创建进度条字符串
+    progress_bar = '[' + '#' * completed_length + '-' * uncompleted_length + ']'
+
+    # 在同一行打印进度条和进度百分比
+    sys.stdout.write("\r" + progress_bar + ' {:.2f}%'.format(progress * 100))
+    sys.stdout.flush()
+
+
 class MetricsTracker:
     """The algorithm's interface to the registered risk and performance metrics
 
     """
 
     def __init__(
             self,
@@ -243,14 +263,15 @@
         self.end_of_session(
             packet,
             self._account,
             completed_session,
             session_ix,
             data_portal,
         )
+        print_progress(self._progress())
         return packet
 
     def handle_simulation_end(self, data_portal: DataPortal):
         """When the simulation is complete, run the full period risk report
         and send it out on the results socket.
         """
         log.info(
@@ -267,8 +288,9 @@
             packet,
             self._account,
             self._trading_calendar,
             self._sessions,
             data_portal,
             self._benchmark_source,
         )
-        return packet
+        print_progress(1)
+        return packet
```

### Comparing `torchqtm-0.2.0/torchqtm/finance/models/cancel_policy.py` & `torchqtm-0.3.0/torchqtm/finance/models/cancel_policy.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/models/commission.py` & `torchqtm-0.3.0/torchqtm/finance/models/commission.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/models/slippage.py` & `torchqtm-0.3.0/torchqtm/finance/models/slippage.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/orders/order.py` & `torchqtm-0.3.0/torchqtm/finance/orders/order.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/orders/tracker.py` & `torchqtm-0.3.0/torchqtm/finance/orders/tracker.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/portfolio.py` & `torchqtm-0.3.0/torchqtm/finance/portfolio.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/positions/position.py` & `torchqtm-0.3.0/torchqtm/finance/positions/position.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/positions/tracker.py` & `torchqtm-0.3.0/torchqtm/finance/positions/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,20 @@
         # positions = self._positions_store
         #
         # for asset, position in self.positions.items():
         #     positions[asset] = position
         # TODO: 尽量只写
         return self.data
 
+    def get_position(self, asset: Asset) -> Position:
+        try:
+            return self.data[asset]
+        except KeyError:
+            return Position(asset)
+
     def get_position_list(self) -> typing.List[Position]:
         return [
             pos for asset, pos in self.data.items() if pos.amount != 0
         ]
 
     def sync_last_sale_price(
             self,
```

### Comparing `torchqtm-0.2.0/torchqtm/finance/transaction.py` & `torchqtm-0.3.0/torchqtm/finance/transaction.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/finance/zp_math.py` & `torchqtm-0.3.0/torchqtm/finance/zp_math.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/op/_numba.py` & `torchqtm-0.3.0/torchqtm/op/_numba.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/op/algos.py` & `torchqtm-0.3.0/torchqtm/op/algos.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/op/functional.py` & `torchqtm-0.3.0/torchqtm/op/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,18 @@
         return pd.DataFrame(aux_func(x.values, d), index=x.index, columns=x.columns)
 
 
 def ts_delay(x, d):
     if isinstance(x, pd.DataFrame) or isinstance(x, pd.Series):
         return x.shift(d)
     elif isinstance(x, np.ndarray):
-        return pd.DataFrame(x).shift(d).values
+        if len(x) == 2:
+            return pd.DataFrame(x).shift(d).values
+        else:
+            return pd.Series(x).shift(d).values
     else:
         raise TypeError("Input should be a pandas DataFrame, Series or a numpy ndarray.")
 
 
 def ts_delta(x, d):
     return sub(x, ts_delay(x, d))
```

### Comparing `torchqtm-0.2.0/torchqtm/tdbt/backtest.py` & `torchqtm-0.3.0/torchqtm/tdbt/backtest.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/types.py` & `torchqtm-0.3.0/torchqtm/types.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/__init__.py` & `torchqtm-0.3.0/torchqtm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/benchmark.py` & `torchqtm-0.3.0/torchqtm/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/datetime_utils.py` & `torchqtm-0.3.0/torchqtm/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/exchange_calendar.py` & `torchqtm-0.3.0/torchqtm/utils/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/rebalance.py` & `torchqtm-0.3.0/torchqtm/utils/rebalance.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/stats.py` & `torchqtm-0.3.0/torchqtm/utils/stats.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/universe.py` & `torchqtm-0.3.0/torchqtm/utils/universe.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/visualization.py` & `torchqtm-0.3.0/torchqtm/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm/utils/warnings.py` & `torchqtm-0.3.0/torchqtm/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `torchqtm-0.2.0/torchqtm.egg-info/PKG-INFO` & `torchqtm-0.3.0/torchqtm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchqtm
-Version: 0.2.0
+Version: 0.3.0
 Summary: None
 Home-page: https://github.com/nymath/torchqtm
 Download-URL: https://github.com/nymath/torchqtm/releases/tag/
 Author: ny
 Author-email: nymath@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `torchqtm-0.2.0/torchqtm.egg-info/SOURCES.txt` & `torchqtm-0.3.0/torchqtm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 test/testFunctional.py
 test/testRolling.py
 test/test_calendar.py
 test/testfunc_.py
 test/testgplearn.py
@@ -61,14 +62,16 @@
 torchqtm/derivatives/__init__.py
 torchqtm/derivatives/option/Option.py
 torchqtm/derivatives/option/__init__.py
 torchqtm/derivatives/option/functional.py
 torchqtm/derivatives/option/main.py
 torchqtm/derivatives/option/data/__init__.py
 torchqtm/derivatives/option/data/load_data.py
+torchqtm/dl/__init__.py
+torchqtm/dl/data_loader.py
 torchqtm/edbt/__init__.py
 torchqtm/edbt/algorithm.py
 torchqtm/edbt/run_algo.py
 torchqtm/edbt/sim_params.py
 torchqtm/edbt/gens/__init__.py
 torchqtm/edbt/gens/sim_engine.py
 torchqtm/edbt/temp/__init__.py
```

