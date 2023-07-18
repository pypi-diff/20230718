# Comparing `tmp/sharetop-1.4.5.tar.gz` & `tmp/sharetop-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.4.5.tar", last modified: Mon Jul  3 03:57:20 2023, max compression
+gzip compressed data, was "sharetop-2.4.5.tar", last modified: Tue Jul 18 11:58:10 2023, max compression
```

## Comparing `sharetop-1.4.5.tar` & `sharetop-2.4.5.tar`

### file list

```diff
@@ -1,90 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.513057 sharetop-1.4.5/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.4.5/LICENSE
--rw-rw-rw-   0        0        0    51232 2023-07-03 03:57:20.512673 sharetop-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    49753 2023-05-25 04:36:48.000000 sharetop-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 03:57:20.513057 sharetop-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.436267 sharetop-1.4.5/sharetop/
--rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-1.4.5/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-07-03 03:53:57.000000 sharetop-1.4.5/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.459158 sharetop-1.4.5/sharetop/api/
--rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-1.4.5/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.461390 sharetop-1.4.5/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.4.5/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4459 2023-07-03 03:12:50.000000 sharetop-1.4.5/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.465391 sharetop-1.4.5/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.4.5/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.470390 sharetop-1.4.5/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.4.5/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.4.5/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.4.5/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.4.5/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.472634 sharetop-1.4.5/sharetop/core/capital_flow/
--rw-rw-rw-   0        0        0      322 2023-05-25 04:33:54.000000 sharetop-1.4.5/sharetop/core/capital_flow/__init__.py
--rw-rw-rw-   0        0        0     6235 2023-05-25 04:36:48.000000 sharetop-1.4.5/sharetop/core/capital_flow/capital_flow_monitor.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.476972 sharetop-1.4.5/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.4.5/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     3721 2023-05-25 01:16:42.000000 sharetop-1.4.5/sharetop/core/common/common_base.py
--rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-1.4.5/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12268 2023-07-03 03:49:09.000000 sharetop-1.4.5/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.4.5/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.479539 sharetop-1.4.5/sharetop/core/country/
--rw-rw-rw-   0        0        0      101 2023-05-16 01:30:15.000000 sharetop-1.4.5/sharetop/core/country/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-1.4.5/sharetop/core/country/config.py
--rw-rw-rw-   0        0        0      506 2023-07-03 01:12:16.000000 sharetop-1.4.5/sharetop/core/country/country_base_info.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.490394 sharetop-1.4.5/sharetop/core/fund/
--rw-rw-rw-   0        0        0      931 2023-05-03 07:19:55.000000 sharetop-1.4.5/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.4.5/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0    12687 2023-05-03 07:31:14.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_rank.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.4.5/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.4.5/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.491346 sharetop-1.4.5/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.4.5/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.4.5/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.494346 sharetop-1.4.5/sharetop/core/oil/
--rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/oil/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-1.4.5/sharetop/core/oil/config.py
--rw-rw-rw-   0        0        0     2970 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/oil/oil_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.496728 sharetop-1.4.5/sharetop/core/pig/
--rw-rw-rw-   0        0        0       76 2023-05-16 01:17:51.000000 sharetop-1.4.5/sharetop/core/pig/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-1.4.5/sharetop/core/pig/config.py
--rw-rw-rw-   0        0        0     1127 2023-05-16 00:59:27.000000 sharetop-1.4.5/sharetop/core/pig/pig_detail.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.503658 sharetop-1.4.5/sharetop/core/stock/
--rw-rw-rw-   0        0        0      453 2023-05-18 12:23:41.000000 sharetop-1.4.5/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.4.5/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.4.5/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14368 2023-05-04 12:15:59.000000 sharetop-1.4.5/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.4.5/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.4.5/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0      377 2023-05-02 14:39:20.000000 sharetop-1.4.5/sharetop/core/stock/stock_base_info.py
--rw-rw-rw-   0        0        0     6349 2023-05-04 04:01:07.000000 sharetop-1.4.5/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.505673 sharetop-1.4.5/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.4.5/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      861 2023-05-11 04:25:42.000000 sharetop-1.4.5/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     3298 2023-05-24 14:55:28.000000 sharetop-1.4.5/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.506672 sharetop-1.4.5/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.4.5/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0     4239 2023-05-23 12:33:52.000000 sharetop-1.4.5/sharetop/parser/base.py
--rw-rw-rw-   0        0        0     2906 2023-05-19 00:08:10.000000 sharetop-1.4.5/sharetop/parser/config.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.511672 sharetop-1.4.5/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.4.5/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-1.4.5/sharetop/test/captial.py
--rw-rw-rw-   0        0        0      336 2023-07-03 03:45:37.000000 sharetop-1.4.5/sharetop/test/test1.py
--rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-1.4.5/sharetop/test/test2-akshare.py
--rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-1.4.5/sharetop/test/test3.py
--rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-1.4.5/sharetop/test/test4.py
--rw-rw-rw-   0        0        0      643 2023-05-24 14:56:05.000000 sharetop-1.4.5/sharetop/test/test5.py
--rw-rw-rw-   0        0        0      860 2023-06-04 02:11:02.000000 sharetop-1.4.5/sharetop/test/test6.py
-drwxrwxrwx   0        0        0        0 2023-07-03 03:57:20.457651 sharetop-1.4.5/sharetop.egg-info/
--rw-rw-rw-   0        0        0    51232 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2165 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-03 03:57:20.000000 sharetop-1.4.5/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.213199 sharetop-2.4.5/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0    51253 2023-07-18 11:58:10.212184 sharetop-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0    49774 2023-07-15 03:35:16.000000 sharetop-2.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:58:10.214185 sharetop-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.275451 sharetop-2.4.5/sharetop/
+-rw-rw-rw-   0        0        0      297 2023-05-18 12:23:41.000000 sharetop-2.4.5/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-07-18 11:57:20.000000 sharetop-2.4.5/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.337640 sharetop-2.4.5/sharetop/api/
+-rw-rw-rw-   0        0        0      306 2023-07-02 13:11:41.000000 sharetop-2.4.5/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.363930 sharetop-2.4.5/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-2.4.5/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4459 2023-07-16 22:42:50.000000 sharetop-2.4.5/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.403177 sharetop-2.4.5/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-2.4.5/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.485378 sharetop-2.4.5/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      592 2023-07-15 11:00:24.000000 sharetop-2.4.5/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-2.4.5/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9571 2023-07-16 01:28:38.000000 sharetop-2.4.5/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19614 2023-07-15 10:59:53.000000 sharetop-2.4.5/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-2.4.5/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.514515 sharetop-2.4.5/sharetop/core/capital_flow/
+-rw-rw-rw-   0        0        0      367 2023-07-15 15:19:38.000000 sharetop-2.4.5/sharetop/core/capital_flow/__init__.py
+-rw-rw-rw-   0        0        0     6356 2023-07-15 15:19:38.000000 sharetop-2.4.5/sharetop/core/capital_flow/capital_flow_monitor.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.574929 sharetop-2.4.5/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-2.4.5/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     3727 2023-07-15 09:06:11.000000 sharetop-2.4.5/sharetop/core/common/common_base.py
+-rw-rw-rw-   0        0        0     8688 2023-05-25 01:16:42.000000 sharetop-2.4.5/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12428 2023-07-16 01:53:16.000000 sharetop-2.4.5/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-2.4.5/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.614658 sharetop-2.4.5/sharetop/core/country/
+-rw-rw-rw-   0        0        0       91 2023-07-16 02:39:07.000000 sharetop-2.4.5/sharetop/core/country/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-09 01:30:20.000000 sharetop-2.4.5/sharetop/core/country/config.py
+-rw-rw-rw-   0        0        0      697 2023-07-16 02:39:07.000000 sharetop-2.4.5/sharetop/core/country/country_base_info.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.780117 sharetop-2.4.5/sharetop/core/fund/
+-rw-rw-rw-   0        0        0     1017 2023-07-15 10:39:55.000000 sharetop-2.4.5/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      904 2023-07-07 04:55:12.000000 sharetop-2.4.5/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2593 2023-07-06 01:13:48.000000 sharetop-2.4.5/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1694 2023-07-15 09:54:03.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2490 2023-07-15 10:09:17.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3716 2023-07-15 10:12:05.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5474 2023-07-15 10:19:50.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0    12057 2023-07-15 10:32:02.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_rank.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-2.4.5/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2497 2023-07-15 10:37:11.000000 sharetop-2.4.5/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2451 2023-07-15 10:39:55.000000 sharetop-2.4.5/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.808215 sharetop-2.4.5/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      250 2023-07-16 02:07:46.000000 sharetop-2.4.5/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0    10057 2023-07-16 02:09:22.000000 sharetop-2.4.5/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.842958 sharetop-2.4.5/sharetop/core/oil/
+-rw-rw-rw-   0        0        0      402 2023-05-16 01:17:51.000000 sharetop-2.4.5/sharetop/core/oil/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-05-15 00:28:25.000000 sharetop-2.4.5/sharetop/core/oil/config.py
+-rw-rw-rw-   0        0        0     3614 2023-07-10 00:25:56.000000 sharetop-2.4.5/sharetop/core/oil/oil_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.877195 sharetop-2.4.5/sharetop/core/pig/
+-rw-rw-rw-   0        0        0       84 2023-07-15 10:46:51.000000 sharetop-2.4.5/sharetop/core/pig/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-16 00:42:46.000000 sharetop-2.4.5/sharetop/core/pig/config.py
+-rw-rw-rw-   0        0        0     1428 2023-07-15 10:46:51.000000 sharetop-2.4.5/sharetop/core/pig/pig_detail.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.964515 sharetop-2.4.5/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      662 2023-07-15 09:27:19.000000 sharetop-2.4.5/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4705 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1924 2023-07-17 00:35:01.000000 sharetop-2.4.5/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14859 2023-07-17 00:49:08.000000 sharetop-2.4.5/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10345 2023-07-15 08:48:35.000000 sharetop-2.4.5/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10130 2023-07-15 08:58:53.000000 sharetop-2.4.5/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0      520 2023-07-10 12:22:58.000000 sharetop-2.4.5/sharetop/core/stock/stock_base_info.py
+-rw-rw-rw-   0        0        0     7299 2023-07-10 03:31:49.000000 sharetop-2.4.5/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.004552 sharetop-2.4.5/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-2.4.5/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0     1088 2023-07-16 09:52:34.000000 sharetop-2.4.5/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     3271 2023-07-09 23:57:40.000000 sharetop-2.4.5/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.034783 sharetop-2.4.5/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-2.4.5/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0     4239 2023-05-23 12:33:52.000000 sharetop-2.4.5/sharetop/parser/base.py
+-rw-rw-rw-   0        0        0     2906 2023-05-19 00:08:10.000000 sharetop-2.4.5/sharetop/parser/config.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:10.211184 sharetop-2.4.5/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-2.4.5/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      432 2023-07-16 01:29:33.000000 sharetop-2.4.5/sharetop/test/bond_test.py
+-rw-rw-rw-   0        0        0      199 2023-05-17 04:49:54.000000 sharetop-2.4.5/sharetop/test/captial.py
+-rw-rw-rw-   0        0        0      172 2023-07-16 02:38:09.000000 sharetop-2.4.5/sharetop/test/country_test.py
+-rw-rw-rw-   0        0        0      523 2023-07-15 15:16:22.000000 sharetop-2.4.5/sharetop/test/flow_monitor_test.py
+-rw-rw-rw-   0        0        0     1450 2023-07-16 01:04:05.000000 sharetop-2.4.5/sharetop/test/fund_test.py
+-rw-rw-rw-   0        0        0      382 2023-07-16 02:09:22.000000 sharetop-2.4.5/sharetop/test/futures_test.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 00:25:56.000000 sharetop-2.4.5/sharetop/test/oil_test.py
+-rw-rw-rw-   0        0        0      198 2023-07-15 10:47:58.000000 sharetop-2.4.5/sharetop/test/pig_test.py
+-rw-rw-rw-   0        0        0     1318 2023-07-18 04:55:00.000000 sharetop-2.4.5/sharetop/test/stock_test.py
+-rw-rw-rw-   0        0        0      992 2023-07-17 01:23:58.000000 sharetop-2.4.5/sharetop/test/test1.py
+-rw-rw-rw-   0        0        0     1997 2023-05-02 03:48:40.000000 sharetop-2.4.5/sharetop/test/test2-akshare.py
+-rw-rw-rw-   0        0        0     3709 2023-05-03 07:10:48.000000 sharetop-2.4.5/sharetop/test/test3.py
+-rw-rw-rw-   0        0        0      219 2023-05-04 04:00:10.000000 sharetop-2.4.5/sharetop/test/test4.py
+-rw-rw-rw-   0        0        0      690 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/test/test5.py
+-rw-rw-rw-   0        0        0     1227 2023-07-15 03:35:15.000000 sharetop-2.4.5/sharetop/test/test6.py
+-rw-rw-rw-   0        0        0      643 2023-07-05 12:16:23.000000 sharetop-2.4.5/sharetop/test/test7.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:58:09.327276 sharetop-2.4.5/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    51253 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2417 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 11:58:09.000000 sharetop-2.4.5/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.4.5/LICENSE` & `sharetop-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/PKG-INFO` & `sharetop-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.4.5
+Version: 2.4.5
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -283,15 +283,15 @@
 
 ```
 
 - 股票历史单子流入数据(日级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_history_bill('300033')
+>>> sp.capital_flow.get_stock_history_capital('300033')
     股票名称    股票代码          日期        主力净流入        小单净流入        中单净流入        大单净流入  ...  主力净流入占比  小单流入净占 比  中单流入净占比  大单流入净占比  超大单流入净占比     收盘价    涨跌幅
 0    同花顺  300033  2022-11-25     882089.0     224019.0   -1106108.0   -5475560.0  ...     0.23     0.06    -0.29    -1.42      1.65   91.70  -0.17
 1    同花顺  300033  2022-11-28  -26657991.0   -1271355.0   27929346.0    7247576.0  ...    -7.12    -0.34     7.46     1.94     -9.06   89.77  -2.10
 2    同花顺  300033  2022-11-29  -28424729.0   -7268909.0   35693632.0   -5113388.0  ...    -3.41    -0.87     4.28    -0.61     -2.79   95.87   6.80
 3    同花顺  300033  2022-11-30   79732027.0  -38462589.0  -41269424.0  -15238245.0  ...     8.88    -4.28    -4.59    -1.70     10.57   98.06   2.28
 4    同花顺  300033  2022-12-01  -78911985.0    2884073.0   76027920.0  -66718656.0  ...    -6.96     0.25     6.71    -5.88     -1.08  103.92   5.98
 ..   ...     ...         ...          ...          ...          ...          ...  ...      ...      ...      ...      ...       ...     ...    ...
@@ -304,15 +304,15 @@
 [102 rows x 15 columns]
 ```
 
 - 股票最新一个交易日单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_history_bill('300033')
