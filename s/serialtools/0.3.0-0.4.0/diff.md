# Comparing `tmp/serialtools-0.3.0.tar.gz` & `tmp/serialtools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serialtools-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "serialtools-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `serialtools-0.3.0.tar` & `serialtools-0.4.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.3.0/.gitignore
--rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.3.0/LICENSE
--rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.3.0/README.md
--rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/Makefile
--rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.3.0/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/modules.rst.txt
--rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
--rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
--rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.rst.txt
--rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
--rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.bus.rst.txt
--rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.database.rst.txt
--rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.3.0/docs/build/html/_sources/serialtools.database_config.rst.txt
--rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_sources/serialtools.rst.txt
--rw-r--r--   0        0        0     4289 2023-06-26 12:52:22.152933 serialtools-0.3.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    14813 2023-06-26 12:52:23.526288 serialtools-0.3.0/docs/build/html/_static/basic.css
--rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/doctools.js
--rw-r--r--   0        0        0      421 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/file.png
--rw-r--r--   0        0        0    89501 2023-06-26 12:52:22.152933 serialtools-0.3.0/docs/build/html/_static/jquery.js
--rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/js/theme.js
--rw-r--r--   0        0        0     4758 2023-06-26 12:52:23.529621 serialtools-0.3.0/docs/build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/minus.png
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/plus.png
--rw-r--r--   0        0        0     4819 2023-06-26 12:52:23.522954 serialtools-0.3.0/docs/build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/sphinx_paramlinks.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.3.0/docs/build/html/_static/tab-size.css
--rw-r--r--   0        0        0    28033 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/genindex.html
--rw-r--r--   0        0        0    15719 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/index.html
--rw-r--r--   0        0        0    10407 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/modules.html
--rw-r--r--   0        0        0     1318 2023-06-26 12:52:23.542955 serialtools-0.3.0/docs/build/html/objects.inv
--rw-r--r--   0        0        0     6959 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/py-modindex.html
--rw-r--r--   0        0        0     4930 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/search.html
--rw-r--r--   0        0        0    24058 2023-06-26 12:52:23.539621 serialtools-0.3.0/docs/build/html/searchindex.js
--rw-r--r--   0        0        0    14727 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.decode.html
--rw-r--r--   0        0        0    12315 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.dump.html
--rw-r--r--   0        0        0    10619 2023-06-26 12:53:35.177407 serialtools-0.3.0/docs/build/html/serialtools.apps.html
--rw-r--r--   0        0        0    13490 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.apps.rawsplit.html
--rw-r--r--   0        0        0    10817 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.apps.send.html
--rw-r--r--   0        0        0    44921 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.bus.html
--rw-r--r--   0        0        0    71095 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.database.html
--rw-r--r--   0        0        0    34482 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.database_config.html
--rw-r--r--   0        0        0    31448 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/build/html/serialtools.html
--rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/source/_static/no-ligatures-in-code.css
--rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.3.0/docs/source/_static/tab-size.css
--rw-r--r--   0        0        0     3095 2023-06-26 12:53:35.180740 serialtools-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0     1014 2023-06-26 12:52:21.286253 serialtools-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       70 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/modules.rst
--rw-r--r--   0        0        0      157 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.decode.rst
--rw-r--r--   0        0        0      151 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.apps.dump.rst
--rw-r--r--   0        0        0      163 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.rawsplit.rst
--rw-r--r--   0        0        0      302 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.rst
--rw-r--r--   0        0        0      151 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.apps.send.rst
--rw-r--r--   0        0        0      133 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.bus.rst
--rw-r--r--   0        0        0      148 2023-06-26 12:52:21.226252 serialtools-0.3.0/docs/source/serialtools.database.rst
--rw-r--r--   0        0        0      171 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.database_config.rst
--rw-r--r--   0        0        0      360 2023-06-26 12:52:21.222918 serialtools-0.3.0/docs/source/serialtools.rst
--rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.3.0/mypy.ini
--rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.3.0/prepare_for_gitlab_pages.py
--rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.3.0/pyproject.toml
--rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.3.0/release.sh
--rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.3.0/requirements-release.txt
--rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.3.0/requirements-test.txt
--rw-r--r--   0        0        0       87 2023-06-26 12:53:34.554064 serialtools-0.3.0/src/serialtools/__init__.py
--rw-r--r--   0        0        0     1448 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/__main__.py
--rw-r--r--   0        0        0      345 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/__init__.py
--rw-r--r--   0        0        0     1143 2023-06-26 12:52:21.222918 serialtools-0.3.0/src/serialtools/apps/decode.py
--rw-r--r--   0        0        0     1346 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/dump.py
--rw-r--r--   0        0        0     1369 2023-06-26 12:52:21.219585 serialtools-0.3.0/src/serialtools/apps/rawsplit.py
--rw-r--r--   0        0        0      880 2023-06-26 12:52:21.222918 serialtools-0.3.0/src/serialtools/apps/send.py
--rw-r--r--   0        0        0     6136 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/bus.py
--rw-r--r--   0        0        0    13898 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/database.py
--rw-r--r--   0        0        0     5193 2023-06-26 12:52:21.216252 serialtools-0.3.0/src/serialtools/database_config.py
--rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.3.0/src/serialtools/py.typed
--rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.3.0/tox.ini
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2023-06-02 06:55:40.811546 serialtools-0.4.0/.gitignore
+-rw-r--r--   0        0        0      119 2023-06-21 10:33:17.761717 serialtools-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      657 2023-06-21 08:53:39.687960 serialtools-0.4.0/LICENSE
+-rw-r--r--   0        0        0      444 2023-06-21 10:33:17.761717 serialtools-0.4.0/README.md
+-rw-r--r--   0        0        0      638 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1014 2023-06-26 12:52:04.102651 serialtools-0.4.0/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0       70 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      157 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.decode.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.dump.rst.txt
+-rw-r--r--   0        0        0      163 2023-06-26 12:52:04.102651 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.rawsplit.rst.txt
+-rw-r--r--   0        0        0      302 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.rst.txt
+-rw-r--r--   0        0        0      151 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.apps.send.rst.txt
+-rw-r--r--   0        0        0      133 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.bus.rst.txt
+-rw-r--r--   0        0        0      148 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.database.rst.txt
+-rw-r--r--   0        0        0      171 2023-06-21 10:33:17.761717 serialtools-0.4.0/docs/build/html/_sources/serialtools.database_config.rst.txt
+-rw-r--r--   0        0        0      360 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_sources/serialtools.rst.txt
+-rw-r--r--   0        0        0     4289 2023-07-18 09:23:16.478727 serialtools-0.4.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    14813 2023-07-18 09:23:17.898724 serialtools-0.4.0/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     3229 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0    87624 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2023-06-21 10:33:17.765050 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2023-06-21 10:33:17.768383 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2023-06-21 10:33:17.771717 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2023-06-21 10:33:17.775050 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2023-06-21 10:33:17.778383 serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0   135314 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0     4472 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      421 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2023-07-18 09:23:16.478727 serialtools-0.4.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0      934 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4758 2023-07-18 09:23:17.902057 serialtools-0.4.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0       90 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4819 2023-07-18 09:23:17.892057 serialtools-0.4.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      204 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/sphinx_paramlinks.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.781717 serialtools-0.4.0/docs/build/html/_static/tab-size.css
+-rw-r--r--   0        0        0    28591 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/genindex.html
+-rw-r--r--   0        0        0    15924 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/index.html
+-rw-r--r--   0        0        0    10612 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/modules.html
+-rw-r--r--   0        0        0     1348 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     6959 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4930 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/search.html
+-rw-r--r--   0        0        0    24908 2023-07-18 09:25:09.201822 serialtools-0.4.0/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0    14727 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.decode.html
+-rw-r--r--   0        0        0    12315 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.dump.html
+-rw-r--r--   0        0        0    10619 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.html
+-rw-r--r--   0        0        0    13490 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.rawsplit.html
+-rw-r--r--   0        0        0    10817 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.apps.send.html
+-rw-r--r--   0        0        0    48292 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.bus.html
+-rw-r--r--   0        0        0    74268 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.database.html
+-rw-r--r--   0        0        0    34482 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.database_config.html
+-rw-r--r--   0        0        0    32348 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/build/html/serialtools.html
+-rw-r--r--   0        0        0      804 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0       46 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/source/_static/no-ligatures-in-code.css
+-rw-r--r--   0        0        0      117 2023-06-21 10:33:17.785050 serialtools-0.4.0/docs/source/_static/tab-size.css
+-rw-r--r--   0        0        0     3095 2023-07-18 09:25:09.205155 serialtools-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1014 2023-07-18 09:23:15.592062 serialtools-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0       70 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/modules.rst
+-rw-r--r--   0        0        0      157 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.decode.rst
+-rw-r--r--   0        0        0      151 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.apps.dump.rst
+-rw-r--r--   0        0        0      163 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.rawsplit.rst
+-rw-r--r--   0        0        0      302 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.rst
+-rw-r--r--   0        0        0      151 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.apps.send.rst
+-rw-r--r--   0        0        0      133 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.bus.rst
+-rw-r--r--   0        0        0      148 2023-07-18 09:23:15.518728 serialtools-0.4.0/docs/source/serialtools.database.rst
+-rw-r--r--   0        0        0      171 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.database_config.rst
+-rw-r--r--   0        0        0      360 2023-07-18 09:23:15.515395 serialtools-0.4.0/docs/source/serialtools.rst
+-rw-r--r--   0        0        0      170 2023-06-23 15:21:45.869968 serialtools-0.4.0/mypy.ini
+-rw-r--r--   0        0        0     4135 2023-06-21 10:33:17.785050 serialtools-0.4.0/prepare_for_gitlab_pages.py
+-rw-r--r--   0        0        0      786 2023-06-23 15:21:45.869968 serialtools-0.4.0/pyproject.toml
+-rwxr-xr-x   0        0        0    12230 2023-06-21 10:33:17.785050 serialtools-0.4.0/release.sh
+-rw-r--r--   0        0        0       83 2023-06-21 10:33:17.785050 serialtools-0.4.0/requirements-release.txt
+-rw-r--r--   0        0        0       22 2023-06-21 10:33:17.785050 serialtools-0.4.0/requirements-test.txt
+-rw-r--r--   0        0        0       87 2023-07-18 09:25:09.205155 serialtools-0.4.0/src/serialtools/__init__.py
+-rw-r--r--   0        0        0     1448 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/__main__.py
+-rw-r--r--   0        0        0      345 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/__init__.py
+-rw-r--r--   0        0        0     1143 2023-07-18 09:23:15.515395 serialtools-0.4.0/src/serialtools/apps/decode.py
+-rw-r--r--   0        0        0     1346 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/dump.py
+-rw-r--r--   0        0        0     1369 2023-07-18 09:23:15.512062 serialtools-0.4.0/src/serialtools/apps/rawsplit.py
+-rw-r--r--   0        0        0      880 2023-07-18 09:23:15.515395 serialtools-0.4.0/src/serialtools/apps/send.py
+-rw-r--r--   0        0        0     7356 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/bus.py
+-rw-r--r--   0        0        0    15004 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/database.py
+-rw-r--r--   0        0        0     5481 2023-07-18 09:25:09.208488 serialtools-0.4.0/src/serialtools/database_config.py
+-rw-r--r--   0        0        0        0 2022-11-03 16:33:53.710006 serialtools-0.4.0/src/serialtools/py.typed
+-rw-r--r--   0        0        0      336 2023-06-23 15:21:45.869968 serialtools-0.4.0/tox.ini
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 serialtools-0.4.0/PKG-INFO
```

### Comparing `serialtools-0.3.0/LICENSE` & `serialtools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/Makefile` & `serialtools-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_sources/index.rst.txt` & `serialtools-0.4.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js` & `serialtools-0.4.0/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/basic.css` & `serialtools-0.4.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/badge_only.css` & `serialtools-0.4.0/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `serialtools-0.4.0/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/css/theme.css` & `serialtools-0.4.0/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/doctools.js` & `serialtools-0.4.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/jquery.js` & `serialtools-0.4.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/js/badge_only.js` & `serialtools-0.4.0/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `serialtools-0.4.0/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/js/html5shiv.min.js` & `serialtools-0.4.0/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/js/theme.js` & `serialtools-0.4.0/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/language_data.js` & `serialtools-0.4.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/pygments.css` & `serialtools-0.4.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/searchtools.js` & `serialtools-0.4.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/_static/sphinx_highlight.js` & `serialtools-0.4.0/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/build/html/genindex.html` & `serialtools-0.4.0/docs/build/html/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; serialtools v0.3.0 documentation</title>
+  <title>Index &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -112,42 +112,46 @@
         <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.add_arguments">(in module serialtools.apps.decode)</a>
 </li>
         <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_arguments">(in module serialtools.apps.rawsplit)</a>
 </li>
         <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.add_arguments">(serialtools.bus.BusCreator method)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.apps.decode.html#serialtools.apps.decode.add_parser">add_parser() (in module serialtools.apps.decode)</a>
 
       <ul>
         <li><a href="serialtools.apps.dump.html#serialtools.apps.dump.add_parser">(in module serialtools.apps.dump)</a>
 </li>
         <li><a href="serialtools.apps.rawsplit.html#serialtools.apps.rawsplit.add_parser">(in module serialtools.apps.rawsplit)</a>
 </li>
         <li><a href="serialtools.apps.send.html#serialtools.apps.send.add_parser">(in module serialtools.apps.send)</a>
 </li>
       </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.MessageSpec.ADDRESS">ADDRESS (serialtools.database.MessageSpec attribute)</a>
 </li>
