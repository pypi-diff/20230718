# Comparing `tmp/astronomia-1.2.9.tar.gz` & `tmp/astronomia-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomia-1.2.9.tar", last modified: Mon Jan 16 17:54:43 2023, max compression
+gzip compressed data, was "astronomia-2.0.0.tar", last modified: Tue Jul 18 02:56:20 2023, max compression
```

## Comparing `astronomia-1.2.9.tar` & `astronomia-2.0.0.tar`

### file list

```diff
@@ -1,83 +1,82 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.562476 astronomia-1.2.9/
--rw-rw-r--   0 tim       (1000) tim       (1000)      102 2022-10-07 11:36:31.000000 astronomia-1.2.9/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-01-07 21:38:51.000000 astronomia-1.2.9/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-01-07 22:48:43.000000 astronomia-1.2.9/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      263 2020-02-20 11:58:46.000000 astronomia-1.2.9/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2922 2023-01-07 22:48:43.000000 astronomia-1.2.9/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)      100 2020-02-20 11:58:56.000000 astronomia-1.2.9/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1023 2022-09-27 21:29:39.000000 astronomia-1.2.9/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      818 2023-01-16 06:13:30.000000 astronomia-1.2.9/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3080 2021-06-20 00:18:52.000000 astronomia-1.2.9/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)    18092 2020-02-20 11:58:56.000000 astronomia-1.2.9/LICENSE.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      169 2020-02-20 11:58:56.000000 astronomia-1.2.9/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-16 17:54:43.562476 astronomia-1.2.9/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2775 2022-09-27 21:30:22.000000 astronomia-1.2.9/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-01-16 06:13:30.000000 astronomia-1.2.9/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/devutils/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1247 2022-10-07 11:36:31.000000 astronomia-1.2.9/devutils/create_binary_vsop_db.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     4565 2022-10-05 03:28:35.000000 astronomia-1.2.9/devutils/create_text_vsop_db.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1467 2022-10-07 11:36:31.000000 astronomia-1.2.9/devutils/time_vsop_db_loads.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)      488 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/applications.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1445 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/astronomia.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/authors.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     7980 2022-10-07 11:36:31.000000 astronomia-1.2.9/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      623 2022-11-23 03:14:16.000000 astronomia-1.2.9/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:14:19.000000 astronomia-1.2.9/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)     2979 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/models.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:58:54.000000 astronomia-1.2.9/docs/readme.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      932 2021-06-20 00:18:52.000000 astronomia-1.2.9/docs/todo.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.550476 astronomia-1.2.9/params/
--rw-r--r--   0 tim       (1000) tim       (1000)      347 2021-06-20 00:18:52.000000 astronomia-1.2.9/params/astronomia_params.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2734 2023-01-16 06:13:30.000000 astronomia-1.2.9/pyproject.toml
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-01-16 17:54:43.562476 astronomia-1.2.9/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      599 2022-10-07 11:36:31.000000 astronomia-1.2.9/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.546476 astronomia-1.2.9/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.554476 astronomia-1.2.9/src/astronomia/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1055 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/__init__.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia/apps/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     1594 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/apps/check_perihelion.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     9770 2023-01-07 21:17:53.000000 astronomia-1.2.9/src/astronomia/apps/cronus.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     2256 2022-10-05 03:37:33.000000 astronomia-1.2.9/src/astronomia/apps/solstice.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4223 2023-01-07 21:15:37.000000 astronomia-1.2.9/src/astronomia/astronomia.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    16040 2023-01-07 22:36:31.000000 astronomia-1.2.9/src/astronomia/calendar.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia/cgi/
--rwxrwxr-x   0 tim       (1000) tim       (1000)     5748 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/cgi/easter_cgi.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     8598 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/cgi/solstice_cgi.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1788 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/commonterms.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1790 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/constants.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3721 2023-01-07 22:40:15.000000 astronomia-1.2.9/src/astronomia/coordinates.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    69493 2023-01-07 22:10:13.000000 astronomia-1.2.9/src/astronomia/dynamical.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5236 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/equinox.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/globals.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    11529 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/lunar.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7159 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/nutation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6626 2023-01-07 21:17:53.000000 astronomia-1.2.9/src/astronomia/planets.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6343 2023-01-07 21:57:09.000000 astronomia-1.2.9/src/astronomia/riseset.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     6976 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/sun.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     9723 2023-01-07 22:25:43.000000 astronomia-1.2.9/src/astronomia/util.py
--rw-rw-r--   0 tim       (1000) tim       (1000)  1955695 2022-10-07 11:36:31.000000 astronomia-1.2.9/src/astronomia/vsop87d_dict.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.558476 astronomia-1.2.9/src/astronomia.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4092 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1640 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      153 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      189 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       11 2023-01-16 17:54:43.000000 astronomia-1.2.9/src/astronomia.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-01-16 17:54:43.562476 astronomia-1.2.9/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4757 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_calendar.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      987 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_coordinates.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1993 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_dynamical.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2132 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_easter.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4935 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_elp2000.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     5476 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_equinox.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1507 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_nutation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3418 2023-01-07 21:17:53.000000 astronomia-1.2.9/tests/test_sun.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      453 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_util.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2689 2022-10-07 11:36:31.000000 astronomia-1.2.9/tests/test_vsop.py
--rw-r--r--   0 tim       (1000) tim       (1000)   104342 2021-06-20 00:18:52.000000 astronomia-1.2.9/tests/vsop87.chk
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:12:57.000000 astronomia-2.0.0/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.899778 astronomia-2.0.0/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.899778 astronomia-2.0.0/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-17 22:12:57.000000 astronomia-2.0.0/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:12:57.000000 astronomia-2.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      271 2023-03-05 18:50:47.000000 astronomia-2.0.0/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-18 02:41:46.000000 astronomia-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)      100 2020-02-20 11:58:56.000000 astronomia-2.0.0/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1023 2022-09-27 21:29:39.000000 astronomia-2.0.0/BADGES.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1256 2023-07-18 02:41:52.000000 astronomia-2.0.0/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3080 2021-06-20 00:18:52.000000 astronomia-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)    18092 2020-02-20 11:58:56.000000 astronomia-2.0.0/LICENSE.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      163 2023-06-11 16:51:56.000000 astronomia-2.0.0/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4081 2023-07-18 02:56:20.903778 astronomia-2.0.0/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2684 2023-06-21 04:45:37.000000 astronomia-2.0.0/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-07-18 02:41:52.000000 astronomia-2.0.0/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.899778 astronomia-2.0.0/devutils/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1247 2023-01-22 03:38:21.000000 astronomia-2.0.0/devutils/create_binary_vsop_db.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     4565 2023-01-22 03:38:21.000000 astronomia-2.0.0/devutils/create_text_vsop_db.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1467 2023-01-22 03:38:21.000000 astronomia-2.0.0/devutils/time_vsop_db_loads.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.899778 astronomia-2.0.0/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)      488 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/applications.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1445 2021-06-20 00:18:52.000000 astronomia-2.0.0/docs/astronomia.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 00:18:52.000000 astronomia-2.0.0/docs/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7980 2023-01-22 03:38:21.000000 astronomia-2.0.0/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      623 2022-11-23 03:14:16.000000 astronomia-2.0.0/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:14:19.000000 astronomia-2.0.0/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)     2979 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/models.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:58:54.000000 astronomia-2.0.0/docs/readme.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      932 2021-06-20 00:18:52.000000 astronomia-2.0.0/docs/todo.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2858 2023-07-18 02:41:52.000000 astronomia-2.0.0/pyproject.toml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-18 02:56:20.903778 astronomia-2.0.0/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      467 2023-06-11 00:48:37.000000 astronomia-2.0.0/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.899778 astronomia-2.0.0/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/src/astronomia/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1055 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/__init__.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/src/astronomia/apps/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     1594 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/apps/check_perihelion.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     9851 2023-02-25 04:40:17.000000 astronomia-2.0.0/src/astronomia/apps/cronus.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2164 2023-02-25 04:40:17.000000 astronomia-2.0.0/src/astronomia/apps/solstice.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4210 2023-02-25 04:40:17.000000 astronomia-2.0.0/src/astronomia/astronomia.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      347 2021-06-20 00:18:52.000000 astronomia-2.0.0/src/astronomia/astronomia_params.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16040 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/calendar.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/src/astronomia/cgi/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     5748 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/cgi/easter_cgi.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     8591 2023-02-13 05:07:44.000000 astronomia-2.0.0/src/astronomia/cgi/solstice_cgi.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1788 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/commonterms.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1790 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/constants.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3721 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/coordinates.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    69493 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/dynamical.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5236 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/equinox.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2550 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/globals.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11529 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/lunar.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7159 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/nutation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6626 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/planets.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6343 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/riseset.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6847 2023-02-13 05:07:44.000000 astronomia-2.0.0/src/astronomia/sun.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10771 2023-06-11 00:36:07.000000 astronomia-2.0.0/src/astronomia/util.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)  1955695 2023-01-22 03:38:21.000000 astronomia-2.0.0/src/astronomia/vsop87d_dict.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/src/astronomia.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4081 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1648 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      153 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      264 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       11 2023-07-18 02:56:20.000000 astronomia-2.0.0/src/astronomia.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-18 02:56:20.903778 astronomia-2.0.0/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4757 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_calendar.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      987 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_coordinates.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1993 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_dynamical.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2132 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_easter.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4935 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_elp2000.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5476 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_equinox.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1507 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_nutation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3418 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_sun.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      453 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_util.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2689 2023-01-22 03:38:21.000000 astronomia-2.0.0/tests/test_vsop.py
+-rw-r--r--   0 tim       (1000) tim       (1000)   104342 2021-06-20 00:18:52.000000 astronomia-2.0.0/tests/vsop87.chk
```

### Comparing `astronomia-1.2.9/.github/workflows/python-package.yml` & `astronomia-2.0.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/.pre-commit-config.yaml` & `astronomia-2.0.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,95 @@
 ---
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
+
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
           - id: check-case-conflict
           - id: check-docstring-first
           - id: check-executables-have-shebangs
           - id: check-json
           - id: check-merge-conflict
           - id: check-shebang-scripts-are-executable
           - id: check-toml
           - id: check-xml
