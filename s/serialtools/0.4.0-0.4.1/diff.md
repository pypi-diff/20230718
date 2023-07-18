# Comparing `tmp/serialtools-0.4.0.tar.gz` & `tmp/serialtools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.4.0.tar` & `serialtools-0.4.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.4.0/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.4.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.4.0/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.4.0/README.md
--rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/Makefile
--rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.4.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-07-18 09:23:16.478727 serialtools-0.4.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-07-18 09:23:17.898724 serialtools-0.4.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-07-18 09:23:16.478727 serialtools-0.4.0/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-07-18 09:23:17.902057 serialtools-0.4.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-07-18 09:23:17.892057 serialtools-0.4.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    28591 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0    15924 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/index.html
--rw-r--r--   0        0        0    10612 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/modules.html
--rw-r--r--   0        0        0     1348 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6959 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4930 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/search.html
--rw-r--r--   0        0        0    24908 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14727 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12315 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10619 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    13490 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.rawsplit.html
--rw-r--r--   0        0        0    10817 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    48292 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    74268 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    34482 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    32348 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/source/conf.py
--rw-r--r--   0        0        0     1014 2023-07-18 09:23:15.592062 serialtools-0.4.0/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      163 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.rawsplit.rst
--rw-r--r--   0        0        0      302 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.4.0/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.4.0/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.4.0/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.4.0/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.4.0/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.4.0/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-07-18 09:25:09.205155 serialtools-0.4.0/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1448 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/__main__.py
--rw-r--r--   0        0        0      345 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-07-18 09:23:15.515395 serialtools-0.4.0/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1346 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0     1369 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/rawsplit.py
--rw-r--r--   0        0        0      880 2023-07-18 09:23:15.515395 serialtools-0.4.0/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     7356 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/bus.py
--rw-r--r--   0        0        0    15004 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/database.py
--rw-r--r--   0        0        0     5481 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.4.0/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.4.0/tox.ini
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.4.1/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.4.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.4.1/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.4.1/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/Makefile
+-rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.4.1/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.4.1/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.4.1/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-07-18 10:11:01.875621 serialtools-0.4.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-07-18 10:11:03.242286 serialtools-0.4.1/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-07-18 10:11:01.875621 serialtools-0.4.1/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-07-18 10:11:03.242286 serialtools-0.4.1/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-07-18 10:11:03.238953 serialtools-0.4.1/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.4.1/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    28591 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    15924 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/index.html
+-rw-r--r--   0        0        0    10612 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1348 2023-07-18 10:11:03.255620 serialtools-0.4.1/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6959 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4930 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/search.html
+-rw-r--r--   0        0        0    24908 2023-07-18 10:11:03.252286 serialtools-0.4.1/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14727 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12315 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10619 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    13490 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/serialtools.apps.rawsplit.html
+-rw-r--r--   0        0        0    10817 2023-07-18 10:11:24.508912 serialtools-0.4.1/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    48292 2023-07-18 10:11:24.512245 serialtools-0.4.1/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    74268 2023-07-18 10:11:24.512245 serialtools-0.4.1/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    34482 2023-07-18 10:11:24.512245 serialtools-0.4.1/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    32348 2023-07-18 10:11:24.512245 serialtools-0.4.1/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.4.1/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.4.1/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.4.1/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-07-18 10:11:24.512245 serialtools-0.4.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1014 2023-07-18 10:11:01.032288 serialtools-0.4.1/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      163 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.apps.rawsplit.rst
+-rw-r--r--   0        0        0      302 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-07-18 10:11:00.968955 serialtools-0.4.1/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.4.1/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.4.1/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.4.1/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.4.1/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.4.1/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.4.1/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-07-18 10:11:24.512245 serialtools-0.4.1/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-18 10:11:00.965622 serialtools-0.4.1/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      345 2023-07-18 10:11:00.965622 serialtools-0.4.1/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-18 10:11:00.968955 serialtools-0.4.1/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1380 2023-07-18 10:11:24.512245 serialtools-0.4.1/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0     1369 2023-07-18 10:11:00.965622 serialtools-0.4.1/src/serialtools/apps/rawsplit.py
+-rw-r--r--   0        0        0      880 2023-07-18 10:11:00.968955 serialtools-0.4.1/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     7356 2023-07-18 10:11:00.962288 serialtools-0.4.1/src/serialtools/bus.py
+-rw-r--r--   0        0        0    15004 2023-07-18 10:11:00.962288 serialtools-0.4.1/src/serialtools/database.py
+-rw-r--r--   0        0        0     5481 2023-07-18 10:11:00.962288 serialtools-0.4.1/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.4.1/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.4.1/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.4.1/PKG-INFO
```

### Comparing `serialtools-0.4.0/LICENSE` & `serialtools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/Makefile` & `serialtools-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_sources/index.rst.txt` & `serialtools-0.4.1/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.4.1/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/basic.css` & `serialtools-0.4.1/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/badge_only.css` & `serialtools-0.4.1/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.4.1/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/css/theme.css` & `serialtools-0.4.1/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/doctools.js` & `serialtools-0.4.1/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/jquery.js` & `serialtools-0.4.1/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/js/badge_only.js` & `serialtools-0.4.1/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.4.1/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.4.1/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/js/theme.js` & `serialtools-0.4.1/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/language_data.js` & `serialtools-0.4.1/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/pygments.css` & `serialtools-0.4.1/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/searchtools.js` & `serialtools-0.4.1/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.4.1/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/genindex.html` & `serialtools-0.4.1/docs/build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.4.0 documentation</title>
+  <title>Index &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -31,15 +31,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.0/docs/build/html/index.html` & `serialtools-0.4.1/docs/build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.4.0 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.0/docs/build/html/modules.html` & `serialtools-0.4.1/docs/build/html/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -32,15 +32,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.0/docs/build/html/objects.inv` & `serialtools-0.4.1/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/py-modindex.html` & `serialtools-0.4.1/docs/build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.4.0 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.0/docs/build/html/search.html` & `serialtools-0.4.1/docs/build/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.4.0 documentation</title>
+  <title>Search &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
     
   <!--[if lt IE 9]>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.4.0/docs/build/html/searchindex.js` & `serialtools-0.4.1/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.4.1/docs/build/html/serialtools.apps.decode.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.4.1/docs/build/html/serialtools.apps.dump.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.apps.html` & `serialtools-0.4.1/docs/build/html/serialtools.apps.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.apps.rawsplit.html` & `serialtools-0.4.1/docs/build/html/serialtools.apps.rawsplit.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -33,15 +33,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
           o add_arguments()
           o add_parser()
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.apps.send.html` & `serialtools-0.4.1/docs/build/html/serialtools.apps.send.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.bus.html` & `serialtools-0.4.1/docs/build/html/serialtools.bus.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.database.html` & `serialtools-0.4.1/docs/build/html/serialtools.database.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.database_config.html` & `serialtools-0.4.1/docs/build/html/serialtools.database_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
```

### Comparing `serialtools-0.4.0/docs/build/html/serialtools.html` & `serialtools-0.4.1/docs/build/html/serialtools.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.4.0 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.4.1 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
       <link rel="stylesheet" href="_static/sphinx_paramlinks.css" type="text/css" />
       <link rel="stylesheet" href="_static/no-ligatures-in-code.css" type="text/css" />
       <link rel="stylesheet" href="_static/tab-size.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
