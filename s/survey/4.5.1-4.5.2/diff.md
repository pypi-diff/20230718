# Comparing `tmp/survey-4.5.1.tar.gz` & `tmp/survey-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-4.5.1.tar", last modified: Tue Jul 11 18:16:41 2023, max compression
+gzip compressed data, was "survey-4.5.2.tar", last modified: Tue Jul 18 08:45:11 2023, max compression
```

## Comparing `survey-4.5.1.tar` & `survey-4.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.329490 survey-4.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.317489 survey-4.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.321490 survey-4.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 18:16:27.000000 survey-4.5.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-11 18:16:27.000000 survey-4.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 18:16:27.000000 survey-4.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-11 18:16:27.000000 survey-4.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 18:16:41.329490 survey-4.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 18:16:27.000000 survey-4.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.321490 survey-4.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 18:16:27.000000 survey-4.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.317489 survey-4.5.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.325490 survey-4.5.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/graphics.lineprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/graphics.spinprogress-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/printers.done-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/printers.fail-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/printers.info-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.basket-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.basket-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.conceal-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.datetime-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.datetime-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.form-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.input-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.input-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.inquire-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.numeric-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.numeric-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.select-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/routines.select-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/showcase-1.gif
--rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-11 18:16:27.000000 survey-4.5.1/docs/_static/images/showcase-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 18:16:27.000000 survey-4.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 18:16:27.000000 survey-4.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-11 18:16:27.000000 survey-4.5.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-11 18:16:27.000000 survey-4.5.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:16:41.329490 survey-4.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-11 18:16:27.000000 survey-4.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.325490 survey-4.5.1/survey/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-11 18:16:27.000000 survey-4.5.1/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_controls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.329490 survey-4.5.1/survey/_core/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_console.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_io_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_io_os_nt.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_io_os_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_core/_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_funnels.py
--rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_mutates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_printers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_searches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_visuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    58112 2023-07-11 18:16:27.000000 survey-4.5.1/survey/_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:16:41.329490 survey-4.5.1/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-11 18:16:41.000000 survey-4.5.1/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-11 18:16:41.000000 survey-4.5.1/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:16:41.000000 survey-4.5.1/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 18:16:41.000000 survey-4.5.1/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 18:16:41.000000 survey-4.5.1/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 08:44:57.000000 survey-4.5.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-18 08:44:57.000000 survey-4.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 08:44:57.000000 survey-4.5.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-18 08:44:57.000000 survey-4.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-18 08:45:11.228669 survey-4.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-18 08:44:57.000000 survey-4.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-18 08:44:57.000000 survey-4.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.220670 survey-4.5.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.224670 survey-4.5.2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/graphics.lineprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/graphics.spinprogress-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.done-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.fail-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/printers.info-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92650 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.basket-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    64730 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.basket-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.conceal-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    46839 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.datetime-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    25618 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.datetime-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    52677 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.form-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.input-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.input-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.inquire-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.numeric-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.numeric-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    27647 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.select-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39313 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/routines.select-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   472099 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/showcase-1.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   121555 2023-07-18 08:44:57.000000 survey-4.5.2/docs/_static/images/showcase-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-18 08:44:57.000000 survey-4.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-18 08:44:57.000000 survey-4.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 08:44:57.000000 survey-4.5.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 08:44:57.000000 survey-4.5.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:45:11.228669 survey-4.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-18 08:44:57.000000 survey-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-18 08:44:57.000000 survey-4.5.2/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30730 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58184 2023-07-18 08:44:57.000000 survey-4.5.2/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:45:11.228669 survey-4.5.2/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 08:45:11.000000 survey-4.5.2/survey.egg-info/top_level.txt
```

### Comparing `survey-4.5.1/.github/workflows/publish.yml` & `survey-4.5.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/.gitignore` & `survey-4.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/LICENSE` & `survey-4.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/PKG-INFO` & `survey-4.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.1
+Version: 4.5.2
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.1/README.rst` & `survey-4.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/Makefile` & `survey-4.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/graphics.lineprogress-1.gif` & `survey-4.5.2/docs/_static/images/graphics.lineprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/graphics.spinprogress-1.gif` & `survey-4.5.2/docs/_static/images/graphics.spinprogress-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/printers.done-1.png` & `survey-4.5.2/docs/_static/images/printers.done-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/printers.fail-1.png` & `survey-4.5.2/docs/_static/images/printers.fail-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/printers.info-1.png` & `survey-4.5.2/docs/_static/images/printers.info-1.png`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.basket-1.gif` & `survey-4.5.2/docs/_static/images/routines.basket-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.basket-2.gif` & `survey-4.5.2/docs/_static/images/routines.basket-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.conceal-1.gif` & `survey-4.5.2/docs/_static/images/routines.conceal-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.datetime-1.gif` & `survey-4.5.2/docs/_static/images/routines.datetime-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.datetime-2.gif` & `survey-4.5.2/docs/_static/images/routines.datetime-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.form-1.gif` & `survey-4.5.2/docs/_static/images/routines.form-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.input-1.gif` & `survey-4.5.2/docs/_static/images/routines.input-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.input-2.gif` & `survey-4.5.2/docs/_static/images/routines.input-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.inquire-1.gif` & `survey-4.5.2/docs/_static/images/routines.inquire-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.numeric-1.gif` & `survey-4.5.2/docs/_static/images/routines.numeric-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.numeric-2.gif` & `survey-4.5.2/docs/_static/images/routines.numeric-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.select-1.gif` & `survey-4.5.2/docs/_static/images/routines.select-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/routines.select-2.gif` & `survey-4.5.2/docs/_static/images/routines.select-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/showcase-1.gif` & `survey-4.5.2/docs/_static/images/showcase-1.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/_static/images/showcase-2.gif` & `survey-4.5.2/docs/_static/images/showcase-2.gif`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/conf.py` & `survey-4.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/index.rst` & `survey-4.5.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/make.bat` & `survey-4.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/docs/reference.rst` & `survey-4.5.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/setup.py` & `survey-4.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/__init__.py` & `survey-4.5.2/survey/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_colors.py` & `survey-4.5.2/survey/_colors.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_controls.py` & `survey-4.5.2/survey/_controls.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/__init__.py` & `survey-4.5.2/survey/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_ansi.py` & `survey-4.5.2/survey/_core/_ansi.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_console.py` & `survey-4.5.2/survey/_core/_console.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_cursor.py` & `survey-4.5.2/survey/_core/_cursor.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_handle.py` & `survey-4.5.2/survey/_core/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_helpers.py` & `survey-4.5.2/survey/_core/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_io.py` & `survey-4.5.2/survey/_core/_io.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_io_os.py` & `survey-4.5.2/survey/_core/_io_os.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_io_os_nt.py` & `survey-4.5.2/survey/_core/_io_os_nt.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_io_os_posix.py` & `survey-4.5.2/survey/_core/_io_os_posix.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_render.py` & `survey-4.5.2/survey/_core/_render.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_screen.py` & `survey-4.5.2/survey/_core/_screen.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_core/_source.py` & `survey-4.5.2/survey/_core/_source.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_funnels.py` & `survey-4.5.2/survey/_funnels.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_graphics.py` & `survey-4.5.2/survey/_graphics.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_handle.py` & `survey-4.5.2/survey/_handle.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_helpers.py` & `survey-4.5.2/survey/_helpers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_mutates.py` & `survey-4.5.2/survey/_mutates.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_printers.py` & `survey-4.5.2/survey/_printers.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_routines.py` & `survey-4.5.2/survey/_routines.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_searches.py` & `survey-4.5.2/survey/_searches.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_stage.py` & `survey-4.5.2/survey/_stage.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_theme.py` & `survey-4.5.2/survey/_theme.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_utils.py` & `survey-4.5.2/survey/_utils.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_visuals.py` & `survey-4.5.2/survey/_visuals.py`

 * *Files identical despite different names*

### Comparing `survey-4.5.1/survey/_widgets.py` & `survey-4.5.2/survey/_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
         Used as :paramref:`.handle.Handle.callback`.
     :param delegate:
         Used with ``(event)`` and decides whether to continue the invokation.
     :param validate:
         Used with ``(result)`` upon submission, forbidden by raising :exc:`.Abort`.
     """
 
-    _mark_result_c = object()
+    _product_mark = object()
 
-    __slots__ = ('_mutate', '_handle', '_visual', '_delegate', '_validate', '_escapable', '_result_c')
+    __slots__ = ('_mutate', '_handle', '_visual', '_delegate', '_validate', '_escapable', '_product')
 
     def __init_subclass__(cls, controls = (), **kwargs):
 
         pre_controls = getattr(cls, '_controls', ())
         
         cls._controls = (*pre_controls, *controls)
 
@@ -96,15 +96,15 @@
                  callback : _type_Widget_init_callback  = None, 
                  delegate : _type_Widget_init_delegate  = None,
                  validate : _type_Widget_init_validate  = None,
                  escapable: _type_Widget_init_escapable = False):
         
         self._delegate = delegate
         self._validate = validate
-        self._result_c = self._mark_result_c
+        self._product = self._product_mark
 
         self._mutate = mutate
 
         handle = _handle.Handle(mutate, callback = callback)
 
         for control in self._controls:
             handle.add(control)
@@ -119,46 +119,52 @@
 
         """
         The underlying mutate.
         """
 
         return self._mutate
     
+    def _prepare(self, value):
+
+        return value
+    
     def _resolve(self):
 
         raise NotImplemented()
     
     def resolve(self):
 
         """
         Get the resolved value.
         """
 
-        result = self._result_c
+        value = self._product
 
-        if result is self._mark_result_c:
-            result = self._resolve()
+        if value is self._product_mark:
+            value = self._resolve()
 
-        return result
+        value = self._prepare(value)
+
+        return value
     
     def _invoke_validate(self):
 
         validate = self._validate
 
         if validate is None:
             return
 
-        result = self._result_c
+        value = self._product
 
-        if result is self._mark_result_c:
-            result = self._result_c = self._resolve()
+        if value is self._product_mark:
+            value = self._product = self._resolve()
 
-        validate(result)
+        validate(value)
         
-        self._result_c = self._mark_result_c
+        self._product = self._product_mark
 
     def _invoke(self, event, *args, **kwargs):
 
         if self._delegate and not self._delegate(event):
             return
 
         try:
@@ -636,25 +642,25 @@
             value = value,
             funnel_leave = funnel_leave,
             **kwargs
         )
 
     def _resolve(self):
 
-        result = super()._resolve()
+        value = super()._resolve()
 
-        if result == '-':
-            result = '0'
+        if value == '-':
+            value = '0'
 
-        if result.endswith('.'):
-            result = f'{result}0'
+        if value.endswith('.'):
+            value = f'{value}0'
 
-        result = self._transform(self._transform_abort_message, result)
+        value = self._transform(self._transform_abort_message, value)
 
-        return result
+        return value
 
 
 _type_Conceal_init_rune  = str
 _type_Conceal_init_color = typing.Union[None, int]
 
 
 class Conceal(Input):
@@ -742,15 +748,15 @@
         handle = _handle.Handle()
 
         @handle.add
         @_controls.get((_handle.EventType.enter, _core.Event.enter))
         def _control_submit_enter(info):
             if _helpers.check_lines(self._mutate.lines) or default is self._default_mark:
                 raise Abort(None)
-            self._result_c = default
+            self._product = default
             raise _core.Terminate()
 
         _state = NotImplemented
         
         @handle.add
         @_controls.get((_handle.EventType.enter, _core.Event.insert))
         def _control_insert_enter(info):
@@ -765,15 +771,15 @@
                 value = transform(value)
             try:
                 evaluate(value)
             except Abort:
                 self._mutate.set_state(_state); raise
             if not validate(value):
                 return
-            self._result_c = value
+            self._product = value
             raise _core.Terminate()
         
         callback = _helpers.chain_functions(callback, handle.invoke)
 
         super().__init__(
             *args, 
             validate = None,
@@ -816,40 +822,40 @@
                  **kwargs):
 
         if not transform is None:
             options = dict(zip(map(transform, options), options.values()))
 
         self._options = options
         
-        def evaluate(result):
+        def evaluate(value):
             for option in options:
-                if option.startswith(result):
+                if option.startswith(value):
                     return
             raise Abort(None)
         
-        def validate(result):
-            return result in options
+        def validate(value):
+            return value in options
         
         super().__init__(
             evaluate, 
             validate, 
             *args, 
             transform = transform,
             **kwargs
         )
 
-    def _resolve(self):
+    def _prepare(self, value):
 
-        result = super()._resolve()
+        value = super()._prepare(value)
 
-        option = self._options[result]
+        value = self._options[value]
 
-        return option
+        return value
+    
     
-
 def _focus_nil(spot):
 
     return False
 
 
 def _focus_all(spot): 
 
@@ -1710,17 +1716,17 @@
         kwargs = {}
         for (index, name) in enumerate(self._datetime_attrs):
             spot = _get_mesh_spot(self._axis, index)
             tile = self._mutate.tiles[spot]
             value = tile.resolve()
             kwargs[name] = value
 
-        result = self._convert(kwargs)
+        value = self._convert(kwargs)
 
-        return result
+        return value
     
 
 _Form_tile_focus = lambda event: True
     
 
 class Form(BaseList):
```

### Comparing `survey-4.5.1/survey.egg-info/PKG-INFO` & `survey-4.5.2/survey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 4.5.1
+Version: 4.5.2
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
 Requires-Python: >=3.7
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `survey-4.5.1/survey.egg-info/SOURCES.txt` & `survey-4.5.2/survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

