# Comparing `tmp/damo-1.8.9.tar.gz` & `tmp/damo-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.9.tar", last modified: Mon Jul 10 18:38:44 2023, max compression
+gzip compressed data, was "damo-1.9.0.tar", last modified: Mon Jul 17 23:20:07 2023, max compression
```

## Comparing `damo-1.8.9.tar` & `damo-1.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.584291 damo-1.8.9/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-10 18:38:44.584291 damo-1.8.9/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-10 18:38:40.000000 damo-1.8.9/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.8.9/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-10 18:38:44.584291 damo-1.8.9/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.8.9/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.568291 damo-1.8.9/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.580291 damo-1.8.9/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:40.000000 damo-1.8.9/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.8.9/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9841 2023-07-09 19:46:58.000000 damo-1.8.9/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35332 2023-07-09 19:39:19.000000 damo-1.8.9/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.8.9/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    27404 2023-07-09 19:29:35.000000 damo-1.8.9/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.8.9/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3991 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.8.9/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.8.9/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.8.9/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.8.9/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3766 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.8.9/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    12170 2023-07-09 19:59:30.000000 damo-1.8.9/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.8.9/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2382 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1043 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3149 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      986 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-06-25 17:28:02.000000 damo-1.8.9/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.8.9/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.8.9/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.8.9/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-10 18:37:33.000000 damo-1.8.9/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5551 2023-07-04 00:27:48.000000 damo-1.8.9/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-10 18:38:44.584291 damo-1.8.9/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-10 18:38:44.000000 damo-1.8.9/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.296029 damo-1.9.0/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-17 23:20:07.296029 damo-1.9.0/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-07-17 23:20:02.000000 damo-1.9.0/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.0/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-07-17 23:20:07.296029 damo-1.9.0/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.0/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.268030 damo-1.9.0/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.292029 damo-1.9.0/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:02.000000 damo-1.9.0/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.0/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35212 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    11838 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.0/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-16 17:20:38.000000 damo-1.9.0/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19598 2023-07-02 18:42:47.000000 damo-1.9.0/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3991 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.0/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.0/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.0/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.0/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.0/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    12741 2023-07-16 18:22:40.000000 damo-1.9.0/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.0/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2602 2023-07-16 18:13:27.000000 damo-1.9.0/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      878 2023-07-16 18:10:50.000000 damo-1.9.0/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-07-16 18:14:49.000000 damo-1.9.0/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      822 2023-07-16 18:11:19.000000 damo-1.9.0/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3354 2023-07-16 18:27:07.000000 damo-1.9.0/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.0/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.0/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.0/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.0/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-07-17 23:18:25.000000 damo-1.9.0/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.0/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-07-17 23:20:07.296029 damo-1.9.0/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1249 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-07-17 23:20:07.000000 damo-1.9.0/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.9/PKG-INFO` & `damo-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.9
+Version: 1.9.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.9/README.md` & `damo-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -47,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.9/setup.py` & `damo-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_deprecated.py` & `damo-1.9.0/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_deprecation_notice.py` & `damo-1.9.0/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_dist.py` & `damo-1.9.0/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_fmt_str.py` & `damo-1.9.0/src/damo/_damo_fmt_str.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,36 +296,36 @@
     success, number = try_common_input(txt)
     if success:
         return number
 
     return text_to_ms(txt) / 1000
 
 def text_to_ratio(txt):
-    success, number = try_common_input(txt, 0.0, 1.0)
+    success, number = try_common_input(txt, 0.0)
     if success:
         return number
 
     is_percent = False
     if txt[-1] == '%':
         is_percent = True
         txt = txt[:-1]
     ratio = text_to_nr(txt)
     if is_percent:
         ratio /= 100.0
     return ratio
 
 def text_to_permil(txt):
-    success, number = try_common_input(txt, 0, 1000)
+    success, number = try_common_input(txt, 0)
     if success:
         return number
 
     return text_to_ratio(txt) * 1000
 
 def text_to_percent(txt):
-    success, number = try_common_input(txt, 0, 100)
+    success, number = try_common_input(txt, 0)
     if success:
         return number
 
     return text_to_ratio(txt) * 100
 
 def text_to_nr_unit(txt):
     fields = txt.split()
```

### Comparing `damo-1.8.9/src/damo/_damo_fs.py` & `damo-1.9.0/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_paddr_layout.py` & `damo-1.9.0/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damo_subcmds.py` & `damo-1.9.0/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damon.py` & `damo-1.9.0/src/damo/_damon.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,23 +84,27 @@
 unit_aggr_intervals = 'aggr_intervals'
 
 class DamonNrAccesses:
     samples = None
     percent = None
 
     def __init__(self, val, unit):
+        if val == None or unit == None:
+            return
         if unit == unit_samples:
-            self.samples = val
+            self.samples = _damo_fmt_str.text_to_nr(val)
         elif unit == unit_percent:
-            self.percent = val
+            self.percent = _damo_fmt_str.text_to_percent(val)
+        else:
+            raise Exception('invalid DamonNrAccesses unit \'%s\'' % unit)
 
     def __eq__(self, other):
         return (type(self) == type(other) and
-                (self.samples == other.samples or
-                    self.percent == other.percent))
+                ((self.samples != None and self.samples == other.samples) or
+                    (self.percent != None and self.percent == other.percent)))
 
     def add_unset_unit(self, intervals):
         if self.samples != None and self.percent != None:
             return
         max_val = intervals.aggr / intervals.sample
         if self.samples == None:
             self.samples = int(self.percent * max_val / 100)