-          # - id: check-yaml
           - id: end-of-file-fixer
             exclude: notebooks/tstoolbox_plot_bash.sh
           - id: fix-encoding-pragma
             args: [--remove]
           - id: mixed-line-ending
           - id: trailing-whitespace
             exclude: notebooks/tstoolbox_plot_bash.sh
 
-
-    - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-      rev: v2.5.0
+    - repo: https://github.com/pappasam/toml-sort
+      rev: v0.23.1
       hooks:
-          # - id: pretty-format-toml
-          #   args: [--autofix]
-          - id: pretty-format-java
-            args: [--autofix]
-          - id: pretty-format-kotlin
-            args: [--autofix]
+          - id: toml-sort-fix
+            args: [--in-place, --spaces-indent-inline-array, '4']
 
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.28.0
+      rev: v1.32.0
       hooks:
           - id: yamllint
             args: [--format, parsable, --strict]
 
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
 
+    - repo: https://github.com/jumanjihouse/pre-commit-hooks
+      rev: 3.0.0
+      hooks:
+          - id: shellcheck
+            args: [-s, bash]
+
+    - repo: https://github.com/lovesegfault/beautysh
+      rev: v6.2.1
+      hooks:
+          - id: beautysh
+            args: [--indent-size, '4']
+
     - repo: https://github.com/psf/black