+>>> sp.capital_flow.get_stock_real_time_daily_capital('300033')
       股票名称    股票代码                时间        主力净流入        小单净流入        中单净流入       大单净流入       超大单净流入
 0    同花顺  300033  2023-04-26 09:31   -3217110.0     282877.0    2934232.0  -2000281.0   -1216829.0
 1    同花顺  300033  2023-04-26 09:32   -2170472.0    1124259.0    1046212.0    155117.0   -2325589.0
 2    同花顺  300033  2023-04-26 09:33   -9655528.0    6350780.0    3304748.0  -1823981.0   -7831547.0
 3    同花顺  300033  2023-04-26 09:34  -16808716.0    9597965.0    7210752.0  -5368535.0  -11440181.0
 4    同花顺  300033  2023-04-26 09:35  -20358486.0   12331063.0    8027424.0  -5877906.0  -14480580.0
 ..   ...     ...               ...          ...          ...          ...         ...          ...
@@ -325,15 +325,15 @@
 [240 rows x 8 columns]
 ```
 
 - 股票实时的单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_capital_flow('002714')
+>>> sp.capital_flow.get_stock_real_time_sum_capital('002714')
       今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
 
 [1 rows x 28 columns]
 >>> sp.capital_flow.get_real_time_capital_flow(['002714', '300033'])
 {'002714':        今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
```

### Comparing `sharetop-1.4.5/README.md` & `sharetop-2.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
 ```
 
 - 股票历史单子流入数据(日级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_history_bill('300033')
+>>> sp.capital_flow.get_stock_history_capital('300033')
     股票名称    股票代码          日期        主力净流入        小单净流入        中单净流入        大单净流入  ...  主力净流入占比  小单流入净占 比  中单流入净占比  大单流入净占比  超大单流入净占比     收盘价    涨跌幅
 0    同花顺  300033  2022-11-25     882089.0     224019.0   -1106108.0   -5475560.0  ...     0.23     0.06    -0.29    -1.42      1.65   91.70  -0.17
 1    同花顺  300033  2022-11-28  -26657991.0   -1271355.0   27929346.0    7247576.0  ...    -7.12    -0.34     7.46     1.94     -9.06   89.77  -2.10
 2    同花顺  300033  2022-11-29  -28424729.0   -7268909.0   35693632.0   -5113388.0  ...    -3.41    -0.87     4.28    -0.61     -2.79   95.87   6.80
 3    同花顺  300033  2022-11-30   79732027.0  -38462589.0  -41269424.0  -15238245.0  ...     8.88    -4.28    -4.59    -1.70     10.57   98.06   2.28
 4    同花顺  300033  2022-12-01  -78911985.0    2884073.0   76027920.0  -66718656.0  ...    -6.96     0.25     6.71    -5.88     -1.08  103.92   5.98
 ..   ...     ...         ...          ...          ...          ...          ...  ...      ...      ...      ...      ...       ...     ...    ...
@@ -284,15 +284,15 @@
 [102 rows x 15 columns]
 ```
 
 - 股票最新一个交易日单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_history_bill('300033')
+>>> sp.capital_flow.get_stock_real_time_daily_capital('300033')
       股票名称    股票代码                时间        主力净流入        小单净流入        中单净流入       大单净流入       超大单净流入
 0    同花顺  300033  2023-04-26 09:31   -3217110.0     282877.0    2934232.0  -2000281.0   -1216829.0
 1    同花顺  300033  2023-04-26 09:32   -2170472.0    1124259.0    1046212.0    155117.0   -2325589.0
 2    同花顺  300033  2023-04-26 09:33   -9655528.0    6350780.0    3304748.0  -1823981.0   -7831547.0
 3    同花顺  300033  2023-04-26 09:34  -16808716.0    9597965.0    7210752.0  -5368535.0  -11440181.0
 4    同花顺  300033  2023-04-26 09:35  -20358486.0   12331063.0    8027424.0  -5877906.0  -14480580.0
 ..   ...     ...               ...          ...          ...          ...         ...          ...
@@ -305,15 +305,15 @@
 [240 rows x 8 columns]
 ```
 
 - 股票实时的单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_capital_flow('002714')
+>>> sp.capital_flow.get_stock_real_time_sum_capital('002714')
       今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
 
 [1 rows x 28 columns]
 >>> sp.capital_flow.get_real_time_capital_flow(['002714', '300033'])
 {'002714':        今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
```