+      <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.auto_create_virtual_bus">auto_create_virtual_bus (serialtools.bus.BusCreator attribute)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="B">B</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.baudrate">baudrate (serialtools.bus.BusCreator attribute)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.Endianness.BIG">BIG (serialtools.database.Endianness attribute)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.Type.BOOL">BOOL (serialtools.database.Type attribute)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="serialtools.bus.html#serialtools.bus.bus_creator">bus_creator (in module serialtools.bus)</a>
+</li>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator">BusCreator (class in serialtools.bus)</a>
 </li>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.bytesize">bytesize (serialtools.bus.BusCreator attribute)</a>
 </li>
       <li><a href="serialtools.database.html#serialtools.database.ByteSpec">ByteSpec (class in serialtools.database)</a>
 </li>
   </ul></td>
@@ -286,14 +290,16 @@
 </tr></table>
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Reader.ignore_bytes_between_messages">ignore_bytes_between_messages (serialtools.database.Reader attribute)</a>
 </li>
+      <li><a href="serialtools.database.html#serialtools.database.Signal.init">init() (serialtools.database.Signal method)</a>
+</li>
       <li><a href="serialtools.database_config.html#serialtools.database_config.Message.init_parser">init_parser() (serialtools.database_config.Message method)</a>
 
       <ul>
         <li><a href="serialtools.database_config.html#serialtools.database_config.Param.init_parser">(serialtools.database_config.Param method)</a>
 </li>
         <li><a href="serialtools.database_config.html#serialtools.database_config.Signal.init_parser">(serialtools.database_config.Signal method)</a>
 </li>
@@ -554,14 +560,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.virtual">virtual (serialtools.bus.BusCreator attribute)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.vport">vport (serialtools.bus.BusCreator attribute)</a>
 </li>
+      <li><a href="serialtools.bus.html#serialtools.bus.BusCreator.vport_other">vport_other (serialtools.bus.BusCreator attribute)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="W">W</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="serialtools.database.html#serialtools.database.Database.word_length_in_bits">word_length_in_bits (serialtools.database.Database attribute)</a>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -19,34 +19,40 @@
     * serialtools.database_config_module
    serialtools
     * Index
 ===============================================================================
 ****** Index ******
 A | B | C | D | E | F | G | I | L | M | P | R | S | T | U | V | W | X
 ***** A *****
-                                            * add_parser()_(in_module
-    * add_arguments()_(in_module              serialtools.apps.decode)
-      serialtools.apps)                           o (in_module
-          o (in_module                              serialtools.apps.dump)
-            serialtools.apps.decode)              o (in_module
-          o (in_module                              serialtools.apps.rawsplit)
-            serialtools.apps.rawsplit)            o (in_module
-          o (serialtools.bus.BusCreator             serialtools.apps.send)
-            method)                         * ADDRESS_
-                                              (serialtools.database.MessageSpec
-                                              attribute)
+    * add_arguments()_(in_module
+      serialtools.apps)
+          o (in_module
+            serialtools.apps.decode)
+          o (in_module
+            serialtools.apps.rawsplit)      * ADDRESS_
+          o (serialtools.bus.BusCreator       (serialtools.database.MessageSpec
+            method)                           attribute)
+    * add_parser()_(in_module               * auto_create_virtual_bus_
+      serialtools.apps.decode)                (serialtools.bus.BusCreator
+          o (in_module                        attribute)
+            serialtools.apps.dump)
+          o (in_module
+            serialtools.apps.rawsplit)
+          o (in_module
+            serialtools.apps.send)
 ***** B *****
-    * baudrate_                            * BusCreator_(class_in
+    * baudrate_                            * bus_creator_(in_module
       (serialtools.bus.BusCreator            serialtools.bus)
-      attribute)                           * bytesize_
-    * BIG_                                   (serialtools.bus.BusCreator
-      (serialtools.database.Endianness       attribute)
+      attribute)                           * BusCreator_(class_in
+    * BIG_                                   serialtools.bus)
+      (serialtools.database.Endianness     * bytesize_
+      attribute)                             (serialtools.bus.BusCreator
+    * BOOL_(serialtools.database.Type        attribute)
       attribute)                           * ByteSpec_(class_in
-    * BOOL_(serialtools.database.Type        serialtools.database)
-      attribute)
+                                             serialtools.database)
 ***** C *****
     * cancel_read()_                            * close()_
       (serialtools.bus.ReadFromFileBus            (serialtools.bus.ReadFromFileBus
       method)                                     method)
           o (serialtools.bus.WriteToFileBus           o (serialtools.bus.WriteToFileBus
             method)                                     method)
     * cancel_write()_                           * create_args()_