-      rev: 22.12.0
+      rev: 23.7.0
       hooks:
           - id: black
-            language_version: python
+          - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
-      rev: 5.11.4
+      rev: 5.12.0
       hooks:
           - id: isort
             name: isort (python)
-            # yamllint disable-line rule:line-length
-            args: [--profile, black, --filter-files, --line-length, '88', --multi-line, '3']
+            args: [--profile, black, --filter-files]
           - id: isort
             name: isort (cython)
             types: [cython]
-            # yamllint disable-line rule:line-length
-            args: [--profile, black, --filter-files, --line-length, '88', --multi-line, '3']
+            args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
-            # yamllint disable-line rule:line-length
-            args: [--profile, black, --filter-files, --line-length, '88', --multi-line, '3']
-
-    - repo: https://github.com/dfm/black_nbconvert
-      rev: v0.4.0
-      hooks:
-          - id: black_nbconvert
+            args: [--profile, black, --filter-files]
 
     - repo: https://github.com/asottile/blacken-docs
-      rev: v1.12.1
+      rev: 1.15.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.1
+      rev: v3.9.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: v2.39.1
+      rev: 3.5.3
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.4
+      rev: v1.14.7
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `astronomia-1.2.9/BADGES.rst` & `astronomia-2.0.0/BADGES.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/CONTRIBUTING.rst` & `astronomia-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/LICENSE.txt` & `astronomia-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/PKG-INFO` & `astronomia-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: astronomia
-Version: 1.2.9
+Version: 2.0.0
 Summary: Library for calculation of ephemeris and other astronomical calculations
 Author-email: Tim Cera <tim@cerazone.net>
-License: GPL-2.0-only
+License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/astronomia/docs/index.html#astronomia-documentation
 Project-URL: github, https://github.com/timcera/astronomia
 Project-URL: bitbucket, https://bitbucket.org/timcera/astronomia/src/main/
 Keywords: ephemeris,astronomy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 .. image:: https://github.com/timcera/astronomia/actions/workflows/python-package.yml/badge.svg
     :alt: Tests
     :target: https://github.com/timcera/astronomia/actions/workflows/python-package.yml
@@ -79,20 +81,15 @@
 
 Installation
 ~~~~~~~~~~~~
 At the command line::
 
     $ pip install astronomia
     # OR
-    $ easy_install astronomia
-
-Or, if you have virtualenvwrapper installed::
-
-    $ mkvirtualenv astronomia
-    $ pip install astronomia
+    $ conda install -c conda-forge astronomia
 
 Usage
 ~~~~~
 To use Astronomia in a project::
 
 	import astronomia
```