### Comparing `sharetop-1.4.5/setup.py` & `sharetop-2.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/application/base.py` & `sharetop-2.4.5/sharetop/application/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/bond/config.py` & `sharetop-2.4.5/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/bond/get_bond_info.py` & `sharetop-2.4.5/sharetop/core/bond/get_bond_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pandas as pd
 from typing import List
 from ..common.config import EASTMONEY_REQUEST_HEADERS, FS_DICT
 from .config import EASTMONEY_BOND_BASE_INFO_FIELDS
 from ..utils import requests_obj
 from ...crawl.settings import *
-from ..utils import to_numeric, process_dataframe_and_series
+from ..utils import to_numeric, process_dataframe_and_series, validate_request
 from ..common import get_market_realtime_by_fs
 
 
-def get_bond_base_info_list() -> pd.DataFrame:
+@validate_request
+def get_bond_base_info_list(token: str) -> pd.DataFrame:
     """
     获取全部债券基本信息列表
     Returns
     -------
     DataFrame
         债券一些基本信息
     Examples
@@ -26,14 +27,15 @@
     ..     ...    ...     ...   ...  ...                  ...        ...         ...                  ...                  ...     ...                                                ...
     80  110227   赤化转债  600227   圣济堂  AAA  2007-10-10 00:00:00   4.500000    0.158854  2007-10-23 00:00:00  2009-05-25 00:00:00  1.6192  票面利率和付息日期:本次发行的债券票面利率第一 年为1.5%、第二年为1.8%、第三年为2....
     81  126006  07深高债  600548   深高速  AAA  2007-10-09 00:00:00  15.000000    0.290304  2007-10-30 00:00:00  2013-10-09 00:00:00       6                                               None
     82  110971   恒源转债  600971  恒源煤电  AAA  2007-09-24 00:00:00   4.000000    5.311774  2007-10-12 00:00:00  2009-12-21 00:00:00  2.2484  票面利率为:第一年年利率1.5%,第二年年利率1.8%,第三年年利率2.1%,第四年年利率2...
     83  110567   山鹰转债  600567  山鹰国际   AA  2007-09-05 00:00:00   4.700000    0.496391  2007-09-17 00:00:00  2010-02-01 00:00:00  2.4055  票面利率和付息日期:本次发行的债券票面利率第一年为1.4%,第二年为1.7%,第三年为2....
     84  110026   中海转债  600026  中远海能  AAA  2007-07-02 00:00:00  20.000000    1.333453  2007-07-12 00:00:00  2008-03-27 00:00:00   0.737  票面利率:第一年为1.84%,第二年为2.05%,第三年为2.26%,第四年为2.47%,第...
     """
+
     page = 1
     dfs: List[pd.DataFrame] = []
     columns = EASTMONEY_BOND_BASE_INFO_FIELDS
     while 1:
         params = (
             ('sortColumns', 'PUBLIC_START_DATE'),
             ('sortTypes', '-1'),
@@ -80,46 +82,51 @@
     394  123066  赛意转债   -6.0   193.08  203.999   193.08   203.0  -12.32   323.13   0.22     -   133317   261546032.0   205.4    79660753    79660753  0.123066   深A
     """
     df = get_market_realtime_by_fs(FS_DICT['bond'], **kwargs)
     df.rename(columns={'代码': '债券代码', '名称': '债券名称'}, inplace=True)
     return df
 
 
+@validate_request
 @to_numeric
-def get_bond_base_info(bond_code: str) -> pd.Series:
+def get_bond_base_info(token: str, bond_code: str) -> pd.Series:
     """
     获取单只债券基本信息
     Parameters
     ----------
     bond_code : str
         债券代码
     Returns
     -------
     Series
         债券的一些基本信息
+        :param bond_code:
+        :param token:
     """
     columns = EASTMONEY_BOND_BASE_INFO_FIELDS
     params = (
         ('reportName', 'RPT_BOND_CB_LIST'),
         ('columns', 'ALL'),
         ('source', 'WEB'),
         ('client', 'WEB'),
         ('filter', f'(SECURITY_CODE="{bond_code}")'),
     )
     url = ''.join(bond_base_info_url)
     json_response = requests_obj.get(url, params, headers=EASTMONEY_REQUEST_HEADERS).json()
+    print("json_response============:", json_response)
     if json_response['result'] is None:
         return pd.Series(index=columns.values(), dtype='object')
     items = json_response['result']['data']
     s = pd.Series(items[0]).rename(index=columns)
     s = s[columns.values()]
     return s
 
 
-def get_bond_public() -> pd.DataFrame:
+@validate_request
+def get_bond_public(token: str) -> pd.DataFrame:
     """
     中国-债券信息披露-债券发行
     http://www.chinamoney.com.cn/chinese/xzjfx/
     :return: 债券发行
     :rtype: pandas.DataFrame
     """
     url = "https://www.chinamoney.com.cn/ags/ms/cm-u-bond-an/bnBondEmit"
```

### Comparing `sharetop-1.4.5/sharetop/core/bond/get_bond_public_info.py` & `sharetop-2.4.5/sharetop/core/bond/get_bond_public_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     }
     params = {
         "sdate": "-".join([start_date[:4], start_date[4:6], start_date[6:]]),
         "edate": "-".join([end_date[:4], end_date[4:6], end_date[6:]]),
     }
     r = requests.post(url, headers=headers, params=params)
     data_json = r.json()
+    print("data_json======:", data_json)
     temp_df = pd.DataFrame(data_json["records"])
     temp_df.rename(
         columns={
             "F009D": "缴款日",
             "SECNAME": "债券简称",
             "DECLAREDATE": "公告日期",
             "F004D": "发行起始日",
```

### Comparing `sharetop-1.4.5/sharetop/core/cache.py` & `sharetop-2.4.5/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/capital_flow/capital_flow_monitor.py` & `sharetop-2.4.5/sharetop/core/capital_flow/capital_flow_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from ..utils import to_numeric
+from ..utils import to_numeric, validate_request
 from ..common.getter import get_history_bill as get_history_bill_for_stock
 from ..common.getter import get_real_time_bill_data_one
 from ..common.common_base import CommonFunc
 from typing import Dict, List, Union
 import pandas as pd
 
 common_func_obj = CommonFunc()
 
 
+@validate_request
 @to_numeric
-def get_history_bill(stock_code: str) -> pd.DataFrame:
+def get_stock_history_capital(token: str, stock_code: str) -> pd.DataFrame:
     """
     获取单只股票历史单子流入流出数据
     Parameters
     ----------
     stock_code : str
         股票代码
     Returns
@@ -30,23 +31,25 @@
     4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
     ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
     97   贵州茅台  600519  2021-07-26 -1.564233e+09  13142211.0  1.551091e+09 -1.270400e+08 -1.437193e+09    -8.74     0.07     8.67    -0.71     -8.03  1804.11 -5.05
     98   贵州茅台  600519  2021-07-27 -7.803296e+08 -10424715.0  7.907544e+08  6.725104e+07 -8.475807e+08    -5.12    -0.07     5.19     0.44     -5.56  1712.89 -5.06
     99   贵州茅台  600519  2021-07-28  3.997645e+08   2603511.0 -4.023677e+08  2.315648e+08  1.681997e+08     2.70     0.02    -2.72     1.57      1.14  1768.90  3.27
     100  贵州茅台  600519  2021-07-29 -9.209842e+08  -2312235.0  9.232964e+08 -3.959741e+08 -5.250101e+08    -8.15    -0.02     8.17    -3.50     -4.65  1749.79 -1.08
     101  贵州茅台  600519  2021-07-30 -1.524740e+09  -6020099.0  1.530761e+09  1.147248e+08 -1.639465e+09   -11.63    -0.05    11.68     0.88    -12.51  1678.99 -4.05
+    :param stock_code:
+    :param token:
 
     """
     df = get_history_bill_for_stock(stock_code)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
     return df
 
 
 @to_numeric
-def get_real_time_history_bill(stock_code: str) -> pd.DataFrame:
+def get_stock_real_time_daily_capital(stock_code: str) -> pd.DataFrame:
     """
     获取单只股票最新交易日的日内分钟级单子流入流出数据
 
     Parameters
     ----------
     stock_code : str
         股票代码
@@ -70,39 +73,41 @@
     238  600519  2021-07-29 14:59 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
     239  600519  2021-07-29 15:00 -920984196.0 -2312233.0  923296442.0 -395974137.0 -525010059.0
     """
     df = get_real_time_bill_data_one(stock_code)
     return df
 
 
-def get_real_time_capital_flow(stock_codes: Union[str, List[str]],
+def get_stock_real_time_sum_capital(stock_codes: Union[str, List[str]],
                                ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
-    获取单只股票最新交易日的日内分钟级单子流入流出数据
+    获取单只股票最新交易日的日内最新单子流入流出数据
     Parameters
     ----------
     stock_codes : 股票、债券代码 str 或者是 list
     如果是 str，为单支股票，如果为list，为多支股票
     Returns
     -------
     DataFrame
         单支或者多支股票、债券最新交易日的日内实时子流入流出数据
     """
-    base_func_name = get_real_time_capital_flow.__name__
+    base_func_name = get_stock_real_time_sum_capital.__name__
     return common_func_obj.get_common_func(stock_codes, base_func_name)
 
 
-def get_sector_real_time_capital_flow(sector: str, monitor_time: str):
+def get_stock_real_time_sector_capital(sector: str, monitor_time: str):
     """
     :param sector: industry: 行业, concept: 概念, area: 地域
     :param monitor_time: 1: 当天, 5: 5日,  10: 10日
     :return:
     """
     allowed_values = ['industry', 'concept', 'area']
     if sector not in allowed_values:
         raise ValueError(f"Invalid input: {sector}. Allowed values are {allowed_values}")
     monitor_time_allowed_values = ['1', '5', '10']
     if monitor_time not in monitor_time_allowed_values:
         raise ValueError(f"Invalid input: {monitor_time}. Allowed values are {monitor_time_allowed_values}")
     kwargs = {"monitor_time": monitor_time}
-    base_func_name = get_sector_real_time_capital_flow.__name__
+    base_func_name = get_stock_real_time_sector_capital.__name__
     return common_func_obj.get_common_func(sector, base_func_name, **kwargs)
+
+
```

### Comparing `sharetop-1.4.5/sharetop/core/common/common_base.py` & `sharetop-2.4.5/sharetop/core/common/common_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,28 +57,28 @@
         url = ''.join(stock_base_info_url)
         data = {"code": use_code}
         json_response = requests_obj.get(url, data).json()
         return parse_obj.parse_stock_base_info(json_response)
 
     @staticmethod
     @to_numeric
-    def get_real_time_capital_flow_data_one(code: str, **kwargs) -> pd.DataFrame:
+    def get_stock_real_time_sum_capital_data_one(code: str, **kwargs) -> pd.DataFrame:
         quote_id = get_quote_id(code)
         params = (
             ('secids', quote_id),
             ('fields',
              'f62,f184,f66,f69,f72,f75,f78,f81,f84,f87,f64,f65,f70,f71,f76,f77,f82,f83,f252,f253,f254,f255,f256,f278,f279,f280,f281,f282'),
         )
         url = ''.join(capital_flow_real_time_url_list)
         json_response = requests_obj.get(url, params).json()
         return parse_obj.parse_capital_flow_json(json_response)
 
     @staticmethod
     @to_numeric
-    def get_sector_real_time_capital_flow_data_one(sector: str, **kwargs) -> pd.DataFrame:
+    def get_stock_real_time_sector_capital_data_one(sector: str, **kwargs) -> pd.DataFrame:
         monitor_time = kwargs.get("monitor_time")
         params_base = {"po": "1", "pz": "500", "pn": "1", "np": "1", "fltt": "2", "invt": "2"}
         params_dict = sector_dict[monitor_time]
         fields_map = params_dict.pop("fields_map")
         drop_field = params_dict.pop("drop_field")
         params_base.update(params_dict)
         params_base.update(sector_dict2[sector])
```

### Comparing `sharetop-1.4.5/sharetop/core/common/config.py` & `sharetop-2.4.5/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/common/getter.py` & `sharetop-2.4.5/sharetop/core/common/getter.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     rows = [kline.split(',') for kline in klines]
     df = pd.DataFrame(rows, columns=columns)
     df.insert(0, '股票代码', code)
     df.insert(0, '股票名称', name)
     return df
 
 
-
 @to_numeric
 def get_history_bill(code: str) -> pd.DataFrame:
     """
     获取单支股票、债券的历史单子流入流出数据
 
     Parameters
     ----------
@@ -309,15 +308,16 @@
     获取多只股票、债券历史行情信息 或者实时行情
     """
     s = traceback.extract_stack()
     base_func_name = s[-2][2]
     total = len(codes)
     pool = Pool(total)
     func = globals()[f"{base_func_name}_data_one"]
-    coroutine_list = [pool.spawn(func, x, beg=beg, end=end, klt=klt, fqt=fqt, report_class=report_class, **kwargs) for x in codes]
+    coroutine_list = [pool.spawn(func, x, beg=beg, end=end, klt=klt, fqt=fqt, report_class=report_class, **kwargs) for x
+                      in codes]
     gevent.joinall(coroutine_list)
     df_value = [_.value for _ in coroutine_list]
     dfs = dict(zip(codes, df_value))
     return dfs
 
 
 @to_numeric
@@ -327,15 +327,16 @@
         ('ut', 'fa5fd1943c7b386f172d6893dbfba10b'),
         ('invt', '2'),
         ('fltt', '2'),
         ('fields', fields),
         ('secid', quote_id),
     )
     url = 'http://push2.eastmoney.com/api/qt/stock/get'