@@ -97,19 +103,21 @@
       serialtools.database_config)                       (serialtools.database.Database
     * get_endianness_fmt()_                              method)
       (serialtools.database.Database_method)           * get_timestamp()_(in_module
                                                          serialtools.bus)
 ***** I *****
     * ignore_bytes_between_messages_
       (serialtools.database.Reader_attribute)
-    * init_parser()_                                * INT_
-      (serialtools.database_config.Message            (serialtools.database.Type
-      method)                                         attribute)
-          o (serialtools.database_config.Param      * integer()_(in_module
-            method)                                   serialtools.database_config)
+    * init()_(serialtools.database.Signal
+      method)                                       * INT_
+    * init_parser()_                                  (serialtools.database.Type
+      (serialtools.database_config.Message            attribute)
+      method)                                       * integer()_(in_module
+          o (serialtools.database_config.Param        serialtools.database_config)
+            method)
           o (serialtools.database_config.Signal
             method)
 ***** L *****
     * LITTLE_(serialtools.database.Endianness_attribute)
 ***** M *****
     * main()_(in_module
       serialtools.apps.decode)
@@ -181,17 +189,19 @@
       (serialtools.bus.ReadFromFileBus            serialtools.database)
       attribute)
           o (serialtools.bus.WriteToFileBus
             attribute)
 ***** U *****
     * UINT_(serialtools.database.Type_attribute)
 ***** V *****
