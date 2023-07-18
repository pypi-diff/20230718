# Comparing `tmp/pyDecision-3.0.2.tar.gz` & `tmp/pyDecision-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-3.0.2.tar", last modified: Sun Jul 16 16:30:04 2023, max compression
+gzip compressed data, was "dist\pyDecision-3.0.3.tar", last modified: Tue Jul 18 01:05:03 2023, max compression
```

## Comparing `pyDecision-3.0.2.tar` & `pyDecision-3.0.3.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-3.0.2/LICENSE
--rw-rw-rw-   0        0        0    13520 2023-07-16 16:30:04.000000 pyDecision-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13123 2023-07-16 16:23:47.000000 pyDecision-3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 16:30:03.000000 pyDecision-3.0.2/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-3.0.2/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     1994 2023-07-16 16:15:27.000000 pyDecision-3.0.2/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-3.0.2/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-3.0.2/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-3.0.2/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-3.0.2/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0      801 2023-07-15 20:46:57.000000 pyDecision-3.0.2/pyDecision/algorithm/cilos.py
--rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-3.0.2/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-3.0.2/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-3.0.2/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-3.0.2/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-3.0.2/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-3.0.2/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-3.0.2/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-3.0.2/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-3.0.2/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-3.0.2/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-3.0.2/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-3.0.2/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-3.0.2/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2551 2023-07-16 13:00:46.000000 pyDecision-3.0.2/pyDecision/algorithm/mairca.py
--rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-3.0.2/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-3.0.2/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0      967 2023-07-15 20:29:25.000000 pyDecision-3.0.2/pyDecision/algorithm/merec.py
--rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-3.0.2/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-3.0.2/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-3.0.2/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-3.0.2/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-3.0.2/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-3.0.2/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-3.0.2/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-3.0.2/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-3.0.2/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-3.0.2/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-3.0.2/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2115 2023-07-16 16:14:56.000000 pyDecision-3.0.2/pyDecision/algorithm/piv.py
--rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-3.0.2/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-3.0.2/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-3.0.2/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-3.0.2/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-3.0.2/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-3.0.2/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-3.0.2/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/pyDecision/util/
--rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-3.0.2/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-3.0.2/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-3.0.2/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-16 16:30:03.000000 pyDecision-3.0.2/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    13520 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1820 2023-07-16 16:30:02.000000 pyDecision-3.0.2/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 16:30:04.000000 pyDecision-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-16 16:25:42.000000 pyDecision-3.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-3.0.3/LICENSE
+-rw-rw-rw-   0        0        0    13774 2023-07-18 01:05:03.000000 pyDecision-3.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13376 2023-07-18 01:03:18.000000 pyDecision-3.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-3.0.3/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     2035 2023-07-18 00:56:12.000000 pyDecision-3.0.3/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-3.0.3/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-3.0.3/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-3.0.3/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-3.0.3/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      862 2023-07-18 00:52:46.000000 pyDecision-3.0.3/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-3.0.3/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-3.0.3/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-3.0.3/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     2302 2023-07-18 00:55:14.000000 pyDecision-3.0.3/pyDecision/algorithm/cradis.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-3.0.3/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-3.0.3/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-3.0.3/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-3.0.3/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-3.0.3/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-3.0.3/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-3.0.3/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-3.0.3/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-3.0.3/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-3.0.3/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-3.0.3/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-3.0.3/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2551 2023-07-16 13:00:46.000000 pyDecision-3.0.3/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-3.0.3/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-3.0.3/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      967 2023-07-15 20:29:25.000000 pyDecision-3.0.3/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-3.0.3/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-3.0.3/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-3.0.3/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-3.0.3/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-3.0.3/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-3.0.3/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-3.0.3/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-3.0.3/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-3.0.3/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-3.0.3/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-3.0.3/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2115 2023-07-16 16:14:56.000000 pyDecision-3.0.3/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-3.0.3/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-3.0.3/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-3.0.3/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-3.0.3/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-3.0.3/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-3.0.3/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-3.0.3/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision/util/
+-rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-3.0.3/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-3.0.3/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-3.0.3/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:05:03.000000 pyDecision-3.0.3/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    13774 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1851 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 01:05:02.000000 pyDecision-3.0.3/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 01:05:03.000000 pyDecision-3.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-07-18 01:04:43.000000 pyDecision-3.0.3/setup.py
```

### Comparing `pyDecision-3.0.2/LICENSE` & `pyDecision-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/PKG-INFO` & `pyDecision-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 3.0.2
+Version: 3.0.3
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -67,14 +67,15 @@
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
```

### Comparing `pyDecision-3.0.2/README.md` & `pyDecision-3.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -56,14 +56,15 @@
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
```

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/__init__.py` & `pyDecision-3.0.3/pyDecision/algorithm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .aras          import aras_method
 from .borda         import borda_method
 from .bwm           import bw_method
 from .cilos         import cilos_method
 from .cocoso        import cocoso_method
 from .codas         import codas_method
 from .copras        import copras_method
+from .cradis        import cradis_method
 from .critic        import critic_method
 from .dematel       import dematel_method
 from .e_i           import electre_i
 from .e_i_s         import electre_i_s
 from .e_i_v         import electre_i_v
 from .e_ii          import electre_ii
 from .e_iii         import electre_iii
```

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/ahp.py` & `pyDecision-3.0.3/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/aras.py` & `pyDecision-3.0.3/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/borda.py` & `pyDecision-3.0.3/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/bwm.py` & `pyDecision-3.0.3/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/cilos.py` & `pyDecision-3.0.3/pyDecision/algorithm/cilos.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 # Function: CILOS (Criterion Impact LOSs)
 def cilos_method(dataset, criterion_type):
     X = np.copy(dataset)/1.0
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
             X[:,j] = np.min(X[:,j]) / X[:,j]