### Comparing `astronomia-1.2.9/README.rst` & `astronomia-2.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,15 @@
 
 Installation
 ~~~~~~~~~~~~
 At the command line::
 
     $ pip install astronomia
     # OR
-    $ easy_install astronomia
-
-Or, if you have virtualenvwrapper installed::
-
-    $ mkvirtualenv astronomia
-    $ pip install astronomia
+    $ conda install -c conda-forge astronomia
 
 Usage
 ~~~~~
 To use Astronomia in a project::
 
 	import astronomia
```

### Comparing `astronomia-1.2.9/devutils/create_binary_vsop_db.py` & `astronomia-2.0.0/devutils/create_binary_vsop_db.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/devutils/create_text_vsop_db.py` & `astronomia-2.0.0/devutils/create_text_vsop_db.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/devutils/time_vsop_db_loads.py` & `astronomia-2.0.0/devutils/time_vsop_db_loads.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/Makefile` & `astronomia-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/astronomia.rst` & `astronomia-2.0.0/docs/astronomia.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/conf.py` & `astronomia-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/index.rst` & `astronomia-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/make.bat` & `astronomia-2.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/models.rst` & `astronomia-2.0.0/docs/models.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/docs/todo.rst` & `astronomia-2.0.0/docs/todo.rst`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/pyproject.toml` & `astronomia-2.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,115 @@
 [build-system]
+build-backend = "setuptools.build_meta"
 requires = [
-    "setuptools>=45",
+    "setuptools>=61.0.0",
     "setuptools_scm[toml]>=6.2",
     "wheel",
-    "oldest-supported-numpy",
+    "oldest-supported-numpy"
 ]
-build-backend = "setuptools.build_meta"
 
 [project]
 name = "astronomia"
 dynamic = ["readme", "version"]
 description = "Library for calculation of ephemeris and other astronomical calculations"
 dependencies = [
     "cltoolbox",
     "numpy",
     "pandas",
-    "toolbox_utils",
-    ]
-license = {text = "GPL-2.0-only"}
+    "toolbox_utils >= 5.0.0, < 6.0.0"
+]
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
-    ]
+]
 classifiers = [
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Science/Research",
-        "Intended Audience :: End Users/Desktop",
-        "Intended Audience :: Developers",
-        "Environment :: Console",
-        "License :: OSI Approved :: BSD License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ]  # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Environment :: Console",
+    "License :: OSI Approved :: BSD License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Software Development :: Libraries :: Python Modules"
+] # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
 keywords = ["ephemeris", "astronomy"]
+license = {text = "BSD-3-Clause"}
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = [
+    "bandit",
     "black",
+    "blacken-docs",
+    "black-nbconvert",
     "cleanpy",
-    "twine",
+    "commitizen",
+    "coverage[toml]",
+    "isort",
+    "mypy",
+    "pre-commit",
+    "pyflakes",
+    "pylama",
+    "pyle",
+    "pylint",
+    "pyre",
+    "pyroma",
     "pytest",
-    "coverage",
-    "flake8",
     "pytest-cov",
     "pytest-mpl",
-    "pre-commit",
-    "black-nbconvert",
-    "blacken-docs",
-    "velin",
-    "isort",
-    "pyroma",
     "pyupgrade",
-    "commitizen",
-    ]
+    "twine",
+    "unimport",
+    "velin",
+    "vulture"
+]
 
 [project.scripts]
 solstice = "astronomia.apps.solstice:main"
 check_perihelion = "astronomia.apps.check_perihelion:main"
 cronus = "astronomia.apps.cronus:main"
 
 [project.urls]
 documentation = "https://timcera.bitbucket.io/astronomia/docs/index.html#astronomia-documentation"
 github = "https://github.com/timcera/astronomia"
 bitbucket = "https://bitbucket.org/timcera/astronomia/src/main/"
 
 [tool]
 
 [tool.check-manifest]
-ignore = ["docs/_function_autosummary/*",
-          ".coverage",
-          ".deepsource.toml",
-          ".ipynb_checkpoints/*"]
+ignore = [
+    "docs/_function_autosummary/*",
+    ".coverage",
+    ".deepsource.toml",
+    ".ipynb_checkpoints/*"
+]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.2.9"
 tag_format = "v$version"
-version_files = ["VERSION"]
 update_changelog_on_bump = true
+version = "2.0.0"
+version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
 version = {file = "VERSION"}
 
 [tool.setuptools.packages.find]
-where = ["src"]
 exclude = ["examples*", "tools*", "docs*", "astronomia.tests*"]
+where = ["src"]
 
 [tool.setuptools_scm]
```

