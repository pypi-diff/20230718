# Comparing `tmp/labml-0.4.98.tar.gz` & `tmp/labml-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/labml-0.4.98.tar", last modified: Thu Jan 28 02:23:13 2021, max compression
+gzip compressed data, was "dist/labml-0.4.99.tar", last modified: Thu Jan 28 02:30:34 2021, max compression
```

## Comparing `labml-0.4.98.tar` & `labml-0.4.99.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/
--rw-r--r--   0 varuna     (501) staff       (20)       19 2020-06-05 09:45:19.000000 labml-0.4.98/MANIFEST.in
--rw-r--r--   0 varuna     (501) staff       (20)     6542 2021-01-28 02:23:13.000000 labml-0.4.98/PKG-INFO
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/
--rw-r--r--   0 varuna     (501) staff       (20)       23 2021-01-28 02:22:57.000000 labml-0.4.98/labml/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/analytics/
--rw-r--r--   0 varuna     (501) staff       (20)    16617 2020-10-29 01:38:06.000000 labml-0.4.98/labml/analytics/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      662 2020-06-05 09:45:19.000000 labml-0.4.98/labml/analytics/matplotlib.py
--rw-r--r--   0 varuna     (501) staff       (20)     4221 2021-01-12 09:10:41.000000 labml-0.4.98/labml/cli.py
--rw-r--r--   0 varuna     (501) staff       (20)     6243 2020-11-14 04:46:19.000000 labml-0.4.98/labml/configs.py
--rw-r--r--   0 varuna     (501) staff       (20)    11739 2021-01-28 02:22:57.000000 labml-0.4.98/labml/experiment.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/
--rw-r--r--   0 varuna     (501) staff       (20)       92 2020-12-10 02:22:40.000000 labml-0.4.98/labml/internal/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/analytics/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/analytics/altair/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/altair/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3877 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/altair/binned_heatmap.py
--rw-r--r--   0 varuna     (501) staff       (20)     4116 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/altair/density.py
--rw-r--r--   0 varuna     (501) staff       (20)     5069 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/altair/density_multi.py
--rw-r--r--   0 varuna     (501) staff       (20)     1261 2020-06-14 04:30:33.000000 labml-0.4.98/labml/internal/analytics/altair/histogram.py
--rw-r--r--   0 varuna     (501) staff       (20)     4428 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/altair/scatter.py
--rw-r--r--   0 varuna     (501) staff       (20)      250 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/altair/utils.py
--rw-r--r--   0 varuna     (501) staff       (20)      924 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/analytics.py
--rw-r--r--   0 varuna     (501) staff       (20)     5396 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/cache.py
--rw-r--r--   0 varuna     (501) staff       (20)     5532 2020-06-29 04:44:18.000000 labml-0.4.98/labml/internal/analytics/indicators.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/analytics/matplotlib/
--rw-r--r--   0 varuna     (501) staff       (20)      667 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/matplotlib/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2628 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/matplotlib/tb.py
--rw-r--r--   0 varuna     (501) staff       (20)     1410 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/sqlite.py
--rw-r--r--   0 varuna     (501) staff       (20)     2033 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/analytics/tensorboard.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/api/
--rw-r--r--   0 varuna     (501) staff       (20)     7226 2021-01-12 08:52:24.000000 labml-0.4.98/labml/internal/api/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3110 2021-01-02 08:22:16.000000 labml-0.4.98/labml/internal/api/experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)     2981 2020-12-21 03:50:41.000000 labml-0.4.98/labml/internal/api/logs.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/computer/
--rw-r--r--   0 varuna     (501) staff       (20)       27 2021-01-12 08:59:29.000000 labml-0.4.98/labml/internal/computer/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2545 2021-01-12 09:13:46.000000 labml-0.4.98/labml/internal/computer/configs.py
--rw-r--r--   0 varuna     (501) staff       (20)     5404 2021-01-28 02:22:57.000000 labml-0.4.98/labml/internal/computer/monitor.py
--rw-r--r--   0 varuna     (501) staff       (20)     1575 2021-01-28 02:22:57.000000 labml-0.4.98/labml/internal/computer/process.py
--rw-r--r--   0 varuna     (501) staff       (20)     3796 2020-12-29 04:30:26.000000 labml-0.4.98/labml/internal/computer/writer.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/configs/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.98/labml/internal/configs/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)    18506 2021-01-25 12:02:12.000000 labml-0.4.98/labml/internal/configs/base.py
--rw-r--r--   0 varuna     (501) staff       (20)     4910 2020-11-14 04:46:19.000000 labml-0.4.98/labml/internal/configs/config_function.py
--rw-r--r--   0 varuna     (501) staff       (20)      834 2020-09-29 11:33:48.000000 labml-0.4.98/labml/internal/configs/config_item.py
--rw-r--r--   0 varuna     (501) staff       (20)      223 2020-11-14 04:46:19.000000 labml-0.4.98/labml/internal/configs/eval_function.py
--rw-r--r--   0 varuna     (501) staff       (20)     2869 2020-11-14 04:46:19.000000 labml-0.4.98/labml/internal/configs/processor.py
--rw-r--r--   0 varuna     (501) staff       (20)     4622 2020-11-14 04:46:19.000000 labml-0.4.98/labml/internal/configs/utils.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/experiment/
--rw-r--r--   0 varuna     (501) staff       (20)    16968 2021-01-12 08:51:32.000000 labml-0.4.98/labml/internal/experiment/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)    12845 2021-01-28 02:22:57.000000 labml-0.4.98/labml/internal/experiment/experiment_run.py
--rw-r--r--   0 varuna     (501) staff       (20)     2194 2020-07-06 12:38:31.000000 labml-0.4.98/labml/internal/experiment/pytorch.py
--rw-r--r--   0 varuna     (501) staff       (20)      822 2020-07-06 12:38:31.000000 labml-0.4.98/labml/internal/experiment/sklearn.py
--rw-r--r--   0 varuna     (501) staff       (20)      489 2020-11-07 04:56:54.000000 labml-0.4.98/labml/internal/experiment/watcher.py
--rw-r--r--   0 varuna     (501) staff       (20)     6711 2021-01-15 17:31:39.000000 labml-0.4.98/labml/internal/lab.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/logger/
--rw-r--r--   0 varuna     (501) staff       (20)      948 2020-12-22 02:46:11.000000 labml-0.4.98/labml/internal/logger/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/logger/destinations/
--rw-r--r--   0 varuna     (501) staff       (20)      294 2020-11-27 03:09:18.000000 labml-0.4.98/labml/internal/logger/destinations/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1553 2020-12-22 02:48:39.000000 labml-0.4.98/labml/internal/logger/destinations/console.py
--rw-r--r--   0 varuna     (501) staff       (20)      707 2020-12-22 02:49:21.000000 labml-0.4.98/labml/internal/logger/destinations/factory.py
--rw-r--r--   0 varuna     (501) staff       (20)     3230 2020-12-22 03:14:00.000000 labml-0.4.98/labml/internal/logger/destinations/ipynb.py
--rw-r--r--   0 varuna     (501) staff       (20)     2546 2020-12-22 03:15:47.000000 labml-0.4.98/labml/internal/logger/destinations/ipynb_pycharm.py
--rw-r--r--   0 varuna     (501) staff       (20)     8450 2020-11-08 09:14:49.000000 labml-0.4.98/labml/internal/logger/inspect.py
--rw-r--r--   0 varuna     (501) staff       (20)      147 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/logger/types.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/manage/
--rw-r--r--   0 varuna     (501) staff       (20)        0 2020-11-07 07:42:56.000000 labml-0.4.98/labml/internal/manage/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2799 2020-11-07 07:59:10.000000 labml-0.4.98/labml/internal/manage/process.py
--rw-r--r--   0 varuna     (501) staff       (20)     1747 2021-01-28 02:22:57.000000 labml-0.4.98/labml/internal/manage/runs.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/monitor/
--rw-r--r--   0 varuna     (501) staff       (20)     8045 2020-12-28 06:01:49.000000 labml-0.4.98/labml/internal/monitor/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     2601 2020-11-07 02:29:49.000000 labml-0.4.98/labml/internal/monitor/iterator.py
--rw-r--r--   0 varuna     (501) staff       (20)     4451 2020-11-07 02:19:05.000000 labml-0.4.98/labml/internal/monitor/loop.py
--rw-r--r--   0 varuna     (501) staff       (20)     3372 2020-12-28 06:00:02.000000 labml-0.4.98/labml/internal/monitor/mix.py
--rw-r--r--   0 varuna     (501) staff       (20)     8403 2020-12-21 05:41:47.000000 labml-0.4.98/labml/internal/monitor/sections.py
--rw-r--r--   0 varuna     (501) staff       (20)      606 2020-08-28 10:35:43.000000 labml-0.4.98/labml/internal/track_debug.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/tracker/
--rw-r--r--   0 varuna     (501) staff       (20)     7308 2021-01-05 14:25:35.000000 labml-0.4.98/labml/internal/tracker/__init__.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/tracker/indicators/
--rw-r--r--   0 varuna     (501) staff       (20)      808 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/indicators/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1368 2020-12-06 16:06:33.000000 labml-0.4.98/labml/internal/tracker/indicators/aggregate.py
--rw-r--r--   0 varuna     (501) staff       (20)     5515 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/indicators/artifacts.py
--rw-r--r--   0 varuna     (501) staff       (20)     1820 2020-12-06 16:06:33.000000 labml-0.4.98/labml/internal/tracker/indicators/factory.py
--rw-r--r--   0 varuna     (501) staff       (20)     1716 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/indicators/indexed.py
--rw-r--r--   0 varuna     (501) staff       (20)     2726 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/indicators/numeric.py
--rw-r--r--   0 varuna     (501) staff       (20)      429 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/namespace.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/tracker/writers/
--rw-r--r--   0 varuna     (501) staff       (20)      441 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/writers/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3927 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/writers/file.py
--rw-r--r--   0 varuna     (501) staff       (20)     4794 2021-01-20 17:20:18.000000 labml-0.4.98/labml/internal/tracker/writers/screen.py
--rw-r--r--   0 varuna     (501) staff       (20)     3598 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/writers/sqlite.py
--rw-r--r--   0 varuna     (501) staff       (20)     1499 2020-11-06 14:29:30.000000 labml-0.4.98/labml/internal/tracker/writers/tensorboard.py
--rw-r--r--   0 varuna     (501) staff       (20)     3334 2021-01-20 17:20:18.000000 labml-0.4.98/labml/internal/tracker/writers/web_api.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/util/
--rw-r--r--   0 varuna     (501) staff       (20)     1493 2021-01-15 17:04:32.000000 labml-0.4.98/labml/internal/util/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     3427 2020-11-01 09:14:27.000000 labml-0.4.98/labml/internal/util/colors.py
--rw-r--r--   0 varuna     (501) staff       (20)      958 2020-10-25 05:22:57.000000 labml-0.4.98/labml/internal/util/strings.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/internal/util/tensorboard_writer/
--rw-r--r--   0 varuna     (501) staff       (20)     1323 2021-01-15 17:08:47.000000 labml-0.4.98/labml/internal/util/tensorboard_writer/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)     1346 2020-11-19 10:12:43.000000 labml-0.4.98/labml/internal/util/tensorboard_writer/pytorch.py
--rw-r--r--   0 varuna     (501) staff       (20)     1355 2020-10-29 01:38:06.000000 labml-0.4.98/labml/internal/util/tensorboard_writer/tensorflow.py
--rw-r--r--   0 varuna     (501) staff       (20)      670 2020-10-25 05:34:38.000000 labml-0.4.98/labml/internal/util/values.py
--rw-r--r--   0 varuna     (501) staff       (20)      786 2020-11-07 08:54:19.000000 labml-0.4.98/labml/lab.py
--rw-r--r--   0 varuna     (501) staff       (20)     4364 2020-11-27 03:11:54.000000 labml-0.4.98/labml/logger.py
--rw-r--r--   0 varuna     (501) staff       (20)      556 2020-11-07 07:58:52.000000 labml-0.4.98/labml/manage.py
--rw-r--r--   0 varuna     (501) staff       (20)     4102 2020-12-28 06:02:56.000000 labml-0.4.98/labml/monit.py
--rw-r--r--   0 varuna     (501) staff       (20)     5518 2020-12-16 15:22:31.000000 labml-0.4.98/labml/tracker.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml/utils/
--rw-r--r--   0 varuna     (501) staff       (20)      879 2021-01-15 17:31:24.000000 labml-0.4.98/labml/utils/__init__.py
--rw-r--r--   0 varuna     (501) staff       (20)      790 2020-12-31 03:57:47.000000 labml-0.4.98/labml/utils/cache.py
--rw-r--r--   0 varuna     (501) staff       (20)     1071 2020-06-05 09:45:19.000000 labml-0.4.98/labml/utils/delayed_keyboard_interrupt.py
--rw-r--r--   0 varuna     (501) staff       (20)      454 2021-01-23 10:24:47.000000 labml-0.4.98/labml/utils/download.py
--rw-r--r--   0 varuna     (501) staff       (20)       43 2020-06-05 09:45:19.000000 labml-0.4.98/labml/utils/errors.py
--rw-r--r--   0 varuna     (501) staff       (20)     1112 2020-10-29 01:38:06.000000 labml-0.4.98/labml/utils/keras.py
--rw-r--r--   0 varuna     (501) staff       (20)     1368 2020-12-21 15:19:26.000000 labml-0.4.98/labml/utils/lightning.py
--rw-r--r--   0 varuna     (501) staff       (20)      704 2020-10-29 01:38:06.000000 labml-0.4.98/labml/utils/notice.py
--rw-r--r--   0 varuna     (501) staff       (20)     2549 2020-12-22 05:42:28.000000 labml-0.4.98/labml/utils/pytorch.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/labml.egg-info/
--rw-r--r--   0 varuna     (501) staff       (20)     6542 2021-01-28 02:23:12.000000 labml-0.4.98/labml.egg-info/PKG-INFO
--rw-r--r--   0 varuna     (501) staff       (20)     3601 2021-01-28 02:23:13.000000 labml-0.4.98/labml.egg-info/SOURCES.txt
--rw-r--r--   0 varuna     (501) staff       (20)        1 2021-01-28 02:23:12.000000 labml-0.4.98/labml.egg-info/dependency_links.txt
--rw-r--r--   0 varuna     (501) staff       (20)       42 2021-01-28 02:23:12.000000 labml-0.4.98/labml.egg-info/entry_points.txt
--rw-r--r--   0 varuna     (501) staff       (20)       23 2021-01-28 02:23:12.000000 labml-0.4.98/labml.egg-info/requires.txt
--rw-r--r--   0 varuna     (501) staff       (20)        6 2021-01-28 02:23:12.000000 labml-0.4.98/labml.egg-info/top_level.txt
--rw-r--r--   0 varuna     (501) staff       (20)       38 2021-01-28 02:23:13.000000 labml-0.4.98/setup.cfg
--rw-r--r--   0 varuna     (501) staff       (20)     1545 2021-01-15 17:03:52.000000 labml-0.4.98/setup.py
-drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:23:13.000000 labml-0.4.98/test/
--rw-r--r--   0 varuna     (501) staff       (20)      300 2021-01-02 08:08:13.000000 labml-0.4.98/test/test_experiment.py
--rw-r--r--   0 varuna     (501) staff       (20)      549 2020-07-12 14:36:26.000000 labml-0.4.98/test/test_inspect.py
--rw-r--r--   0 varuna     (501) staff       (20)      531 2020-12-08 08:14:23.000000 labml-0.4.98/test/test_tracker.py
--rw-r--r--   0 varuna     (501) staff       (20)      556 2020-08-31 08:27:27.000000 labml-0.4.98/test/test_watcher.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/
+-rw-r--r--   0 varuna     (501) staff       (20)       19 2020-06-05 09:45:19.000000 labml-0.4.99/MANIFEST.in
+-rw-r--r--   0 varuna     (501) staff       (20)     6542 2021-01-28 02:30:34.000000 labml-0.4.99/PKG-INFO
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/
+-rw-r--r--   0 varuna     (501) staff       (20)       23 2021-01-28 02:30:29.000000 labml-0.4.99/labml/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/analytics/
+-rw-r--r--   0 varuna     (501) staff       (20)    16617 2020-10-29 01:38:06.000000 labml-0.4.99/labml/analytics/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      662 2020-06-05 09:45:19.000000 labml-0.4.99/labml/analytics/matplotlib.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4221 2021-01-12 09:10:41.000000 labml-0.4.99/labml/cli.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6243 2020-11-14 04:46:19.000000 labml-0.4.99/labml/configs.py
+-rw-r--r--   0 varuna     (501) staff       (20)    11739 2021-01-28 02:22:57.000000 labml-0.4.99/labml/experiment.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/
+-rw-r--r--   0 varuna     (501) staff       (20)       92 2020-12-10 02:22:40.000000 labml-0.4.99/labml/internal/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/analytics/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/analytics/altair/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/altair/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3877 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/altair/binned_heatmap.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4116 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/altair/density.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5069 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/altair/density_multi.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1261 2020-06-14 04:30:33.000000 labml-0.4.99/labml/internal/analytics/altair/histogram.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4428 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/altair/scatter.py
+-rw-r--r--   0 varuna     (501) staff       (20)      250 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/altair/utils.py
+-rw-r--r--   0 varuna     (501) staff       (20)      924 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/analytics.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5396 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/cache.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5532 2020-06-29 04:44:18.000000 labml-0.4.99/labml/internal/analytics/indicators.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/analytics/matplotlib/
+-rw-r--r--   0 varuna     (501) staff       (20)      667 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/matplotlib/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2628 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/matplotlib/tb.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1410 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/sqlite.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2033 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/analytics/tensorboard.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/api/
+-rw-r--r--   0 varuna     (501) staff       (20)     7226 2021-01-12 08:52:24.000000 labml-0.4.99/labml/internal/api/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3110 2021-01-02 08:22:16.000000 labml-0.4.99/labml/internal/api/experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2981 2020-12-21 03:50:41.000000 labml-0.4.99/labml/internal/api/logs.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/computer/
+-rw-r--r--   0 varuna     (501) staff       (20)       27 2021-01-12 08:59:29.000000 labml-0.4.99/labml/internal/computer/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2545 2021-01-12 09:13:46.000000 labml-0.4.99/labml/internal/computer/configs.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5404 2021-01-28 02:22:57.000000 labml-0.4.99/labml/internal/computer/monitor.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1575 2021-01-28 02:22:57.000000 labml-0.4.99/labml/internal/computer/process.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3796 2020-12-29 04:30:26.000000 labml-0.4.99/labml/internal/computer/writer.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/configs/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-06-05 09:45:19.000000 labml-0.4.99/labml/internal/configs/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    18506 2021-01-25 12:02:12.000000 labml-0.4.99/labml/internal/configs/base.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4910 2020-11-14 04:46:19.000000 labml-0.4.99/labml/internal/configs/config_function.py
+-rw-r--r--   0 varuna     (501) staff       (20)      834 2020-09-29 11:33:48.000000 labml-0.4.99/labml/internal/configs/config_item.py
+-rw-r--r--   0 varuna     (501) staff       (20)      223 2020-11-14 04:46:19.000000 labml-0.4.99/labml/internal/configs/eval_function.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2869 2020-11-14 04:46:19.000000 labml-0.4.99/labml/internal/configs/processor.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4622 2020-11-14 04:46:19.000000 labml-0.4.99/labml/internal/configs/utils.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/experiment/
+-rw-r--r--   0 varuna     (501) staff       (20)    16968 2021-01-12 08:51:32.000000 labml-0.4.99/labml/internal/experiment/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)    12845 2021-01-28 02:22:57.000000 labml-0.4.99/labml/internal/experiment/experiment_run.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2194 2020-07-06 12:38:31.000000 labml-0.4.99/labml/internal/experiment/pytorch.py
+-rw-r--r--   0 varuna     (501) staff       (20)      822 2020-07-06 12:38:31.000000 labml-0.4.99/labml/internal/experiment/sklearn.py
+-rw-r--r--   0 varuna     (501) staff       (20)      489 2020-11-07 04:56:54.000000 labml-0.4.99/labml/internal/experiment/watcher.py
+-rw-r--r--   0 varuna     (501) staff       (20)     6711 2021-01-15 17:31:39.000000 labml-0.4.99/labml/internal/lab.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/logger/
+-rw-r--r--   0 varuna     (501) staff       (20)      948 2020-12-22 02:46:11.000000 labml-0.4.99/labml/internal/logger/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/logger/destinations/
+-rw-r--r--   0 varuna     (501) staff       (20)      294 2020-11-27 03:09:18.000000 labml-0.4.99/labml/internal/logger/destinations/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1553 2020-12-22 02:48:39.000000 labml-0.4.99/labml/internal/logger/destinations/console.py
+-rw-r--r--   0 varuna     (501) staff       (20)      707 2020-12-22 02:49:21.000000 labml-0.4.99/labml/internal/logger/destinations/factory.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3230 2020-12-22 03:14:00.000000 labml-0.4.99/labml/internal/logger/destinations/ipynb.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2546 2020-12-22 03:15:47.000000 labml-0.4.99/labml/internal/logger/destinations/ipynb_pycharm.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8450 2020-11-08 09:14:49.000000 labml-0.4.99/labml/internal/logger/inspect.py
+-rw-r--r--   0 varuna     (501) staff       (20)      147 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/logger/types.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/manage/
+-rw-r--r--   0 varuna     (501) staff       (20)        0 2020-11-07 07:42:56.000000 labml-0.4.99/labml/internal/manage/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2799 2020-11-07 07:59:10.000000 labml-0.4.99/labml/internal/manage/process.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1811 2021-01-28 02:30:29.000000 labml-0.4.99/labml/internal/manage/runs.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/monitor/
+-rw-r--r--   0 varuna     (501) staff       (20)     8045 2020-12-28 06:01:49.000000 labml-0.4.99/labml/internal/monitor/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2601 2020-11-07 02:29:49.000000 labml-0.4.99/labml/internal/monitor/iterator.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4451 2020-11-07 02:19:05.000000 labml-0.4.99/labml/internal/monitor/loop.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3372 2020-12-28 06:00:02.000000 labml-0.4.99/labml/internal/monitor/mix.py
+-rw-r--r--   0 varuna     (501) staff       (20)     8403 2020-12-21 05:41:47.000000 labml-0.4.99/labml/internal/monitor/sections.py
+-rw-r--r--   0 varuna     (501) staff       (20)      606 2020-08-28 10:35:43.000000 labml-0.4.99/labml/internal/track_debug.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/tracker/
+-rw-r--r--   0 varuna     (501) staff       (20)     7308 2021-01-05 14:25:35.000000 labml-0.4.99/labml/internal/tracker/__init__.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/tracker/indicators/
+-rw-r--r--   0 varuna     (501) staff       (20)      808 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/indicators/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1368 2020-12-06 16:06:33.000000 labml-0.4.99/labml/internal/tracker/indicators/aggregate.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5515 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/indicators/artifacts.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1820 2020-12-06 16:06:33.000000 labml-0.4.99/labml/internal/tracker/indicators/factory.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1716 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/indicators/indexed.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2726 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/indicators/numeric.py
+-rw-r--r--   0 varuna     (501) staff       (20)      429 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/namespace.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/tracker/writers/
+-rw-r--r--   0 varuna     (501) staff       (20)      441 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/writers/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3927 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/writers/file.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4794 2021-01-20 17:20:18.000000 labml-0.4.99/labml/internal/tracker/writers/screen.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3598 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/writers/sqlite.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1499 2020-11-06 14:29:30.000000 labml-0.4.99/labml/internal/tracker/writers/tensorboard.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3334 2021-01-20 17:20:18.000000 labml-0.4.99/labml/internal/tracker/writers/web_api.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/util/
+-rw-r--r--   0 varuna     (501) staff       (20)     1493 2021-01-15 17:04:32.000000 labml-0.4.99/labml/internal/util/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     3427 2020-11-01 09:14:27.000000 labml-0.4.99/labml/internal/util/colors.py
+-rw-r--r--   0 varuna     (501) staff       (20)      958 2020-10-25 05:22:57.000000 labml-0.4.99/labml/internal/util/strings.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/internal/util/tensorboard_writer/
+-rw-r--r--   0 varuna     (501) staff       (20)     1323 2021-01-15 17:08:47.000000 labml-0.4.99/labml/internal/util/tensorboard_writer/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1346 2020-11-19 10:12:43.000000 labml-0.4.99/labml/internal/util/tensorboard_writer/pytorch.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1355 2020-10-29 01:38:06.000000 labml-0.4.99/labml/internal/util/tensorboard_writer/tensorflow.py
+-rw-r--r--   0 varuna     (501) staff       (20)      670 2020-10-25 05:34:38.000000 labml-0.4.99/labml/internal/util/values.py
+-rw-r--r--   0 varuna     (501) staff       (20)      786 2020-11-07 08:54:19.000000 labml-0.4.99/labml/lab.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4364 2020-11-27 03:11:54.000000 labml-0.4.99/labml/logger.py
+-rw-r--r--   0 varuna     (501) staff       (20)      556 2020-11-07 07:58:52.000000 labml-0.4.99/labml/manage.py
+-rw-r--r--   0 varuna     (501) staff       (20)     4102 2020-12-28 06:02:56.000000 labml-0.4.99/labml/monit.py
+-rw-r--r--   0 varuna     (501) staff       (20)     5518 2020-12-16 15:22:31.000000 labml-0.4.99/labml/tracker.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml/utils/
+-rw-r--r--   0 varuna     (501) staff       (20)      879 2021-01-15 17:31:24.000000 labml-0.4.99/labml/utils/__init__.py
+-rw-r--r--   0 varuna     (501) staff       (20)      790 2020-12-31 03:57:47.000000 labml-0.4.99/labml/utils/cache.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1071 2020-06-05 09:45:19.000000 labml-0.4.99/labml/utils/delayed_keyboard_interrupt.py
+-rw-r--r--   0 varuna     (501) staff       (20)      454 2021-01-23 10:24:47.000000 labml-0.4.99/labml/utils/download.py
+-rw-r--r--   0 varuna     (501) staff       (20)       43 2020-06-05 09:45:19.000000 labml-0.4.99/labml/utils/errors.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1112 2020-10-29 01:38:06.000000 labml-0.4.99/labml/utils/keras.py
+-rw-r--r--   0 varuna     (501) staff       (20)     1368 2020-12-21 15:19:26.000000 labml-0.4.99/labml/utils/lightning.py
+-rw-r--r--   0 varuna     (501) staff       (20)      704 2020-10-29 01:38:06.000000 labml-0.4.99/labml/utils/notice.py
+-rw-r--r--   0 varuna     (501) staff       (20)     2549 2020-12-22 05:42:28.000000 labml-0.4.99/labml/utils/pytorch.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/
+-rw-r--r--   0 varuna     (501) staff       (20)     6542 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/PKG-INFO
+-rw-r--r--   0 varuna     (501) staff       (20)     3601 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/SOURCES.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        1 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/dependency_links.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       42 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/entry_points.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       23 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/requires.txt
+-rw-r--r--   0 varuna     (501) staff       (20)        6 2021-01-28 02:30:34.000000 labml-0.4.99/labml.egg-info/top_level.txt
+-rw-r--r--   0 varuna     (501) staff       (20)       38 2021-01-28 02:30:34.000000 labml-0.4.99/setup.cfg
+-rw-r--r--   0 varuna     (501) staff       (20)     1545 2021-01-15 17:03:52.000000 labml-0.4.99/setup.py
+drwxr-xr-x   0 varuna     (501) staff       (20)        0 2021-01-28 02:30:34.000000 labml-0.4.99/test/
+-rw-r--r--   0 varuna     (501) staff       (20)      300 2021-01-02 08:08:13.000000 labml-0.4.99/test/test_experiment.py
+-rw-r--r--   0 varuna     (501) staff       (20)      549 2020-07-12 14:36:26.000000 labml-0.4.99/test/test_inspect.py
+-rw-r--r--   0 varuna     (501) staff       (20)      531 2020-12-08 08:14:23.000000 labml-0.4.99/test/test_tracker.py
+-rw-r--r--   0 varuna     (501) staff       (20)      556 2020-08-31 08:27:27.000000 labml-0.4.99/test/test_watcher.py
```

### Comparing `labml-0.4.98/PKG-INFO` & `labml-0.4.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml
-Version: 0.4.98
+Version: 0.4.99
 Summary: Organize Machine Learning Experiments
 Home-page: https://github.com/lab-ml/labml
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://lab-ml.com/
 Description: <div align="center" style="margin-bottom: 100px;">