+        else:
+            X[:,j] = X[:,j] / np.max(X[:,j])
         X[:,j] = X[:,j] / np.sum(X[:,j])
     A = X[np.argmax(X, axis = 0)]
     P = (np.diag(A) - A) / np.diag(A)
     F = P - np.diag(np.sum(P, axis = 0))
     q = null_space(F)
     q = (q / np.sum(q)).flatten()
     return q
```

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/cocoso.py` & `pyDecision-3.0.3/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/codas.py` & `pyDecision-3.0.3/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/copras.py` & `pyDecision-3.0.3/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/critic.py` & `pyDecision-3.0.3/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/dematel.py` & `pyDecision-3.0.3/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_i.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_i_s.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_i_v.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_ii.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_iii.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_iv.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/e_tri_b.py` & `pyDecision-3.0.3/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/edas.py` & `pyDecision-3.0.3/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-3.0.3/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/gra.py` & `pyDecision-3.0.3/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/idocriw.py` & `pyDecision-3.0.3/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/mabac.py` & `pyDecision-3.0.3/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/mairca.py` & `pyDecision-3.0.3/pyDecision/algorithm/mairca.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/marcos.py` & `pyDecision-3.0.3/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/maut.py` & `pyDecision-3.0.3/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/merec.py` & `pyDecision-3.0.3/pyDecision/algorithm/merec.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/moora.py` & `pyDecision-3.0.3/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/moosra.py` & `pyDecision-3.0.3/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/multimoora.py` & `pyDecision-3.0.3/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/ocra.py` & `pyDecision-3.0.3/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_i.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_ii.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_iii.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_iv.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_v.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_vi.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/p_xgaia.py` & `pyDecision-3.0.3/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/piv.py` & `pyDecision-3.0.3/pyDecision/algorithm/piv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/saw.py` & `pyDecision-3.0.3/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/smart.py` & `pyDecision-3.0.3/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/todim.py` & `pyDecision-3.0.3/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/topsis.py` & `pyDecision-3.0.3/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/vikor.py` & `pyDecision-3.0.3/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/waspas.py` & `pyDecision-3.0.3/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/algorithm/wings.py` & `pyDecision-3.0.3/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/util/ga.py` & `pyDecision-3.0.3/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision/util/gwo.py` & `pyDecision-3.0.3/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-3.0.2/pyDecision.egg-info/PKG-INFO` & `pyDecision-3.0.3/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 3.0.2
+Version: 3.0.3
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRADIS** (Compromise Ranking of Alternatives from Distance to Ideal Solution); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -67,14 +67,15 @@
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
 - CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
+- CRADIS ([ Colab Demo ](https://colab.research.google.com/drive/1p7AQmPIOsZFxaypqMsiRIWW8mIvDtoLi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007%2Fs10668-021-01902-2))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
 - Fuzzy EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1kw2LwztNAU9Asjj6BvBmvk11wvk8R3V6?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-32-9072-3_63))
 - ELECTRE I     ([ Colab Demo ](https://colab.research.google.com/drive/1KFqRPBRyv-fxiu2B1y7VNkP5pCCbILF1?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/blob/master/MCDA/E01.pdf))
 - ELECTRE I_s   ([ Colab Demo ](https://colab.research.google.com/drive/1ngxsQPh2QULjd1_AifFofbukq5zIOePd?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
```

### Comparing `pyDecision-3.0.2/pyDecision.egg-info/SOURCES.txt` & `pyDecision-3.0.3/pyDecision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pyDecision/algorithm/aras.py
 pyDecision/algorithm/borda.py
 pyDecision/algorithm/bwm.py
 pyDecision/algorithm/cilos.py
 pyDecision/algorithm/cocoso.py
 pyDecision/algorithm/codas.py
 pyDecision/algorithm/copras.py
+pyDecision/algorithm/cradis.py
 pyDecision/algorithm/critic.py
 pyDecision/algorithm/dematel.py
 pyDecision/algorithm/e_i.py
 pyDecision/algorithm/e_i_s.py
 pyDecision/algorithm/e_i_v.py
 pyDecision/algorithm/e_ii.py
 pyDecision/algorithm/e_iii.py
```

### Comparing `pyDecision-3.0.2/setup.py` & `pyDecision-3.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='3.0.2',
+    version='3.0.3',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