-    json_response = requests_obj.get(url, params, headers=EASTMONEY_REQUEST_HEADERS)
+    json_response = requests_obj.get(url, params, headers=EASTMONEY_REQUEST_HEADERS).json()
+    print("json_response=================:", json_response)
     items = json_response['data']
     if not items:
         return pd.Series(index=EASTMONEY_BASE_INFO_FIELDS.values(), dtype='object')
     s = pd.Series(items, dtype='object').rename(index=EASTMONEY_BASE_INFO_FIELDS)
     return s
 
 
@@ -367,15 +368,16 @@
     params = (
         ('secid', quote_id),
         ('fields1', 'f1,f2,f3,f4,f5'),
         ('fields2', 'f51,f52,f53,f54,f55'),
         ('pos', f'-{int(max_count)}'),
     )
     url = 'https://push2.eastmoney.com/api/qt/stock/details/get'
-    json_response = requests_obj.get(url, params)
+    json_response = requests_obj.get(url, params).json()
+    # print("json_response==================:", json_response)
     lines: List[str] = json_response['data']['details']
     rows = [line.split(',')[:4] for line in lines]
     df = pd.DataFrame(columns=columns, index=range(len(rows)))
     df.loc[:, '代码'] = code
     df.loc[:, '名称'] = name
     detail_df = pd.DataFrame(rows, columns=['时间', '成交价', '成交量', '单数'])
     detail_df.insert(1, '昨收', json_response['data']['prePrice'])
```

### Comparing `sharetop-1.4.5/sharetop/core/config.py` & `sharetop-2.4.5/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/fund/fund_list.py` & `sharetop-2.4.5/sharetop/core/fund/fund_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import pandas as pd
 from retry import retry
-from ..utils import requests_obj
+from ..utils import requests_obj, validate_request
 from ..common.getter import BaseApplication
 
 
+@validate_request
 @retry(tries=3)