-    * virtual_                        * vport_(serialtools.bus.BusCreator
-      (serialtools.bus.BusCreator       attribute)
-      attribute)
+                                      * vport_(serialtools.bus.BusCreator
+    * virtual_                          attribute)
+      (serialtools.bus.BusCreator     * vport_other_
+      attribute)                        (serialtools.bus.BusCreator
+                                        attribute)
 ***** W *****
                                                              * write()_
     * word_length_in_bits_(serialtools.database.Database       (serialtools.bus.ReadFromFileBus
       attribute)                                               method)
           o (serialtools.database_config.DatabaseCreator           o (serialtools.bus.WriteToFileBus
             attribute)                                               method)
                                                              * WriteToFileBus_(class_in
```

### Comparing `serialtools-0.3.0/docs/build/html/index.html` & `serialtools-0.4.0/docs/build/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.3.0 documentation</title>
+  <title>Welcome to serialtools’ documentation! &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -123,14 +123,15 @@
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromParameterBus"><code class="docutils literal notranslate"><span class="pre">ReadFromParameterBus</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus</span></code></a></li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.bus_creator"><code class="docutils literal notranslate"><span class="pre">bus_creator</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.get_timestamp"><code class="docutils literal notranslate"><span class="pre">get_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database"><code class="docutils literal notranslate"><span class="pre">Database</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a></li>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -49,14 +49,15 @@
           o main()
           o send()
     * serialtools.bus_module
           o BusCreator
           o ReadFromFileBus
           o ReadFromParameterBus
           o WriteToFileBus
+          o bus_creator
           o get_timestamp()
     * serialtools.database_module
           o ByteSpec
           o Database
           o Endianness
           o Message
           o MessageSpec
```

### Comparing `serialtools-0.3.0/docs/build/html/modules.html` & `serialtools-0.4.0/docs/build/html/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -96,14 +96,15 @@
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#submodules">Submodules</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromParameterBus"><code class="docutils literal notranslate"><span class="pre">ReadFromParameterBus</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.bus_creator"><code class="docutils literal notranslate"><span class="pre">bus_creator</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.get_timestamp"><code class="docutils literal notranslate"><span class="pre">get_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Database"><code class="docutils literal notranslate"><span class="pre">Database</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="serialtools.database.html#serialtools.database.Endianness"><code class="docutils literal notranslate"><span class="pre">Endianness</span></code></a></li>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
@@ -29,14 +29,15 @@
                       # Module_contents
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
                       # ReadFromParameterBus
                       # WriteToFileBus
+                      # bus_creator
                       # get_timestamp()
                 # serialtools.database_module
                       # ByteSpec
                       # Database
                       # Endianness
                       # Message
                       # MessageSpec
```

### Comparing `serialtools-0.3.0/docs/build/html/py-modindex.html` & `serialtools-0.4.0/docs/build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; serialtools v0.3.0 documentation</title>
+  <title>Python Module Index &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.3.0/docs/build/html/search.html` & `serialtools-0.4.0/docs/build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; serialtools v0.3.0 documentation</title>
+  <title>Search &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
```

### Comparing `serialtools-0.3.0/docs/build/html/searchindex.js` & `serialtools-0.4.0/docs/build/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -187,15 +187,15 @@
         "0": 9,
         "scale": 9,
         "offset": 9,
         "unit": 9,
         "The": [9, 10],
         "e": 9,
         "g": 9,
-        "us": [9, 10],
+        "us": [8, 9, 10],
         "request": 9,
         "batteri": 9,
         "size": 9,
         "default": [9, 10],
         "word": 9,
         "identifi": 9,
         "sever": 9,
@@ -230,15 +230,15 @@
         "argument": 10,
         "same": 10,
         "like": 10,
         "abstract": 10,
         "method": 10,
         "must": 10,
         "subclass": 10,
-        "list": 10,
+        "list": [9, 10],
         "defin": 10,
         "command": 10,
         "val": 10,
         "sourc": 0,
         "code": 0,
         "bug": 0,
         "tracker": 0,
@@ -251,15 +251,33 @@
         "create_arg": [2, 8],
         "send_msg": [2, 9],
         "rawsplit": 0,
         "messagespec": [0, 1, 2, 9, 10],
         "split": 6,
         "implicit_address": 9,
         "require_sign": 10,
-        "true": 10
+        "true": 10,
+        "bus_creat": [0, 1, 2, 8],
+        "auto_create_virtual_bu": [2, 8],
+        "vport_oth": [2, 8],
+        "init": [2, 9],
+        "creat": 8,
+        "new": 8,
+        "lsb": 9,
+        "transmit": 9,
+        "belong": 9,
+        "least": 9,
+        "signific": 9,
+        "mutual": 9,
+        "exclus": 9,
+        "onli": 9,
+        "one": 9,
+        "them": 9,
+        "mai": 9,
+        "pass": 9
     },
     "objects": {
         "": [
             [2, 0, 0, "-", "serialtools"]
         ],
         "serialtools": [
             [3, 0, 0, "-", "apps"],
@@ -299,29 +317,32 @@
             [7, 1, 1, "", "send"]
         ],
         "serialtools.bus": [
             [8, 2, 1, "", "BusCreator"],
             [8, 2, 1, "", "ReadFromFileBus"],
             [8, 2, 1, "", "ReadFromParameterBus"],
             [8, 2, 1, "", "WriteToFileBus"],
+            [8, 6, 1, "", "bus_creator"],
             [8, 1, 1, "", "get_timestamp"]
         ],
         "serialtools.bus.BusCreator": [
             [8, 3, 1, "", "add_arguments"],
+            [8, 4, 1, "", "auto_create_virtual_bus"],
             [8, 4, 1, "", "baudrate"],
             [8, 4, 1, "", "bytesize"],
             [8, 3, 1, "", "create_args"],
             [8, 3, 1, "", "create_bus"],
             [8, 4, 1, "", "dsrdtr"],
             [8, 4, 1, "", "parity"],
             [8, 4, 1, "", "port"],
             [8, 4, 1, "", "rtscts"],
             [8, 4, 1, "", "stopbits"],
             [8, 4, 1, "", "virtual"],
             [8, 4, 1, "", "vport"],
+            [8, 4, 1, "", "vport_other"],
             [8, 4, 1, "", "xonxoff"]
         ],
         "serialtools.bus.ReadFromFileBus": [
             [8, 3, 1, "", "cancel_read"],
             [8, 3, 1, "", "cancel_write"],
             [8, 3, 1, "", "close"],
             [8, 3, 1, "", "read"],
@@ -388,15 +409,16 @@
             [9, 3, 1, "", "read_in_other_thread"],
             [9, 3, 1, "", "read_msg"],
             [9, 3, 1, "", "read_n_bytes"],
             [9, 3, 1, "", "send_msg"],
             [9, 3, 1, "", "stop"]
         ],
         "serialtools.database.Signal": [
-            [9, 3, 1, "", "get_bitstruct_fmt"]
+            [9, 3, 1, "", "get_bitstruct_fmt"],
+            [9, 3, 1, "", "init"]
         ],
         "serialtools.database.Type": [
             [9, 4, 1, "", "BOOL"],
             [9, 4, 1, "", "FLOAT"],
             [9, 4, 1, "", "INT"],
             [9, 4, 1, "", "TEXT"],
             [9, 4, 1, "", "UINT"]
@@ -442,23 +464,25 @@
     },
     "objtypes": {
         "0": "py:module",
         "1": "py:function",
         "2": "py:class",
         "3": "py:method",
         "4": "py:attribute",
-        "5": "py:parameter"
+        "5": "py:parameter",
+        "6": "py:data"
     },
     "objnames": {
         "0": ["py", "module", "Python module"],
         "1": ["py", "function", "Python function"],
         "2": ["py", "class", "Python class"],
         "3": ["py", "method", "Python method"],
         "4": ["py", "attribute", "Python attribute"],
-        "5": ["py", "parameter", "Python parameter"]
+        "5": ["py", "parameter", "Python parameter"],
+        "6": ["py", "data", "Python data"]
     },
     "titleterms": {
         "welcom": 0,
         "serialtool": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
         "": [],
         "document": 0,
         "indic": 0,
@@ -640,17 +664,23 @@
         ],
         "writetofilebus (class in serialtools.bus)": [
             [8, "serialtools.bus.WriteToFileBus"]
         ],
         "add_arguments() (serialtools.bus.buscreator method)": [
             [8, "serialtools.bus.BusCreator.add_arguments"]
         ],
+        "auto_create_virtual_bus (serialtools.bus.buscreator attribute)": [
+            [8, "serialtools.bus.BusCreator.auto_create_virtual_bus"]
+        ],
         "baudrate (serialtools.bus.buscreator attribute)": [
             [8, "serialtools.bus.BusCreator.baudrate"]
         ],
+        "bus_creator (in module serialtools.bus)": [
+            [8, "serialtools.bus.bus_creator"]
+        ],
         "bytesize (serialtools.bus.buscreator attribute)": [
             [8, "serialtools.bus.BusCreator.bytesize"]
         ],
         "cancel_read() (serialtools.bus.readfromfilebus method)": [
             [8, "serialtools.bus.ReadFromFileBus.cancel_read"]
         ],
         "cancel_read() (serialtools.bus.writetofilebus method)": [
@@ -709,14 +739,17 @@
         ],
         "virtual (serialtools.bus.buscreator attribute)": [
             [8, "serialtools.bus.BusCreator.virtual"]
         ],
         "vport (serialtools.bus.buscreator attribute)": [
             [8, "serialtools.bus.BusCreator.vport"]
         ],
+        "vport_other (serialtools.bus.buscreator attribute)": [
+            [8, "serialtools.bus.BusCreator.vport_other"]
+        ],
         "write() (serialtools.bus.readfromfilebus method)": [
             [8, "serialtools.bus.ReadFromFileBus.write"]
         ],
         "write() (serialtools.bus.writetofilebus method)": [
             [8, "serialtools.bus.WriteToFileBus.write"]
         ],
         "xonxoff (serialtools.bus.buscreator attribute)": [
@@ -811,14 +844,17 @@
         ],
         "get_start_bit() (serialtools.database.database method)": [
             [9, "serialtools.database.Database.get_start_bit"]
         ],
         "ignore_bytes_between_messages (serialtools.database.reader attribute)": [
             [9, "serialtools.database.Reader.ignore_bytes_between_messages"]
         ],
+        "init() (serialtools.database.signal method)": [
+            [9, "serialtools.database.Signal.init"]
+        ],
         "message_spec (serialtools.database.database attribute)": [
             [9, "serialtools.database.Database.message_spec"]
         ],
         "read() (serialtools.database.reader method)": [
             [9, "serialtools.database.Reader.read"]
         ],
         "read_byte() (serialtools.database.reader method)": [
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.apps.decode.html` & `serialtools-0.4.0/docs/build/html/serialtools.apps.decode.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.decode module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.apps.decode module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.apps.dump.html` & `serialtools-0.4.0/docs/build/html/serialtools.apps.dump.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.dump module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.apps.dump module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.apps.html` & `serialtools-0.4.0/docs/build/html/serialtools.apps.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps package &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.apps package &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.apps.rawsplit.html` & `serialtools-0.4.0/docs/build/html/serialtools.apps.rawsplit.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.apps.rawsplit module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
           o add_arguments()
           o add_parser()
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.apps.send.html` & `serialtools-0.4.0/docs/build/html/serialtools.apps.send.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.apps.send module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.apps.send module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
                       # Submodules
                       # Module_contents
           o Submodules
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.bus.html` & `serialtools-0.4.0/docs/build/html/serialtools.bus.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.bus module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.bus module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -53,14 +53,15 @@
 <li class="toctree-l2"><a class="reference internal" href="serialtools.html#subpackages">Subpackages</a></li>
 <li class="toctree-l2 current"><a class="reference internal" href="serialtools.html#submodules">Submodules</a><ul class="current">
 <li class="toctree-l3 current"><a class="current reference internal" href="#">serialtools.bus module</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.ReadFromFileBus"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.ReadFromParameterBus"><code class="docutils literal notranslate"><span class="pre">ReadFromParameterBus</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.WriteToFileBus"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus</span></code></a></li>
+<li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.bus_creator"><code class="docutils literal notranslate"><span class="pre">bus_creator</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="#serialtools.bus.get_timestamp"><code class="docutils literal notranslate"><span class="pre">get_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 </li>
@@ -70,25 +71,27 @@
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.decode.html">serialtools.apps.decode module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.dump.html">serialtools.apps.dump module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.rawsplit.html">serialtools.apps.rawsplit module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.apps.send.html">serialtools.apps.send module</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.add_arguments"><code class="docutils literal notranslate"><span class="pre">BusCreator.add_arguments()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.auto_create_virtual_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.auto_create_virtual_bus</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.baudrate"><code class="docutils literal notranslate"><span class="pre">BusCreator.baudrate</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.bytesize"><code class="docutils literal notranslate"><span class="pre">BusCreator.bytesize</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.create_args"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_args()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.create_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_bus()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.dsrdtr"><code class="docutils literal notranslate"><span class="pre">BusCreator.dsrdtr</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.parity"><code class="docutils literal notranslate"><span class="pre">BusCreator.parity</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.port"><code class="docutils literal notranslate"><span class="pre">BusCreator.port</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.rtscts"><code class="docutils literal notranslate"><span class="pre">BusCreator.rtscts</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.stopbits"><code class="docutils literal notranslate"><span class="pre">BusCreator.stopbits</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.virtual"><code class="docutils literal notranslate"><span class="pre">BusCreator.virtual</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.vport"><code class="docutils literal notranslate"><span class="pre">BusCreator.vport</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.vport_other"><code class="docutils literal notranslate"><span class="pre">BusCreator.vport_other</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.BusCreator.xonxoff"><code class="docutils literal notranslate"><span class="pre">BusCreator.xonxoff</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.ReadFromFileBus"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.ReadFromFileBus.cancel_read"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.cancel_read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.ReadFromFileBus.cancel_write"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.cancel_write()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.ReadFromFileBus.close"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.close()</span></code></a></li>
@@ -103,14 +106,15 @@
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.WriteToFileBus.cancel_write"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.cancel_write()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.WriteToFileBus.close"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.close()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.WriteToFileBus.read"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.WriteToFileBus.timestamp"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.timestamp</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.bus.WriteToFileBus.write"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.write()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.bus_creator"><code class="docutils literal notranslate"><span class="pre">bus_creator</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.bus.get_timestamp"><code class="docutils literal notranslate"><span class="pre">get_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database_config.html">serialtools.database_config module</a></li>
 </ul>
 
@@ -147,14 +151,22 @@
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.add_arguments">
 <span class="sig-name descname"><span class="pre">add_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">parser</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser" title="(in Python v3.11)"><span class="pre">ArgumentParser</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rx_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.bus.BusCreator.add_arguments" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="serialtools.bus.BusCreator.auto_create_virtual_bus">
+<span class="sig-name descname"><span class="pre">auto_create_virtual_bus</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.auto_create_virtual_bus" title="Permalink to this definition"></a></dt>
+<dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
+<p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
+If you want to get this object you need to access it as a class attribute.</p>
+</dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.baudrate">
 <span class="sig-name descname"><span class="pre">baudrate</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.baudrate" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
@@ -229,26 +241,34 @@
 <span class="sig-name descname"><span class="pre">vport</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.vport" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
 <dl class="py attribute">
+<dt class="sig sig-object py" id="serialtools.bus.BusCreator.vport_other">
+<span class="sig-name descname"><span class="pre">vport_other</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.vport_other" title="Permalink to this definition"></a></dt>
+<dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
+<p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
+If you want to get this object you need to access it as a class attribute.</p>
+</dd></dl>
+
+<dl class="py attribute">
 <dt class="sig sig-object py" id="serialtools.bus.BusCreator.xonxoff">
 <span class="sig-name descname"><span class="pre">xonxoff</span></span><a class="headerlink" href="#serialtools.bus.BusCreator.xonxoff" title="Permalink to this definition"></a></dt>
 <dd><p>Each instance of this class represents a setting which can be changed in a config file.</p>
 <p>This class implements the <a class="reference external" href="https://docs.python.org/3/reference/datamodel.html#implementing-descriptors">descriptor protocol</a> to return <code class="xref py py-attr docutils literal notranslate"><span class="pre">value</span></code> if an instance of this class is accessed as an instance attribute.
 If you want to get this object you need to access it as a class attribute.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.bus.ReadFromFileBus">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.bus.</span></span><span class="sig-name descname"><span class="pre">ReadFromFileBus</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.bus.ReadFromFileBus" title="Permalink to this definition"></a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.bus.</span></span><span class="sig-name descname"><span class="pre">ReadFromFileBus</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.TextIO" title="(in Python v3.11)"><span class="pre">TextIO</span></a></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.bus.ReadFromFileBus" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="serialtools.bus.ReadFromFileBus.params.fn"></span><strong>fn</strong><a class="paramlink headerlink reference internal" href="#serialtools.bus.ReadFromFileBus.params.fn">¶</a> – file name of file containing data to be read. Data is in the output format of <cite>serialtools dump</cite>, hex values separated by spaces and optionally lines starting with a time stamps in parentheses.</p>
 </dd>
 </dl>
 <dl class="py method">
@@ -326,14 +346,20 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.bus.WriteToFileBus.write">
 <span class="sig-name descname"><span class="pre">write</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">data</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#bytes" title="(in Python v3.11)"><span class="pre">bytes</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.bus.WriteToFileBus.write" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
+<dl class="py data">
+<dt class="sig sig-object py" id="serialtools.bus.bus_creator">
+<span class="sig-prename descclassname"><span class="pre">serialtools.bus.</span></span><span class="sig-name descname"><span class="pre">bus_creator</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">&lt;serialtools.bus.BusCreator</span> <span class="pre">object&gt;</span></em><a class="headerlink" href="#serialtools.bus.bus_creator" title="Permalink to this definition"></a></dt>
+<dd><p>Use this to create a new bus</p>
+</dd></dl>
+
 <dl class="py function">
 <dt class="sig sig-object py" id="serialtools.bus.get_timestamp">
 <span class="sig-prename descclassname"><span class="pre">serialtools.bus.</span></span><span class="sig-name descname"><span class="pre">get_timestamp</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">bus</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Serial</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.ReadFromFileBus" title="serialtools.bus.ReadFromFileBus"><span class="pre">ReadFromFileBus</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#serialtools.bus.WriteToFileBus" title="serialtools.bus.WriteToFileBus"><span class="pre">WriteToFileBus</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/datetime.html#datetime.datetime" title="(in Python v3.11)"><span class="pre">datetime</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.bus.get_timestamp" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </section>
```

#### html2text {}

```diff
@@ -5,46 +5,49 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                       # BusCreator
                       # ReadFromFileBus
                       # ReadFromParameterBus
                       # WriteToFileBus
+                      # bus_creator
                       # get_timestamp()
                 # serialtools.database_module
                 # serialtools.database_config_module
           o Module_contents
     * serialtools.apps.decode_module
     * serialtools.apps.dump_module
     * serialtools.apps.rawsplit_module
     * serialtools.apps.send_module
     * serialtools.bus_module
           o BusCreator
                 # BusCreator.add_arguments()
+                # BusCreator.auto_create_virtual_bus
                 # BusCreator.baudrate
                 # BusCreator.bytesize
                 # BusCreator.create_args()
                 # BusCreator.create_bus()
                 # BusCreator.dsrdtr
                 # BusCreator.parity
                 # BusCreator.port
                 # BusCreator.rtscts
                 # BusCreator.stopbits
                 # BusCreator.virtual
                 # BusCreator.vport
+                # BusCreator.vport_other
                 # BusCreator.xonxoff
           o ReadFromFileBus
                 # ReadFromFileBus.cancel_read()
                 # ReadFromFileBus.cancel_write()
                 # ReadFromFileBus.close()
                 # ReadFromFileBus.read()
                 # ReadFromFileBus.timestamp
@@ -53,27 +56,34 @@
           o WriteToFileBus
                 # WriteToFileBus.cancel_read()
                 # WriteToFileBus.cancel_write()
                 # WriteToFileBus.close()
                 # WriteToFileBus.read()
                 # WriteToFileBus.timestamp
                 # WriteToFileBus.write()
+          o bus_creator
           o get_timestamp()
     * serialtools.database_module
     * serialtools.database_config_module
    serialtools
     * serialtools_package
     * serialtools.bus module
     * View_page_source
 ===============================================================================
 ****** serialtools.bus moduleï ******
   classserialtools.bus.BusCreatorï
       Bases: object
         add_arguments(parser: ArgumentParser, *, rx_only: bool = False)
         &#x2192; Noneï
+        auto_create_virtual_busï
+            Each instance of this class represents a setting which can be
+            changed in a config file.
+            This class implements the descriptor_protocol to return value if an
+            instance of this class is accessed as an instance attribute. If you
+            want to get this object you need to access it as a class attribute.
         baudrateï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
         bytesizeï
@@ -124,21 +134,27 @@
             want to get this object you need to access it as a class attribute.
         vportï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
+        vport_otherï
+            Each instance of this class represents a setting which can be
+            changed in a config file.
+            This class implements the descriptor_protocol to return value if an
+            instance of this class is accessed as an instance attribute. If you
+            want to get this object you need to access it as a class attribute.
         xonxoffï
             Each instance of this class represents a setting which can be
             changed in a config file.
             This class implements the descriptor_protocol to return value if an
             instance of this class is accessed as an instance attribute. If you
             want to get this object you need to access it as a class attribute.
-  classserialtools.bus.ReadFromFileBus(fn: str)ï
+  classserialtools.bus.ReadFromFileBus(fn: str | TextIO)ï
       Bases: object
         Parameters:
             fnÂ¶ â file name of file containing data to be read. Data is in
             the output format ofserialtools dump, hex values separated by
             spaces and optionally lines starting with a time stamps in
             parentheses.
         cancel_read() &#x2192; Noneï
@@ -159,13 +175,15 @@
       Bases: object
         cancel_read() &#x2192; Noneï
         cancel_write() &#x2192; Noneï
         close() &#x2192; Noneï
         read(n: int) &#x2192; bytesï
         timestamp: datetime | None= Noneï
         write(data: bytes) &#x2192; Noneï
+  serialtools.bus.bus_creator= <serialtools.bus.BusCreator object>ï
+      Use this to create a new bus
   serialtools.bus.get_timestamp(bus: Serial | ReadFromFileBus | WriteToFileBus)
   &#x2192; datetime | Noneï
 Previous Next
 ===============================================================================
 © Copyright 2023, erzo.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.database.html` & `serialtools-0.4.0/docs/build/html/serialtools.database.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.database module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -119,14 +119,15 @@
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Signal.init"><code class="docutils literal notranslate"><span class="pre">Signal.init()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Type.BOOL"><code class="docutils literal notranslate"><span class="pre">Type.BOOL</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Type.FLOAT"><code class="docutils literal notranslate"><span class="pre">Type.FLOAT</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Type.INT"><code class="docutils literal notranslate"><span class="pre">Type.INT</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="#serialtools.database.Type.TEXT"><code class="docutils literal notranslate"><span class="pre">Type.TEXT</span></code></a></li>
@@ -343,15 +344,15 @@
 <span class="sig-name descname"><span class="pre">stop</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Reader.stop" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Signal">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Signal</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Type" title="serialtools.database.Type"><span class="pre">Type</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">bits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">startbit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">scale</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">unit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Signal" title="Permalink to this definition"></a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Signal</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Type" title="serialtools.database.Type"><span class="pre">Type</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">address</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">bits</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">startbit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">lsb</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><span class="pre">int</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">scale</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#float" title="(in Python v3.11)"><span class="pre">float</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">unit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">''</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Signal" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/functions.html#object" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></a></p>
 <dl class="field-list simple">
 <dt class="field-odd">Paramref name<span class="colon">:</span></dt>
 <dd class="field-odd"><p>The name of the signal</p>
 </dd>
 <dt class="field-even">Paramref type<span class="colon">:</span></dt>
 <dd class="field-even"><p>The data type, e.g. INT, UINT, FLOAT</p>
@@ -359,34 +360,42 @@
 <dt class="field-odd">Paramref address<span class="colon">:</span></dt>
 <dd class="field-odd"><p>The address which is used to request this value from the battery</p>
 </dd>
 <dt class="field-even">Paramref bits<span class="colon">:</span></dt>
 <dd class="field-even"><p>The size of this signal in bits, defaults to <a class="reference internal" href="#serialtools.database.Database.word_length_in_bits" title="serialtools.database.Database.word_length_in_bits"><code class="xref py py-attr docutils literal notranslate"><span class="pre">Database.word_length_in_bits</span></code></a></p>
 </dd>
 <dt class="field-odd">Paramref startbit<span class="colon">:</span></dt>
-<dd class="field-odd"><p>If the word identified by <a class="reference internal" href="#serialtools.database.Signal.params.address" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">address</span></code></a> contains several smaller values the startbit specifies where the signal starts inside of the word</p>
+<dd class="field-odd"><p>If the word identified by <a class="reference internal" href="#serialtools.database.Signal.params.address" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">address</span></code></a> contains several smaller values the startbit specifies the first transmitted bit in the word belonging to the signal. Bit 0 is the first bit transmitted, not the least significant bit.</p>
 </dd>
-<dt class="field-even">Paramref scale<span class="colon">:</span></dt>
-<dd class="field-even"><p>A factor which is multiplied to the raw value received on the bus in order to get a value of <a class="reference internal" href="#serialtools.database.Signal.params.unit" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">unit</span></code></a></p>
+<dt class="field-even">Paramref lsb<span class="colon">:</span></dt>
+<dd class="field-even"><p>If the word identified by <a class="reference internal" href="#serialtools.database.Signal.params.address" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">address</span></code></a> contains several smaller values the lsb specifies where the list significant bit of the signal is inside of the word. <a class="reference internal" href="#serialtools.database.Signal.params.startbit" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">startbit</span></code></a> and <a class="reference internal" href="#serialtools.database.Signal.params.lsb" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">lsb</span></code></a> are mutually exclusive, only one of them may be passed.</p>
 </dd>
-<dt class="field-odd">Paramref offset<span class="colon">:</span></dt>
-<dd class="field-odd"><p>A summand which is added to the raw value received on the bus in order to get a value of <a class="reference internal" href="#serialtools.database.Signal.params.unit" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">unit</span></code></a></p>
+<dt class="field-odd">Paramref scale<span class="colon">:</span></dt>
+<dd class="field-odd"><p>A factor which is multiplied to the raw value received on the bus in order to get a value of <a class="reference internal" href="#serialtools.database.Signal.params.unit" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">unit</span></code></a></p>
 </dd>
-<dt class="field-even">Paramref unit<span class="colon">:</span></dt>
-<dd class="field-even"><p>The unit of the value</p>
+<dt class="field-even">Paramref offset<span class="colon">:</span></dt>
+<dd class="field-even"><p>A summand which is added to the raw value received on the bus in order to get a value of <a class="reference internal" href="#serialtools.database.Signal.params.unit" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">unit</span></code></a></p>
+</dd>
+<dt class="field-odd">Paramref unit<span class="colon">:</span></dt>
+<dd class="field-odd"><p>The unit of the value</p>
 </dd>
 </dl>
 <p>When decoding data from bytes received on the bus to human readable floats in the given unit
 the raw value is first multiplied with <a class="reference internal" href="#serialtools.database.Signal.params.scale" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">scale</span></code></a> and then <a class="reference internal" href="#serialtools.database.Signal.params.offset" title="serialtools.database.Signal"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">offset</span></code></a> is added to it
 as in <a class="reference external" href="https://github.com/cantools/cantools/blob/1ca17757c89ae1c1a97076e684e6aaa808b2d221/cantools/database/conversion.py#L197">cantools</a>.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="serialtools.database.Signal.get_bitstruct_fmt">
 <span class="sig-name descname"><span class="pre">get_bitstruct_fmt</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#serialtools.database.Signal.get_bitstruct_fmt" title="Permalink to this definition"></a></dt>
 <dd></dd></dl>
 
+<dl class="py method">
+<dt class="sig sig-object py" id="serialtools.database.Signal.init">
+<span class="sig-name descname"><span class="pre">init</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#serialtools.database.Database" title="serialtools.database.Database"><span class="pre">Database</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span></span><a class="headerlink" href="#serialtools.database.Signal.init" title="Permalink to this definition"></a></dt>
+<dd></dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="serialtools.database.Type">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">serialtools.database.</span></span><span class="sig-name descname"><span class="pre">Type</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">names</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">module</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">qualname</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">boundary</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#serialtools.database.Type" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <a class="reference external" href="https://docs.python.org/3/library/enum.html#enum.Enum" title="(in Python v3.11)"><code class="xref py py-class docutils literal notranslate"><span class="pre">Enum</span></code></a></p>
 <dl class="py attribute">
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                       # ByteSpec
@@ -63,14 +63,15 @@
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
                 # Reader.send_msg()
                 # Reader.stop()
           o Signal
                 # Signal.get_bitstruct_fmt()
+                # Signal.init()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
                 # Type.TEXT
                 # Type.UINT
           o format_bytes()
@@ -140,41 +141,49 @@
         read_in_other_thread(callback: Callable[[Message], None]) &#x2192;
         Noneï
         read_msg() &#x2192; Message | Noneï
         read_n_bytes(n: int) &#x2192; bytesï
         send_msg(msg: Message) &#x2192; Noneï
         stop() &#x2192; Noneï
   classserialtools.database.Signal(name: str, type: Type, address: int, *,
-  bits: int | None = None, startbit: int = 0, scale: float = 1, offset: float =
-  0, unit: str = '')ï
+  bits: int | None = None, startbit: int | None = None, lsb: int | None = None,
+  scale: float = 1, offset: float = 0, unit: str = '')ï
       Bases: object
         Paramref name:
             The name of the signal
         Paramref type:
             The data type, e.g. INT, UINT, FLOAT
         Paramref address:
             The address which is used to request this value from the battery
         Paramref bits:
             The size of this signal in bits, defaults to
             Database.word_length_in_bits
         Paramref startbit:
             If the word identified by address contains several smaller values
-            the startbit specifies where the signal starts inside of the word
+            the startbit specifies the first transmitted bit in the word
+            belonging to the signal. Bit 0 is the first bit transmitted, not
+            the least significant bit.
+        Paramref lsb:
+            If the word identified by address contains several smaller values
+            the lsb specifies where the list significant bit of the signal is
+            inside of the word. startbit and lsb are mutually exclusive, only
+            one of them may be passed.
         Paramref scale:
             A factor which is multiplied to the raw value received on the bus
             in order to get a value of unit
         Paramref offset:
             A summand which is added to the raw value received on the bus in
             order to get a value of unit
         Paramref unit:
             The unit of the value
       When decoding data from bytes received on the bus to human readable
       floats in the given unit the raw value is first multiplied with scale and
       then offset is added to it as in cantools.
         get_bitstruct_fmt() &#x2192; strï
+        init(db: Database) &#x2192; Noneï
   classserialtools.database.Type(value, names=None, *, module=None,
   qualname=None, type=None, start=1, boundary=None)ï
       Bases: Enum
         BOOL= 'b'ï
         FLOAT= 'f'ï
         INT= 's'ï
         TEXT= 't'ï
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.database_config.html` & `serialtools-0.4.0/docs/build/html/serialtools.database_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools.database_config module &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools.database_config module &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
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
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
                 # serialtools.database_config_module
```

### Comparing `serialtools-0.3.0/docs/build/html/serialtools.html` & `serialtools-0.4.0/docs/build/html/serialtools.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>serialtools package &mdash; serialtools v0.3.0 documentation</title>
+  <title>serialtools package &mdash; serialtools v0.4.0 documentation</title>
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
-                v0.3.0
+                v0.4.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -138,25 +138,27 @@
 <section id="submodules">
 <h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this heading"></a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.bus.html">serialtools.bus module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator"><code class="docutils literal notranslate"><span class="pre">BusCreator</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.add_arguments"><code class="docutils literal notranslate"><span class="pre">BusCreator.add_arguments()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.auto_create_virtual_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.auto_create_virtual_bus</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.baudrate"><code class="docutils literal notranslate"><span class="pre">BusCreator.baudrate</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.bytesize"><code class="docutils literal notranslate"><span class="pre">BusCreator.bytesize</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.create_args"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_args()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.create_bus"><code class="docutils literal notranslate"><span class="pre">BusCreator.create_bus()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.dsrdtr"><code class="docutils literal notranslate"><span class="pre">BusCreator.dsrdtr</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.parity"><code class="docutils literal notranslate"><span class="pre">BusCreator.parity</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.port"><code class="docutils literal notranslate"><span class="pre">BusCreator.port</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.rtscts"><code class="docutils literal notranslate"><span class="pre">BusCreator.rtscts</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.stopbits"><code class="docutils literal notranslate"><span class="pre">BusCreator.stopbits</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.virtual"><code class="docutils literal notranslate"><span class="pre">BusCreator.virtual</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.vport"><code class="docutils literal notranslate"><span class="pre">BusCreator.vport</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.vport_other"><code class="docutils literal notranslate"><span class="pre">BusCreator.vport_other</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.BusCreator.xonxoff"><code class="docutils literal notranslate"><span class="pre">BusCreator.xonxoff</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus.cancel_read"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.cancel_read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus.cancel_write"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.cancel_write()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.ReadFromFileBus.close"><code class="docutils literal notranslate"><span class="pre">ReadFromFileBus.close()</span></code></a></li>
@@ -171,14 +173,15 @@
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus.cancel_write"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.cancel_write()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus.close"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.close()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus.read"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.read()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus.timestamp"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.timestamp</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.WriteToFileBus.write"><code class="docutils literal notranslate"><span class="pre">WriteToFileBus.write()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.bus_creator"><code class="docutils literal notranslate"><span class="pre">bus_creator</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.bus.html#serialtools.bus.get_timestamp"><code class="docutils literal notranslate"><span class="pre">get_timestamp()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="serialtools.database.html">serialtools.database module</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec"><code class="docutils literal notranslate"><span class="pre">ByteSpec</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec.format_allowed_values"><code class="docutils literal notranslate"><span class="pre">ByteSpec.format_allowed_values()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.ByteSpec.get_length"><code class="docutils literal notranslate"><span class="pre">ByteSpec.get_length()</span></code></a></li>
@@ -221,14 +224,15 @@
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.read_n_bytes"><code class="docutils literal notranslate"><span class="pre">Reader.read_n_bytes()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.send_msg"><code class="docutils literal notranslate"><span class="pre">Reader.send_msg()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Reader.stop"><code class="docutils literal notranslate"><span class="pre">Reader.stop()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal"><code class="docutils literal notranslate"><span class="pre">Signal</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal.get_bitstruct_fmt"><code class="docutils literal notranslate"><span class="pre">Signal.get_bitstruct_fmt()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Signal.init"><code class="docutils literal notranslate"><span class="pre">Signal.init()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type"><code class="docutils literal notranslate"><span class="pre">Type</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type.BOOL"><code class="docutils literal notranslate"><span class="pre">Type.BOOL</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type.FLOAT"><code class="docutils literal notranslate"><span class="pre">Type.FLOAT</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type.INT"><code class="docutils literal notranslate"><span class="pre">Type.INT</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="serialtools.database.html#serialtools.database.Type.TEXT"><code class="docutils literal notranslate"><span class="pre">Type.TEXT</span></code></a></li>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 
 
 serialtools
-v0.3.0
+v0.4.0
 [q                   ]
     * serialtools_package
           o Subpackages
                 # serialtools.apps_package
           o Submodules
                 # serialtools.bus_module
                 # serialtools.database_module
@@ -51,25 +51,27 @@
           o Module_contents
                 # add_arguments()
 
 ***** Submodulesï *****
     * serialtools.bus_module
           o BusCreator
                 # BusCreator.add_arguments()
+                # BusCreator.auto_create_virtual_bus
                 # BusCreator.baudrate
                 # BusCreator.bytesize
                 # BusCreator.create_args()
                 # BusCreator.create_bus()
                 # BusCreator.dsrdtr
                 # BusCreator.parity
                 # BusCreator.port
                 # BusCreator.rtscts
                 # BusCreator.stopbits
                 # BusCreator.virtual
                 # BusCreator.vport
+                # BusCreator.vport_other
                 # BusCreator.xonxoff
           o ReadFromFileBus
                 # ReadFromFileBus.cancel_read()
                 # ReadFromFileBus.cancel_write()
                 # ReadFromFileBus.close()
                 # ReadFromFileBus.read()
                 # ReadFromFileBus.timestamp
@@ -78,14 +80,15 @@
           o WriteToFileBus
                 # WriteToFileBus.cancel_read()
                 # WriteToFileBus.cancel_write()
                 # WriteToFileBus.close()
                 # WriteToFileBus.read()
                 # WriteToFileBus.timestamp
                 # WriteToFileBus.write()
+          o bus_creator
           o get_timestamp()
     * serialtools.database_module
           o ByteSpec
                 # ByteSpec.format_allowed_values()
                 # ByteSpec.get_length()
           o Database
                 # Database.decode()
@@ -114,14 +117,15 @@
                 # Reader.read_in_other_thread()
                 # Reader.read_msg()
                 # Reader.read_n_bytes()
                 # Reader.send_msg()
                 # Reader.stop()
           o Signal
                 # Signal.get_bitstruct_fmt()
+                # Signal.init()
           o Type
                 # Type.BOOL
                 # Type.FLOAT
                 # Type.INT
                 # Type.TEXT
                 # Type.UINT
           o format_bytes()
```

### Comparing `serialtools-0.3.0/docs/make.bat` & `serialtools-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/docs/source/conf.py` & `serialtools-0.4.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'serialtools'
 copyright = '2023, erzo'
 author = 'erzo'
-release = 'v0.3.0'
+release = 'v0.4.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx_paramlinks']
 
 templates_path = ['_templates']