@@ -127,25 +131,31 @@
                 [('samples', self.samples), ('percent', self.percent)])
 
 class DamonAge:
     usec = None
     aggr_intervals = None
 
     def __init__(self, val, unit):
+        if val == None and unit != None:
+            self.unit = unit
+            return
+        if val == None and unit == None:
+            return
         if unit == unit_usec:
-            self.usec = val
+            self.usec = _damo_fmt_str.text_to_us(val)
         elif unit == unit_aggr_intervals:
-            self.aggr_intervals = val
+            self.aggr_intervals = _damo_fmt_str.text_to_nr(val)
         else:
             raise Exception('DamonAge unsupported unit (%s)' % unit)
 
     def __eq__(self, other):
         return (type(self) == type(other) and
-                (self.usec == other.usec or
-                    self.aggr_intervals == other.aggr_intervals))
+                ((self.usec != None and self.usec == other.usec) or
+                    (self.aggr_intervals != None and
+                        self.aggr_intervals == other.aggr_intervals)))
 
     def add_unset_unit(self, intervals):
         if self.usec != None and self.aggr_intervals != None:
             return
         if self.usec == None:
             self.usec = self.aggr_intervals * intervals.aggr
         elif self.aggr_intervals == None:
@@ -155,15 +165,15 @@
         if unit == unit_usec:
             return _damo_fmt_str.format_time_us_exact(self.usec, raw)
         return '%s %s' % (_damo_fmt_str.format_nr(self.aggr_intervals, raw),
                 unit_aggr_intervals)
 
     @classmethod
     def from_kvpairs(cls, kv):
-        ret = DamonAge(None, unit_usec)
+        ret = DamonAge(None, None)
         if kv['usec'] != None:
             ret.usec = _damo_fmt_str.text_to_us(kv['usec'])
         if kv['aggr_intervals'] != None:
             ret.aggr_intervals = _damo_fmt_str.text_to_nr(kv['aggr_intervals'])
         return ret
 
     def to_kvpairs(self, raw=False):
@@ -240,14 +250,17 @@
                 ('end', _damo_fmt_str.format_nr(self.end, raw))])
         return collections.OrderedDict([
             ('start', _damo_fmt_str.format_nr(self.start, raw)),
             ('end', _damo_fmt_str.format_nr(self.end, raw)),
             ('nr_accesses', self.nr_accesses.to_kvpairs(raw)),
             ('age', self.age.to_kvpairs(raw))])
 
+    def size(self):
+        return self.end - self.start
+
 class DamonTarget:
     pid = None
     regions = None
 
     def __init__(self, pid, regions):
         self.pid = pid
         self.regions = regions
@@ -285,36 +298,20 @@
     # every region by default, so that it can be used for monitoring
     def __init__(self, sz_bytes=['min', 'max'],
             nr_accesses=['min', 'max'], nr_accesses_unit=unit_percent,
             age=['min', 'max'], age_unit=unit_usec):
         self.sz_bytes = [_damo_fmt_str.text_to_bytes(sz_bytes[0]),
                 _damo_fmt_str.text_to_bytes(sz_bytes[1])]
 
-        parsers_for_unit = {
-                unit_percent: _damo_fmt_str.text_to_percent,
-                unit_samples: _damo_fmt_str.text_to_nr,
-                unit_usec: _damo_fmt_str.text_to_us,
-                unit_aggr_intervals: _damo_fmt_str.text_to_nr}
-
-        if not nr_accesses_unit in parsers_for_unit:
-            raise Exception('invalid access pattern nr_accesses_unit \'%s\'' %
-                    nr_accesses_unit)
-        if not age_unit in parsers_for_unit:
-            raise Exception('invalid access pattern age_unit \'%s\'' %
-                    age_unit)
-
-        fn = parsers_for_unit[nr_accesses_unit]
         self.nr_acc_min_max = [
-                DamonNrAccesses(fn(nr_accesses[0]), nr_accesses_unit),
-                DamonNrAccesses(fn(nr_accesses[1]), nr_accesses_unit)]
+                DamonNrAccesses(nr_accesses[0], nr_accesses_unit),
+                DamonNrAccesses(nr_accesses[1], nr_accesses_unit)]
         self.nr_accesses_unit = nr_accesses_unit
-        fn = parsers_for_unit[age_unit]
         self.age_min_max = [
-                DamonAge(fn(age[0]), age_unit),
-                DamonAge(fn(age[1]), age_unit)]
+                DamonAge(age[0], age_unit), DamonAge(age[1], age_unit)]
         self.age_unit = age_unit
 
     def to_str(self, raw):
         lines = [
             'sz: [%s, %s]' % (_damo_fmt_str.format_sz(self.sz_bytes[0], raw),
                 _damo_fmt_str.format_sz(self.sz_bytes[1], raw)),
             ]
@@ -639,15 +636,15 @@
             self.tried_regions = []
         self.tried_bytes = 0
         if tried_bytes:
             self.tried_bytes = _damo_fmt_str.text_to_bytes(
                     tried_bytes)
         else:
             for region in self.tried_regions:
-                self.tried_bytes += (region.end - region.start)
+                self.tried_bytes += region.size()
 
     def to_str(self, raw):
         lines = ['action: %s' % self.action]
         lines.append('target access pattern')
         lines.append(_damo_fmt_str.indent_lines(
             self.access_pattern.to_str(raw), 4))
         lines.append('quotas')
```

### Comparing `damo-1.8.9/src/damo/_damon_args.py` & `damo-1.9.0/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damon_dbgfs.py` & `damo-1.9.0/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/_damon_result.py` & `damo-1.9.0/src/damo/_damon_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,34 +21,45 @@
     Contains a snapshot of data access monitoring results
     '''
     start_time = None
     end_time = None
     regions = None
     total_bytes = None
 
-    def __init__(self, start_time, end_time):
+    def update_total_bytes(self):
+        self.total_bytes = sum([r.size() for r in self.regions])
+
+    def __init__(self, start_time, end_time, regions, total_bytes):
         self.start_time = start_time
         self.end_time = end_time
-        self.regions = []
+        self.regions = regions
+        self.total_bytes = total_bytes
+        if self.total_bytes == None:
+            self.update_total_bytes()
 
     @classmethod
     def from_kvpairs(cls, kv):
-        snapshot = DamonSnapshot(_damo_fmt_str.text_to_ns(kv['start_time']),
-                _damo_fmt_str.text_to_ns(kv['end_time']))
-        snapshot.regions = [_damon.DamonRegion.from_kvpairs(r)
-                for r in kv['regions']]
-        return snapshot
+        return DamonSnapshot(
+                _damo_fmt_str.text_to_ns(kv['start_time']),
+                _damo_fmt_str.text_to_ns(kv['end_time']),
+                [_damon.DamonRegion.from_kvpairs(r) for r in kv['regions']],
+                _damo_fmt_str.text_to_bytes(kv['total_bytes'])
+                if 'total_bytes' in kv and kv['total_bytes'] != None
+                else None)
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('start_time', _damo_fmt_str.format_time_ns_exact(
                 self.start_time, raw)),
             ('end_time', _damo_fmt_str.format_time_ns_exact(
                 self.end_time, raw)),
-            ('regions', [r.to_kvpairs() for r in self.regions])])
+            ('regions', [r.to_kvpairs() for r in self.regions]),
+            ('total_bytes', _damo_fmt_str.format_sz(self.total_bytes, raw)
+                if self.total_bytes != None else None),
+            ])
 
 class DamonRecord:
     '''
     Contains data access monitoring results for single target
     '''
     kdamond_idx = None
     context_idx = None
@@ -135,16 +146,15 @@
             add_region(new_regions, region, nr_acc_to_add)
         for region in nr_acc_to_add:
             region.nr_accesses.samples += nr_acc_to_add[region]
             region.nr_accesses.val = region.nr_accesses.samples
             region.nr_accesses.unit = _damon.unit_samples
 
     new_snapshot = DamonSnapshot(snapshots[0].start_time,
-            snapshots[-1].end_time)
-    new_snapshot.regions = new_regions
+            snapshots[-1].end_time, new_regions, None)
     return new_snapshot
 
 def adjusted_snapshots(snapshots, aggregate_interval_us):
     adjusted = []
     to_aggregate = []
     for snapshot in snapshots:
         to_aggregate.append(snapshot)
@@ -178,25 +188,25 @@
         return None
     sec = struct.unpack('l', timebin[0:8])[0]
     nsec = struct.unpack('l', timebin[8:16])[0]
     end_time = sec * 1000000000 + nsec
     return end_time
 
 def read_snapshot_from_record_file(f, start_time, end_time):
-    snapshot = DamonSnapshot(start_time, end_time)
     nr_regions = struct.unpack('I', f.read(4))[0]
+    regions = []
     for r in range(nr_regions):
         start_addr = struct.unpack('L', f.read(8))[0]
         end_addr = struct.unpack('L', f.read(8))[0]
         nr_accesses = struct.unpack('I', f.read(4))[0]
         region = _damon.DamonRegion(start_addr, end_addr,
                 nr_accesses, _damon.unit_samples,
                 None, _damon.unit_aggr_intervals)
-        snapshot.regions.append(region)
-    return snapshot
+        regions.append(region)
+    return DamonSnapshot(start_time, end_time, regions, None)
 
 # if number of snapshots is one and the file type is record or perf script,
 # write_damon_records() adds a fake snapshot for snapshot start time deduction.
 def is_fake_snapshot(snapshot):
     if len(snapshot.regions) != 1:
         return False
     r = snapshot.regions[0]
@@ -313,22 +323,26 @@
             start_time = None
         else:
             start_time = record.snapshots[-1].end_time
             if start_time > end_time:
                 return None, 'trace is not time-sorted'
 
         if snapshot == None:
-            snapshot = DamonSnapshot(start_time, end_time)
+            snapshot = DamonSnapshot(start_time, end_time, [], None)
             record.snapshots.append(snapshot)
         snapshot = record.snapshots[-1]
         snapshot.regions.append(region)
 
         if len(snapshot.regions) == nr_regions:
             snapshot = None
 
+    for record in records:
+        for snapshot in record.snapshots:
+            snapshot.update_total_bytes()
+
     set_first_snapshot_start_time(records)
     return records, None
 
 def set_perf_path(perf_path):
     global PERF
     PERF = perf_path
 
@@ -383,16 +397,20 @@
     if file_type == 'ASCII text':
         with open(result_file, 'r') as f:
             perf_script_output = f.read()
     else:
         # might be perf data
         try:
             with open(os.devnull, 'w') as fnull:
+                # in some setup, perf record file ends up having no proper
+                # ownership.  There's no reason to be strict about that from
+                # damo.  As long as we can, just parse it with '--force'
+                # option.
                 perf_script_output = subprocess.check_output(
-                        [PERF, 'script', '-i', result_file],
+                        [PERF, 'script', '--force', '-i', result_file],
                         stderr=fnull).decode()
         except:
             # Should be record format file
             pass
     if perf_script_output != None:
         return parse_perf_script(perf_script_output, monitoring_intervals)
     return parse_binary_format_record(result_file, monitoring_intervals)
@@ -419,19 +437,19 @@
 
     for record in records:
         snapshots = record.snapshots
         if len(snapshots) != 1:
             continue
         snapshot = snapshots[0]
         snap_duration = snapshot.end_time - snapshot.start_time
-        fake_snapshot = DamonSnapshot(snapshot.end_time,
-                snapshot.end_time + snap_duration)
         # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
-        fake_snapshot.regions = [_damon.DamonRegion(0, 0,
+        fake_regions = [_damon.DamonRegion(0, 0,
             -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
+        fake_snapshot = DamonSnapshot(snapshot.end_time,
+                snapshot.end_time + snap_duration, fake_regions, None)
         snapshots.append(fake_snapshot)
 
 def write_binary(records, file_path, format_version):
     warn_record_type_deprecation()
     add_fake_snapshot_if_needed(records)
 
     with open(file_path, 'wb') as f:
@@ -591,38 +609,52 @@
     if installed:
         err = _damon.commit(kdamonds)
         if err != None:
             return (False, [],
                     'committing scheme installed kdamonds failed: %s' % err)
     return installed, indices, None
 
-def tried_regions_to_snapshot(tried_regions, intervals):
+def tried_regions_to_snapshot(scheme, intervals, merge_regions):
     snapshot_end_time_ns = time.time() * 1000000000
     snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
-    snapshot = DamonSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
+    regions = []
+
+    for tried_region in scheme.tried_regions:
+        '''Merge regions that having same access pattern, since DAMON usually
+        splits regions unnecessarily to keep the min_nr_regions'''
+        if merge_regions and len(regions) > 0:
+            last_region = regions[-1]
+            if (last_region.end == tried_region.start and
+                    last_region.nr_accesses == tried_region.nr_accesses and
+                    last_region.age == tried_region.age):
+                last_region.end = tried_region.end
+                continue
+        regions.append(tried_region)
+    if scheme.tried_bytes != None:
+        total_bytes = scheme.tried_bytes
+    else:
+        total_bytes = None
 
-    for tried_region in tried_regions:
-        snapshot.regions.append(tried_region)
-    return snapshot
+    return DamonSnapshot(snapshot_start_time_ns, snapshot_end_time_ns, regions,
+            total_bytes)
 
-def tried_regions_to_records_of(idxs):
+def tried_regions_to_records_of(idxs, merge_regions):
     '''idxs: list of kdamond/context/scheme indices to get records for.  If it
     is None, return records for all schemes'''
     records = []
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
         for ctx_idx, ctx in enumerate(kdamond.contexts):
             for scheme_idx, scheme in enumerate(ctx.schemes):
                 if not [kdamond_idx, ctx_idx, scheme_idx] in idxs:
                     continue
 
-                snapshot = tried_regions_to_snapshot(scheme.tried_regions,
-                        ctx.intervals)
-                snapshot.total_bytes = scheme.tried_bytes
+                snapshot = tried_regions_to_snapshot(scheme, ctx.intervals,
+                        merge_regions)
 
                 records.append(DamonRecord(kdamond_idx, ctx_idx, ctx.intervals,
                     scheme_idx, None))
                 records[-1].snapshots.append(snapshot)
                 break
     return records
 
@@ -682,15 +714,15 @@
         for ctx in kd.contexts:
             if ctx.ops != 'vaddr':
                 continue
             for target in ctx.targets:
                 target.regions = []
     return err
 
-def get_snapshot_records(access_pattern, total_sz_only):
+def get_snapshot_records(access_pattern, total_sz_only, merge_regions):
     'return DamonRecord objects each having single DamonSnapshot and an error'
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
     orig_kdamonds = _damon.current_kdamonds()
 
@@ -702,15 +734,15 @@
     installed, idxs, err = find_install_scheme(monitor_scheme)
     if err:
         return None, 'monitoring scheme install failed: %s' % err
 
     if total_sz_only:
         err = _damon.update_schemes_tried_bytes(running_kdamond_idxs)
         if err == None:
-            records = tried_regions_to_records_of(idxs)
+            records = tried_regions_to_records_of(idxs, merge_regions)
 
             if installed:
                 err = _damon.commit(orig_kdamonds)
                 if err:
                     return records, 'monitoring scheme uninstall failed: %s' % err
             return records, None
 
@@ -718,34 +750,34 @@
     if err != None:
         if installed:
             err = _damon.commit(orig_kdamonds)
             if err:
                 return None, 'monitoring scheme uninstall failed: %s' % err
         return None, 'updating schemes tried regions fail: %s' % err
 
-    records = tried_regions_to_records_of(idxs)
+    records = tried_regions_to_records_of(idxs, merge_regions)
 
     if installed:
         err = _damon.commit(orig_kdamonds)
         if err:
             return records, 'monitoring scheme uninstall failed: %s' % err
     return records, None
 
-def get_snapshot_records_for_schemes(idxs, total_sz_only):
+def get_snapshot_records_for_schemes(idxs, total_sz_only, merge_regions):
     '''idxs: list of kdamond/context/scheme indices to get records for.
     Return DamonRecord objects each having single DamonSnapshot and an error'''
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
         return None, 'no kdamond running'
 
     if total_sz_only:
         err = _damon.update_schemes_tried_bytes(running_kdamond_idxs)
         if err == None:
-            records = tried_regions_to_records_of(idxs)
+            records = tried_regions_to_records_of(idxs, merge_regions)
             return records, None
 
     err = _damon.update_schemes_tried_regions(running_kdamond_idxs)
     if err != None:
         return None, 'updating schemes tried regions fail: %s' % err
 
-    records = tried_regions_to_records_of(idxs)
+    records = tried_regions_to_records_of(idxs, merge_regions)
     return records, None
```

### Comparing `damo-1.8.9/src/damo/_damon_sysfs.py` & `damo-1.9.0/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo.py` & `damo-1.9.0/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_adjust.py` & `damo-1.9.0/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_convert_record_format.py` & `damo-1.9.0/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_features.py` & `damo-1.9.0/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_fmt_json.py` & `damo-1.9.0/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_heats.py` & `damo-1.9.0/src/damo/damo_heats.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_lru_sort.py` & `damo-1.9.0/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_monitor.py` & `damo-1.9.0/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_nr_regions.py` & `damo-1.9.0/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_reclaim.py` & `damo-1.9.0/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_record.py` & `damo-1.9.0/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_record_info.py` & `damo-1.9.0/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_report.py` & `damo-1.9.0/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_report_raw.py` & `damo-1.9.0/src/damo/damo_report_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,16 @@
             print('target_id: %s' % record.target_id)
             print('nr_regions: %s' % len(snapshot.regions))
             print('# %10s %12s  %12s  %11s %5s' %
                     ('start_addr', 'end_addr', 'length', 'nr_accesses', 'age'))
             for r in snapshot.regions:
                 print("%012x-%012x (%12s) %11d %5d" %
                         (r.start, r.end,
-                            _damo_fmt_str.format_sz(r.end - r.start,
-                                args.raw_number), r.nr_accesses.samples,
-                                r.age.aggr_intervals
+                            _damo_fmt_str.format_sz(r.size(), args.raw_number),
+                            r.nr_accesses.samples, r.age.aggr_intervals
                                 if r.age.aggr_intervals != None else -1))
             print('')
 
 def set_argparser(parser):
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
     parser.add_argument('--duration', type=float, metavar='<seconds>', nargs=2,
```

### Comparing `damo-1.8.9/src/damo/damo_schemes.py` & `damo-1.9.0/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_show.py` & `damo-1.9.0/src/damo/damo_show.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,82 @@
 import os
 
 import _damo_fmt_str
 import _damon
 import _damon_args
 import _damon_result
 
+record_formatters = {
+        '<kdamond index>': lambda record, raw:
+            '%s' % record.kdamond_idx,
+        '<context index>': lambda record, raw:
+            '%s' % record.context_idx,
+        '<scheme index>': lambda record, raw:
+            '%s' % record.scheme_idx,
+        '<target id>': lambda record, raw:
+            '%s' % record.target_id,
+        '<record start abs time>': lambda record, raw:
+            _dmo_fmt_str.format_ns(record.snapshots[0].start_time, raw),
+        '<record duration>': lambda record, raw:
+            _damo_fmt_str.format_time_ns(
+                record.snapshots[-1].end_time - record.snapshots[0].start_time,
+                raw)
+            }
+
+snapshot_formatters = {
+        '<total bytes>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_sz(snapshot.total_bytes, raw),
+        '<monitor duration>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_time_ns(
+                snapshot.end_time - snapshot.start_time, raw),
+        '<monitor start time>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_time_ns(
+                snapshot.start_time - record.snapshots[0].start_time, raw),
+        '<monitor end time>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_time_ns(
+                snapshot.end_time - record.snapshots[0].start_time, raw),
+        '<monitor start abs time>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_time_ns(snapshot.start_time, raw),
+        '<monitor end abs time>': lambda snapshot, record, raw:
+            _damo_fmt_str.format_time_ns(snapshot.end_time, raw),
+            }
+
+region_formatters = {
+        '<index>': lambda index, region, raw:
+            _damo_fmt_str.format_nr(index, raw),
+        '<start address>': lambda index, region, raw:
+            _damo_fmt_str.format_sz(region.start, raw),
+        '<end address>': lambda index, region, raw:
+            _damo_fmt_str.format_sz(region.end, raw),
+        '<region size>': lambda index, region, raw:
+            _damo_fmt_str.format_sz(region.size(), raw),
+        '<access rate>': lambda index, region, raw:
+            _damo_fmt_str.format_percent(region.nr_accesses.percent, raw),
+        '<age>': lambda index, region, raw:
+            _damo_fmt_str.format_time_us(region.age.usec, raw)
+        }
+
+formatters = {
+        'record': record_formatters,
+        'snapshot': snapshot_formatters,
+        'region': region_formatters
+        }
+
+def __age_size_heat_box(region, record,
+        usec_per_column, bytes_per_row, nr_per_access_rate_percent):
+    '''
+    Generate a string that represents a box.  The box represents age, size, and
+    heat of the region with length (number of columns), height (number of
+    rows), and number, respectively.
+    '''
+    nr_columns = int(region.age.usec / usec_per_column)
+    nr_rows = int(region.size() / bytes_per_row)
+    heat_nr = int(region.nr_accesses.percent / nr_per_access_rate_percent)
+    return '\n'.join([('%d' % heat_nr) * nr_columns] * nr_rows)
+
 def apply_min_chars(min_chars, field_name, txt):
     # min_chars: [[<field name>, <number of min chars>]...]
     for name, nr in min_chars:
         try:
             nr = int(nr)
         except:
             print('wrong min_chars: %s' % min_chars)
@@ -20,90 +88,31 @@
         if name == field_name:
             if len(txt) >= nr:
                 return txt
             txt += ' ' * (nr - len(txt))
             return txt
     return txt
 
-def format_field(min_chars, field_name, index, region, snapshot, record, raw):
-    if field_name == '<index>':
-        txt = _damo_fmt_str.format_nr(index, raw)
-    elif field_name == '<start address>':
-        txt = _damo_fmt_str.format_sz(region.start, raw)
-    elif field_name == '<end address>':
-        txt = _damo_fmt_str.format_sz(region.end, raw)
-    elif field_name == '<region size>':
-        txt = _damo_fmt_str.format_sz(region.end - region.start, raw)
-    elif field_name == '<access rate>':
-        txt = _damo_fmt_str.format_percent(region.nr_accesses.percent, raw)
-    elif field_name == '<age>':
-        txt = _damo_fmt_str.format_time_us(region.age.usec, raw)
-    elif field_name == '<total bytes>':
-        if snapshot.total_bytes == None:
-            snapshot.total_bytes = sum([r.end - r.start
-                for r in snapshot.regions])
-        txt = _damo_fmt_str.format_sz(snapshot.total_bytes, raw)
-    elif field_name == '<monitor duration>':
-        txt = _damo_fmt_str.format_time_ns(
-                snapshot.end_time - snapshot.start_time, raw)
-    elif field_name == '<monitor start time>':
-        base_time = record.snapshots[0].start_time
-        txt = _damo_fmt_str.format_time_ns(
-                snapshot.start_time - base_time, raw)
-    elif field_name == '<monitor end time>':
-        base_time = record.snapshots[0].start_time
-        txt = _damo_fmt_str.format_time_ns(snapshot.end_time - base_time, raw)
-    elif field_name == '<monitor start abs time>':
-        txt = _damo_fmt_str.format_time_ns(snapshot.start_time, raw)
-    elif field_name == '<monitor end abs time>':
-        txt = _damo_fmt_str.format_time_ns(snapshot.end_time, raw)
-    elif field_name == '<kdamond index>':
-        txt = '%s' % record.kdamond_idx
-    elif field_name == '<context index>':
-        txt = '%s' % record.context_idx
-    elif field_name == '<scheme index>':
-        txt = '%s' % record.scheme_idx
-    elif field_name == '<target id>':
-        txt = '%s' % record.target_id
-    elif field_name == '<record start abs time>':
-        txt = _damo_fmt_str.format_time_ns(record.snapshots[0].start_time, raw)
-    elif field_name == '<record duration>':
-        txt = _damo_fmt_str.format_time_ns(
-                record.snapshots[-1].end_time - record.snapshots[0].start_time,
-                raw)
-    else:
-        print(field_name)
-        raise(Exception)
-
-    return apply_min_chars(min_chars, field_name, txt)
-
-def format_pretty(template, min_chars, index, region, snapshot, record, raw):
-    for field_name in [
-            # for region pretty
-            '<index>', '<start address>', '<end address>', '<region size>',
-            '<access rate>', '<age>',
-            # for snapshot pretty
-            '<total bytes>', '<monitor duration>',
-            '<monitor start time>', '<monitor end time>',
-            '<monitor start abs time>', '<monitor end abs time>',
-            # for record pretty
-            '<kdamond index>', '<context index>', '<scheme index>',
-            '<target id>', '<record start abs time>', '<record duration>']:
-        if template.find(field_name) == -1:
-            continue
-        template = template.replace(field_name, format_field(min_chars,
-            field_name, index, region, snapshot, record, raw))
-    template = template.replace('\\n', '\n')
-    return template
-
 def format_pr(template, min_chars, index, region, snapshot, record, raw):
     if template == '':
         return
-    print(format_pretty(template, min_chars, index, region, snapshot, record,
-        raw))
+    for category, category_formatters in formatters.items():
+        for field_name, formatter in category_formatters.items():
+            if template.find(field_name) == -1:
+                continue
+            if category == 'record':
+                txt = formatter(record, raw)
+            elif category == 'snapshot':
+                txt = formatter(snapshot, record, raw)
+            elif category == 'region':
+                txt = formatter(index, region, raw)
+            txt = apply_min_chars(min_chars, field_name, txt)
+            template = template.replace(field_name, txt)
+    template = template.replace('\\n', '\n')
+    print(template)
 
 def set_formats(args, records):
     if args.format_record_head == None:
         if len(records) > 1:
             args.format_record_head = 'kdamond <kdamond index> / context <context index> / scheme <scheme index> / target id <target id> / recorded for <record duration> from <record start abs time>'
         else:
             args.format_record_head = ''
@@ -128,15 +137,15 @@
         if field == 'address':
             regions = sorted(regions, key=lambda r: r.start)
         elif field == 'access_rate':
             regions = sorted(regions, key=lambda r: r.nr_accesses.percent)
         elif field == 'age':
             regions = sorted(regions, key=lambda r: r.age.usec)
         elif field == 'size':
-            regions = sorted(regions, key=lambda r: r.end - r.start)
+            regions = sorted(regions, key=lambda r: r.size())
     return regions
 
 def pr_records(args, records):
     if args.json:
         print(json.dumps([r.to_kvpairs(args.raw_number)
             for r in records], indent=4))
         exit(0)
@@ -170,15 +179,15 @@
     sz_bytes = access_pattern.sz_bytes
     nr_acc = access_pattern.nr_acc_min_max
     age = access_pattern.age_min_max
 
     for snapshot in record.snapshots:
         filtered = []
         for region in snapshot.regions:
-            sz = region.end - region.start
+            sz = region.size()
             if sz < sz_bytes[0] or sz_bytes[1] < sz:
                 continue
             intervals = record.intervals
             if intervals == None:
                 filtered.append(region)
                 continue
             region.nr_accesses.add_unset_unit(intervals)
@@ -213,42 +222,45 @@
             metavar=('<kdamond idx>', '<context idx>', '<scheme idx>'),
             help='show tried regions of given schemes')
 
     # how to show
 
     # don't set default for record head and snapshot head because it depends on
     # given number of record and snapshots.  Decide those in set_formats().
-    parser.add_argument('--format_record_head',
+    parser.add_argument('--format_record_head', metavar='<template>',
             help='record output head format')
-    parser.add_argument('--format_record_tail', default='',
+    parser.add_argument('--format_record_tail', metavar='<template>',
+            default='',
             help='record output tail format')
-    parser.add_argument('--format_snapshot_head',
+    parser.add_argument('--format_snapshot_head', metavar='<template>',
             help='snapshot output tail format')
-    parser.add_argument('--format_snapshot_tail',
+    parser.add_argument('--format_snapshot_tail', metavar='<template>',
             default='total size: <total bytes>',
             help='snapshot output tail format')
-    parser.add_argument('--format_region',
+    parser.add_argument('--format_region', metavar='<template>',
             default='<index> addr [<start address>, <end address>) (<region size>) access <access rate> age <age>',
             help='region output format')
     parser.add_argument('--min_chars_field', nargs=2,
-            metavar=('<field name> <number>'), action='append',
+            metavar=('<field name>', '<number>'), action='append',
             default=[['<index>', 3],
                 ['<start address>', 12],['<end address>', 11],
                 ['<region size>', 11], ['<access rate>', 5]],
             help='minimum character for each field')
     parser.add_argument('--total_sz_only', action='store_true',
             help='print only total size of the regions')
     parser.add_argument('--raw_number', action='store_true',
             help='use machine-friendly raw numbers')
     parser.add_argument('--json', action='store_true',
             help='print in json format')
     parser.add_argument('--sort_regions_by',
             choices=['address', 'access_rate', 'age', 'size'], nargs='+',
             default=['address'],
             help='fields to sort regions by')
+    parser.add_argument('--dont_merge_regions', action='store_true',
+            help='don\'t merge contiguous regions of same access pattern')
 
     parser.description='Show DAMON-monitored access pattern'
     parser.epilog='If --input_file is not provided, capture snapshot'
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
@@ -259,15 +271,15 @@
             args.access_rate, _damon.unit_percent, args.age * 1000000,
             _damon.unit_usec)
 
     if args.input_file == None and args.tried_regions_of == None:
         _damon.ensure_root_and_initialized(args)
 
         records, err = _damon_result.get_snapshot_records(access_pattern,
-                args.total_sz_only)
+                args.total_sz_only, not args.dont_merge_regions)
         if err != None:
             print(err)
             exit(1)
     elif args.input_file != None:
         if not os.path.isfile(args.input_file):
             print('--input_file (%s) is not file' % args.input_file)
             exit(1)
@@ -279,15 +291,16 @@
             exit(1)
         for record in records:
             filter_by_pattern(record, access_pattern)
     elif args.tried_regions_of != None:
         _damon.ensure_root_and_initialized(args)
 
         records, err = _damon_result.get_snapshot_records_for_schemes(
-                args.tried_regions_of, args.total_sz_only)
+                args.tried_regions_of, args.total_sz_only,
+                not args.dont_merge_regions)
         if err != None:
             print(err)
             exit(1)
 
     for record in records:
         try:
             pr_records(args, records)
```

### Comparing `damo-1.8.9/src/damo/damo_start.py` & `damo-1.9.0/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_stat.py` & `damo-1.9.0/src/damo/damo_stat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import signal
 import time
 
+import _damo_deprecation_notice
 import _damo_subcmds
 import _damon
 import _damon_args
 import damo_stat_kdamonds
 import damo_stat_regions
 import damo_stat_schemes
 
@@ -60,14 +61,17 @@
     while args.count == 0 or i < args.count:
         func(args)
         if i != args.count - 1:
             time.sleep(args.delay)
         i += 1
 
 def main(args=None):
+    _damo_deprecation_notice.deprecated('\'damo stat\'', 'next week',
+            do_exit=False, exit_code=1,
+            additional_notice='Use \'damo status\' or \'damo show\' instead')
     if not args:
         parser = set_argparser(None)
         args = parser.parse_args()
 
     for subcmd in subcmds:
         if subcmd.name == args.stat_type:
             subcmd.execute(args)
```

### Comparing `damo-1.8.9/src/damo/damo_stat_kdamonds.py` & `damo-1.9.0/src/damo/damo_stat_kdamonds.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 
-import _damo_deprecation_notice
 import _damo_fmt_str
 import _damon
 import damo_stat
 import damo_status
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
@@ -19,17 +18,14 @@
 def __main(args):
     if not args.detail:
         damo_status.update_pr_kdamonds_summary(args.json, args.raw)
     else:
         damo_status.update_pr_kdamonds(args.json, args.raw)
 
 def main(args=None):
-    _damo_deprecation_notice.will_be_deprecated('\'damo stat kdamonds\'',
-            'near future', 'Use \'damo status\' instead')
-
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.9/src/damo/damo_stat_regions.py` & `damo-1.9.0/src/damo/damo_stat_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
-import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 import _damon_result
 import damo_stat
 
 def priority(region, weights):
@@ -22,22 +21,22 @@
         regions.sort(key=lambda region: priority(region, prio_weights))
 
     total_sz = 0
     for region in regions:
         if not size_only:
             print(region.to_str(raw_nr, intervals))
         else:
-            total_sz += (region.end - region.start)
+            total_sz += region.size()
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
 
 def update_pr_schemes_tried_regions(access_pattern, size_only, sortby,
         prio_weights, raw_nr):
     records, err = _damon_result.get_snapshot_records(access_pattern,
-            total_sz_only=False)
+            total_sz_only=False, merge_regions=False)
     if err != None:
         print(err)
     if records == None:
         return
 
     for record in records:
         print('kdamond %s ctx %s' % (record.kdamond_idx, record.context_idx))
@@ -66,16 +65,14 @@
             help='priority weights for priority calculation')
 
 def __main(args):
     update_pr_schemes_tried_regions(args.access_pattern, args.size_only,
             args.sortby, args.priority_weights, args.raw)
 
 def main(args=None):
-    _damo_deprecation_notice.will_be_deprecated('\'damo stat regions\'',
-            'near future', 'Use \'damo show\' instead')
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.9/src/damo/damo_stat_schemes.py` & `damo-1.9.0/src/damo/damo_stat_schemes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
-import _damo_deprecation_notice
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 import damo_stat
 import damo_status
 
 def set_argparser(parser):
@@ -15,16 +14,14 @@
 def __main(args):
     if args.stat_type == 'schemes_stats':
         damo_status.update_pr_schemes_stats(args.raw)
     elif args.stat_type == 'schemes_tried_regions':
         damo_status.update_pr_schemes_tried_regions(args.raw)
 
 def main(args=None):
-    _damo_deprecation_notice.will_be_deprecated('\'damo stat schemes*\'',
-            'near future', 'Use \'damo status\' instead')
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_and_initialized(args)
```

### Comparing `damo-1.8.9/src/damo/damo_status.py` & `damo-1.9.0/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_stop.py` & `damo-1.9.0/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_translate_damos.py` & `damo-1.9.0/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_tune.py` & `damo-1.9.0/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_validate.py` & `damo-1.9.0/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.9/src/damo/damo_wss.py` & `damo-1.9.0/src/damo/damo_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         wss_dist = []
         for snapshot in record.snapshots:
             wss = 0
             for r in snapshot.regions:
                 # Ignore regions not fulfill working set conditions
                 if r.nr_accesses.samples < acc_thres:
                     continue
-                if r.end - r.start < sz_thres:
+                if r.size() < sz_thres:
                     continue
-                wss += r.end - r.start
+                wss += r.size()
             wss_dist.append(wss)
         if do_sort:
             wss_dist.sort(reverse=False)
         wss_dists[record.target_id] = wss_dist
     return wss_dists
 
 def pr_wss_dists(wss_dists, percentiles, raw_number, nr_cols_bar, pr_all_wss):
```

### Comparing `damo-1.8.9/src/damo.egg-info/PKG-INFO` & `damo-1.9.0/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.9
+Version: 1.9.0
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.9/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.0/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.9/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.0/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.8.9/src/damo.egg-info/SOURCES.txt` & `damo-1.9.0/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