### Comparing `astronomia-1.2.9/src/astronomia/__init__.py` & `astronomia-2.0.0/src/astronomia/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/apps/check_perihelion.py` & `astronomia-2.0.0/src/astronomia/apps/check_perihelion.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/apps/cronus.py` & `astronomia-2.0.0/src/astronomia/apps/cronus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,9 @@
 #! /usr/bin/env python
 """
-A clock application that displays a variety of celestial events in the
-order they occur.
-
-Usage:
-
-    ./cronus.py start_year [stop_year]
-
-To do:
-    -- Add many more events
-    -- Support both real-time and "fast" modes
-    -- Allow finer start and stop times
-
-Currently the program always runs in "fast" mode, queueing and
-displaying events in the future as fast as possible. Eventually
-I would like to have enough events covered so that the display
-runs continuously even in real-time. Since the next event of
-a given type needs to be calculated only when the previous one
-has been delivered, this is not as computationally intense as it
-sounds.
-
     Astrolabe copyright 2000, 2001 William McClain
     Astrolabe forked to Astronomia 2013
     Astronomia copyright 2013
 
     This file is part of Astronomia.
 
     Astronomia is free software; you can redistribute it and/or modify
@@ -37,19 +17,20 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with Astronomia; if not, write to the Free Software
     Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 """
 
-import os
-import sys
 from heapq import heappop, heappush
 from math import *
 