```

### Comparing `serialtools-0.3.0/docs/source/index.rst` & `serialtools-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/prepare_for_gitlab_pages.py` & `serialtools-0.4.0/prepare_for_gitlab_pages.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/pyproject.toml` & `serialtools-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/release.sh` & `serialtools-0.4.0/release.sh`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/__main__.py` & `serialtools-0.4.0/src/serialtools/__main__.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/apps/decode.py` & `serialtools-0.4.0/src/serialtools/apps/decode.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/apps/dump.py` & `serialtools-0.4.0/src/serialtools/apps/dump.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/apps/rawsplit.py` & `serialtools-0.4.0/src/serialtools/apps/rawsplit.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/apps/send.py` & `serialtools-0.4.0/src/serialtools/apps/send.py`

 * *Files identical despite different names*

### Comparing `serialtools-0.3.0/src/serialtools/bus.py` & `serialtools-0.4.0/src/serialtools/bus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
 import os
+import sys
 import time
 import datetime
 import logging
 import typing
 import argparse
 
 import serial
@@ -17,19 +18,21 @@
 
 TIMESTAMP_FORMAT = '%Y-%m-%d %H:%M:%S.%f'
 
 class ReadFromFileBus:
 
 	timestamp: 'datetime.datetime|None' = None
 
