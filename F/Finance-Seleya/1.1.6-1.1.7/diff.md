# Comparing `tmp/Finance-Seleya-1.1.6.tar.gz` & `tmp/Finance-Seleya-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Seleya-1.1.6.tar", last modified: Tue Jul 18 11:57:07 2023, max compression
+gzip compressed data, was "dist/Finance-Seleya-1.1.7.tar", last modified: Tue Jul 18 11:57:55 2023, max compression
```

## Comparing `Finance-Seleya-1.1.6.tar` & `Finance-Seleya-1.1.7.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3059 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/Finance_Seleya.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-05 06:31:30.000000 Finance-Seleya-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/requirements/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/requirements/py2.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.6/requirements/py3.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/Toolset/
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/Toolset/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/Toolset/audit/esg_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/Toolset/blob_service.py
--rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/calendar.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-07-05 03:01:47.000000 Finance-Seleya-1.1.6/seleya/Toolset/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/Toolset/portfolio/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/Toolset/portfolio/esg_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/Toolset/tests/
--rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/tests/runner.py
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/tests/suite.py
--rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/Toolset/translator.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-07-05 03:10:06.000000 Finance-Seleya-1.1.6/seleya/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/config/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-18 11:47:55.000000 Finance-Seleya-1.1.6/seleya/config/default_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.6/seleya/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.6/seleya/core/env.pyx
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.6/seleya/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.6/seleya/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.6/seleya/core/parallel.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/
--rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/ESG.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/GD.py
--rw-r--r--   0 root         (0) root         (0)     5077 2023-07-18 11:34:40.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/SEARCH.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-07-18 10:51:16.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/USER.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/http/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/mongo/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/mongo/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36463 2023-07-17 02:48:21.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7428 2023-07-17 00:04:32.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/sly/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/sly/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/DataAPI/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/basic.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/engine.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/basic.py
--rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/company.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/engine.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/industry.py
--rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/metrics.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/sector.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/qrank/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/qrank/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7687 2023-06-24 10:01:03.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/qrank/glassdoor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/sbti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/sbti/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22737 2023-07-12 05:50:32.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/sbti/emission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/aerosol.py
--rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/s2f.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/mfc/micro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.6/seleya/mfc/micro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/seleya.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/seleya/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-07-18 11:56:06.000000 Finance-Seleya-1.1.6/seleya/utilities/api_base.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.6/seleya/utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.6/seleya/utilities/kd_logger.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/utilities/singleton.py
--rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.6/seleya/utilities/warning.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 11:56:51.000000 Finance-Seleya-1.1.6/seleya/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:57:07.000000 Finance-Seleya-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3457 2023-07-18 11:56:32.000000 Finance-Seleya-1.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/Finance_Seleya.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-05 06:31:30.000000 Finance-Seleya-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/requirements/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/requirements/py2.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.7/requirements/py3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/Toolset/
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/Toolset/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/Toolset/audit/esg_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/Toolset/blob_service.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-07-05 03:01:47.000000 Finance-Seleya-1.1.7/seleya/Toolset/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/Toolset/portfolio/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/Toolset/portfolio/esg_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/Toolset/tests/
+-rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/tests/runner.py
+-rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/tests/suite.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/Toolset/translator.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-07-05 03:10:06.000000 Finance-Seleya-1.1.7/seleya/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-07-18 11:47:55.000000 Finance-Seleya-1.1.7/seleya/config/default_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.7/seleya/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.7/seleya/core/env.pyx
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.7/seleya/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.7/seleya/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.7/seleya/core/parallel.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/ESG.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/GD.py
+-rw-r--r--   0 root         (0) root         (0)     5077 2023-07-18 11:34:40.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/SEARCH.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-07-18 10:51:16.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/USER.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/http/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/mongo/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/mongo/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36463 2023-07-17 02:48:21.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2023-07-17 00:04:32.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/sly/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/sly/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/DataAPI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/engine.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/basic.py
+-rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/company.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/engine.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/sector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/qrank/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/qrank/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7687 2023-06-24 10:01:03.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/qrank/glassdoor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/sbti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/sbti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22737 2023-07-12 05:50:32.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/sbti/emission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/aerosol.py
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/s2f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/mfc/micro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.7/seleya/mfc/micro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/seleya.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/seleya/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-07-18 11:56:06.000000 Finance-Seleya-1.1.7/seleya/utilities/api_base.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.7/seleya/utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.7/seleya/utilities/kd_logger.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/utilities/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.7/seleya/utilities/warning.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 11:57:45.000000 Finance-Seleya-1.1.7/seleya/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:57:55.000000 Finance-Seleya-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3457 2023-07-18 11:57:49.000000 Finance-Seleya-1.1.7/setup.py
```

### Comparing `Finance-Seleya-1.1.6/Finance_Seleya.egg-info/SOURCES.txt` & `Finance-Seleya-1.1.7/Finance_Seleya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/audit/esg_metrics.py` & `Finance-Seleya-1.1.7/seleya/Toolset/audit/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/blob_service.py` & `Finance-Seleya-1.1.7/seleya/Toolset/blob_service.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/calendar.py` & `Finance-Seleya-1.1.7/seleya/Toolset/calendar.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/file_util.py` & `Finance-Seleya-1.1.7/seleya/Toolset/file_util.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/portfolio/esg_metrics.py` & `Finance-Seleya-1.1.7/seleya/Toolset/portfolio/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/tests/runner.py` & `Finance-Seleya-1.1.7/seleya/Toolset/tests/runner.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/Toolset/translator.py` & `Finance-Seleya-1.1.7/seleya/Toolset/translator.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/__init__.py` & `Finance-Seleya-1.1.7/seleya/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/config/default_config.py` & `Finance-Seleya-1.1.7/seleya/config/default_config.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/core/env.pyx` & `Finance-Seleya-1.1.7/seleya/core/env.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/core/fixes.pyx` & `Finance-Seleya-1.1.7/seleya/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/core/helper.pyx` & `Finance-Seleya-1.1.7/seleya/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/core/parallel.pyx` & `Finance-Seleya-1.1.7/seleya/core/parallel.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/http/ESG.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/http/ESG.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/http/GD.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/http/GD.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/http/SEARCH.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/http/SEARCH.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/http/USER.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/http/USER.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/http/utils.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/http/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/mongo/mongodb.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/mongo/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/db_factory.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/db_factory.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/fetch_engine.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/fetch_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/DataAPI/sqlatom/sly/sly_engine.py` & `Finance-Seleya-1.1.7/seleya/data/DataAPI/sqlatom/sly/sly_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/basic.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/engine.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/__init__.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/basic.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/company.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/company.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/engine.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/feature_importance.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/feature_importance.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/industry.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/metrics.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/data/SurfaceAPI/sqlatom/sector.py` & `Finance-Seleya-1.1.7/seleya/data/SurfaceAPI/sqlatom/sector.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/mfc/alchemy/qrank/glassdoor.py` & `Finance-Seleya-1.1.7/seleya/mfc/alchemy/qrank/glassdoor.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/mfc/alchemy/sbti/emission.py` & `Finance-Seleya-1.1.7/seleya/mfc/alchemy/sbti/emission.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/aerosol.py` & `Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/aerosol.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/mfc/alchemy/tsi/s2f.py` & `Finance-Seleya-1.1.7/seleya/mfc/alchemy/tsi/s2f.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/utilities/api_base.py` & `Finance-Seleya-1.1.7/seleya/utilities/api_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/seleya/utilities/kd_logger.py` & `Finance-Seleya-1.1.7/seleya/utilities/kd_logger.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.6/setup.py` & `Finance-Seleya-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from distutils.cmd import Command
 from distutils.extension import Extension
 from Cython.Build import cythonize
 from Cython.Distutils import build_ext
 import Cython.Compiler.Options
 import os, sys, io, subprocess, platform
 
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 
 Cython.Compiler.Options.annotate = True
 
 PACKAGE = "seleya"
 NAME = "Finance-Seleya"
 VERSION = __version__
 DESCRIPTION = "FinSeleya " + VERSION
```