```

### Comparing `labml-0.4.98/labml/analytics/__init__.py` & `labml-0.4.99/labml/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/analytics/matplotlib.py` & `labml-0.4.99/labml/analytics/matplotlib.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/cli.py` & `labml-0.4.99/labml/cli.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/configs.py` & `labml-0.4.99/labml/configs.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/experiment.py` & `labml-0.4.99/labml/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/altair/binned_heatmap.py` & `labml-0.4.99/labml/internal/analytics/altair/binned_heatmap.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/altair/density.py` & `labml-0.4.99/labml/internal/analytics/altair/density.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/altair/density_multi.py` & `labml-0.4.99/labml/internal/analytics/altair/density_multi.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/altair/histogram.py` & `labml-0.4.99/labml/internal/analytics/altair/histogram.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/altair/scatter.py` & `labml-0.4.99/labml/internal/analytics/altair/scatter.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/analytics.py` & `labml-0.4.99/labml/internal/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/cache.py` & `labml-0.4.99/labml/internal/analytics/cache.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/indicators.py` & `labml-0.4.99/labml/internal/analytics/indicators.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/matplotlib/__init__.py` & `labml-0.4.99/labml/internal/analytics/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/matplotlib/tb.py` & `labml-0.4.99/labml/internal/analytics/matplotlib/tb.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/sqlite.py` & `labml-0.4.99/labml/internal/analytics/sqlite.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/analytics/tensorboard.py` & `labml-0.4.99/labml/internal/analytics/tensorboard.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/api/__init__.py` & `labml-0.4.99/labml/internal/api/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/api/experiment.py` & `labml-0.4.99/labml/internal/api/experiment.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/api/logs.py` & `labml-0.4.99/labml/internal/api/logs.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/computer/configs.py` & `labml-0.4.99/labml/internal/computer/configs.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/computer/monitor.py` & `labml-0.4.99/labml/internal/computer/monitor.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/computer/process.py` & `labml-0.4.99/labml/internal/computer/process.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/computer/writer.py` & `labml-0.4.99/labml/internal/computer/writer.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/configs/base.py` & `labml-0.4.99/labml/internal/configs/base.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/configs/config_function.py` & `labml-0.4.99/labml/internal/configs/config_function.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/configs/config_item.py` & `labml-0.4.99/labml/internal/configs/config_item.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/configs/processor.py` & `labml-0.4.99/labml/internal/configs/processor.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/configs/utils.py` & `labml-0.4.99/labml/internal/configs/utils.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/experiment/__init__.py` & `labml-0.4.99/labml/internal/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/experiment/experiment_run.py` & `labml-0.4.99/labml/internal/experiment/experiment_run.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/experiment/pytorch.py` & `labml-0.4.99/labml/internal/experiment/pytorch.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/experiment/sklearn.py` & `labml-0.4.99/labml/internal/experiment/sklearn.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/lab.py` & `labml-0.4.99/labml/internal/lab.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/__init__.py` & `labml-0.4.99/labml/internal/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/destinations/console.py` & `labml-0.4.99/labml/internal/logger/destinations/console.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/destinations/factory.py` & `labml-0.4.99/labml/internal/logger/destinations/factory.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/destinations/ipynb.py` & `labml-0.4.99/labml/internal/logger/destinations/ipynb.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/destinations/ipynb_pycharm.py` & `labml-0.4.99/labml/internal/logger/destinations/ipynb_pycharm.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/logger/inspect.py` & `labml-0.4.99/labml/internal/logger/inspect.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/manage/process.py` & `labml-0.4.99/labml/internal/manage/process.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/manage/runs.py` & `labml-0.4.99/labml/internal/manage/runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,17 @@
         if exp_path.name.startswith('_'):
             continue
         for run_path in exp_path.iterdir():
             yield run_path
 
 
 def get_experiments() -> Generator[Path, None, None]:
+    if not lab.get_experiments_path().exists():
+        return
+
     for exp_path in lab.get_experiments_path().iterdir():
         if exp_path.name.startswith('_') or exp_path.name.startswith('.'):
             continue
 
         yield exp_path
```

### Comparing `labml-0.4.98/labml/internal/monitor/__init__.py` & `labml-0.4.99/labml/internal/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/monitor/iterator.py` & `labml-0.4.99/labml/internal/monitor/iterator.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/monitor/loop.py` & `labml-0.4.99/labml/internal/monitor/loop.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/monitor/mix.py` & `labml-0.4.99/labml/internal/monitor/mix.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/monitor/sections.py` & `labml-0.4.99/labml/internal/monitor/sections.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/track_debug.py` & `labml-0.4.99/labml/internal/track_debug.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/__init__.py` & `labml-0.4.99/labml/internal/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/__init__.py` & `labml-0.4.99/labml/internal/tracker/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/aggregate.py` & `labml-0.4.99/labml/internal/tracker/indicators/aggregate.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/artifacts.py` & `labml-0.4.99/labml/internal/tracker/indicators/artifacts.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/factory.py` & `labml-0.4.99/labml/internal/tracker/indicators/factory.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/indexed.py` & `labml-0.4.99/labml/internal/tracker/indicators/indexed.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/indicators/numeric.py` & `labml-0.4.99/labml/internal/tracker/indicators/numeric.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/writers/file.py` & `labml-0.4.99/labml/internal/tracker/writers/file.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/writers/screen.py` & `labml-0.4.99/labml/internal/tracker/writers/screen.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/writers/sqlite.py` & `labml-0.4.99/labml/internal/tracker/writers/sqlite.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/writers/tensorboard.py` & `labml-0.4.99/labml/internal/tracker/writers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/tracker/writers/web_api.py` & `labml-0.4.99/labml/internal/tracker/writers/web_api.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/__init__.py` & `labml-0.4.99/labml/internal/util/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/colors.py` & `labml-0.4.99/labml/internal/util/colors.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/strings.py` & `labml-0.4.99/labml/internal/util/strings.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/tensorboard_writer/__init__.py` & `labml-0.4.99/labml/internal/util/tensorboard_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/tensorboard_writer/pytorch.py` & `labml-0.4.99/labml/internal/util/tensorboard_writer/pytorch.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/tensorboard_writer/tensorflow.py` & `labml-0.4.99/labml/internal/util/tensorboard_writer/tensorflow.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/internal/util/values.py` & `labml-0.4.99/labml/internal/util/values.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/lab.py` & `labml-0.4.99/labml/lab.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/logger.py` & `labml-0.4.99/labml/logger.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/manage.py` & `labml-0.4.99/labml/manage.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/monit.py` & `labml-0.4.99/labml/monit.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/tracker.py` & `labml-0.4.99/labml/tracker.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/__init__.py` & `labml-0.4.99/labml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/cache.py` & `labml-0.4.99/labml/utils/cache.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/delayed_keyboard_interrupt.py` & `labml-0.4.99/labml/utils/delayed_keyboard_interrupt.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/keras.py` & `labml-0.4.99/labml/utils/keras.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/lightning.py` & `labml-0.4.99/labml/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/notice.py` & `labml-0.4.99/labml/utils/notice.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml/utils/pytorch.py` & `labml-0.4.99/labml/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/labml.egg-info/PKG-INFO` & `labml-0.4.99/labml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labml
-Version: 0.4.98
+Version: 0.4.99
 Summary: Organize Machine Learning Experiments
 Home-page: https://github.com/lab-ml/labml
 Author: Varuna Jayasiri, Nipun Wijerathne
 Author-email: vpjayasiri@gmail.com, hnipun@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://lab-ml.com/
 Description: <div align="center" style="margin-bottom: 100px;">
```

### Comparing `labml-0.4.98/labml.egg-info/SOURCES.txt` & `labml-0.4.99/labml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/setup.py` & `labml-0.4.99/setup.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/test/test_inspect.py` & `labml-0.4.99/test/test_inspect.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/test/test_tracker.py` & `labml-0.4.99/test/test_tracker.py`

 * *Files identical despite different names*

### Comparing `labml-0.4.98/test/test_watcher.py` & `labml-0.4.99/test/test_watcher.py`

 * *Files identical despite different names*