-	def __init__(self, fn: str) -> None:
+	def __init__(self, fn: 'str|typing.TextIO') -> None:
 		'''
 		:param fn: file name of file containing data to be read. Data is in the output format of `serialtools dump`, hex values separated by spaces and optionally lines starting with a time stamps in parentheses.
 		'''
-		self.f = open(fn, 'rt')
+		if isinstance(fn, str):
+			fn = open(fn, 'rt')
+		self.f = fn
 
 	def read(self, n: int) -> bytes:
 		out = []
 		for i in range(n):
 			h = ''
 			while True:
 				try:
@@ -52,15 +55,18 @@
 						elif c == ')':
 							self.timestamp = datetime.datetime.strptime(timestamp, TIMESTAMP_FORMAT)
 							break
 						elif c == '(':
 							raise ValueError("syntax error in {self.f.name!r}: {c!r} in timestamp")
 						timestamp += c
 					continue
-
+				if not h and c == '#':
+					while self.f.read(1) != '\n':
+						pass
+					continue
 				h += c
 				if len(h) >= 2:
 					break
 
 			b = int(h, base=16)
 			out.append(b)
 		return bytes(out)
@@ -142,14 +148,16 @@
 # ------- create bus -------
 
 class BusCreator:
 
 	# https://pythonhosted.org/pyserial/pyserial_api.html
 	port = Config('bus.port', '/dev/ttyUSB0')
 	vport = Config('bus.virtual-port', '/tmp/vserial1')