@@ -34,15 +34,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             serialtools
           </a>
               <div class="version">
-                v0.4.0
+                v0.4.1
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.4.0
+v0.4.1
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
```

### Comparing `serialtools-0.4.0/docs/make.bat` & `serialtools-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/docs/source/conf.py` & `serialtools-0.4.1/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.4.0'
+release = 'v0.4.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.4.0/docs/source/index.rst` & `serialtools-0.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/prepare_for_gitlab_pages.py` & `serialtools-0.4.1/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/pyproject.toml` & `serialtools-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/release.sh` & `serialtools-0.4.1/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/__main__.py` & `serialtools-0.4.1/src/serialtools/__main__.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/apps/decode.py` & `serialtools-0.4.1/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/apps/dump.py` & `serialtools-0.4.1/src/serialtools/apps/dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 from serialtools.bus import bus_creator, Bus, WriteToFileBus
 
 
 break_time_ms = Config('dump.break-time', 100, unit='ms', help="When nothing is received for this time span a line break and time stamp are written, a negative value disables line breaks and time stamps")
 
 def add_parser(subparsers: 'argparse._SubParsersAction[typing.Any]') -> None:
 	parser = subparsers.add_parser(__name__.rsplit('.', 1)[-1], help=__doc__)
-	parser.add_argument('--break-time', default=break_time_ms.value, help=typing.cast(str, break_time_ms.help))
+	parser.add_argument('--break-time', type=int, help=typing.cast(str, break_time_ms.help))
 	bus_creator.add_arguments(parser)
 	parser.set_defaults(func=main)
 
 def main(args: 'argparse.Namespace') -> None:
 	bus = bus_creator.create_bus(args)
-	dump(bus, break_time_ms=args.break_time)
+	dump(bus,
+		break_time_ms = break_time_ms if args.break_time is None else args.break_time,
+	)
 
 def dump(bus: Bus, *, break_time_ms: int = break_time_ms.value, file: 'typing.TextIO|None' = None) -> None:
 	out = WriteToFileBus(file, break_time_ms=break_time_ms)
 	while True:
 		try:
 			read_bytes = bus.read(1)
 		except serial.serialutil.SerialException as e:
```

### Comparing `serialtools-0.4.0/src/serialtools/apps/rawsplit.py` & `serialtools-0.4.1/src/serialtools/apps/rawsplit.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/apps/send.py` & `serialtools-0.4.1/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/bus.py` & `serialtools-0.4.1/src/serialtools/bus.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/database.py` & `serialtools-0.4.1/src/serialtools/database.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/src/serialtools/database_config.py` & `serialtools-0.4.1/src/serialtools/database_config.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.4.0/PKG-INFO` & `serialtools-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