+import cltoolbox
+from cltoolbox.rst_text_formatter import RSTHelpFormatter
+
 import astronomia.globals
 from astronomia.calendar import cal_to_jd, easter, lt_to_str, ut_to_lt
 from astronomia.constants import (
     days_per_minute,
     days_per_second,
     standard_rst_altitude,
     sun_rst_altitude,
@@ -308,46 +289,68 @@
         h0List.append(sun_rst_altitude)
     rstDict["Sun"] = RiseSetTransit("Sun", raList, decList, h0List)
 
     # all Rise-Set-Transit events
     heappush(taskQueue, Task(HIGH_PRIORITY, doRiseSetTransit, (start_jd,)))
 
 
-def main():
+@cltoolbox.command(formatter_class=RSTHelpFormatter)
+def cronus(start, stop=None):
+    """Displays a variety of celestial events in the order they occur.
+
+    To do::
+
+        -- Add many more events
+        -- Support both real-time and "fast" modes
+        -- Allow finer start and stop times
+
+    Currently the program always runs in "fast" mode, queueing and
+    displaying events in the future as fast as possible. Eventually
+    I would like to have enough events covered so that the display
+    runs continuously even in real-time. Since the next event of
+    a given type needs to be calculated only when the previous one
+    has been delivered, this is not as computationally intense as it
+    sounds.
+
+    Parameters
+    ----------
+    start : int
+        The year to start the display.
+    stop : int, optional
+        The year to stop the display. If not given, the display
+        continues until 10,000AD.
+    """
     global vsop
     global sun
-    if len(sys.argv) < 2:
-        print(__doc__)
-        os._exit(0)
-    if len(sys.argv) < 3:
-        start_year = int(sys.argv[1])
-        stop_jd = cal_to_jd(10000)  # default stopping date: 10,000AD
-    elif len(sys.argv) < 4:
-        start_year = int(sys.argv[1])
-        stop_jd = cal_to_jd(int(sys.argv[2]))
+    start = int(start)
+    if stop is None:
+        stop = cal_to_jd(stop)
     else:
-        print(__doc__)
-        os._exit(0)
+        stop = int(stop)
 
     load_params()
     vsop = VSOP87d()
     sun = Sun()
 
     # Easter
-    heappush(taskQueue, Task(HIGH_PRIORITY, doEaster, (start_year,)))
+    heappush(taskQueue, Task(HIGH_PRIORITY, doEaster, (start,)))
 
     # four equinox/solstice events
     for season in astronomia.globals.season_names:
-        heappush(taskQueue, Task(HIGH_PRIORITY, doEquinox, (start_year, season)))
+        heappush(taskQueue, Task(HIGH_PRIORITY, doEquinox, (start, season)))
 
     # initialize rise-set-transit objects
-    initRST(start_year)
+    initRST(start)
 
     # start the task loop
     t = heappop(taskQueue)
-    while t.jd < stop_jd:
+    while t.jd < stop:
         t.func(*t.args)
         t = heappop(taskQueue)
 
 
+def main():
+    cltoolbox.main()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `astronomia-1.2.9/src/astronomia/apps/solstice.py` & `astronomia-2.0.0/src/astronomia/apps/solstice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,9 @@
 #! /usr/bin/env python
 """
-Usage:
-
-    ./solstice.py start_year [stop_year]
-
-Displays the instants of equinoxes and solstices for a range of years.
-Times are accurate to one second.
-
-The arguments must be integers.
-
-If one argument is given, the display is for that year.
-
-If two arguments are given, the display is for that range of
-years.
-
     Astrolabe copyright 2000, 2001 William McClain
     Astrolabe forked to Astronomia 2013
     Astronomia copyright 2013
 
     This file is part of Astronomia.
 
     Astronomia is free software; you can redistribute it and/or modify
@@ -31,47 +17,58 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with Astronomia; if not, write to the Free Software
     Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 """
-import sys
+
+import cltoolbox
+from cltoolbox.rst_text_formatter import RSTHelpFormatter
 
 import astronomia.globals
 from astronomia.calendar import lt_to_str, ut_to_lt
 from astronomia.constants import days_per_second
 from astronomia.dynamical import dt_to_ut
 from astronomia.equinox import equinox, equinox_approx
 from astronomia.util import load_params
 
 tab = 4 * " "
 
 
-def main(start=None, stop=None):
-    if len(sys.argv) < 2:
-        print(__doc__)
-        sys.exit(1)
-    elif len(sys.argv) < 3:
-        start = int(sys.argv[1])
+@cltoolbox.command(formatter_class=RSTHelpFormatter)
+def solstice(start, stop=None):
+    """Displays the instants of equinoxes and solstices for a range of years.
+
+    Times are accurate to one second.
+
+    Parameters
+    ----------
+    start : int
+        The start year, or if stop is not given, the year to display.
+    stop : int
+        The end year.
+    """
+    start = int(start)
+    if stop is None:
         stop = start
-    elif len(sys.argv) < 4:
-        start = int(sys.argv[1])
-        stop = int(sys.argv[2])
     else:
-        print(__doc__)
-        sys.exit(1)
+        stop = int(stop)
 
     load_params()
 
     for yr in range(start, stop + 1):
         print(yr)
         for season in astronomia.globals.season_names:
             approx_jd = equinox_approx(yr, season)
             jd = equinox(approx_jd, season, days_per_second)
             ut = dt_to_ut(jd)
             lt, zone = ut_to_lt(ut)
             print(tab, season, lt_to_str(lt, zone))
 
 
+def main():
+    cltoolbox.main()
+
+
 if __name__ == "__main__":
-    main(start, stop)
+    main()
```

### Comparing `astronomia-1.2.9/src/astronomia/astronomia.py` & `astronomia-2.0.0/src/astronomia/astronomia.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         supplied also.  The pandas date offset code used to create the
         index.
     """
     if input_ts is not None:
         start_date = input_ts.index[0]
         end_date = input_ts.index[-1]
     tindex = pd.date_range(start=start_date, end=end_date, freq=freq)
-    usets = pd.DataFrame([0.0] * len(tindex), index=tindex)
+    pd.DataFrame([0.0] * len(tindex), index=tindex)
     # Finish!!!!!
 
 
 @cltoolbox.command(formatter_class=RSTHelpFormatter)
 def risesettransit(
     latitude, longitude, start_date, end_date, body, h0=0, times="rise,set"
 ):
@@ -79,15 +79,15 @@
             "transit" for the transit time
 
         Defaults to "rise,set".
     """
     start_date = tsutils.parsedate(start_date)
     end_date = tsutils.parsedate(end_date)
 
-    dr = pd.date_range(start=start_date, end=end_date).to_julian_date()
+    pd.date_range(start=start_date, end=end_date).to_julian_date()
     start_jd = cal_to_jd(start_date)
 
     #
     # We need nutation values for each of three days
     #
     nutation = {}
     for day in (-1, 0, 1):
```

### Comparing `astronomia-1.2.9/src/astronomia/calendar.py` & `astronomia-2.0.0/src/astronomia/calendar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/cgi/easter_cgi.py` & `astronomia-2.0.0/src/astronomia/cgi/easter_cgi.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/cgi/solstice_cgi.py` & `astronomia-2.0.0/src/astronomia/cgi/solstice_cgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 #
 # Collect the input parameters
 #
 
 
 def display_form():
     fields = time.localtime(time.time())
-    year = fields[0]
+    fields[0]
 
     print("Content-type: text/html")
     print()
     print("<HEAD>")
     print("<TITLE>Astronomia Solstice Parameters</TITLE>")
     print("</HEAD>")
```

### Comparing `astronomia-1.2.9/src/astronomia/commonterms.py` & `astronomia-2.0.0/src/astronomia/commonterms.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/constants.py` & `astronomia-2.0.0/src/astronomia/constants.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/coordinates.py` & `astronomia-2.0.0/src/astronomia/coordinates.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/dynamical.py` & `astronomia-2.0.0/src/astronomia/dynamical.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/equinox.py` & `astronomia-2.0.0/src/astronomia/equinox.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/globals.py` & `astronomia-2.0.0/src/astronomia/globals.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/lunar.py` & `astronomia-2.0.0/src/astronomia/lunar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/nutation.py` & `astronomia-2.0.0/src/astronomia/nutation.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/planets.py` & `astronomia-2.0.0/src/astronomia/planets.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/riseset.py` & `astronomia-2.0.0/src/astronomia/riseset.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia/sun.py` & `astronomia-2.0.0/src/astronomia/sun.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,20 +22,18 @@
 
 Geocentric solar position and radius, both low and high precision.
 """
 import numpy as np
 
 from . import calendar
 from . import globals as globls
-from .calendar import cal_to_jd, jd_to_jcent
-from .constants import days_per_second
+from .calendar import jd_to_jcent
 from .coordinates import ecl_to_equ
-from .lunar import Lunar
-from .nutation import nutation_in_longitude, nutation_in_obliquity, obliquity
-from .planets import VSOP87d, geocentric_planet, vsop_to_fk5
+from .nutation import nutation_in_longitude
+from .planets import VSOP87d, vsop_to_fk5
 from .util import _scalar_if_one, d_to_r, dms_to_d, modpi2, polynomial
 
 
 class Error(Exception):
     """Local exception class."""
 
 
@@ -238,15 +236,14 @@
     year,
     month,
     day,
     longitude=globls.longitude,
     latitude=globls.latitude,
     gregorian=True,
 ):
-
     from .constants import sun_rst_altitude
 
     jd = calendar.cal_to_jd(year, month, day, gregorian=gregorian)
 
     sun = Sun()
     #
     # Sun
```

### Comparing `astronomia-1.2.9/src/astronomia/util.py` & `astronomia-2.0.0/src/astronomia/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 
 Collection of miscellaneous functions
 """
 
 import os
 import shlex
-import sys
 
 import numpy as np
 
 from . import globals as globls
 from .constants import minutes_per_day, pi2, seconds_per_day
 
 
@@ -196,22 +195,58 @@
     Returns:
         nothing
     """
     fname = os.environ.get("ASTRONOMIA_PARAMS", "astronomia_params.txt")
 
     if not os.path.exists(fname):
         # last resort
-        fname = os.path.join(sys.prefix, "share", "astronomia", "astronomia_params.txt")
+        fname = os.path.join(
+            os.path.dirname(__file__),
+            os.path.pardir,
+            "share",
+            "astronomia",
+            "astronomia_params.txt",
+        )
+        print(
+            f"""WARNING: Using system wide settings file at
+"{fname}".
+You may want to set the ASTRONOMIA_PARAMS environment variable to point to the
+file you want, or create a "astronomia_params.txt" file in the current
+directory."""
+        )
+    if not os.path.exists(fname):
+        # really last resort
+        fname = os.path.join(
+            os.path.dirname(__file__),
+            os.path.pardir,
+            os.path.pardir,
+            "params",
+            "astronomia_params.txt",
+        )
         print(
             f"""WARNING: Using system wide settings file at
 "{fname}".
 You may want to set the ASTRONOMIA_PARAMS environment variable to point to the
 file you want, or create a "astronomia_params.txt" file in the current
 directory."""
         )
+    if not os.path.exists(fname):
+        # really last resort
+        fname = os.path.join(
+            os.path.dirname(__file__),
+            "astronomia_params.txt",
+        )
+        print(
+            f"""WARNING: Using system wide settings file at
+"{fname}".
+You may want to set the ASTRONOMIA_PARAMS environment variable to point to the
+file you want, or create a "astronomia_params.txt" file in the current
+directory."""
+        )
+
     try:
         f = open(fname)
     except OSError as value:
         raise Error(
             """
 Unable to open param file. Either set ASTRONOMIA_PARAMS correctly or create
 astronomia_params.txt in the current directory"""
```

### Comparing `astronomia-1.2.9/src/astronomia/vsop87d_dict.py` & `astronomia-2.0.0/src/astronomia/vsop87d_dict.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/src/astronomia.egg-info/PKG-INFO` & `astronomia-2.0.0/src/astronomia.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: astronomia
-Version: 1.2.9
+Version: 2.0.0
 Summary: Library for calculation of ephemeris and other astronomical calculations
 Author-email: Tim Cera <tim@cerazone.net>
-License: GPL-2.0-only
+License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/astronomia/docs/index.html#astronomia-documentation
 Project-URL: github, https://github.com/timcera/astronomia
 Project-URL: bitbucket, https://bitbucket.org/timcera/astronomia/src/main/
 Keywords: ephemeris,astronomy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 .. image:: https://github.com/timcera/astronomia/actions/workflows/python-package.yml/badge.svg
     :alt: Tests
     :target: https://github.com/timcera/astronomia/actions/workflows/python-package.yml
@@ -79,20 +81,15 @@
 
 Installation
 ~~~~~~~~~~~~
 At the command line::
 
     $ pip install astronomia
     # OR
-    $ easy_install astronomia
-
-Or, if you have virtualenvwrapper installed::
-
-    $ mkvirtualenv astronomia
-    $ pip install astronomia
+    $ conda install -c conda-forge astronomia
 
 Usage
 ~~~~~
 To use Astronomia in a project::
 
 	import astronomia
```

### Comparing `astronomia-1.2.9/src/astronomia.egg-info/SOURCES.txt` & `astronomia-2.0.0/src/astronomia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/make.bat
 docs/models.rst
 docs/readme.rst
 docs/todo.rst
-params/astronomia_params.txt
 src/astronomia/__init__.py
 src/astronomia/astronomia.py
+src/astronomia/astronomia_params.txt
 src/astronomia/calendar.py
 src/astronomia/commonterms.py
 src/astronomia/constants.py
 src/astronomia/coordinates.py
 src/astronomia/dynamical.py
 src/astronomia/equinox.py
 src/astronomia/globals.py
```

### Comparing `astronomia-1.2.9/tests/test_calendar.py` & `astronomia-2.0.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_coordinates.py` & `astronomia-2.0.0/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_dynamical.py` & `astronomia-2.0.0/tests/test_dynamical.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_easter.py` & `astronomia-2.0.0/tests/test_easter.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_elp2000.py` & `astronomia-2.0.0/tests/test_elp2000.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_equinox.py` & `astronomia-2.0.0/tests/test_equinox.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_nutation.py` & `astronomia-2.0.0/tests/test_nutation.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_sun.py` & `astronomia-2.0.0/tests/test_sun.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/test_vsop.py` & `astronomia-2.0.0/tests/test_vsop.py`

 * *Files identical despite different names*

### Comparing `astronomia-1.2.9/tests/vsop87.chk` & `astronomia-2.0.0/tests/vsop87.chk`

 * *Files identical despite different names*