-def get_fund_codes(ft: str = None) -> pd.DataFrame:
+def get_fund_codes(token: str, ft: str = None) -> pd.DataFrame:
     """
     获取天天基金网公开的全部公墓基金名单
     Parameters
     ----------
     ft : str, optional
         基金类型可选示例如下
         - ``'zq'``  : 债券类型基金
@@ -35,14 +36,16 @@
     4     004041             金鹰医疗健康产业C
     ...      ...                   ...
     1981  012503      国泰中证环保产业50ETF联接A
     1982  012517  国泰中证细分机械设备产业主题ETF联接C
     1983  012600             中银内核驱动股票C
     1984  011043             国泰价值先锋股票C
     1985  012516  国泰中证细分机械设备产业主题ETF联接A
+    :param ft:
+    :param token:
     """
     params = [
         ('op', 'dy'),
         ('dt', 'kf'),
         ('rs', ''),
         ('gs', '0'),
         ('sc', 'qjzf'),
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_base_info.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_base_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import rich
 import uuid
 import pandas as pd
 from retry import retry
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
 
 
+@validate_request
 @retry(tries=3)
 @to_numeric
-def get_base_info(fund_code: str) -> pd.Series:
+def get_fund_base_info(token: str, fund_code: str) -> pd.Series:
     """
     获取基金的一些基本信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
     -------
     Series
         基金的一些基本信息
+        :param fund_code:
+        :param token:
     """
     str_uuid = str(uuid.uuid4()).upper()
     params = (
         ('FCODE', fund_code),
         ('deviceid', str_uuid),
         ('plat', 'Iphone'),
         ('product', 'EFund'),
@@ -35,14 +38,17 @@
         'SHORTNAME': '基金简称',
         'ESTABDATE': '成立日期',
         'RZDF': '涨跌幅',
         'DWJZ': '最新净值',
         'JJGS': '基金公司',
         'FSRQ': '净值更新日期',
         'COMMENTS': '简介',
+        'ENDNAV': '基金规模',
+        'FEGMRQ': '基金规模更新时间',
+        'RLEVEL_SZ': '最新评级'
     }
     items = json_response['Datas']
     if not items:
         rich.print('基金代码', fund_code, '可能有误')
         return pd.Series(index=columns.values())
 
     s = pd.Series(json_response['Datas']).rename(index=columns)[columns.values()]
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_history_data.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_history_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pandas as pd
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from retry import retry
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
 
 
+@validate_request
 @retry(tries=3)
 @to_numeric
-def get_fund_history(fund_code: str, pz: int = 40000) -> pd.DataFrame:
+def get_fund_history_price(token: str, fund_code: str, pz: int = 40000) -> pd.DataFrame:
     """
     根据基金代码和要获取的页码抓取基金净值信息
 
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -33,14 +34,17 @@
     4    2021-06-07  1.6466  3.2777    1.61
     ...         ...     ...     ...     ...
     1469 2015-06-08  1.0380  1.0380  2.5692
     1470 2015-06-05  1.0120  1.0120  1.5045
     1471 2015-06-04  0.9970  0.9970      --
     1472 2015-05-29  0.9950  0.9950      --
     1473 2015-05-27  1.0000  1.0000      --
+    :param pz:
+    :param fund_code:
+    :param token:
 
     """
     data = {
         'FCODE': f'{fund_code}',
         'IsShareNet': 'true',
         'MobileKey': '1',
         'appType': 'ttjj',
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_industry_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import uuid
 import pandas as pd
 from typing import List, Union
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from ...crawl.settings import *
 from .config import EastmoneyFundHeaders
 
 
+@validate_request
 @to_numeric
-def get_industry_distribution(
-    fund_code: str, dates: Union[str, List[str]] = None
+def get_fund_industry_distribution(
+    token: str, fund_code: str, dates: Union[str, List[str]] = None
 ) -> pd.DataFrame:
     """
     获取指定基金行业分布信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -44,14 +45,17 @@
     13  161725            住宿和餐饮业     --  2021-06-30              --
     14  161725              房地产业     --  2021-06-30              --
     15  161725     居民服务、修理和其他服务业     --  2021-06-30              --
     16  161725           卫生和社会工作     --  2021-06-30              --
     17  161725         文化、体育和娱乐业     --  2021-06-30              --
     18  161725                综合     --  2021-06-30              --
     19  161725                合计  93.08  2021-06-30  6493286.808514
+    :param dates:
+    :param fund_code:
+    :param token:
     """
     columns = {'HYMC': '行业名称', 'ZJZBL': '持仓比例', 'FSRQ': '公布日期', 'SZ': '市值'}
     str_uuid = str(uuid.uuid4()).upper()
     df = pd.DataFrame(columns=columns.values())
     if isinstance(dates, str):
         dates = [dates]
     elif dates is None:
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_invest_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import uuid
 import pandas as pd
 from typing import List, Union
 from retry import retry
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from jsonpath import jsonpath
 from .config import EastmoneyFundHeaders
 
 
+@validate_request
 @retry(tries=3)
 @to_numeric
-def get_invest_position(
+def get_fund_invest_position(token: str,
     fund_code: str, dates: Union[str, List[str]] = None
 ) -> pd.DataFrame:
     """
     获取基金持仓占比数据
-
     Parameters
     ----------
     fund_code : str
         基金代码
     dates : Union[str, List[str]], optional
         日期或者日期构成的列表
         可选示例如下
@@ -106,15 +106,16 @@
     fields = ['基金代码'] + list(columns.values()) + ['公开日期']
     if not dfs:
         return pd.DataFrame(columns=fields)
     df = pd.concat(dfs, axis=0, ignore_index=True).rename(columns=columns)[fields]
     return df
 
 
-def get_public_dates(fund_code: str) -> List[str]:
+@validate_request
+def get_fund_public_dates(token: str, fund_code: str) -> List[str]:
     """
     获取历史上更新持仓情况的日期列表
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_rank.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_rank.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import requests
 import datetime
 import re
 import pandas as pd
-from ..utils import requests_obj, parse_obj
+from ..utils import requests_obj, parse_obj, validate_request
+from .config import fund_money_cloumns
 
 
 def fund_export_df(text_data):
     json_data = parse_obj.parse_fund_json(text_data)
     temp_df = pd.DataFrame(json_data)
     temp_df = temp_df.iloc[:, 0].str.split(",", expand=True)
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
     return temp_df
 
 
-def fund_open_fund_rank(symbol: str = "全部") -> pd.DataFrame:
+@validate_request
+def get_fund_open_rank(token: str, symbol: str = "全部") -> pd.DataFrame:
     """
     东方财富网-数据中心-开放基金排行
     https://fund.eastmoney.com/data/fundranking.html
     :param symbol: choice of {"全部", "股票型", "混合型", "债券型", "指数型", "QDII", "LOF", "FOF"}
     :type symbol: str
     :return: 开放基金排行
     :rtype: pandas.DataFrame
@@ -109,15 +111,16 @@
             "自定义",
             "手续费",
         ]
     ]
     return temp_df
 
 
-def fund_exchange_rank() -> pd.DataFrame:
+@validate_request
+def get_fund_exchange_rank(token: str) -> pd.DataFrame:
     """
     东方财富网-数据中心-场内交易基金排行
     https://fund.eastmoney.com/data/fbsfundranking.html
     :return: 场内交易基金数据
     :rtype: pandas.DataFrame
     """
     url = "http://fund.eastmoney.com/data/rankhandler.aspx"
@@ -199,15 +202,16 @@
     temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
     temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
     temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
     temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return temp_df
 
 
-def fund_money_rank() -> pd.DataFrame:
+@validate_request
+def get_fund_money_rank(token: str) -> pd.DataFrame:
     """
     东方财富网-数据中心-货币型基金排行
     https://fund.eastmoney.com/data/hbxfundranking.html
     :return: 货币型基金排行
     :rtype: pandas.DataFrame
     """
     url = "http://api.fund.eastmoney.com/FundRank/GetHbRankList"
@@ -223,67 +227,25 @@
     }
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
         "Referer": "http://fund.eastmoney.com/fundguzhi.html",
     }
     r = requests_obj.get(url, params, headers=headers)
     json_data = r.json()
-    temp_df = pd.DataFrame(json_data["Data"])
+    temp_data_json = []
+    for _ in json_data["Data"]:
+        temp_dict = {}
+        for k, v in _.items():
+            if k in fund_money_cloumns:
+                temp_dict[k] = v
+        temp_data_json.append(temp_dict)
+    temp_df = pd.DataFrame(temp_data_json)
+    temp_df.rename(columns=fund_money_cloumns, inplace=True)
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
-    temp_df.columns = [
-        "序号",
-        "近1年",
-        "近2年",
-        "近3年",
-        "近5年",
-        "基金代码",
-        "基金简称",
-        "日期",
-        "万份收益",
-        "年化收益率7日",
-        "_",
-        "年化收益率14日",
-        "年化收益率28日",
-        "近1月",
-        "近3月",
-        "近6月",
-        "今年来",
-        "成立来",
-        "_",
-        "手续费",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-    ]
-    temp_df = temp_df[
-        [
-            "序号",
-            "基金代码",
-            "基金简称",
-            "日期",
-            "万份收益",
-            "年化收益率7日",
-            "年化收益率14日",
-            "年化收益率28日",
-            "近1月",
-            "近3月",
-            "近6月",
-            "近1年",
-            "近2年",
-            "近3年",
-            "近5年",
-            "今年来",
-            "成立来",
-            "手续费",
-        ]
-    ]
     temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
     temp_df['万份收益'] = pd.to_numeric(temp_df['万份收益'], errors="coerce")
     temp_df['年化收益率7日'] = pd.to_numeric(temp_df['年化收益率7日'], errors="coerce")
     temp_df['年化收益率14日'] = pd.to_numeric(temp_df['年化收益率14日'], errors="coerce")
     temp_df['年化收益率28日'] = pd.to_numeric(temp_df['年化收益率28日'], errors="coerce")
     temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
     temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
@@ -293,15 +255,16 @@
     temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
     temp_df['近5年'] = pd.to_numeric(temp_df['近5年'], errors="coerce")
     temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
     temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return temp_df
 
 
-def fund_hk_rank() -> pd.DataFrame:
+@validate_request
+def fund_hk_rank(token: str) -> pd.DataFrame:
     """
     东方财富网-数据中心-香港基金排行
     https://overseas.1234567.com.cn/FundList
     :return: 香港基金排行
     :rtype: pandas.DataFrame
     """
     format_date = datetime.datetime.now().date().isoformat()
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_fund_real_time.py` & `sharetop-2.4.5/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_period_change_info.py` & `sharetop-2.4.5/sharetop/core/fund/get_period_change_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import uuid
 import pandas as pd
 from retry import retry
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from ...crawl.settings import *
 
 
+@validate_request
 @retry(tries=3)
 @to_numeric
-def get_period_change(fund_code: str) -> pd.DataFrame:
+def get_fund_period_change(token: str, fund_code: str) -> pd.DataFrame:
     """
     获取基金阶段涨跌幅度
     Parameters
     ----------
     fund_code : str
         6 位基金代码
     Returns
@@ -28,14 +29,16 @@
     3  161725   22.93  10.39    79  1223   近六月
     4  161725  103.76  33.58     7  1118   近一年
     5  161725  166.59  55.42     9   796   近两年
     6  161725  187.50  48.17     2   611   近三年
     7  161725  519.44  61.62     1   389   近五年
     8  161725    6.46   5.03   423  1243  今年以来
     9  161725  477.00                     成立以来
+    :param fund_code:
+    :param token:
     """
     str_uuid = str(uuid.uuid4()).upper()
     params = (
         ('AppVersion', '6.3.8'),
         ('FCODE', fund_code),
         ('MobileKey', str_uuid),
         ('OSVersion', '14.3'),
```

### Comparing `sharetop-1.4.5/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-2.4.5/sharetop/core/fund/get_types_percentage_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from retry import retry
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from .config import EastmoneyFundHeaders
 from typing import List, Union
 from ...crawl.settings import *
 import pandas as pd
 
 
+@validate_request
 @retry(tries=3)
 @to_numeric
-def get_types_percentage(
-    fund_code: str, dates: Union[List[str], str, None] = None
+def get_fund_types_percentage(
+    token: str, fund_code: str, dates: Union[List[str], str, None] = None
 ) -> pd.DataFrame:
     """
     获取指定基金不同类型占比信息
     Parameters
     ----------
     fund_code : str
         6 位基金代码
@@ -28,14 +29,17 @@
     DataFrame
         指定基金的在不同日期的不同类型持仓占比信息
     Examples
     --------
         基金代码   股票比重 债券比重  现金比重         总规模(亿元) 其他比重
     0  005827   94.4   --  6.06  880.1570625231    0
     0  005827  94.09   --  7.63   677.007455712    0
+    :param dates:
+    :param fund_code:
+    :param token:
     """
     columns = {'GP': '股票比重', 'ZQ': '债券比重', 'HB': '现金比重', 'JZC': '总规模(亿元)', 'QT': '其他比重'}
     df = pd.DataFrame(columns=columns.values())
     if not isinstance(dates, List):
         dates = [dates]
     elif dates is None:
         dates = [None]
```

### Comparing `sharetop-1.4.5/sharetop/core/futures/get_futures_info.py` & `sharetop-2.4.5/sharetop/core/futures/get_futures_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pandas as pd
 from ..common.config import FS_DICT
 from typing import Dict, List, Union
 from ..common.getter import get_market_realtime_by_fs, get_deal_detail
-from ..utils import process_dataframe_and_series
+from ..utils import process_dataframe_and_series, validate_request
 from ..common import get_history as get_quote_history_for_futures
 
 
-def get_futures_base_info() -> pd.DataFrame:
+@validate_request
+def get_futures_base_info(token: str) -> pd.DataFrame:
     """
     获取四个交易所全部期货基本信息
     Returns
     -------
     DataFrame
         四个交易所全部期货一些基本信息
     Examples
@@ -27,20 +28,22 @@
     848  070131   IH次主力合约    8.070131        中金所
     849  070120    IH当月连续     8.07012        中金所
     850  lu2109  低硫燃油2109  142.lu2109  上海能源期货交易所
     Notes
     -----
     """
     columns = ['期货代码', '期货名称', '行情ID', '市场类型']
-    df = get_realtime_quotes()
+    df = get_future_all_realtime_quotes()
     df = df[columns]
     return df
 
 
-def get_history_data(
+@validate_request
+def get_future_history_data(
+    token: str,
     quote_ids: Union[str, List[str]],
     beg: str = '19000101',
     end: str = '20500101',
     klt: int = 101,
     fqt: int = 1,
     **kwargs
 ) -> pd.DataFrame:
@@ -122,21 +125,19 @@
             df[stock_code].rename(columns={'代码': '期货代码', '名称': '期货名称'}, inplace=True)
             # NOTE 扩展接口 设定此关键词即返回 DataFrame 而不是 dict
         if kwargs.get('return_df'):
             df: pd.DataFrame = pd.concat(df, axis=0, ignore_index=True)
     return df
 
 
-
-
+@validate_request
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
-def get_realtime_quotes() -> pd.DataFrame:
+def get_future_all_realtime_quotes(token: str) -> pd.DataFrame:
     """
     获取期货最新行情总体情况
-
     Returns
     -------
     DataFrame
         期货市场的最新行情信息（涨跌幅、换手率等信息）
 
     Examples
     --------
```

### Comparing `sharetop-1.4.5/sharetop/core/oil/config.py` & `sharetop-2.4.5/sharetop/core/oil/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/core/oil/oil_detail.py` & `sharetop-2.4.5/sharetop/core/oil/oil_detail.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,100 @@
 import pandas as pd
+import copy
 from .config import oil_reserves_url, oil_reserves_field_dict, oil_products_field_dict, oil_products_url, \
     oil_consumption_url, oil_consumption_field_dict, oil_refinerythroughput_field_dict, oil_refinerythroughput_url, \
     oil_refinerycapacity_url, oil_refinerycapacity_field_dict, oil_crudeoilpricehistory_field_dict, \
     oil_crudeoilpricehistory_url
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
 
 
 @to_numeric
-def get_oil_data_common(oil_url: str, field_dict: dict, data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_data_common(token: str, oil_url: str, field_dict: dict, data_type: str = None,
+                        limit: int = None) -> pd.DataFrame:
     """
+    :param token:
     :param field_dict: 字段对应关系
     :param oil_url:  具体是石油数据url
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    base_url_list.append(oil_url)
+    copy_base_url_list = copy.deepcopy(base_url_list)
+    copy_base_url_list.append(oil_url)
     data = {}
+    headers = {"token": token}
     if data_type:
         data["data_type"] = data_type
     if limit:
         data['limit'] = limit
-    r = requests_obj.get("".join(base_url_list), data=data)
+    r = requests_obj.get("".join(copy_base_url_list), data=data, headers=headers)
+    if isinstance(r, dict):
+        return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, field_dict)
     return df
 
 
-def get_oil_reserves(data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_reserves(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取机构的石油储量
+    :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(oil_reserves_url, oil_reserves_field_dict, data_type, limit)
+    return get_oil_data_common(token, oil_reserves_url, oil_reserves_field_dict, data_type, limit)
 
 
-def get_oil_products(data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_products(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取机构的石油产量
+    :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(oil_products_url, oil_products_field_dict, data_type, limit)
+    return get_oil_data_common(token, oil_products_url, oil_products_field_dict, data_type, limit)
 
 
-def get_oil_consumption(data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_consumption(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取机构的消费量
+    :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(oil_consumption_url, oil_consumption_field_dict, data_type, limit)
+    return get_oil_data_common(token, oil_consumption_url, oil_consumption_field_dict, data_type, limit)
 
 
-def get_oil_refinerythroughput(data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_refinerythroughput(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取石油的加工量
+    :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(oil_refinerythroughput_url, oil_refinerythroughput_field_dict, data_type, limit)
+    return get_oil_data_common(token, oil_refinerythroughput_url, oil_refinerythroughput_field_dict, data_type, limit)
 
 
-def get_oil_refinerycapacity(data_type: str = None, limit: int = None) -> pd.DataFrame:
+def get_oil_refinerycapacity(token: str, data_type: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取石油的产能
+    :param token:
     :param data_type: 1为国家数据 2为机构数据 4为大洲数据
     :param limit:
     :return:
     """
-    return get_oil_data_common(oil_refinerycapacity_url, oil_refinerycapacity_field_dict, data_type, limit)
+    return get_oil_data_common(token, oil_refinerycapacity_url, oil_refinerycapacity_field_dict, data_type, limit)
 
 
-def get_oil_crudeoilpricehistory(limit: int = None) -> pd.DataFrame:
+def get_oil_crudeoilpricehistory(token: str, limit: int = None) -> pd.DataFrame:
     """
+    获取石油的历史价格
+    :param token:
     :param limit: 数据限制
     :return:
     """
-    return get_oil_data_common(oil_crudeoilpricehistory_url, oil_crudeoilpricehistory_field_dict, limit=limit)
+    return get_oil_data_common(token, oil_crudeoilpricehistory_url, oil_crudeoilpricehistory_field_dict, limit=limit)
```

### Comparing `sharetop-1.4.5/sharetop/core/pig/pig_detail.py` & `sharetop-2.4.5/sharetop/core/pig/pig_detail.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,46 @@
+import copy
 import pandas as pd
 from .config import pig_fcr_url, pig_fcr_field_dict
 from ...crawl.settings import *
 from ..utils import to_numeric, requests_obj, parse_obj
 
 
 @to_numeric
-def get_pig_data_common(pig_url: str, field_dict: dict, start_date: str, end_date: str, limit: int) -> pd.DataFrame:
+def get_pig_data_common(token: str, pig_url: str, field_dict: dict, start_date: str, end_date: str, limit: int) -> pd.DataFrame:
     """
+    :param token:
     :param field_dict:
     :param pig_url:
     :param start_date:
     :param end_date: 字段对应关系
     :param limit:
     :return:
     """
-    base_url_list.append(pig_url)
+    headers = {"token": token}
+    copy_base_url_list = copy.deepcopy(base_url_list)
+    copy_base_url_list.append(pig_url)
     data = {}
     if start_date:
         data["start_date"] = start_date
     if end_date:
         data['end_date'] = end_date
     if limit:
         data['limit'] = limit
-    r = requests_obj.get("".join(base_url_list), data=data)
+    r = requests_obj.get("".join(copy_base_url_list), data=data, headers=headers)
+    if isinstance(r, dict):
+        return r
     data_json = r.json()
     df = parse_obj.parse_god_cup_json(data_json, field_dict)
     return df
 
 
-def get_fcr(start_date: str = None, end_date: str = None, limit: int = None) -> pd.DataFrame:
+def get_pig_fcr(token: str, start_date: str = None, end_date: str = None, limit: int = None) -> pd.DataFrame:
     """
+    获取猪周期的历史猪肉价格和猪粮比
+    :param token:
     :param end_date:
     :param start_date:
     :param limit:
     :return:
     """
-    return get_pig_data_common(pig_fcr_url, pig_fcr_field_dict, start_date, end_date,  limit)
+    return get_pig_data_common(token, pig_fcr_url, pig_fcr_field_dict, start_date, end_date,  limit)
```

### Comparing `sharetop-1.4.5/sharetop/core/stock/bill_monitor.py` & `sharetop-2.4.5/sharetop/core/stock/bill_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from ..utils import to_numeric
+from ..utils import to_numeric, validate_request
 from ..common.getter import get_history_bill as get_history_bill_for_stock
 from ..common.getter import get_real_time_bill_data_one
 import pandas as pd
 
 
+@validate_request
 @to_numeric
-def get_history_bill(stock_code: str) -> pd.DataFrame:
+def get_stock_history_capital(token: str, stock_code: str) -> pd.DataFrame:
     """
     获取单只股票历史单子流入流出数据
     Parameters
     ----------
     stock_code : str
         股票代码
     Returns
@@ -26,15 +27,16 @@
     4    贵州茅台  600519  2021-03-10 -2.044173e+08  -1551798.0  2.059690e+08 -2.378506e+08  3.343331e+07    -2.02    -0.02     2.03    -2.35      0.33  1950.72  1.72
     ..    ...     ...         ...           ...         ...           ...           ...           ...      ...      ...      ...      ...       ...      ...   ...
     97   贵州茅台  600519  2021-07-26 -1.564233e+09  13142211.0  1.551091e+09 -1.270400e+08 -1.437193e+09    -8.74     0.07     8.67    -0.71     -8.03  1804.11 -5.05
     98   贵州茅台  600519  2021-07-27 -7.803296e+08 -10424715.0  7.907544e+08  6.725104e+07 -8.475807e+08    -5.12    -0.07     5.19     0.44     -5.56  1712.89 -5.06
     99   贵州茅台  600519  2021-07-28  3.997645e+08   2603511.0 -4.023677e+08  2.315648e+08  1.681997e+08     2.70     0.02    -2.72     1.57      1.14  1768.90  3.27
     100  贵州茅台  600519  2021-07-29 -9.209842e+08  -2312235.0  9.232964e+08 -3.959741e+08 -5.250101e+08    -8.15    -0.02     8.17    -3.50     -4.65  1749.79 -1.08
     101  贵州茅台  600519  2021-07-30 -1.524740e+09  -6020099.0  1.530761e+09  1.147248e+08 -1.639465e+09   -11.63    -0.05    11.68     0.88    -12.51  1678.99 -4.05
-
+    :param stock_code:
+    :param token:
     """
     df = get_history_bill_for_stock(stock_code)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
     return df
 
 
 @to_numeric
```

### Comparing `sharetop-1.4.5/sharetop/core/stock/getter.py` & `sharetop-2.4.5/sharetop/core/stock/getter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import Dict, List, Union
 import pandas as pd
 from ..common import get_history as get_history_data_for_stock
 from ..common import get_real_time
 from ..common.config import FS_DICT
 from ..common import get_market_realtime_by_fs
-from ..utils import to_numeric, process_dataframe_and_series
+from ..utils import to_numeric, process_dataframe_and_series, validate_request
+from .config import get_stock_market_real_time_data_fields
 
 
-def get_history_data(
+@validate_request
+def get_stock_kline_data(
+        token: str,
         stock_codes: Union[str, List[str]],
         beg: str = '19000101',
         end: str = '20500101',
         klt: int = 101,
         fqt: int = 1,
         **kwargs,
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
@@ -88,37 +91,38 @@
         df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
     elif isinstance(df, dict):
         for stock_code in df.keys():
             df[stock_code].rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
     return df
 
 
-def get_real_time_data(
+def get_stock_real_time_data(
         stock_codes: Union[str, List[str]],
 ) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
+    获取单个或者多个股票的实时股价
     :param stock_codes: 单个或者多个股票代码
     也可以是1.000001 0为深证，1为上证， 116为港股
     :return: 获取单个或者多个股票的实时股价和相关信息
     """
     df = get_real_time(stock_codes)
     return df
 
 
+@validate_request
 @process_dataframe_and_series(remove_columns_and_indexes=['市场编号'])
 @to_numeric
-def get_market_real_time(fs: Union[str, List[str]] = None, **kwargs) -> pd.DataFrame:
+def get_stock_market_real_time_data(token: str, fs: Union[str, List[str]] = None, is_explain: bool = False,
+                                    **kwargs) -> pd.DataFrame:
     """
         获取单个或者多个市场行情的最新状况
-
         Parameters
         ----------
         fs : Union[str, List[str]], optional
             行情名称或者多个行情名列表 可选值及示例如下
-
             - ``None``  沪深京A股市场行情
             - ``'沪深A股'`` 沪深A股市场行情
             - ``'沪A'`` 沪市A股市场行情
             - ``'深A'`` 深市A股市场行情
             - ``北A``   北证A股市场行情
             - ``'可转债'``  沪深可转债市场行情
             - ``'期货'``    期货市场行情
@@ -134,15 +138,14 @@
             - ``'概念板块'``    概念板块市场行情
             - ``'沪深系列指数'``    沪深系列指数市场行情
             - ``'上证系列指数'``    上证系列指数市场行情
             - ``'深证系列指数'``    深证系列指数市场行情
             - ``'ETF'`` ETF 基金市场行情
             - ``'LOF'`` LOF 基金市场行情
 
-
         Returns
         -------
         DataFrame
             单个或者多个市场行情的最新状况
 
         Raises
         ------
@@ -189,14 +192,16 @@
         551  513000  日经225ETF易方达 -4.49  1.212  1.269   1.21  1.269 -0.057   5.02  2.49     -     25819     3152848.0  1.269     62310617     62310617  1.513000   沪A
         552  513880     日经225ETF -4.59  1.163  1.224  1.162  1.217 -0.056  16.93  0.94     -     71058     8336846.0  1.219     48811110     48811110  1.513880   沪A
         553  513520        日经ETF -4.76    1.2  1.217  1.196  1.217  -0.06   27.7  1.79     -    146520    17645828.0  1.260     63464640     63464640  1.513520   沪A
 
         Notes
         -----
         无论股票、可转债、期货还是基金。第一列表头始终叫 ``股票代码``
+        :param fs:
+        :param is_explain: 是否以中文解释的方式返回数据，默认是FALSE
         """
     fs_list: List[str] = []
     if fs is None:
         fs_list.append(FS_DICT['stock'])
 
     if isinstance(fs, str):
         fs = [fs]
@@ -209,9 +214,11 @@
             fs_list.append(FS_DICT[f])
         # 给空列表时 试用沪深A股行情
         if not fs_list:
             fs_list.append(FS_DICT['stock'])
     fs_str = ','.join(fs_list)
     df = get_market_realtime_by_fs(fs_str, **kwargs)
     df.rename(columns={'代码': '股票代码', '名称': '股票名称'}, inplace=True)
+    if not is_explain:
+        df.rename(columns=get_stock_market_real_time_data_fields, inplace=True)
 
     return df
```

### Comparing `sharetop-1.4.5/sharetop/core/stock/quarterly_report.py` & `sharetop-2.4.5/sharetop/core/stock/quarterly_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import rich
 import pandas as pd
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from typing import List, Union
 from jsonpath import jsonpath
 from ...crawl.settings import *
 from ..common.getter import get_company_report
 
 
-def get_all_report_dates() -> pd.DataFrame:
+@validate_request
+def get_stock_all_report_dates(token: str) -> pd.DataFrame:
     """
     获取沪深市场的全部股票报告期信息
 
     Returns
     -------
     DataFrame
         沪深市场的全部股票报告期信息
@@ -74,29 +75,32 @@
         pd.DataFrame(columns=fields.values())
     df = pd.DataFrame(items)
     df = df.rename(columns=fields)
     df['报告日期'] = df['报告日期'].apply(lambda x: x.split()[0])
     return df
 
 
+@validate_request
 @to_numeric
-def get_company_report_base(stock_codes: Union[str, List[str]], report_class: str = None) -> pd.DataFrame:
+def get_stock_company_report_data(token: str, stock_codes: Union[str, List[str]], report_class: str = None) -> pd.DataFrame:
     """
+    获取单个或者多个上市公司历史年报
+    :param token:
     :param stock_codes: 指定的单个公司或者多个公司
-    :param report_class: 默认为空是全部，一季报，半年报，三季报，年报
+    :param report_class: 默认为空是全部，剩余参数可以为：“一季报”，“半年报”，“三季报”，“年报”
     :return:
     """
     return get_company_report(stock_codes, report_class)
 
 
+@validate_request
 @to_numeric
-def get_all_company_quarterly_report(date: str = None) -> pd.DataFrame:
+def get_stock_all_company_quarterly_report(token: str, date: str = None) -> pd.DataFrame:
     """
     获取沪深市场股票某一季度的表现情况
-
     Parameters
     ----------
     date : str, optional
         报告发布日期 部分可选示例如下(默认为 ``None``)
 
         - ``None`` : 最新季报
         - ``'2021-06-30'`` : 2021 年 Q2 季度报
@@ -155,15 +159,15 @@
         'BPS': '每股净资产',
         'WEIGHTAVG_ROE': '净资产收益率',
         'XSMLL': '销售毛利率',
         'MGJYXJJE': '每股经营现金流量'
         # 'ISNEW':'是否最新'
     }
 
-    dates = get_all_report_dates()['报告日期'].to_list()
+    dates = get_stock_all_report_dates(token)['报告日期'].to_list()
     if date is None:
         date = dates[0]
     if date not in dates:
         rich.print('日期输入有误，可选日期如下:')
         rich.print(dates)
         return pd.DataFrame(columns=fields.values())
```

### Comparing `sharetop-1.4.5/sharetop/core/stock/rank_list.py` & `sharetop-2.4.5/sharetop/core/stock/rank_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pandas as pd
 from datetime import datetime, timedelta
 from retry import retry
 from tqdm import tqdm
-from ..utils import to_numeric, requests_obj
+from ..utils import to_numeric, requests_obj, validate_request
 from typing import List
 from jsonpath import jsonpath
 from .config import (
     EASTMONEY_STOCK_DAILY_BILL_BOARD_FIELDS,
 )
 from ...crawl.settings import *
 
 
+@validate_request
 @to_numeric
 @retry(tries=3)
-def get_daily_billboard(start_date: str = None, end_date: str = None) -> pd.DataFrame:
+def get_stock_dragon_tiger_list(token: str, start_date: str = None, end_date: str = None) -> pd.DataFrame:
     """
     获取指定日期区间的龙虎榜详情数据
-
     Parameters
     ----------
     start_date : str, optional
         开始日期
         部分可选示例如下
 
         - ``None`` 最新一个榜单公开日(默认值)
@@ -61,14 +61,17 @@
     4    001208  华菱线缆  2021-08-27  1家机构买入，成功率40.43%   19.72   4.3386  46.1985  4.055258e+07  1.537821e+08  1.132295e+08  2.670117e+08  1203913048   3.368398   22.178651  2.634710e+09                日换手率达到20%的前5只证券
     ..      ...   ...         ...               ...     ...      ...      ...           ...           ...           ...           ...         ...        ...         ...           ...                            ...
     414  605580  恒盛能源  2021-08-20    买一主买，成功率33.33%   13.28  10.0249   0.4086  2.413149e+06  2.713051e+06  2.999022e+05  3.012953e+06     2713051  88.945937  111.054054  6.640000e+08  有价格涨跌幅限制的日收盘价格涨幅偏离值达到7%的前三只证券
     415  688029  南微医学  2021-08-20  4家机构卖出，成功率55.82%  204.61 -18.5340   8.1809 -1.412053e+08  1.883342e+08  3.295394e+08  5.178736e+08   762045800 -18.529760   67.958326  9.001510e+09    有价格涨跌幅限制的日收盘价格跌幅达到15%的前五只证券
     416  688408   中信博  2021-08-20  4家机构卖出，成功率47.86%  179.98  -0.0666  15.3723 -4.336304e+07  3.750919e+08  4.184550e+08  7.935469e+08   846547400  -5.122340   93.739221  5.695886e+09      有价格涨跌幅限制的日价格振幅达到30%的前五只证券
     417  688556  高测股份  2021-08-20  上海资金买入，成功率60.21%   51.97  17.0495  10.6452 -3.940045e+07  1.642095e+08  2.036099e+08  3.678194e+08   575411600  -6.847351   63.922831  5.739089e+09    有价格涨跌幅限制的日收盘价格涨幅达到15%的前五只证券
     418  688636   智明达  2021-08-20  2家机构买入，成功率47.37%  161.90  15.8332  11.9578  2.922406e+07  6.598126e+07  3.675721e+07  1.027385e+08   188330100  15.517464   54.552336  1.647410e+09    有价格涨跌幅限制的日收盘价格涨幅达到15%的前五只证券
+    :param end_date:
+    :param start_date:
+    :param token:
     """
     today = datetime.today().date()
     mode = 'auto'
     if start_date is None:
         start_date = today
 
     if end_date is None:
```

### Comparing `sharetop-1.4.5/sharetop/core/utils.py` & `sharetop-2.4.5/sharetop/core/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import time
 import rich
 import json
 import re
+import copy
 from retry.api import retry
 from typing import Any, Callable, Dict, List, TypeVar, Union
 from .cache import SEARCH_RESULT_DICT
 from .config import Quote
 from .config import SEARCH_RESULT_CACHE_PATH
 import pandas as pd
 from functools import wraps
 from ..crawl import BaseRequest
 from ..parser import BaseParse
+from ..crawl.settings import base_url_list
+
 
 F = TypeVar('F')
 requests_obj = BaseRequest()
 parse_obj = BaseParse()
 
 
 def to_numeric(func: F) -> F:
@@ -55,14 +58,39 @@
         except:
             pass
         return o
 
     return run
 
 
+def validate_request(func):
+    def wrapper(*args, **kwargs):
+        # 执行校验逻辑，可以是任何你需要的操作
+        if len(args) == 0:
+            return {"msg": "请填写有效token"}
+        token = args[0]
+        headers = {"token": token}
+        data = {}
+        copy_base_url_list = copy.deepcopy(base_url_list)
+        copy_base_url_list.append("/a_stock/base_data/detection")
+        r = requests_obj.get("".join(copy_base_url_list), data=data, headers=headers)
+        if isinstance(r, dict):
+            return r
+        data_json = r.json()
+        msg = data_json['data'].get('msg', "")
+        if msg == "success":
+            # 执行被装饰的函数
+            return func(*args, **kwargs)
+        else:
+            return {"msg": "校验失败，请确认token或者稍后再试或者联系管理员"}
+    return wrapper
+
+
+
+
 def search_quote_locally(keyword: str) -> Union[Quote, None]:
     """
     在本地里面使用搜索记录进行关键词搜索
 
     Parameters
     ----------
     keyword : str
```

### Comparing `sharetop-1.4.5/sharetop/crawl/settings.py` & `sharetop-2.4.5/sharetop/crawl/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,12 +37,13 @@
 bond_base_list_url = ['htt', 'p:/', '/dat', 'acen', 'ter', '-we', 'b.ea', 'stmo', 'ney', '.co', 'm/a', 'pi/d', 'ata', '/v', '1/g', 'et']
 
 bond_base_info_url = ['htt', 'p:/', '/dat', 'acen', 'ter-w', 'eb.e', 'astm', 'one', 'y.co', 'm/ap', 'i/da', 'ta/v', '1/g', 'et']
 
 stock_base_info_url = ['htt', 'p:/', '/em', 'we', 'b.se', 'curi', 'ties.', 'eas', 'tmon', 'ey.c', 'om/P', 'C_HS', 'F10/C', 'ompa', 'nySu', 'rve', 'y/Pa', 'geAj', 'ax']
 
 base_url_list = ['htt', 'p:/', '/sha', 'ret', 'op.', 'to', 'p/s', 'har', 'eto', 'papi']
-# base_url_list = ["htt", "p:/", "/12", "1.37", ".16.", "150:", "686", "9/a", "pi"]
+# base_url_list = ["http://127.0.0.1:8000/sharetopapi"]
+
 
 capital_flow_real_time_url_list = ['htt', 'ps:/', '/pu', 'sh2.e', 'astm', 'oney', '.co', 'm/ap', 'i/q', 't/ul', 'ist.', 'np/g', 'et']
 
 sector_url_list = ['htt', 'ps:/', '/pu', 'sh2', '.eas', 'tmon', 'ey.c', 'om/a', 'pi/q', 't/cl', 'ist', '/g', 'et']
```

### Comparing `sharetop-1.4.5/sharetop/parser/base.py` & `sharetop-2.4.5/sharetop/parser/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/parser/config.py` & `sharetop-2.4.5/sharetop/parser/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/test/test2-akshare.py` & `sharetop-2.4.5/sharetop/test/test2-akshare.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/test/test3.py` & `sharetop-2.4.5/sharetop/test/test3.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.4.5/sharetop/test/test6.py` & `sharetop-2.4.5/sharetop/test/test6.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from sharetop.core.capital_flow.capital_flow_monitor import get_real_time_capital_flow, get_history_bill, get_sector_real_time_capital_flow
+from sharetop.core.capital_flow.capital_flow_monitor import get_stock_real_time_sum_capital, get_stock_history_capital, get_stock_real_time_daily_capital, get_sector_real_time_capital_flow
 from enum import Enum
 # d = {"a": 1, "b":2}
 # d = get_real_time_capital_flow(["002714", "300033"])
 # d = get_real_time_capital_flow(['002714', '300033'])
-# d = get_sector_real_time_capital_flow('area', '10')
+d = get_sector_real_time_capital_flow('area', '10')
 
 # d = get_real_time_capital_flow("000001")
 
 # print(d)
 # print(d.to_dict("records"))
 import requests
 
@@ -22,7 +22,15 @@
 # r = response.text
 #
 # print(r)
 
 # h = "2d029512847cf13c"
 
 # print(len(h))
+
+# from sharetop.core.bond.get_bond_info import get_bond_base_info_list, get_bond_realtime_quotes, get_bond_base_info, get_bond_public
+token = "f109298d079b5f60"
+# d = get_bond_public(token)
+# print("d=============:", d)
+
+# d = get_real_time_capital_flow('002714')
+print("d=============:", d.to_dict("records"))
```

### Comparing `sharetop-1.4.5/sharetop.egg-info/PKG-INFO` & `sharetop-2.4.5/sharetop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.4.5
+Version: 2.4.5
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
@@ -283,15 +283,15 @@
 
 ```
 
 - 股票历史单子流入数据(日级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_history_bill('300033')
+>>> sp.capital_flow.get_stock_history_capital('300033')
     股票名称    股票代码          日期        主力净流入        小单净流入        中单净流入        大单净流入  ...  主力净流入占比  小单流入净占 比  中单流入净占比  大单流入净占比  超大单流入净占比     收盘价    涨跌幅
 0    同花顺  300033  2022-11-25     882089.0     224019.0   -1106108.0   -5475560.0  ...     0.23     0.06    -0.29    -1.42      1.65   91.70  -0.17
 1    同花顺  300033  2022-11-28  -26657991.0   -1271355.0   27929346.0    7247576.0  ...    -7.12    -0.34     7.46     1.94     -9.06   89.77  -2.10
 2    同花顺  300033  2022-11-29  -28424729.0   -7268909.0   35693632.0   -5113388.0  ...    -3.41    -0.87     4.28    -0.61     -2.79   95.87   6.80
 3    同花顺  300033  2022-11-30   79732027.0  -38462589.0  -41269424.0  -15238245.0  ...     8.88    -4.28    -4.59    -1.70     10.57   98.06   2.28
 4    同花顺  300033  2022-12-01  -78911985.0    2884073.0   76027920.0  -66718656.0  ...    -6.96     0.25     6.71    -5.88     -1.08  103.92   5.98
 ..   ...     ...         ...          ...          ...          ...          ...  ...      ...      ...      ...      ...       ...     ...    ...
@@ -304,15 +304,15 @@
 [102 rows x 15 columns]
 ```
 
 - 股票最新一个交易日单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_history_bill('300033')
+>>> sp.capital_flow.get_stock_real_time_daily_capital('300033')
       股票名称    股票代码                时间        主力净流入        小单净流入        中单净流入       大单净流入       超大单净流入
 0    同花顺  300033  2023-04-26 09:31   -3217110.0     282877.0    2934232.0  -2000281.0   -1216829.0
 1    同花顺  300033  2023-04-26 09:32   -2170472.0    1124259.0    1046212.0    155117.0   -2325589.0
 2    同花顺  300033  2023-04-26 09:33   -9655528.0    6350780.0    3304748.0  -1823981.0   -7831547.0
 3    同花顺  300033  2023-04-26 09:34  -16808716.0    9597965.0    7210752.0  -5368535.0  -11440181.0
 4    同花顺  300033  2023-04-26 09:35  -20358486.0   12331063.0    8027424.0  -5877906.0  -14480580.0
 ..   ...     ...               ...          ...          ...          ...         ...          ...
@@ -325,15 +325,15 @@
 [240 rows x 8 columns]
 ```
 
 - 股票实时的单子流入数据(分钟级)
 
 ```python
 >>> import sharetop as sp
->>> sp.capital_flow.get_real_time_capital_flow('002714')
+>>> sp.capital_flow.get_stock_real_time_sum_capital('002714')
       今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
 
 [1 rows x 28 columns]
 >>> sp.capital_flow.get_real_time_capital_flow(['002714', '300033'])
 {'002714':        今日主力净流入        超大单流入        超大单流出  ...      5日大单净流入      5日中单净流入      5日小单净流入
 0 -645896624.0  374761776.0  824220960.0  ... -234025066.0  122677726.0  746371952.0
```