+	vport_other = Config('bus.virtual-port-other', '/tmp/vserial2')
+	auto_create_virtual_bus = Config('bus.auto-create', True, help="If the default virtual port does not exist create it with socat")
 	virtual = Config('bus.virtual', False)
 	baudrate = Config('bus.baudrate', 9600, unit='')
 	bytesize = Config('bus.bytesize', serial.EIGHTBITS, allowed_values={
 		'5': serial.FIVEBITS,
 		'6': serial.SIXBITS,
 		'7': serial.SEVENBITS,
 		'8': serial.EIGHTBITS,
@@ -175,15 +183,18 @@
 		parser.add_argument('-v', '--virtual', action='store_true', default=None)
 		parser.add_argument('-V', '--no-virtual', action='store_false', dest='virtual', default=None)
 		g: 'argparse.ArgumentParser|argparse._MutuallyExclusiveGroup'
 		if rx_only:
 			g = parser.add_mutually_exclusive_group()
 		else:
 			g = parser
-		g.add_argument('-p', '-c', '--port', '--channel')
+		help_port = "the serial port device"
+		if rx_only:
+			help_port += ", a log file or '-' to read from stdin"
+		g.add_argument('-p', '-c', '--port', '--channel', help=help_port)
 		if rx_only:
 			g.add_argument('-m', '--message')
 		parser.add_argument('-b', '--baudrate', type=int)
 		parser.set_defaults(rx_only=rx_only)
 
 	def create_args(self, *, port: 'str|None' = None, baudrate: 'int|None' = None, virtual: 'bool|None' = None) -> argparse.Namespace:
 		parser = argparse.ArgumentParser()
@@ -199,22 +210,34 @@
 			args.append('--virtual')
 		return parser.parse_args(args)
 
 	def create_bus(self, args: 'argparse.Namespace') -> Bus:
 		if args.rx_only:
 			if args.message:
 				return ReadFromParameterBus(args.message)
+			if args.port == '-':
+				return ReadFromFileBus(sys.stdin)
 			if args.port and os.path.isfile(args.port):
 				return ReadFromFileBus(args.port)
 
 		if args.virtual is None:
 			args.virtual = self.virtual
 		if args.virtual:
 			if not args.port:
 				args.port = self.vport
+				if not os.path.exists(args.port):
+					if self.auto_create_virtual_bus:
+						import subprocess, shlex
+						cmd = ['socat', '-d', '-d', 'pty,link=%s,raw,echo=0' % args.port, 'pty,link=%s,raw,echo=0' % self.vport_other]
+						print("creating new virtual bus with %r" % shlex.join(cmd))
+						print("please connect the other side to %r" % self.vport_other)
+						subprocess.Popen(cmd)
+						time.sleep(1)
+					else:
+						raise FileNotFoundError(f"serial bus {args.port!r} does not exist, you can create it with `$ socat -d -d pty,link={args.port},raw,echo=0 pty,link={self.vport_other},raw,echo=0`. Then rerun this program with --port={args.port}.")
 			return serial.Serial(port=args.port)
 
 		if not args.port:
 			args.port = self.port
 		if not args.baudrate:
 			args.baudrate = self.baudrate
 		logger.info(f"initializing serial bus {args.port} with baudrate={args.baudrate}")
@@ -228,8 +251,9 @@
 			xonxoff = self.xonxoff,
 			rtscts = self.rtscts,
 			write_timeout = None,
 			dsrdtr = self.dsrdtr,
 			inter_byte_timeout = None,
 		)
 
+#: Use this to create a new bus
 bus_creator = BusCreator()
```

### Comparing `serialtools-0.3.0/src/serialtools/database.py` & `serialtools-0.4.0/src/serialtools/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,36 +247,37 @@
 	#: The byte order
 	endianness: Endianness
 
 	#: The default length of a signal
 	word_length_in_bits: int
 
 	def __init__(self, message_spec: 'MessageSpec', signals: 'Sequence[Signal]', *, endianness: Endianness, word_length_in_bits: int = 8):
-		signals = list(signals)
-		signals.sort(key=lambda s: s.address*word_length_in_bits + s.startbit)
-
 		self.message_spec = message_spec
 		self.endianness = endianness
 		self.word_length_in_bits = word_length_in_bits
+
+		signals = list(signals)
+		for s in signals:
+			s.init(self)
+
+		signals.sort(key=lambda s: s.address*word_length_in_bits + s.startbit)
+
 		self.signals = signals
 
 		for i in range(len(self.message_spec)):
 			length = self.message_spec[i].length
 			if isinstance(length, str):
 				if length not in [_s.name for _s in self.message_spec[:i]]:
 					spec = self.message_spec[i]
 					raise ValueError("{spec.name!r} has invalid length {spec.length!}, there is no previous byte spec with that name")
 
 		last_i1 = 0
 		last_signal = None
 		used_names: 'set[str]' = set()
 		for s in signals:
-			if not hasattr(s, 'bits'):
-				s.bits = self.word_length_in_bits
-
 			if s.name in used_names:
 				raise ValueError(f"there are two signals with the same name {s.name!r}")
 
 			i0 = self.get_start_bit(s)
 			i1 = i0 + s.bits
 			if i0 < last_i1:
 				assert last_signal is not None
@@ -404,41 +405,61 @@
 				return s
 
 		raise ValueError(f"no signal with name {name!r}")
 
 
 class Signal:
 
-	def __init__(self, name: str, type: Type, address: int, *, bits: 'int|None' = None, startbit: int = 0, scale: float = 1, offset: float = 0, unit: str = ''):
+	def __init__(self, name: str, type: Type, address: int, *, bits: 'int|None' = None, startbit: 'int|None' = None, lsb: 'int|None' = None, scale: float = 1, offset: float = 0, unit: str = ''):
 		'''
 		:paramref name: The name of the signal
 		:paramref type: The data type, e.g. INT, UINT, FLOAT
 		:paramref address: The address which is used to request this value from the battery
 		:paramref bits: The size of this signal in bits, defaults to :attr:`Database.word_length_in_bits <serialtools.database.Database.word_length_in_bits>`
-		:paramref startbit: If the word identified by :paramref:`~serialtools.database.Signal.address` contains several smaller values the startbit specifies where the signal starts inside of the word
+		:paramref startbit: If the word identified by :paramref:`~serialtools.database.Signal.address` contains several smaller values the startbit specifies the first transmitted bit in the word belonging to the signal. Bit 0 is the first bit transmitted, not the least significant bit.
+		:paramref lsb: If the word identified by :paramref:`~serialtools.database.Signal.address` contains several smaller values the lsb specifies where the list significant bit of the signal is inside of the word. :paramref:`~serialtools.database.Signal.startbit` and :paramref:`~serialtools.database.Signal.lsb` are mutually exclusive, only one of them may be passed.
 		:paramref scale: A factor which is multiplied to the raw value received on the bus in order to get a value of :paramref:`~serialtools.database.Signal.unit`
 		:paramref offset: A summand which is added to the raw value received on the bus in order to get a value of :paramref:`~serialtools.database.Signal.unit`
 		:paramref unit: The unit of the value
 
 		When decoding data from bytes received on the bus to human readable floats in the given unit
 		the raw value is first multiplied with :paramref:`~serialtools.database.Signal.scale` and then :paramref:`~serialtools.database.Signal.offset` is added to it
 		as in `cantools <https://github.com/cantools/cantools/blob/1ca17757c89ae1c1a97076e684e6aaa808b2d221/cantools/database/conversion.py#L197>`_.
 		'''
+		if startbit is None and lsb is None:
+			startbit = 0
+		elif startbit is not None and lsb is not None:
+			raise TypeError('got values for startbit and lsb but only one of them may be given')
+		elif startbit is None:
+			assert isinstance(lsb, int)
+			self._lsb = lsb
 		self.name = name
 		self.type = type
 		self.address = address
-		self.startbit = startbit
+		if startbit is not None:
+			self.startbit = startbit
 		self.scale = scale
 		self.offset = offset
 		self.unit = unit
 
 		if bits is not None:
 			self.bits = bits
 		elif type is Type.BOOL:
 			self.bits = 1
 
+	def init(self, db: Database) -> None:
+		if not hasattr(self, 'bits'):
+			self.bits = db.word_length_in_bits
+
+		if not hasattr(self, 'startbit'):
+			startbit = 8 - self.bits - self._lsb
+			if startbit < 0:
+				raise ValueError(f'lsb is not implemented for signals spanning multiple bytes (lsb={self._lsb}, bits={self.bits})')
+			self.startbit = startbit
+
+
 	def get_bitstruct_fmt(self) -> str:
 		return '%s%s' % (self.type.value, self.bits)
 
 
 	def __repr__(self) -> str:
 		return '%s(%s)' % (type(self).__name__, ', '.join('%s=%r' % (a, getattr(self, a)) for a in ('name', 'type', 'address', 'bits', 'startbit', 'offset', 'scale', 'unit')))
```

### Comparing `serialtools-0.3.0/src/serialtools/database_config.py` & `serialtools-0.4.0/src/serialtools/database_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,21 +98,23 @@
 	signals: 'list[db.Signal]' = []
 
 	def init_parser(self, parser: argparse.ArgumentParser) -> None:
 		parser.add_argument('name', help="The name of the signal")
 		self.add_enum_argument(parser, 'type', type=db.Type)
 		parser.add_argument('address', type=integer, help="The address which is used to request this value from the battery")
 		parser.add_argument('--bits', type=integer, help="The size of this signal in bits")
-		parser.add_argument('--startbit', default=0, type=integer, help="If the word identified by address contains several smaller values the startbit specifies where the signal starts inside of the word")
+		group = parser.add_mutually_exclusive_group()
+		group.add_argument('--startbit', default=None, type=integer, help="If the word identified by address contains several smaller values the startbit specifies the first transmitted bit belonging to the signal")
+		group.add_argument('--lsb', default=None, type=integer, help="If the word identified by address contains several smaller values the lsb specifies where the leat significant bit of the signal is inside of the word")
 		parser.add_argument('--scale', type=float, default=1, help="A factor which is multiplied to the raw value received on the bus in order to get a value in the specified unit")
 		parser.add_argument('--offset', type=float, default=0, help="A summand which is added to the raw value received on the bus in order to get a value in the specified unit")
 		parser.add_argument('--unit', default='', help="The unit of the value")
 
 	def run_parsed(self, args: argparse.Namespace) -> None:
-		self.signals.append(db.Signal(args.name, args.type, args.address, bits=args.bits, startbit=args.startbit, scale=args.scale, offset=args.offset, unit=args.unit))
+		self.signals.append(db.Signal(args.name, args.type, args.address, bits=args.bits, startbit=args.startbit, lsb=args.lsb, scale=args.scale, offset=args.offset, unit=args.unit))
 
 class DatabaseCreator:
 
 	word_length_in_bits = Config('db.word-size', 8, unit='bits')
 	endianness = ExplicitConfig('db.endianness', db.Endianness)
 
 	def get(self, *, require_signals: bool = True) -> db.Database:
```

### Comparing `serialtools-0.3.0/PKG-INFO` & `serialtools-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serialtools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools to work with a serial bus
 Author-email: erzo <erzo@posteo.de>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
```

