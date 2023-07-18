# Comparing `tmp/reuse-2.0.0.tar.gz` & `tmp/reuse-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reuse-2.0.0.tar", max compression
+gzip compressed data, was "reuse-2.1.0.tar", max compression
```

## Comparing `reuse-2.0.0.tar` & `reuse-2.1.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1154 2023-06-21 09:24:49.565014 reuse-2.0.0/.reuse/dep5
--rw-r--r--   0        0        0     1814 2023-06-21 09:24:49.565014 reuse-2.0.0/AUTHORS.rst
--rw-r--r--   0        0        0    29293 2023-06-21 11:00:49.131810 reuse-2.0.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/
--rw-r--r--   0        0        0    11358 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    20131 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0        0        0     7048 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0    35149 2023-06-21 09:24:49.569014 reuse-2.0.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     9941 2023-06-21 10:51:41.407169 reuse-2.0.0/README.md
--rw-r--r--   0        0        0     2173 2023-06-21 09:24:49.569014 reuse-2.0.0/_build.py
--rw-r--r--   0        0        0      712 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/Makefile
--rw-r--r--   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      164 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/authors.rst
--rw-r--r--   0        0        0     5955 2023-06-21 10:51:41.407169 reuse-2.0.0/docs/conf.py
--rw-r--r--   0        0        0      643 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/index.rst
--rw-r--r--   0        0        0     4232 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      124 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/requirements.txt.license
--rw-r--r--   0        0        0     5608 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/reuse-r-only.svg
--rw-r--r--   0        0        0      105 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/reuse-r-only.svg.license
--rw-r--r--   0        0        0     5776 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/scripts.rst
--rw-r--r--   0        0        0    12618 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/usage.rst
--rw-r--r--   0        0        0      192 2023-06-21 09:24:49.569014 reuse-2.0.0/docs/usage.rst.license
--rw-r--r--   0        0        0      331 2023-06-21 09:24:49.569014 reuse-2.0.0/po/POTFILES.in
--rw-r--r--   0        0        0    29042 2023-06-21 10:46:01.722193 reuse-2.0.0/po/cs.po
--rw-r--r--   0        0        0    28286 2023-06-21 10:46:01.722193 reuse-2.0.0/po/de.po
--rw-r--r--   0        0        0    31871 2023-06-21 10:46:01.722193 reuse-2.0.0/po/eo.po
--rw-r--r--   0        0        0    33269 2023-06-21 10:46:01.722193 reuse-2.0.0/po/es.po
--rw-r--r--   0        0        0    24933 2023-06-21 10:46:01.722193 reuse-2.0.0/po/fr.po
--rw-r--r--   0        0        0    27746 2023-06-21 10:46:01.722193 reuse-2.0.0/po/gl.po
--rw-r--r--   0        0        0    28199 2023-06-21 10:46:01.722193 reuse-2.0.0/po/it.po
--rw-r--r--   0        0        0    32658 2023-06-21 10:46:01.722193 reuse-2.0.0/po/nl.po
--rw-r--r--   0        0        0    28325 2023-06-21 10:46:01.722193 reuse-2.0.0/po/pt.po
--rw-r--r--   0        0        0    20298 2023-06-21 09:24:49.569014 reuse-2.0.0/po/reuse.pot
--rw-r--r--   0        0        0      108 2023-06-21 09:24:49.569014 reuse-2.0.0/po/reuse.pot.license
--rw-r--r--   0        0        0    27570 2023-06-21 10:46:01.722193 reuse-2.0.0/po/tr.po
--rw-r--r--   0        0        0    42021 2023-06-21 10:46:01.726193 reuse-2.0.0/po/uk.po
--rw-r--r--   0        0        0     3086 2023-06-21 10:51:41.407169 reuse-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5708 2023-06-21 10:51:41.407169 reuse-2.0.0/src/reuse/__init__.py
--rw-r--r--   0        0        0      254 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/__main__.py
--rw-r--r--   0        0        0     1358 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_format.py
--rw-r--r--   0        0        0     2161 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_licenses.py
--rw-r--r--   0        0        0     9668 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_main.py
--rw-r--r--   0        0        0    18609 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/_util.py
--rw-r--r--   0        0        0    24169 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/comment.py
--rw-r--r--   0        0        0     5272 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/download.py
--rw-r--r--   0        0        0    25834 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/header.py
--rw-r--r--   0        0        0     4156 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/init.py
--rw-r--r--   0        0        0     8425 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/lint.py
--rw-r--r--   0        0        0    14788 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/project.py
--rw-r--r--   0        0        0      122 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/py.typed
--rw-r--r--   0        0        0    18953 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/report.py
--rw-r--r--   0        0        0    23174 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/exceptions.json
--rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/exceptions.json.license
--rw-r--r--   0        0        0   251607 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/licenses.json
--rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/resources/licenses.json.license
--rw-r--r--   0        0        0     3132 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/spdx.py
--rw-r--r--   0        0        0     1040 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/supported_licenses.py
--rw-r--r--   0        0        0      281 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/templates/default_template.jinja2
--rw-r--r--   0        0        0      119 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/templates/default_template.jinja2.license
--rw-r--r--   0        0        0     6784 2023-06-21 09:24:49.569014 reuse-2.0.0/src/reuse/vcs.py
--rw-r--r--   0        0        0    11145 2023-06-21 09:24:49.569014 reuse-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      215 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/.reuse/dep5
--rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
--rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
--rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0        0 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
--rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/doc/index.rst
--rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/custom.py
--rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/exception.py
--rw-r--r--   0        0        0       59 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/multiple_licenses.rs
--rw-r--r--   0        0        0      156 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.c
--rw-r--r--   0        0        0      111 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.html
--rw-r--r--   0        0        0      109 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.jinja2
--rw-r--r--   0        0        0      166 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fake_repository/src/source_code.py
--rw-r--r--   0        0        0     5450 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/resources/fsfe.png
--rw-r--r--   0        0        0    14497 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_comment.py
--rw-r--r--   0        0        0     2480 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_core.py
--rw-r--r--   0        0        0     3201 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_download.py
--rw-r--r--   0        0        0    10656 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_header.py
--rw-r--r--   0        0        0     7156 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_lint.py
--rw-r--r--   0        0        0    14494 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main.py
--rw-r--r--   0        0        0    34232 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main_annotate.py
--rw-r--r--   0        0        0     3712 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_main_annotate_merge.py
--rw-r--r--   0        0        0    13333 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_project.py
--rw-r--r--   0        0        0    13056 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_report.py
--rw-r--r--   0        0        0    20096 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_util.py
--rw-r--r--   0        0        0      900 2023-06-21 09:24:49.573014 reuse-2.0.0/tests/test_vcs.py
--rw-r--r--   0        0        0    11431 1970-01-01 00:00:00.000000 reuse-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1154 2023-06-21 09:24:49.565014 reuse-2.1.0/.reuse/dep5
+-rw-r--r--   0        0        0     1814 2023-06-21 09:24:49.565014 reuse-2.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0    32148 2023-07-18 08:51:36.127596 reuse-2.1.0/CHANGELOG.md
+drwxr-xr-x   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.1.0/LICENSES/
+-rw-r--r--   0        0        0    11358 2023-06-21 09:24:49.569014 reuse-2.1.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    20131 2023-06-21 09:24:49.569014 reuse-2.1.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0        0        0     7048 2023-06-21 09:24:49.569014 reuse-2.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0    35149 2023-06-21 09:24:49.569014 reuse-2.1.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     9941 2023-07-18 08:51:36.127596 reuse-2.1.0/README.md
+-rw-r--r--   0        0        0     2173 2023-06-21 09:24:49.569014 reuse-2.1.0/_build.py
+-rw-r--r--   0        0        0      712 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      164 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/authors.rst
+-rw-r--r--   0        0        0     6010 2023-07-18 08:51:36.127596 reuse-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0      643 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/index.rst
+-rw-r--r--   0        0        0     2893 2023-07-18 07:47:38.249276 reuse-2.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0      124 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/requirements.txt.license
+-rw-r--r--   0        0        0     5608 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/reuse-r-only.svg
+-rw-r--r--   0        0        0      105 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/reuse-r-only.svg.license
+-rw-r--r--   0        0        0     5776 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/scripts.rst
+-rw-r--r--   0        0        0    12618 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/usage.rst
+-rw-r--r--   0        0        0      192 2023-06-21 09:24:49.569014 reuse-2.1.0/docs/usage.rst.license
+-rw-r--r--   0        0        0      331 2023-06-21 09:24:49.569014 reuse-2.1.0/po/POTFILES.in
+-rw-r--r--   0        0        0    31043 2023-07-18 08:51:36.127596 reuse-2.1.0/po/cs.po
+-rw-r--r--   0        0        0    29454 2023-07-18 08:51:36.127596 reuse-2.1.0/po/de.po
+-rw-r--r--   0        0        0    33258 2023-07-18 08:51:36.127596 reuse-2.1.0/po/eo.po
+-rw-r--r--   0        0        0    34442 2023-07-18 08:51:36.127596 reuse-2.1.0/po/es.po
+-rw-r--r--   0        0        0    29931 2023-07-18 08:51:36.127596 reuse-2.1.0/po/fr.po
+-rw-r--r--   0        0        0    28895 2023-07-18 08:51:36.127596 reuse-2.1.0/po/gl.po
+-rw-r--r--   0        0        0    29384 2023-07-18 08:51:36.127596 reuse-2.1.0/po/it.po
+-rw-r--r--   0        0        0    33793 2023-07-18 08:51:36.127596 reuse-2.1.0/po/nl.po
+-rw-r--r--   0        0        0    29501 2023-07-18 08:51:36.127596 reuse-2.1.0/po/pt.po
+-rw-r--r--   0        0        0    20582 2023-07-18 08:51:36.127596 reuse-2.1.0/po/reuse.pot
+-rw-r--r--   0        0        0      108 2023-06-21 09:24:49.569014 reuse-2.1.0/po/reuse.pot.license
+-rw-r--r--   0        0        0    28747 2023-07-18 08:51:36.127596 reuse-2.1.0/po/tr.po
+-rw-r--r--   0        0        0    38908 2023-07-18 08:51:36.127596 reuse-2.1.0/po/uk.po
+-rw-r--r--   0        0        0     3189 2023-07-18 08:51:36.127596 reuse-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6131 2023-07-18 08:51:36.127596 reuse-2.1.0/src/reuse/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/__main__.py
+-rw-r--r--   0        0        0     1358 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/_format.py
+-rw-r--r--   0        0        0     2161 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/_licenses.py
+-rw-r--r--   0        0        0     9982 2023-07-18 07:47:38.257276 reuse-2.1.0/src/reuse/_main.py
+-rw-r--r--   0        0        0    18688 2023-07-18 07:47:34.685286 reuse-2.1.0/src/reuse/_util.py
+-rw-r--r--   0        0        0    24211 2023-07-18 07:47:38.257276 reuse-2.1.0/src/reuse/comment.py
+-rw-r--r--   0        0        0     5272 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/download.py
+-rw-r--r--   0        0        0    25834 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/header.py
+-rw-r--r--   0        0        0     4156 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/init.py
+-rw-r--r--   0        0        0     8425 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/lint.py
+-rw-r--r--   0        0        0    15381 2023-07-18 07:47:34.685286 reuse-2.1.0/src/reuse/project.py
+-rw-r--r--   0        0        0      122 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/py.typed
+-rw-r--r--   0        0        0    19063 2023-07-18 07:47:34.685286 reuse-2.1.0/src/reuse/report.py
+-rw-r--r--   0        0        0    23174 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/resources/exceptions.json
+-rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/resources/exceptions.json.license
+-rw-r--r--   0        0        0   251607 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/resources/licenses.json
+-rw-r--r--   0        0        0      100 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/resources/licenses.json.license
+-rw-r--r--   0        0        0     3132 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/spdx.py
+-rw-r--r--   0        0        0     1040 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/supported_licenses.py
+-rw-r--r--   0        0        0      281 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/templates/default_template.jinja2
+-rw-r--r--   0        0        0      119 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/templates/default_template.jinja2.license
+-rw-r--r--   0        0        0     6784 2023-06-21 09:24:49.569014 reuse-2.1.0/src/reuse/vcs.py
+-rw-r--r--   0        0        0    11145 2023-06-21 09:24:49.569014 reuse-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      215 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/.reuse/dep5
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/LICENSES/Autoconf-exception-3.0.txt
+-rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0       13 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0        0 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/LICENSES/LicenseRef-custom.txt
+-rw-r--r--   0        0        0       14 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/doc/index.rst
+-rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/custom.py
+-rw-r--r--   0        0        0       58 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/exception.py
+-rw-r--r--   0        0        0       59 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/multiple_licenses.rs
+-rw-r--r--   0        0        0      156 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/source_code.c
+-rw-r--r--   0        0        0      111 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/source_code.html
+-rw-r--r--   0        0        0      109 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/source_code.jinja2
+-rw-r--r--   0        0        0      166 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fake_repository/src/source_code.py
+-rw-r--r--   0        0        0     5450 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/resources/fsfe.png
+-rw-r--r--   0        0        0    14497 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_comment.py
+-rw-r--r--   0        0        0     3316 2023-07-18 07:47:34.685286 reuse-2.1.0/tests/test_core.py
+-rw-r--r--   0        0        0     3201 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_download.py
+-rw-r--r--   0        0        0    10656 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_header.py
+-rw-r--r--   0        0        0     6012 2023-07-06 08:17:34.509908 reuse-2.1.0/tests/test_lint.py
+-rw-r--r--   0        0        0    14494 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_main.py
+-rw-r--r--   0        0        0    34232 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_main_annotate.py
+-rw-r--r--   0        0        0     3712 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_main_annotate_merge.py
+-rw-r--r--   0        0        0    14154 2023-07-18 07:47:34.685286 reuse-2.1.0/tests/test_project.py
+-rw-r--r--   0        0        0    14672 2023-07-18 07:47:34.685286 reuse-2.1.0/tests/test_report.py
+-rw-r--r--   0        0        0    20096 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_util.py
+-rw-r--r--   0        0        0      900 2023-06-21 09:24:49.573014 reuse-2.1.0/tests/test_vcs.py
+-rw-r--r--   0        0        0    11431 1970-01-01 00:00:00.000000 reuse-2.1.0/PKG-INFO
```

### Comparing `reuse-2.0.0/.reuse/dep5` & `reuse-2.1.0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/AUTHORS.rst` & `reuse-2.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/CHANGELOG.md` & `reuse-2.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,53 @@
 ### Removed
 
 ### Fixed
 
 ### Security
 -->
 
-## 2.0.0 - 2023-06-21
+## Unreleased - YYYY-MM-DD
+
+### Added
+
+### Changed
+
+### Deprecated
+
+### Removed
+
+### Fixed
+
+### Security
+
+## 2.1.0 - 2023-07-18
+
+After the yanked 2.0.0 release, we're excited to announce our latest major
+version packed with new features and improvements! We've expanded our file type
+recognition, now including Fennel, CommonJS, Qt .pro, .pri, .qrc, .qss, .ui,
+Textile, Visual Studio Code workspace, Application Resource Bundle, Svelte
+components, AES encrypted files, Jakarta Server Page, Clang format, Browserslist
+config, Prettier config and ignored files, Flutter pubspec.lock, .metadata,
+Terraform and HCL, Typst and more.
+
+We've also added the ability to detect SPDX snippet tags in files and introduced
+additional license metadata for the Python package. A new `--json` flag has been
+added to the `lint` command, marking the first step towards better integration
+of REUSE output with other tools.
+
+On the changes front, we've bumped the SPDX license list to v3.21 and made
+significant updates to our Sphinx documentation. Please note that Python 3.6 and
+3.7 support has been dropped in this release.
+
+We've fixed several issues including automatic generation of Sphinx
+documentation via readthedocs.io and a compatibility issue where reuse could not
+be installed if gettext is not installed.
+
+This update is all about making your experience better. Enjoy adding copyright
+and licensing information to your code!
 
 ### Added
 
 - Detect SPDX snippet tags in files. (#699)
 - More file types are recognised:
   - Fennel (`.fnl`) (#638)
   - CommonJS (`.cjs`) (#632)
@@ -53,47 +91,60 @@
   - Qt .ui (`.ui`) (#755)
   - Textile (`.textile`) (#712)
   - Visual Studio Code workspace (`.code-workspace`) (#747)
   - Application Resource Bundle (`.arb`) (#749)
   - Svelte components (`.svelte`)
   - AES encrypted files (`.aes`) (#758)
   - Jakarte Server Page (`.jsp`) (#757)
-- More files are recognised:
   - Clang format (`.clang-format`) (#632)
   - Browserslist config (`.browserslist`)
   - Prettier config (`.prettierrc`) and ignored files (`.prettierignore`)
   - Flutter pubspec.lock (`pubspec.lock`) (#751)
   - Flutter .metadata (`.metadata`) (#751)
   - Terraform (`.tf`, `tfvars`) and HCL (`.hcl`). (#756)
+  - Typst (`.typ`)
 - Added loglevel argument to pytest and skip one test if loglevel is too high
   (#645).
 - `--add-license-concluded`, `--creator-person`, and `--creator-organization`
   added to `reuse spdx`. (#623)
 - Additional license metadata for the Python package has been added. The actual
   SPDX license expression remains the same:
   `Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later`. (#733)
 - Added `--contributor` option to `annotate`. (#669)
 - Added `--json` flag to `lint` command (#654).
 - `reuse.ReuseInfo` now has `copy` and `union` methods. (#759)
+- `reuse.ReuseInfo` now stores information about the source from which the
+  information was gathered. (#654, #787)
 - Added Ukrainian and Czech translations (#767)
+- Added `--suppress-deprecation` to hide (verbose) deprecation warnings. (#778)
 
 ### Changed
 
 - Bumped SPDX license list to v3.20. (#692)
 - `reuse.SpdxInfo` was renamed to `reuse.ReuseInfo`. It is now a (frozen)
   dataclass instead of a namedtuple. This is only relevant if you're using reuse
-  as a library in Python. (#669)
+  as a library in Python. Other functions and methods were similarly renamed.
+  (#669)
 - Sphinx documentation: Switched from RTD theme to Furo. (#673, #716)
 - Removed dependency on setuptools' `pkg_resources` to determine the installed
   version of reuse. (#724)
 - Bumped SPDX license list to v3.21. (#763)
-- Bumped REUSE Spec version to 3.1. (#768)
-- Introduce an order of precedence. The copyright and licensing information from
-  different sources (e.g. `.license` or `.reuse/dep5` file) is no longer merged.
-  (#654)
+- `Project.reuse_info_of` now returns a list of `ReuseInfo` objects instead of a
+  single one. This is because the source information is now stored alongside the
+  REUSE information. (#787)
+
+### Deprecated
+
+- Pending deprecation of aggregation of file sources. Presently, when copyright
+  and licensing information is defined both within e.g. the file itself and in
+  the DEP5 file, then the information is merged or aggregated for the purposes
+  of linting and BOM generation. In the future, this will no longer be the case
+  unless explicitly defined. The exact mechanism for this is not yet concrete,
+  but a `PendingDeprecationWarning` will be shown to the user to make them aware
+  of this. (#778)
 
 ### Removed
 
 - Python 3.6 and 3.7 support has been dropped. (#673, #759)
 - Removed runtime and build time dependency on `setuptools`. (#724)
 
 ### Fixed
@@ -103,14 +154,31 @@
 - Fixed a compatibility issue where reuse could not be installed (built) if
   gettext is not installed. (#691)
 - Translations are available in Docker images. (#701)
 - Marked the `/data` directory in Docker containers as safe in Git, preventing
   errors related to linting Git repositories. (#720)
 - Repaired error when using Galician translations. (#719)
 
+### Security
+
+## 2.0.0 - 2023-06-21 [YANKED]
+
+This version was yanked because of an unanticipated workflow that we broke. The
+breaking change is the fact that an order of precedence was defined for
+copyright and licensing information sources. For instance, if a file contained
+the `SPDX-License-Identifier` tag, and if that file was also (explicitly or
+implicitly) covered by DEP5, then the information from the DEP5 setting would no
+longer apply to that file.
+
+While the intention of the breaking change was sound (don't mix information
+sources; define a single source of truth), there were legitimate use-cases that
+were broken as a result of this.
+
+Apologies to everyone whose CI broke. We'll get this one right before long.
+
 ## 1.1.2 - 2023-02-09
 
 ### Fixed
 
 - Note to maintainers: It is now possible/easier to use the `build` module to
   build this module. Previously, there was a namespace conflict. (#640)
```

### Comparing `reuse-2.0.0/LICENSES/Apache-2.0.txt` & `reuse-2.1.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/LICENSES/CC-BY-SA-4.0.txt` & `reuse-2.1.0/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/LICENSES/CC0-1.0.txt` & `reuse-2.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/LICENSES/GPL-3.0-or-later.txt` & `reuse-2.1.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/README.md` & `reuse-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v2.0.0
+    rev: v2.1.0
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
```

### Comparing `reuse-2.0.0/_build.py` & `reuse-2.1.0/_build.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/docs/Makefile` & `reuse-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/docs/conf.py` & `reuse-2.1.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-from importlib.metadata import PackageNotFoundError, version
+from importlib.metadata import PackageNotFoundError
+from importlib.metadata import version as get_version
 from shutil import copyfile
 
 sys.path.insert(0, os.path.abspath("../src/"))
 
 
 # -- General configuration ------------------------------------------------
 
@@ -69,17 +70,17 @@
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
 try:
     # The full version, including alpha/beta/rc tags.
-    release = version("reuse")
+    release = get_version("reuse")
 except PackageNotFoundError:
-    release = "2.0.0"
+    release = "2.1.0"
 
 # The short X.Y.Z version.
 version = ".".join(release.split(".")[:3])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
@@ -122,15 +123,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "reusedoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
+latex_elements: dict = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
```

### Comparing `reuse-2.0.0/docs/index.rst` & `reuse-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/docs/reuse-r-only.svg` & `reuse-2.1.0/docs/reuse-r-only.svg`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/docs/scripts.rst` & `reuse-2.1.0/docs/scripts.rst`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/docs/usage.rst` & `reuse-2.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/po/cs.po` & `reuse-2.1.0/po/cs.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,95 +4,102 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-17 21:21+0000\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: 2023-04-12 13:49+0000\n"
 "Last-Translator: Jiří Podhorecký <j.podhorecky@volny.cz>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/fsfe/reuse-tool/cs/"
 ">\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
 "X-Generator: Weblate 4.17-dev\n"
 
-#: src/reuse/_main.py:33
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
 "reuse je nástrojem pro dodržování doporučení REUSE. Další informace "
 "naleznete na adrese <https://reuse.software/> a online dokumentaci na adrese "
 "<https://reuse.readthedocs.io/>."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr "Tato verze reuse je kompatibilní s verzí {} specifikace REUSE."
 
-#: src/reuse/_main.py:42
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
 msgstr "Podpořte činnost FSFE:"
 
-#: src/reuse/_main.py:46
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
 "Dary jsou pro naši sílu a nezávislost zásadní. Umožňují nám pokračovat v "
 "práci pro svobodný software všude tam, kde je to nutné. Zvažte prosím "
 "možnost přispět na <https://fsfe.org/donate/>."
 
-#: src/reuse/_main.py:69
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
 msgstr "povolit příkazy pro ladění"
 
-#: src/reuse/_main.py:74
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
 msgstr "nepřeskakovat submoduly systému Git"
 
-#: src/reuse/_main.py:79
+#: src/reuse/_main.py:85
 msgid "do not skip over Meson subprojects"
 msgstr "nepřeskakovat podprojekty Meson"
 
-#: src/reuse/_main.py:84
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
 msgstr "nepoužívat multiprocessing"
 
-#: src/reuse/_main.py:91
+#: src/reuse/_main.py:97
 msgid "define root of project"
 msgstr "definovat kořen projektu"
 
-#: src/reuse/_main.py:96
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
 msgstr "zobrazit číslo verze programu a ukončit jej"
 
-#: src/reuse/_main.py:100
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr "dílčí příkazy"
 
-#: src/reuse/_main.py:107
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
 msgstr "přidání autorských práv a licencí do záhlaví souborů"
 
-#: src/reuse/_main.py:110
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
 "The first comment is replaced with a new header containing the new copyright "
 "and licensing information and its former copyright and licensing. If you "
 "want to keep the first comment intact, use --no-replace.\n"
 "\n"
 "The comment style should be auto-detected for your files. If a comment style "
 "could not be detected and --skip-unrecognised is not specified, the process "
 "aborts. Use --style to specify or override the comment style to use.\n"
@@ -122,30 +129,35 @@
 "Styl komentáře by měl být pro vaše soubory automaticky detekován. Pokud se "
 "styl komentáře nepodařilo zjistit a není zadána možnost --skip-unrecognised, "
 "proces se přeruší. Pomocí --style určete nebo přepište styl komentáře, který "
 "se má použít.\n"
 "\n"
 "Pokud je k dispozici jednořádkový styl komentáře, použije se tento styl. "
 "Pokud není k dispozici jednořádkový styl komentáře, použije se víceřádkový "
-"styl komentáře. Určitý styl komentáře můžete vynutit pomocí parametrů "
-"--single-line nebo --multi-line.\n"
+"styl komentáře. Určitý styl komentáře můžete vynutit pomocí parametrů --"
+"single-line nebo --multi-line.\n"
 "\n"
 "Šablonu komentáře záhlaví můžete změnit pomocí příkazu --template. Umístěte "
 "šablonu Jinja2 do souboru .reuse/templates/mytemplate.jinja2. Šablonu můžete "
 "použít zadáním '--template mytemplate'. Přečtěte si online dokumentaci, jak "
 "tuto funkci používat.\n"
 "\n"
 "Pokud je detekován binární soubor nebo pokud je zadán parametr --explicit-"
 "license, je hlavička umístěna do souboru .license."
 
-#: src/reuse/_main.py:158
+#: src/reuse/_main.py:159
+#, fuzzy
+msgid "deprecated in favor of annotate"
+msgstr "'reuse addheader' bylo zrušeno ve prospěch 'reuse annotate'"
+
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "stáhněte si licenci a umístěte ji do adresáře LICENSES/"
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
@@ -163,23 +175,23 @@
 "\n"
 "- Aktuální adresář, pokud je jeho název LICENSES.\n"
 "\n"
 "- Adresář LICENSES/ v aktuálním adresáři.\n"
 "\n"
 "Pokud adresář LICENSES/ nelze nalézt, je jednoduše vytvořen."
 
-#: src/reuse/_main.py:184
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
 msgstr "inicializace projektu REUSE"
 
-#: src/reuse/_main.py:192
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
 msgstr "seznam všech nevyhovujících souborů"
 
-#: src/reuse/_main.py:195
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -207,521 +219,573 @@
 "obsaženy v adresáři LICENSES/?\n"
 "\n"
 "- Jsou v adresáři LICENSES/ obsaženy licence, které se uvnitř projektu "
 "nepoužívají?\n"
 "\n"
 "- Mají všechny soubory platné informace o autorských právech a licencích?"
 
-#: src/reuse/_main.py:222
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
 msgstr "vytisknout výkaz materiálu projektu ve formátu SPDX"
 
-#: src/reuse/_main.py:230
+#: src/reuse/_main.py:239
 msgid "list all supported SPDX licenses"
 msgstr "seznam všech podporovaných licencí SPDX"
 
-#: src/reuse/_util.py:294
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
 msgstr "Nepodařilo se analyzovat '{expression}'"
 
-#: src/reuse/_util.py:418
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
 msgstr "'{}' není soubor"
 
-#: src/reuse/_util.py:421
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
 msgstr "'{}' není adresář"
 
-#: src/reuse/_util.py:424
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
 msgstr "nelze otevřít '{}'"
 
-#: src/reuse/_util.py:429
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
 msgstr "nelze zapisovat do adresáře '{}'"
 
-#: src/reuse/_util.py:435 src/reuse/header.py:558
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
 msgstr "nelze zapisovat do '{}'"
 
-#: src/reuse/_util.py:448
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
 msgstr "nelze číst ani zapisovat '{}'"
 
-#: src/reuse/_util.py:458
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
 msgstr "'{}' není platný výraz SPDX, přeruší se"
 
-#: src/reuse/_util.py:484
+#: src/reuse/_util.py:544
 msgid "'{}' is not a valid SPDX License Identifier."
 msgstr "'{}' není platný identifikátor licence SPDX."
 
-#: src/reuse/_util.py:491
+#: src/reuse/_util.py:551
 msgid "Did you mean:"
 msgstr "Měl jste na mysli:"
 
-#: src/reuse/_util.py:498
+#: src/reuse/_util.py:558
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License "
 "Identifiers."
 msgstr ""
-"Seznam platných identifikátorů licence SPDX naleznete na adrese <https://spdx"
-".org/licenses/>."
+"Seznam platných identifikátorů licence SPDX naleznete na adrese <https://"
+"spdx.org/licenses/>."
 
-#: src/reuse/download.py:84
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
 msgstr "Licence SPDX Identifikátor licence"
 
-#: src/reuse/download.py:89
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
 msgstr "stáhnout všechny chybějící licence zjištěné v projektu"
 
-#: src/reuse/download.py:101
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
 msgstr "Chyba: {spdx_identifier} již existuje."
 
-#: src/reuse/download.py:108
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
 msgstr "Chyba: Nepodařilo se stáhnout licenci."
 
-#: src/reuse/download.py:113
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
 msgstr "Funguje vaše internetové připojení?"
 
-#: src/reuse/download.py:118
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
 msgstr "Úspěšně stažen {spdx_identifier}."
 
-#: src/reuse/download.py:130
+#: src/reuse/download.py:134
 msgid "--output has no effect when used together with --all"
 msgstr "--output nemá žádný účinek, pokud se použije společně s --all"
 
-#: src/reuse/download.py:134
+#: src/reuse/download.py:138
 msgid "the following arguments are required: license"
 msgstr "jsou vyžadovány tyto argumenty: licence"
 
-#: src/reuse/download.py:136
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
 msgstr "nelze použít --output s více než jednou licencí"
 
-#: src/reuse/header.py:121
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
 "ve vygenerovaném komentáři chybí řádky s autorskými právy nebo licenční "
 "výrazy"
 
-#: src/reuse/header.py:401
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
 "'{path}' does not support single-line comments, please do not use --single-"
 "line"
 msgstr ""
 "'{path}' nepodporuje jednořádkové komentáře, nepoužívejte prosím --single-"
 "line"
 
-#: src/reuse/header.py:408
+#: src/reuse/header.py:421
 #, python-brace-format
 msgid ""
 "'{path}' does not support multi-line comments, please do not use --multi-line"
 msgstr "'{path}' nepodporuje víceřádkové komentáře, nepoužívejte --multi-line"
 
-#: src/reuse/header.py:429
+#: src/reuse/header.py:444
 msgid ""
 "The following files do not have a recognised file extension. Please use --"
 "style, --force-dot-license or --skip-unrecognised:"
 msgstr ""
-"Následující soubory nemají rozpoznanou příponu. Použijte prosím --style, "
-"--force-dot-licence nebo --skip-unrecognised:"
+"Následující soubory nemají rozpoznanou příponu. Použijte prosím --style, --"
+"force-dot-licence nebo --skip-unrecognised:"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:497
 #, python-brace-format
 msgid "Skipped unrecognised file {path}"
 msgstr "Přeskočen nerozpoznaný soubor {path}"
 
-#: src/reuse/header.py:494
-#, python-brace-format
-msgid "Skipped file '{path}' already containing SPDX information"
+#: src/reuse/header.py:509
+#, fuzzy, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
 msgstr "Přeskočený soubor '{path}' již obsahuje informace SPDX"
 
-#: src/reuse/header.py:528
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Chyba: Nepodařilo se vytvořit komentář pro '{path}'"
 
-#: src/reuse/header.py:535
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
 "Chyba: Chybí řádky s autorskými právy nebo licenční výrazy v generovaném "
 "záhlaví komentáře pro '{path}'. Šablona je pravděpodobně nesprávná. "
 "Nepodařilo se zapsat novou hlavičku."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:546
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "Úspěšně změněna hlavička {path}"
 
-#: src/reuse/header.py:569
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
 msgstr "prohlášení o autorských právech, opakovatelné"
 
-#: src/reuse/header.py:576
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
 msgstr "Identifikátor SPDX, opakovatelný"
 
-#: src/reuse/header.py:583
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "Identifikátor SPDX, opakovatelný"
+
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
 msgstr "rok vydání prohlášení o autorských právech, nepovinné"
 
-#: src/reuse/header.py:591
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
 msgstr "styl komentáře, který se má použít, nepovinné"
 
-#: src/reuse/header.py:597
+#: src/reuse/header.py:620
 msgid "copyright style to use, optional"
 msgstr "styl autorských práv, který se má použít, nepovinné"
 
-#: src/reuse/header.py:604
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
 msgstr "název šablony, která se má použít, nepovinné"
 
-#: src/reuse/header.py:609
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
 msgstr "neuvádět rok v prohlášení"
 
-#: src/reuse/header.py:614
+#: src/reuse/header.py:637
 msgid "merge copyright lines if copyright statements are identical"
 msgstr ""
 "sloučit řádky s autorskými právy, pokud jsou prohlášení o autorských právech "
 "totožná"
 
-#: src/reuse/header.py:619
+#: src/reuse/header.py:642
 msgid "force single-line comment style, optional"
 msgstr "vynutit jednořádkový styl komentáře, nepovinné"
 
-#: src/reuse/header.py:624
+#: src/reuse/header.py:647
 msgid "force multi-line comment style, optional"
 msgstr "vynutit víceřádkový styl komentáře, nepovinné"
 
-#: src/reuse/header.py:634
+#: src/reuse/header.py:657
 msgid "write a .license file instead of a header inside the file"
 msgstr "zapsat soubor .license místo hlavičky uvnitř souboru"
 
-#: src/reuse/header.py:641
+#: src/reuse/header.py:664
 msgid "add headers to all files under specified directories recursively"
 msgstr "zpětně přidat hlavičky ke všem souborům v zadaných adresářích"
 
-#: src/reuse/header.py:648
+#: src/reuse/header.py:671
 msgid "do not replace the first header in the file; just add a new one"
 msgstr "nenahrazovat první hlavičku v souboru, ale přidat novou"
 
-#: src/reuse/header.py:654
+#: src/reuse/header.py:677
 msgid "skip files with unrecognised comment styles"
 msgstr "přeskočit soubory s nerozpoznanými styly komentářů"
 
-#: src/reuse/header.py:659
-msgid "skip files that already contain SPDX information"
+#: src/reuse/header.py:682
+#, fuzzy
+msgid "skip files that already contain REUSE information"
 msgstr "přeskočit soubory, které již obsahují informace SPDX"
 
-#: src/reuse/header.py:670
+#: src/reuse/header.py:693
 msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
 msgstr "'reuse addheader' bylo zrušeno ve prospěch 'reuse annotate'"
 
-#: src/reuse/header.py:676
-msgid "option --copyright or --license is required"
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
 msgstr "je vyžadována volba --copyright nebo --licence"
 
-#: src/reuse/header.py:680
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
 msgstr "volby --exclude-year a --year se vzájemně vylučují"
 
-#: src/reuse/header.py:685
+#: src/reuse/header.py:710
 msgid "option --single-line and --multi-line are mutually exclusive"
 msgstr "volby --single-line a --multi-line se vzájemně vylučují"
 
-#: src/reuse/header.py:691
+#: src/reuse/header.py:716
 msgid "--skip-unrecognised has no effect when used together with --style"
 msgstr ""
 "--skip-unrecognised nemá žádný účinek, pokud se použije společně s --style"
 
-#: src/reuse/header.py:698
+#: src/reuse/header.py:723
 msgid "--explicit-license has been deprecated in favour of --force-dot-license"
 msgstr "--explicit-license bylo zrušeno ve prospěch --force-dot-license"
 
-#: src/reuse/header.py:742
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
 msgstr "šablonu {template} se nepodařilo najít"
 
-#: src/reuse/header.py:784
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr "'{path}' je binární soubor, proto použijte '{new_path}' pro hlavičku"
 
-#: src/reuse/init.py:24
+#: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
 msgstr "Pod jakou licencí je váš projekt? Uveďte identifikátor licence SPDX."
 
-#: src/reuse/init.py:28
+#: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License "
 "Identifier."
 msgstr ""
 "Pod jakou jinou licencí je váš projekt? Uveďte identifikátor licence SPDX."
 
-#: src/reuse/init.py:39
+#: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
 msgstr "Chcete-li přidávání licencí ukončit, stiskněte klávesu RETURN."
 
-#: src/reuse/init.py:73
+#: src/reuse/init.py:78
 msgid "Project already initialized"
 msgstr "Projekt je již inicializován"
 
-#: src/reuse/init.py:77
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
 msgstr "Inicializace projektu REUSE."
 
-#: src/reuse/init.py:82
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
 msgstr "Jaký je název projektu?"
 
-#: src/reuse/init.py:88
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
 msgstr "Jaká je internetová adresa projektu?"
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
 msgstr "Jak se jmenuje správce?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
 msgstr "Jaká je e-mailová adresa správce?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
 msgstr "Hotovo! Inicializuje se."
 
-#: src/reuse/init.py:114
+#: src/reuse/init.py:119
 msgid "Downloading {}"
 msgstr "Stahování {}"
 
-#: src/reuse/init.py:119
+#: src/reuse/init.py:124
 msgid "{} already exists"
 msgstr "{} již existuje"
 
-#: src/reuse/init.py:122
+#: src/reuse/init.py:127
 msgid "Could not download {}"
 msgstr "Nelze stáhnout {}"
 
-#: src/reuse/init.py:127
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
 msgstr "Vytvoření .reuse/dep5"
 
-#: src/reuse/init.py:150
+#: src/reuse/init.py:155
 msgid "Initialization complete."
 msgstr "Inicializace dokončena."
 
-#: src/reuse/lint.py:56
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
-msgstr "Gratulujeme! Váš projekt je v souladu s verzí {} specifikace REUSE :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
+msgstr ""
 
-#: src/reuse/lint.py:63
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
-msgstr "Váš projekt bohužel není v souladu s verzí {} specifikace REUSE :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
+msgstr ""
 
-#: src/reuse/lint.py:80
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
 msgstr "NEVHODNÉ LICENCE"
 
-#: src/reuse/lint.py:84 src/reuse/lint.py:149
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
 msgstr "'{}' nalezeno v:"
 
-#: src/reuse/lint.py:102
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
 msgstr "ZASTARALÉ LICENCE"
 
-#: src/reuse/lint.py:104
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
 msgstr "Následující licence jsou v SPDX zrušeny:"
 
-#: src/reuse/lint.py:122
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
 msgstr "LICENCE BEZ KONCOVKY SOUBORU"
 
-#: src/reuse/lint.py:124
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
 msgstr "Následující licence nemají příponu souboru:"
 
-#: src/reuse/lint.py:144
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
 msgstr "CHYBĚJÍCÍ LICENCE"
 
-#: src/reuse/lint.py:167
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
 msgstr "NEPOUŽITÉ LICENCE"
 
-#: src/reuse/lint.py:169
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
 msgstr "Následující licence nejsou používány:"
 
-#: src/reuse/lint.py:185
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
 msgstr "CHYBY ČTENÍ"
 
-#: src/reuse/lint.py:187
+#: src/reuse/lint.py:99
 msgid "Could not read:"
 msgstr "Nelze načíst:"
 
-#: src/reuse/lint.py:210
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "CHYBĚJÍCÍ INFORMACE O AUTORSKÝCH PRÁVECH A LICENCÍCH"
 
-#: src/reuse/lint.py:215
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
 "Následující soubory neobsahují žádné informace o autorských právech a "
 "licencích:"
 
-#: src/reuse/lint.py:224
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
 msgstr "Následující soubory nemají žádné informace o autorských právech:"
 
-#: src/reuse/lint.py:230
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
 msgstr "Následující soubory neobsahují žádné licenční informace:"
 
-#: src/reuse/lint.py:244
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
 msgstr "SHRNUTÍ"
 
-#: src/reuse/lint.py:250
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
 msgstr "Neplatné licence:"
 
-#: src/reuse/lint.py:259
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
 msgstr "Zastaralé licence:"
 
-#: src/reuse/lint.py:268
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
 msgstr "Licence bez přípony souboru:"
 
-#: src/reuse/lint.py:277
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
 msgstr "Chybějící licence:"
 
-#: src/reuse/lint.py:286
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
 msgstr "Nepoužité licence:"
 
-#: src/reuse/lint.py:295
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
 msgstr "Použité licence:"
 
-#: src/reuse/lint.py:304
-#, python-brace-format
-msgid "Read errors: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
 msgstr "Chyby čtení: {count}"
 
-#: src/reuse/lint.py:309
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
 msgstr "Soubory s informacemi o autorských právech: {count} / {total}"
 
-#: src/reuse/lint.py:318
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
 msgstr "Soubory s licenčními informacemi: {count} / {total}"
 
-#: src/reuse/project.py:64
-msgid "could not find supported VCS"
-msgstr "nepodařilo se najít podporovaný VCS"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr "Gratulujeme! Váš projekt je v souladu s verzí {} specifikace REUSE :-)"
 
-#: src/reuse/project.py:155
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr "Váš projekt bohužel není v souladu s verzí {} specifikace REUSE :-("
+
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
+
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
 msgstr "'{path}' zahrnuto v .reuse/dep5"
 
-#: src/reuse/project.py:167
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
 "'{path}' obsahuje výraz SPDX, který nelze analyzovat a soubor se přeskočí"
 
-#: src/reuse/project.py:240
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 obsahuje chyby syntaxe"
 
-#: src/reuse/project.py:242
+#: src/reuse/project.py:315
 msgid ".reuse/dep5 could not be parsed as utf-8"
 msgstr ".reuse/dep5 nelze analyzovat jako utf-8"
 
-#: src/reuse/project.py:268
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
 msgstr "určující identifikátor '{path}'"
 
-#: src/reuse/project.py:276
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
 msgstr "{path} nemá příponu souboru"
 
-#: src/reuse/project.py:286
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
 "Nepodařilo se přeložit identifikátor licence SPDX {path}, přeloženo na "
 "{identifier}. Zkontrolujte, zda je licence v seznamu licencí nalezeném na "
 "adrese <https://spdx.org/licenses/> nebo zda začíná znakem 'LicenseRef-' a "
 "zda má příponu souboru."
 
-#: src/reuse/project.py:298
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
-msgstr "{identifier} je identifikátor licence SPDX jak {path}, tak {other_path}"
+msgstr ""
+"{identifier} je identifikátor licence SPDX jak {path}, tak {other_path}"
 
-#: src/reuse/report.py:202
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr "Nepodařilo se načíst '{path}'"
 
-#: src/reuse/report.py:209
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
 msgstr "Při analýze souboru '{path}' došlo k neočekávané chybě"
 
+#: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
 #: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
 msgid ""
 "'{path}' does not match a common SPDX file pattern. Find the suggested "
 "naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
 "standard-data-format-requirements"
 msgstr ""
 "'{path}' neodpovídá běžnému vzoru souboru SPDX. Navrhované konvence pro "
-"pojmenování najdete zde: https://spdx.github.io/spdx-spec/conformance/#44"
-"-standard-data-format-requirements"
+"pojmenování najdete zde: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
 
 #: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
 msgstr "použití: "
 
 #: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
@@ -866,7 +930,22 @@
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
 msgstr "neplatná volba: %(value)r (vyberte z %(choices)s)"
 
 #: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s: chyba: %(message)s\n"
+
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "konfliktní volitelný řetězec: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "konfliktní volitelný řetězec: %s"
+
+#, fuzzy
+#~ msgid "can't open '%s': %s"
+#~ msgstr "nelze otevřít '{}'"
+
+#~ msgid "could not find supported VCS"
+#~ msgstr "nepodařilo se najít podporovaný VCS"
```

### Comparing `reuse-2.0.0/po/de.po` & `reuse-2.1.0/po/tr.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,187 @@
-# SPDX-FileCopyrightText: 2020 Max Mehl
-# SPDX-FileCopyrightText: 2020 Thomas Doczkal
+# SPDX-FileCopyrightText: 2020 T. E. Kalayci <tekrei@member.fsf.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: FSFE reuse\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-09 13:51+0100\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: 2023-06-21 09:53+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: German <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
-"de/>\n"
-"Language: de\n"
+"Language-Team: Turkish <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"tr/>\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.1\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse ist ein Werkzeug, um die Empfehlungen von REUSE umzusetzen und zu "
-"überprüfen. Mehr Informationen finden Sie auf <https://reuse.software/> oder "
-"in der Online-Dokumentation auf <https://reuse.readthedocs.io/>."
+"reuse, REUSE önerileriyle uyum için bir araçtır. Daha fazla bilgi için "
+"<https://reuse.software/> sitesini, çevrimiçi belgelendirme için <https://"
+"reuse.readthedocs.io/> sitesini ziyaret edebilirsiniz."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
-msgstr ""
-"Diese Version von reuse ist kompatibel mit Version {} der REUSE-"
-"Spezifikation."
+msgstr "Bu reuse sürümü, REUSE Belirtiminin {} sürümüyle uyumludur."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
-msgstr "Die Arbeit der FSFE unterstützen:"
+msgstr "FSFE'nin çalışmalarını destekleyin:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
-"Spenden sind entscheidend für unsere Leistungsfähigkeit und Autonomie. Sie "
-"ermöglichen es uns, weiterhin für Freie Software zu arbeiten, wo immer es "
-"nötig ist. Bitte erwägen Sie eine Spende unter <https://fsfe.org/donate/>."
+"Gücümüz ve özerkliğimiz için bağışlar oldukça önemli. Gereken her yerde "
+"Özgür Yazılım için çalışmamızı sağlıyorlar. Lütfen <https://fsfe.org/donate/"
+"> adresi üzerinden bağış yapmayı değerlendirin."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
-msgstr "Debug-Statements aktivieren"
+msgstr "hata ayıklama cümlelerini etkinleştirir"
+
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
-msgstr "Git-Submodules nicht überspringen"
+msgstr "Git alt modüllerini atlamaz"
+
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "Git alt modüllerini atlamaz"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
-msgstr "kein Multiprocessing verwenden"
+msgstr "çoklu işlem kullanmaz"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
-msgstr "Stammverzeichnis des Projekts bestimmen"
+msgstr "projenin kökünü tanımlar"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
-msgstr "zeige die Versionsnummer des Programms und beende"
+msgstr "programın sürüm numarasını gösterip çıkar"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
-msgstr "Unterkommandos"
+msgstr "alt komutlar"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
-msgstr ""
-"schreibe Urheberrechts- und Lizenzinformationen in die Kopfzeilen von Dateien"
+msgstr "dosya başlıklarına telif hakkı ve lisans bilgilerini ekler"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
-"Schreibe Urheberrechts- und Lizenzinformationen in die Kopfzeilen von einer "
-"oder mehr Dateien.\n"
+"Bir veya daha fazla dosya başlığına telif hakkı ve lisans bilgisini ekle.\n"
 "\n"
-"Mit der Benutzung von --copyright und --license können Sie bestimmen, welche "
-"Urheber und Lizenzen Sie in die Kopfzeilen der jeweiligen Dateien hinzufügen."
+"ilgili dosyaların başlığına hangi telif hakkı sahiplerinin ve lisansların "
+"ekleneceğini --copyright ve --license değişkenlerini kullanarak "
+"belirtebilirsiniz.\n"
 "\n"
+"Yorum biçimi dosyalarınız için otomatik olarak belirlenecektir. Eğer bir "
+"yorum biçimi belirlenemezse, süreç iptal edilecektir. Kullanılacak yorum "
+"biçimini belirtmek için --style değişkenini kullanın.\n"
 "\n"
-"Der Kommentarstil wird normalerweise automatisch erkannt. Wenn das nicht der "
-"Fall ist, endet der Vorgang. Benutzen Sie --style um einen Kommentarstil zu "
-"bestimmen oder zu forcieren.\n"
+"Başlık yorumu şablonunu --template değişkenini kullanarak "
+"değiştirebilirsiniz. Bir Jinja2 şablonunu .reuse/templates/mytemplate.jinja2 "
+"içerisine koyun. Şablonu '--template mytemplate' şeklinde kullanabilirsiniz. "
+"Bu özelliği nasıl kullanabileceğinizi çevrimiçi belgelerden "
+"öğrenebilirsiniz.\n"
 "\n"
-"Sie können die Vorlage für die Kopfzeilen-Kommentare mit --template ändern. "
-"Erstellen Sie dazu eine Jinja2-Vorlage in .reuse/templates/"
-"mytemplate.jinja2. Sie können die Vorlage verwenden mithilfe von '--template "
-"mytemplate'. Mehr Informationen zu dieser Funktion in der Online-"
-"Dokumentation.\n"
+"Eğer ikili bir dosya tespit edilirse veya eğer --explicit-license "
+"tanımlıysa, başlık .license dosyasına koyulacaktır.\n"
 "\n"
-"Wenn eine Binärdatei erkannt wurde, oder wenn --explicit-license verwendet "
-"wurde, werden die Kopfzeilen in einer .license-Datei gespeichert.\n"
-"\n"
-"WICHTIG: Diese Funktion ist momentan EXPERIMENTELL!"
+"ÖNEMLİ: Bu şu anda DENEYSELDİR!"
+
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
-msgstr "lade eine Datei herunter und speichere sie im Verzeichnis LICENSES/"
+msgstr "bir lisans indirir ve LICENSES/ dizinine yerleştirir"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
 "- The current directory if its name is LICENSES.\n"
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
-"Lade eine Datei herunter und speichere sie im Verzeichnis LICENSES/.\n"
+"Bir lisans indirir ve LICENSES/ dizinine yerleştirir.\n"
 "\n"
-"Das LICENSES/-Verzeichnis wird automatisch in dieser Reihenfolge gesucht:\n"
+"LICENSES/ dizini şu sırayla otomatik olarak aranır:\n"
 "\n"
-"- Das LICENSES/-Verzeichnis im Wurzelverzeichnis des VCS-Repositorys.\n"
+"- VCS deposunun kökündeki LICENSES/ dizini\n"
 "\n"
-"- Das aktuelle Verzeichnis wenn dessen Name LICENSES ist.\n"
+"- Eğer ismi LICENSES ise mevcut dizin\n"
 "\n"
-"- Das LICENSES/-Verzeichnis im aktuellen Verzeichnis.\n"
+"- Mevcut dizindeki LICENSES/ dizini\n"
 "\n"
-"Wenn das LICENSES/-Verzeichnis nicht gefunden werden kann, wird einfach "
-"eines erstellt."
+"Eğer LICENSES/ dizini bulunamazsa, yeni bir tane oluşturulur."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
-msgstr "REUSE-Projekt initialisieren"
+msgstr "REUSE projesini ilkler"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
-msgstr "alle nicht-konformen Dateien zeigen"
+msgstr "bütün uyumsuz dosyaları listeler"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -177,634 +193,741 @@
 "the LICENSES/ directory?\n"
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
-"Überprüfen Sie das Projektverzeichnis auf die Einhaltung der Version "
-"{reuse_version} der REUSE-Spezifikation. Die neueste Version der "
-"Spezifikation finden Sie unter <https://reuse.software/spec/>.\n"
+"Proje dizinini REUSE Belirtimi {reuse_version} sürümüyle uyumu için inceler. "
+"Belirtimin son sürümüne <https://reuse.software/spec/> adresinden "
+"erişebilirsiniz.\n"
 "\n"
-"Im Einzelnen werden die folgenden Kriterien geprüft:\n"
+"Özellikle aşağıdaki ölçütler denetleniyor:\n"
 "\n"
-"- Sind im Projekt schlechte (nicht erkannte, nicht SPDX-konforme) Lizenzen "
-"vorhanden?\n"
+"- Projede herhangi bir kötü (tanımlanamayan, SPDX ile uyumsuz) lisans var "
+"mı?\n"
 "\n"
-"- Gibt es Lizenzen, auf die innerhalb des Projekts verwiesen wird, die aber "
-"nicht im Verzeichnis LICENSES/ enthalten sind?\n"
+"- Projede belirtilen ama LICENSES/ dizininde yer almayan lisans var mı?\n"
 "\n"
-"- Sind Lizenzen im Verzeichnis LICENSES/ enthalten, die nicht innerhalb des "
-"Projekts verwendet werden?\n"
+"- LICENSES/ dizininde yer alan ama projede kullanılmayan lisanslar var mı?\n"
 "\n"
-"- Sind alle Dateien mit gültigen Urheberrechts- und Lizenzinformationen "
-"versehen?"
+"- Bütün dosyalar telif hakkı ve lisans bilgisi içeriyor mu?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
-msgstr "Komponentenliste im SPDX-Format ausgeben"
+msgstr "projenin malzeme listesini SPDX biçiminde yazdırır"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
-msgstr "Kann '{expression}' nicht parsen"
+msgstr "'{expression}' çözümlenemiyor"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
-msgstr "'{}' ist keine Datei"
+msgstr "'{}' bir dosya değil"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
-msgstr "'{}' ist kein Verzeichnis"
+msgstr "'{}' bir dizin değil"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
-msgstr "kann '{}' nicht öffnen"
+msgstr "'{}' açılamıyor"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
-msgstr "kann nicht in Verzeichnis '{}' schreiben"
+msgstr "'{}' dizinine yazılamıyor"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
-msgstr "kann nicht in '{}' schreiben"
+msgstr "'{}' yazılamıyor"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
-msgstr "kann '{}' nicht lesen oder schreiben"
+msgstr "'{}' okunamıyor veya yazılamıyor"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
-msgstr "'{}' ist kein gültiger SPDX-Ausdruck, breche ab"
+msgstr "'{}' geçerli bir SPDX ifadesi değil, iptal ediliyor"
+
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' geçerli bir SPDX Lisans Kimliği değil."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Geçerli SPDX Lisans Kimlikleri listesi için <https://spdx.org/licenses/> "
+"adresine bakın."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
-msgstr "SPDX-Lizenz-Identifikator der Lizenz"
+msgstr "Lisansın SPDX Lisans Kimliği"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
-msgstr "lade alle fehlenden Lizenzen herunter, die im Projekt gefunden wurden"
+msgstr "projede tespit edilen bütün eksik lisansları indir"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
-msgstr "Fehler: {spdx_identifier} existiert bereits."
+msgstr "Hata: {spdx_identifier} halihazırda mevcut."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
-msgstr "Fehler: Lizenz konnte nicht heruntergeladen werden."
-
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' ist kein gültiger SPDX-Lizenz-Identifikator."
+msgstr "Hata: lisans indirme başarısız oldu."
 
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Besuchen Sie <https://spdx.org/licenses/> für eine Liste von gültigen SPDX-"
-"Lizenz-Identifikatoren."
-
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
-msgstr "Funktioniert Ihre Internetverbindung?"
+msgstr "İnternet bağlantınız çalışıyor mu?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
-msgstr "{spdx_identifier} erfolgreich heruntergeladen."
+msgstr "{spdx_identifier} başarılı bir şekilde indirildi."
 
-#: src/reuse/download.py:136
-msgid "the following arguments are required: license"
-msgstr "Die folgenden Argumente sind erforderlich: license"
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
 
 #: src/reuse/download.py:138
+msgid "the following arguments are required: license"
+msgstr "şu değişkenler gerekiyor: license"
+
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
-msgstr "Kann --output nicht mit mehr als einer Lizenz verwenden"
+msgstr "--output birden fazla lisansla birlikte kullanılamıyor"
 
-#: src/reuse/header.py:103
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
+msgstr "oluşturulan yorumda telif hakkı satırları veya lisans ifadeleri eksik"
+
+#: src/reuse/header.py:414
+#, python-brace-format
+msgid ""
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
 msgstr ""
-"Dem generierten Kommentar fehlen Zeilen zum Urheberrecht oder Lizenzausdrücke"
 
-#: src/reuse/header.py:293
+#: src/reuse/header.py:421
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
-"explicit-license"
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"'{path}' tanınan bir dosya uzantısına sahip değil, lütfen --style veya --"
+"explicit-license değişkenlerini kullanın"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
 msgstr ""
-"'{path}' hat keine erkannte Dateiendung, bitte verwenden Sie --style oder "
-"--explicit-license"
 
-#: src/reuse/header.py:352
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
-msgstr "Fehler: Kann kein Kommentar für '{path}' erstellen"
+msgstr "Hata: '{path}' için yorum oluşturulamıyor"
 
-#: src/reuse/header.py:359
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
-"Fehler: Die generierten Kommentar-Kopfzeilen für '{path}' enthalten fehlende "
-"Urheberrechtszeilen oder Lizenzausdrücke. Die Vorlage ist wahrscheinlich "
-"falsch. Keine neuen Kopfzeile geschrieben."
+"Hata: '{path}' için üretilen başlık yorumu telif hakkı satırlarını veya "
+"lisans ifadelerini içermiyor. Şablon hatalı olabilir. Yeni başlık yazılmadı."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:370
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
-msgstr "Kopfzeilen von {path} erfolgreich geändert"
+msgstr "{path} başlığı başarılı bir şekilde değiştirildi"
 
-#: src/reuse/header.py:383
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
-msgstr "Urheberrechtsinformation, wiederholbar"
+msgstr "telif hakkı ifadesi, tekrarlanabilir"
 
-#: src/reuse/header.py:390
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
-msgstr "SPDX-Lizenz-Identifikator, wiederholbar"
+msgstr "SPDX Kimliği, tekrarlanabilir"
+
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "SPDX Kimliği, tekrarlanabilir"
 
-#: src/reuse/header.py:397
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
-msgstr "Jahr der Urheberrechtsinformation, optional"
+msgstr "telif hakkı ifadesi, isteğe bağlı"
 
-#: src/reuse/header.py:405
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
-msgstr "zu benutzender Kommentarstil, optional"
+msgstr "kullanılacak yorum biçimi, isteğe bağlı"
 
-#: src/reuse/header.py:412
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "kullanılacak yorum biçimi, isteğe bağlı"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
-msgstr "Name der zu verwendenden Vorlage, optional"
+msgstr "kullanılacak şablon ismi, isteğe bağlı"
 
-#: src/reuse/header.py:417
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
-msgstr "füge kein Jahr in Angabe hinzu"
+msgstr "ifadede yıl içerme"
+
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "telif hakkı ifadesi, isteğe bağlı"
 
-#: src/reuse/header.py:422
-msgid "place header in path.license instead of path"
-msgstr "Speichere Kopfzeilen in path.license anstatt path"
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "kullanılacak yorum biçimi, isteğe bağlı"
 
-#: src/reuse/header.py:430
-msgid "option --copyright or --license is required"
-msgstr "Option --copyright oder --license ist erforderlich"
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "kullanılacak yorum biçimi, isteğe bağlı"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
 
-#: src/reuse/header.py:434
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
+msgstr "--copyright veya --license seçenekleri gereklidir"
+
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
-msgstr "Die Optionen --exclude-year und --year schließen sich gegenseitig aus"
+msgstr "--exclude-year ve --year seçeneklerinden biri olmalıdır"
 
-#: src/reuse/header.py:450
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "--exclude-year ve --year seçeneklerinden biri olmalıdır"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
-msgstr "Vorlage {template} konnte nicht gefunden werden"
+msgstr "{template} şablonu bulunamıyor"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr ""
-"'{path}' ist im Binärformat, benutze daher '{new_path}' für die Kopfzeilen"
+"'{path}' ikili bir dosya, bu nedenle başlık için '{new_path}' kullanılacak"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
-msgstr ""
-"Unter welcher Lizenz steht Ihr Projekt? Geben Sie den SPDX-Lizenz-"
-"Identifikator an."
+msgstr "Projeniz hangi lisansa sahip? SPDX Lisans Kimliğini belirtin."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License "
 "Identifier."
-msgstr ""
-"Unter welcher anderen Lizenz steht Ihr Projekt? Geben Sie den SPDX-Lizenz-"
-"Identifikator an."
+msgstr "Projeniz başka hangi lisanslara sahip? SPDX Lisans Kimliğini belirtin."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
-msgstr "Um keine weiteren Lizenzen hinzuzufügen, drücken Sie ENTER."
+msgstr "Lisans eklemeyi durdurmak için ENTER tuşuna basın."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
-msgstr "Projekt bereits initialisiert"
+msgstr "Proje zaten ilklenmiş"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
-msgstr "Initialisiere Projekt für REUSE."
+msgstr "Proje REUSE için ilkleniyor."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
-msgstr "Was ist der Name des Projekts?"
+msgstr "Projenin ismi nedir?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
-msgstr "Was ist die Internetadresse des Projekts?"
+msgstr "Projenin İnternet adresi nedir?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
-msgstr "Was ist der Name der Betreuenden?"
+msgstr "Bakımcının adı nedir?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
-msgstr "Wie lautet die E-Mail-Adresse der Betreuenden?"
+msgstr "Bakımcının e-posta adresi nedir?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
-msgstr "Alles erledigt! Initialisiere jetzt."
+msgstr "Tümü bitti! Şimdi ilkleniyor."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
-msgstr "Lade {} herunter"
+msgstr "{} indiriliyor"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
-msgstr "{} existiert bereits"
+msgstr "{} zaten mevcut"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
-msgstr "Konnte {} nicht herunterladen"
+msgstr "{} indirilemiyor"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
-msgstr "Erstelle .reuse/dep5"
+msgstr ".reuse/dep5 oluşturuluyor"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
-msgstr "Initialisierung vollständig."
+msgstr "İlkleme tamamlandı."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"Herzlichen Glückwunsch! Ihr Projekt ist konform mit Version {} der REUSE-"
-"Spezifikation :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
 msgstr ""
-"Leider ist Ihr Projekt nicht konform mit Version {} der REUSE-Spezifikation "
-":-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
-msgstr "FALSCHE LIZENZEN"
+msgstr "KÖTÜ LİSANSLAR"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
-msgstr "'{}' gefunden in:"
+msgstr "'{}' şurada mevcut:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
-msgstr "VERALTETE LIZENZEN"
+msgstr "MODASI GEÇMİŞ LİSANSLAR"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
-msgstr "Die folgenden Lizenzen wurden von SPDX als veraltetet gekennzeichnet:"
+msgstr "Şu lisanslar artık SPDX tarafından kullanılmıyor:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
-msgstr "LIZENZEN OHNE DATEIENDUNG"
+msgstr "DOSYA UZANTISI OLMAYAN LİSANSLAR"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
-msgstr "Die folgenden Lizenzen haben keine Dateiendung:"
+msgstr "Şu lisansların dosya uzantısı yok:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
-msgstr "FEHLENDE LIZENZEN"
+msgstr "EKSİK LİSANSLAR"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
-msgstr "NICHT VERWENDETE LIZENZEN"
+msgstr "KULLANILMAYAN LİSANSLAR"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
-msgstr "Die folgenden Lizenzen werden nicht benutzt:"
+msgstr "Şu lisanslar kullanılmıyor:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
-msgstr "LESEFEHLER"
+msgstr "OKUMA HATALARI"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
-msgstr "Unlesbar:"
+msgstr "Okunamıyor:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
-msgstr "FEHLENDE URHEBERRECHTS- UND LIZENZINFORMATIONEN"
+msgstr "EKSİK TELİF HAKKI VE LİSANS BİLGİSİ"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
-msgstr ""
-"Die folgenden Dateien haben keine Urheberrechts- und Lizenzinformationen:"
+msgstr "Şu dosyalarda telif hakkı ve lisans bilgisi yok:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
-msgstr "Die folgenden Dateien haben keine Urheberrechtsinformationen:"
+msgstr "Şu dosyalarda telif hakkı bilgisi yok:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
-msgstr "Die folgenden Dateien haben keine Lizenzinformationen:"
+msgstr "Şu dosyalarda lisans bilgisi yok:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
-msgstr "ZUSAMMENFASSUNG"
+msgstr "ÖZET"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
-msgstr "Falsche Lizenzen:"
+msgstr "Kötü lisanslar:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
-msgstr "Veraltete Lizenzen:"
+msgstr "Modası geçmiş lisanslar:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
-msgstr "Lizenzen ohne Dateiendung:"
+msgstr "Dosya uzantısı olmayan lisanslar:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
-msgstr "Fehlende Lizenzen:"
+msgstr "Eksik lisanslar:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
-msgstr "Unbenutzte Lizenzen:"
+msgstr "Kullanılmayan lisanslar:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
-msgstr "Verwendete Lizenzen:"
+msgstr "Kullanılan lisanslar:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
-msgstr "Lesefehler: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
+msgstr "Okuma hataları: {count}"
+
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
+msgstr "Telif hakkı içeren dosyalar: {count}/{total}"
+
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
+msgstr "Lisans bilgisi içeren dosyalar: {count} / {total}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
-msgstr "Dateien mit Urheberrechtsinformationen: {count} / {total}"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr "Tebrikler! Projeniz REUSE Belirtiminin {} sürümüyle uyumlu :-)"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
-msgstr "Dateien mit Lizenzinformationen: {count} / {total}"
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr "Maalesef, projeniz REUSE Belirtiminin {} sürümüyle uyumlu değil :-("
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "konnte Git nicht finden"
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
-msgstr "'{path}' abgedeckt durch .reuse/dep5"
+msgstr "'{path}' .reuse/dep5 ile kapsanıyor"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
+msgstr "'{path}' çözümlenemeyen bir SPDX ifadesine sahip, dosya atlanıyor"
+
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
 msgstr ""
-"'{path}' trägt einen SPDX-Ausdruck, der nicht geparst werden kann. "
-"Überspringe Datei"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
-msgstr ".reuse/dep5 hat Syntaxfehler"
+msgstr ".reuse/dep5 sözdizim hataları içeriyor"
+
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
-msgstr "erkenne Identifikator von '{path}'"
+msgstr "'{path}' kimliği belirleniyor"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
-msgstr "{path} hat keine Dateiendung"
+msgstr "{path} dosya uzantısına sahip değil"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
-"Konnte SPDX-Lizenz-Identifikator von {path} nicht erkennen, der auf "
-"{identifier} verweist. Stellen Sie sicher, dass die Lizenz in der "
-"Lizenzliste unter <https://spdx.org/licenses/> steht oder mit 'LicenseRef-' "
-"beginnt und eine Dateiendung hat."
+"{path} için, {identifier} olarak çözümlenen SPDX Lisans Kimliği "
+"anlaşılamadı. Lisansın <https://spdx.org/licenses/> listesinde bulunduğundan "
+"veya 'LicenseRef-' ile başladığından ve bir dosya uzantısına sahip "
+"olduğundan emin olun."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
-msgstr ""
-"{identifier} ist der SPDX-Lizenz-Identifikator von {path} und {other_path}"
+msgstr "{identifier} hem {path} hem de {other_path} için SPDX Lisans Kimliği"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
-msgstr "Konnte '{path}' nicht lesen"
+msgstr "'{path}' okunamıyor"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
-msgstr "Unerwarteter Fehler beim Parsen von '{path}' aufgetreten"
+msgstr "'{path}' çözümlenirken beklenmedik bir hata oluştu"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' endet nicht mit .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
-msgstr "Benutzung: "
+msgstr "kullanım: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
-msgstr ".__call__() nicht definiert"
+msgstr ".__call__() tanımlı değil"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
-msgstr "unbekannter Parser %(parser_name)r (Auswahl: %(choices)s)"
+msgstr "bilinmeyen ayrıştıcı %(parser_name)r (choices: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
-msgstr "Argument \"-\" mit Modus %r"
+msgstr "%r kipine sahip \"-\" argümanı"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "Kann '%s' nicht öffnen: %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "'%(filename)s' açılamıyor: %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
-msgstr "Kann Aktionen nicht zusammenführen - zwei Gruppen heißen %r"
+msgstr "eylemler birleştirilemiyor - iki grup %r olarak adlandırılmış"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' ist ein ungültiges Argument für Positionsangaben"
+msgstr "'required' konumsal parametre için hatalı bir değişkendir"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
-msgstr ""
-"Ungültige Option %(option)r: Muss mit einem Buchstaben %(prefix_chars)r "
-"beginnen"
+msgstr "hatalı %(option)r seçeneği: %(prefix_chars)r karakteriye başlamalı"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
-msgstr "dest= ist erforderlich für Optionen wie %r"
+msgstr "%r gibi seçenekler için dest= gerekli"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
-msgstr "Ungültiger Wert für conflict_resolution: %r"
+msgstr "hatalı conflict_resolution değeri: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
-msgstr[0] "Widersprüchliche Option: %s"
-msgstr[1] "Widersprüchliche Optionen: %s"
+msgstr[0] "çelişkili seçenek karakter dizisi: %s"
+msgstr[1] "çelişkili seçenek karakter dizisi: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
-msgstr "Sich gegenseitig ausschließende Argumente müssen optional sein"
+msgstr "ayrık seçenekler isteğe bağlı olmalı"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
-msgstr "Positions-Argumente"
+msgstr "konumsal değişkenler"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
-msgstr "Optionale Argumente"
+msgstr "isteğe bağlı değişkenler"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
-msgstr "zeige diese Hilfsnachricht und beende"
+msgstr "bu yardım mesajını gösterip çık"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
-msgstr "mehrere Subparser-Argumente sind nicht möglich"
+msgstr "birden fazla altayrıştırıcı değişkeni içeremez"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2277
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
-msgstr "unbekannte Argumente: %s"
+msgstr "tanımlanamayan değişkenler: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
-msgstr "nicht erlaubt mit Argument %s"
+msgstr "%s değişkeniyle izin yok"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
-msgstr "explizites Argument %r ignoriert"
+msgstr "açık %r değişkeni yok sayıldı"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
-msgstr "die folgenden Argumente sind erforderlich: %s"
+msgstr "şu değişkenler gereklidir: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
-msgstr "eines der Argumente %s ist erforderlich"
+msgstr "%s değişkenlerinden biri gereklidir"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
-msgstr "erwartete ein Argument"
+msgstr "bir değişken bekleniyor"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
-msgstr "erwartete höchstens ein Argument"
+msgstr "en fazla bir değişken bekleniyor"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
-msgstr "erwartete mindestens ein Argument"
+msgstr "en azından bir değişken bekleniyor"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2098
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
-msgstr[0] "erwartete %s Argument"
-msgstr[1] "erwartete %s Argumente"
+msgstr[0] "%s değişkeni bekleniyor"
+msgstr[1] "%s değişkenleri bekleniyor"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2157
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
-msgstr "mehrdeutige Option: %(option)s könnte %(matches)s bedeuten"
+msgstr "belirsiz seçenek: %(option)s, %(matches)s ile eşleşebilir"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2220
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
-msgstr "unerwarteter Options-String: %s"
+msgstr "beklenmedik seçenek karakter dizisi: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2417
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
-msgstr "%r ist nicht aufrufbar"
+msgstr "%r çağrılabilir değil"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2434
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
-msgstr "ungültiger %(type)s Wert: %(value)r"
+msgstr "hatalı %(type)s değeri: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2445
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
-msgstr "ungültige Auswahl: %(value)r (wähle von %(choices)s)"
+msgstr "hatalı tercih: %(value)r (%(choices)s seçilmelidir)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2521
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
-msgstr "%(prog)s: Fehler: %(message)s\n"
+msgstr "%(prog)s: hata: %(message)s\n"
 
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "Kann '%(filename)s' nicht öffnen: %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "çelişkili seçenek karakter dizisi: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "çelişkili seçenek karakter dizisi: %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "'%s' açılamıyor: %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "başlığı path yerine path.license içerisine koy"
+
+#~ msgid "could not find Git"
+#~ msgstr "Git bulunamadı"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' .spdx ile bitmiyor"
```

### Comparing `reuse-2.0.0/po/eo.po` & `reuse-2.1.0/po/eo.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,110 +2,128 @@
 # SPDX-FileCopyrightText: 2018 Tirifto <tirifto@posteo.cz>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: unnamed project\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-12-20 12:18+0100\n"
-"PO-Revision-Date: 2023-02-16 16:01+0000\n"
-"Last-Translator: Carmen Bianca Bakker <account@carmenbianca.eu>\n"
-"Language-Team: Esperanto <https://hosted.weblate.org/projects/fsfe/"
-"reuse-tool/eo/>\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
+"PO-Revision-Date: 2023-07-10 21:48+0000\n"
+"Last-Translator: Carmen Bianca Bakker <carmen@carmenbianca.eu>\n"
+"Language-Team: Esperanto <https://hosted.weblate.org/projects/fsfe/reuse-"
+"tool/eo/>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 5.0-dev\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse estas ilo por konformiĝo al la rekomendoj de REUSE. Vidu <https://reuse"
-".software/> por pli da informo, kaj <https://reuse.readthedocs.io/> por la "
-"reta dokumentado."
+"reuse estas ilo por konformiĝo al la rekomendoj de REUSE. Vidu <https://"
+"reuse.software/> por pli da informo, kaj <https://reuse.readthedocs.io/> por "
+"la reta dokumentado."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr "Ĉi tiu versio de reuse kongruas al versio {} de la REUSE Specifo."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
 msgstr "Subtenu la laboradon de FSFE:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
 "Donacoj estas gravegaj por niaj forto kaj aŭtonomeco. Ili ebligas nin "
 "daŭrigi laboradon por libera programaro, kie ajn tio necesas. Bonvolu "
 "pripensi fari donacon ĉe <https://fsfe.org/donate/>."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
 msgstr "ŝalti sencimigajn ordonojn"
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr "kaŝi avertojn de evitindaĵoj"
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
 msgstr "ne preterpasi Git-submodulojn"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "ne preterpasi Meson-subprojektojn"
+
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
 msgstr "ne uzi plurprocesorado"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
 msgstr "difini radikon de la projekto"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
 msgstr "montri versionumeron de programo kaj eliri"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr "subkomandoj"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
 msgstr "aldoni kopirajtahn kaj permesilajn informojn en la kapojn de dosieroj"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
 "Aldoni kopirajtahn kaj permesilajn informojn en la kapojn de dosieroj.\n"
 "\n"
 "Tra uzi --copyright kaj --license, vi povas specifi kiujn kopirajtajn "
-"proprulojn kaj permesilojn oni aldonu al la kapojn de la specifitaj dosieroj."
-"\n"
+"proprulojn kaj permesilojn oni aldonu al la kapojn de la specifitaj "
+"dosieroj.\n"
 "\n"
 "Oni aŭtomate eltrovos la komentstilon de viaj dosieroj. Se oni ne povas "
 "eltrovi tion, la procezo haltas. Uzu --style por specifi aŭ superskribi la "
 "uzendan komentstilon.\n"
 "\n"
 "Vi povas ŝanĝi la ŝablonon de la kapo tra uzi --template. Metu Jinja2-"
 "ŝablonon en .reuse/templates/miaŝablono.jinja2. Vi povas uzi la ŝablonon tra "
@@ -113,19 +131,23 @@
 "informoj pri ĉi tiu funkcio.\n"
 "\n"
 "Se oni detektas duuman dosieron, aŭ se vi specifas --explicit-license, la "
 "kapon oni metas en .license-dosieron.\n"
 "\n"
 "GRAVA: Ĉi tio estas ĉimomente PROVCELA!"
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr "evitindigita favore al annotate"
+
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "elŝuti permesilon kaj meti ĝin en la LICENSES/-dosierujon"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
@@ -143,23 +165,23 @@
 "\n"
 "- La aktuala dosierujo se ĝia nomo ests LICENSES.\n"
 "\n"
 "- La LICENSES/-dosierujo sub la aktuala dosierujo.\n"
 "\n"
 "Se oni ne povas trovi la LICENSES/-dosierujon, oni kreos ĝin."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
 msgstr "pravalorizi REUSE-projekton"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
 msgstr "listigi ĉiujn nekonformajn dosierojn"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -172,187 +194,283 @@
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
 "Kontroli la projektdosierujon por konformiĝo je versio {reuse_version} de la "
-"REUSE Specifo. Vi povas trovi la lastan version de la specifo ĉe "
-"<https://reuse.software/spec/>.\n"
+"REUSE Specifo. Vi povas trovi la lastan version de la specifo ĉe <https://"
+"reuse.software/spec/>.\n"
 "\n"
 "Specife, oni kontrolas la sekvajn kriteriojn:\n"
 "\n"
 "- Ĉu estas malbonaj (nekonitaj, nekonformaj) permesiloj en la projekto?\n"
 "\n"
-"- Ĉu uziĝas permesiloj en la projekto, kiuj ne estas en la LICENSES/"
-"-dosierujo?\n"
+"- Ĉu uziĝas permesiloj en la projekto, kiuj ne estas en la LICENSES/-"
+"dosierujo?\n"
 "\n"
 "- Ĉu estas permesiloj en la LICENSES/-dosierujo, kiuj estas neuzataj?\n"
 "\n"
 "- Ĉu ĉiuj dosieroj havas validajn kopirajtajn kaj permesilajn informojn?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
 msgstr "presi la pecoliston de la projekto en SPDX-formo"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr "listigi ĉiujn subtenitajn SPDX-permesilojn"
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
 msgstr "Ne povis analizi '{expression}'"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
 msgstr "'{}' ne estas dosiero"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
 msgstr "'{}' ne estas dosierujo"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
 msgstr "ne povas malfermi '{}'"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
 msgstr "ne povas skribi al dosierujo '{}'"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
 msgstr "ne povas skribi al '{}'"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
 msgstr "ne povas legi aŭ skribi '{}'"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
 msgstr "'{}' ne estas valida SPDX-esprimo. Ĉesigante"
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' ne estas valida SPDX Permesila Identigilo."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr "Ĉu vi intencis:"
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Vidu <https://spdx.org/licenses/> por listo de validaj SPDX Permesilaj "
+"Identigiloj."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
 msgstr "SPDX Permesila Identigilo de permesilo"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
 msgstr "elŝuti ĉiujn mankantajn permesilojn kiujn oni eltrovis en la projekto"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
 msgstr "Eraro: {spdx_identifier} jam ekzistas."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
 msgstr "Eraro: Malsukcesis elŝuti permesilon."
 
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' ne estas valida SPDX Permesila Identigilo."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Vidu <https://spdx.org/licenses/> por listo de validaj SPDX Permesilaj "
-"Identigiloj."
-
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
 msgstr "Ĉu via retkonekto funkcias?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
 msgstr "Sukceses elŝutis {spdx_identifier}."
 
-#: src/reuse/download.py:136
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr "--output faras nenion kiam --all ankaŭ uziĝas"
+
+#: src/reuse/download.py:138
 msgid "the following arguments are required: license"
 msgstr "la sekvaj argumentoj nepras: license"
 
-#: src/reuse/download.py:138
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
 msgstr "ne povas uzi --output kun pli ol unu permesilo"
 
-#: src/reuse/header.py:101
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr "al generita komento mankas kopirajtlinioj aŭ permesilesprimoj"
 
-#: src/reuse/header.py:280
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
-"explicit-license"
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
 msgstr ""
-"'{path}' ne havas konatan dosiersufikson, bonvolu uzi --style aŭ --explicit-"
-"license"
+"'{path}' ne subtenas unuopliniajn komentojn, bonvolu ne uzi --single-line"
 
-#: src/reuse/header.py:339
+#: src/reuse/header.py:421
+#, python-brace-format
+msgid ""
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+"'{path}' ne subtenas plurliniajn komentojn, bonvolu ne uzi --multi-line"
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"La sekvaj dosieroj ne havas konatan dosiersufikson. Bonvolu uzi --style, --"
+"force-dot-license aŭ --skip-unrecognised:"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
+msgstr "Preterpasis nekonatan dosieron {path}"
+
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
+msgstr "Preterpasis dosieron '{path}' kiu jam enhavas REUSE-informojn"
+
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Eraro: Ne povis krei komenton por '{path}'"
 
-#: src/reuse/header.py:346
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
 "Eraro: Al generita komentkapo por '{path}' mankas kopirajtlinioj aŭ "
 "permesilesprimoj. La ŝablono probable malbonas. Ne skribis novan kapon."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:357
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "Sukcese ŝanĝis kapon de {path}"
 
-#: src/reuse/header.py:370
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
 msgstr "kopirajtlinio, ripetabla"
 
-#: src/reuse/header.py:377
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
 msgstr "SPDX Identigilo, ripetabla"
 
-#: src/reuse/header.py:384
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "SPDX Identigilo, ripetabla"
+
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
 msgstr "jaro de kopirajtlinio, malnepra"
 
-#: src/reuse/header.py:392
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
 msgstr "uzenda komentstilo, malnepra"
 
-#: src/reuse/header.py:399
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "uzenda komentstilo, malnepra"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
 msgstr "nomo de uzenda ŝablono, malnepra"
 
-#: src/reuse/header.py:404
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
 msgstr "ne inkluzivi jaron en kopirajtlinio"
 
-#: src/reuse/header.py:409
-msgid "place header in path.license instead of path"
-msgstr "meti kapon en path.license anstataŭ path"
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "jaro de kopirajtlinio, malnepra"
 
-#: src/reuse/header.py:417
-msgid "option --copyright or --license is required"
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "uzenda komentstilo, malnepra"
+
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "uzenda komentstilo, malnepra"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
+
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
 msgstr "opcio --copyright aŭ --license necesas"
 
-#: src/reuse/header.py:421
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
 msgstr "opcio --exclude-year kaj --year ekskluzivas unu la alian"
 
-#: src/reuse/header.py:437
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "opcio --exclude-year kaj --year ekskluzivas unu la alian"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
 msgstr "ŝablono {template} netroveblas"
 
-#: src/reuse/header.py:469
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr "'{path}' estas duuma, tiel uzante '{new_path}' por la kapo"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
@@ -367,466 +485,490 @@
 "Sub kiuj aliaj permesiloj estas via projekto? Provizu la SPDX Permesilan "
 "Identigilon."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
 msgstr "Por ĉesigi aldonadon de permesiloj, premu la enigan klavon."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
 msgstr "Projekto jam pravalorizita"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
 msgstr "Pravalorizante projekton por REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
 msgstr "Kiu estas la nomo de la projekto?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
 msgstr "Kiu estas la reta adreso de la projekto?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
 msgstr "Kiu estas la nomo de la daŭriganto?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
 msgstr "Kiu estas la retpoŝtadreso de la daŭriganto?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
 msgstr "Tute farita! Pravalorizante nun."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
 msgstr "Elŝutante {}"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
 msgstr "{} jam ekzistas"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
 msgstr "Ne povis elŝuti {}"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
 msgstr "Krante .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
 msgstr "Finfaris pravalorizadon."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
-msgstr "Gratulon! Via projekto konformas al versio {} de la REUSE Specifo :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
+msgstr ""
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
 msgstr ""
-"Bedaŭrinde, via projekto ne konformas al versio {} de la REUSE Specifo :-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
+msgstr ""
+
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
 msgstr "MALBONAJ PERMESILOJ"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
 msgstr "'{}' trovita en:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
 msgstr "ARĤAIKIGITAJ PERMESILOJ"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
 msgstr "La sekvajn permesilojn arĥaikigis SPDX:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
 msgstr "PERMESILOJ SEN DOSIERSUFIKSO"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
 msgstr "La sekvaj permesiloj ne havas dosiersufikson:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
 msgstr "MANKANTAJ PERMESILOJ"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
 msgstr "NEUZATAJ PERMESILOJ"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
 msgstr "La sekvajn permesilojn oni ne uzas:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
 msgstr "LEG-ERAROJ"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
 msgstr "Ne povis legi:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "MANKANTAJ KOPIRAJTAJ KAJ PERMESILAJ INFORMOJ"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr "La sekvaj dosieroj ne havas kopirajtajn kaj permesilajn informojn:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
 msgstr "La sekvaj dosieroj ne havas kopirajtajn informojn:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
 msgstr "La sekvaj dosieroj ne havas permesilajn informojn:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
 msgstr "RESUMO"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
 msgstr "Malbonaj permesiloj:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
 msgstr "Arĥaikigitaj permesiloj:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
 msgstr "Permesiloj sen dosiersufikso:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
 msgstr "Mankantaj permesiloj:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
 msgstr "Neuzataj permesiloj:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
 msgstr "Uzataj permesiloj:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
 msgstr "Leg-eraroj: {count}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
 msgstr "Dosieroj sen kopirajtinformo: {count} / {total}"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
 msgstr "Dosieroj sen permesilinformo: {count} / {total}"
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "ne povis trovi programaron Git"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr "Gratulon! Via projekto konformas al versio {} de la REUSE Specifo :-)"
+
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Bedaŭrinde, via projekto ne konformas al versio {} de la REUSE Specifo :-("
+
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
 msgstr "'{path}' sub .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
 "'{path}' entenas SPDX-esprimon, kiun oni ne povas analizi; preterpasante la "
 "dosieron"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 havas sintaksajn erarojn"
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
+
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
 msgstr "precizigante identigilon de '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
 msgstr "{path} ne havas dosiersufikson"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
 "Ne povis precizigi SPDX Permesila Identigilo de {path}, uzante {identifier}. "
 "Certigu ke la permesilo estas en la listo ĉe <https://spdx.org/licenses/> aŭ "
 "ke ĝi komencas per 'LicenseRef-' kaj havas dosiersufikson."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
 "{identifier} estas la SPDX Permesila Identigilo de kaj {path} kaj "
 "{other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr "Ne povis legi '{path}'"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
 msgstr "Okazis neanticipita eraro dum analizado de '{path}'"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' ne finiĝas per .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
 msgstr "uzo: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
 msgstr ".__call__() ne difiniĝas"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
 msgstr "nekonata analizilo %(parser_name)r (elektoj: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
 msgstr "argumento \"-\" kun moduso %r"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "ne povas malfermi '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "ne povas malfermi '%(filename)s': %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
 msgstr "ne povas kunigi agojn - du grupoj nomiĝas %r"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
 msgstr "'required' estas nevalida argumento por poziciaj"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
 "nevalida elektebla ĉeno %(option)r: devas komenciĝi per signo "
 "%(prefix_chars)r"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
 msgstr "dest= nepras por elektebloj kiel %r"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
 msgstr "nevalida valoro de conflict_resolution: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "konfliktanta elektebla ĉeno: %s"
 msgstr[1] "konfliktantaj elekteblaj ĉenoj: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
 msgstr "reciproke ekskluzivaj argumentoj devas esti malnepraj"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
 msgstr "poziciaj argumentoj"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
 msgstr "malnepraj argumentoj"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
 msgstr "montri ĉi tiun helpmesaĝon kaj eliri"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
 msgstr "ne povas havi plurajn subanalizilajn argumentojn"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2276
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
 msgstr "nekonataj argumentoj: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
 msgstr "ne permesita kun argumento: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
 msgstr "malatentis malimplicitan argumenton %r"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
 msgstr "la sekvaj argumentoj nepras: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
 msgstr "unu el la argumentoj %s nepras"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
 msgstr "anticipis unu argumenton"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
 msgstr "anticipis maksimume unu argumenton"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
 msgstr "anticipis minimume unu argumenton"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2096
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "anticipis %s argumenton"
 msgstr[1] "anticipis %s argumentojn"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2156
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "dubsenca elekteblo: %(option)s povus egali al %(matches)s"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2219
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
 msgstr "neanticipita elektebla ĉeno: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2416
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
 msgstr "%r ne alvokeblas"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2433
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
 msgstr "nevalida %(type)s-valoro: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2444
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
 msgstr "nevalida elekto: %(value)r (elektu el %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2520
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s: eraro: %(message)s\n"
 
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "ne povas malfermi '%(filename)s': %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "konfliktanta elektebla ĉeno: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "konfliktanta elektebla ĉeno: %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "ne povas malfermi '%s': %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "meti kapon en path.license anstataŭ path"
+
+#~ msgid "could not find Git"
+#~ msgstr "ne povis trovi programaron Git"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' ne finiĝas per .spdx"
 
-#, python-format
 #~ msgid "yielding %s"
 #~ msgstr "traktante %s"
 
-#, python-format
 #~ msgid "currently walking in %s"
 #~ msgstr "ĉimomente irante en %s"
 
-#, python-format
 #~ msgid "ignoring %s"
 #~ msgstr "ignoras %s"
 
-#, python-format
 #~ msgid "searching %s for reuse information"
 #~ msgstr "serĉanta en %s por reuse-informoj"
 
-#, python-format
 #~ msgid "%s could not be decoded"
 #~ msgstr "ne povis malkodi %s"
 
-#, python-brace-format
 #~ msgid ""
 #~ "{path} is licensed under {identifier}, but its license file could not be "
 #~ "found"
 #~ msgstr "{path} subas permesilon {identifier}, sed ties dosiero mankas"
 
-#, python-format
 #~ msgid "searching %s for license tags"
 #~ msgstr "serĉante permesiletikedojn en %s"
 
-#, python-brace-format
 #~ msgid ""
 #~ "Could not resolve SPDX identifier of {path}, resolving to {identifier}"
 #~ msgstr "Ne povis determini SPD-identigilo de {path}, do uziĝas {identifier}"
 
 #~ msgid "no debian/copyright file, or could not read it"
 #~ msgstr "neniu debian/copyright dosiero, aŭ ne povis legi ĝin"
 
@@ -868,15 +1010,14 @@
 #~ "You do not have pygit2 installed.  reuse will slow down significantly "
 #~ "because of this.  For better performance, please install your "
 #~ "distribution's version of pygit2."
 #~ msgstr ""
 #~ "Vi ne jam instalis pygit2.  reuse malrapidiĝas ege pro ĉi tio.  Por akiri "
 #~ "pli bonan rendimenton, bonvolu instali version de pygit2 de via distribuo."
 
-#, python-format
 #~ msgid "could not read %s"
 #~ msgstr "ne povis legi dosieron %s"
 
 #~ msgid "none\n"
 #~ msgstr "neniu\n"
 
 #~ msgid "do not use debian/copyright to extract reuse information"
```

### Comparing `reuse-2.0.0/po/es.po` & `reuse-2.1.0/po/gl.po`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,187 @@
-# SPDX-FileCopyrightText: 2018 pd <euklade@gmail.com>
-# SPDX-FileCopyrightText: 2018 flow <adolflow@sindominio.net>
-# SPDX-FileCopyrightText: 2020 Roberto Bauglir <bauglir@fsfe.org>
+# SPDX-FileCopyrightText: 2020 pd <eukelade@gmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
-"Project-Id-Version: FSFE reuse\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-09-09 15:07+0100\n"
-"PO-Revision-Date: 2023-02-20 19:38+0000\n"
-"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
-"Language-Team: Spanish <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
-"es/>\n"
-"Language: es\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
+"PO-Revision-Date: 2023-06-21 09:53+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Galician <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"gl/>\n"
+"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.1\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse es una herramienta para cumplir con las recomendaciones de la "
-"iniciativa REUSE. Visita <https://reuse.software/> para obtener más "
-"información, y <https://reuse.readthedocs.io/> para acceder a la "
-"documentación en línea."
+"reuse é unha ferramenta para o cumprimento das recomendacións REUSE. Ver "
+"<https://reuse.software/> para máis información e <https://reuse.readthedocs."
+"io/> para a documentación en liña."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr ""
-"Esta versión de reuse es compatible con la versión {} de la Especificación "
-"REUSE."
+"Esta versión de reuse é compatible coa versión {} da especificación REUSE."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
-msgstr "Apoya el trabajo de la FSFE:"
+msgstr "Apoie o traballo da FSFE:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
-"Las donaciones son esenciales para nuestra fortaleza y autonomía. Estas nos "
-"permiten continuar trabajando por el Software Libre allá donde sea "
-"necesario. Por favor, considera el hacer una donación en <https://fsfe.org/"
-"donate/>."
+"As doazóns son críticas para a nosa forza e autonomía. Permítennos seguir "
+"traballando polo software libre onde sexa necesario. Considere facer unha "
+"doazón a <https://fsfe.org/donate/> ."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
-msgstr "habilita instrucciones de depuración"
+msgstr "habilitar sentencias de depuración"
+
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
-msgstr "no omitas los submódulos de Git"
+msgstr "non salte os submódulos de Git"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "non salte os submódulos de Git"
+
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
-msgstr "no utilices multiproceso"
+msgstr "non empregue multiprocesamento"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
-msgstr "define el origen del proyecto"
+msgstr "definir a raíz do proxecto"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
-msgstr "muestra la versión del programa y sale"
+msgstr "mostrar o número de versión do programa e saír"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr "subcomandos"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
-msgstr "agrega el copyright y la licencia a la cabecera de los ficheros"
+msgstr "engadir copyright e licenza na cabeceira dos arquivos"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
-"Añade copyright y licencias en la cabecera de uno o más archivos.\n"
+"Engadir copyright e información da licenza na cabeceira de un ou varios "
+"arquivos\n"
 "\n"
-"Usando --copyright y --license, puede especificar qué titulares de derechos "
-"de autor y licencias añadir a las cabeceras de los archivos dados.\n"
+"Pódese especificar mediante --license e --copyright a licenza e os donos do "
+"copyright a engadir nas cabeceiras dos arquivos indicados.\n"
 "\n"
-"El estilo de comentario debería detectarse automáticamente para sus "
-"archivos. Si no se puede detectar un estilo de comentario, el proceso se "
-"aborta. Utilice --style para especificar o anular el estilo de comentario a "
-"utilizar.\n"
+"O estilo dos comentarios dos arquivos debería detectarse automáticamente, de "
+"non se detectar o proceso abórtase. Pódese usar --style para definir ou "
+"forzar o estilo de comentario a usar.\n"
 "\n"
-"Puede cambiar la plantilla del comentario de cabecera usando --template. "
-"Coloque una plantilla Jinja2 en .reuse/templates/mytemplate.jinja2. Puedes "
-"usar la plantilla especificando '--template mytemplate'. Lea la información "
-"en internet sobre cómo utilizar esta función.\n"
+"É posible cambiar o modelo do comentario de cabeceira usando --template. Por "
+"exemplo, gardando o modelo Jinja2 na carpeta .reuse/templates/mytemplate."
+"jinja2 pode usar este modelo indicando  '--template mytemplate'. Consulte a "
+"documentación en liña para máis información sobre esta característica.\n"
 "\n"
-"Si se detecta un archivo binario, o si se especifica --explicit-license, la "
-"cabecera se coloca en un archivo .license.\n"
+"Se o arquivo é binario ou se especifica --explicit-license, a cabeceira "
+"gárdase nun arquivo .license.\n"
 "\n"
-"IMPORTANTE: ¡Esto está actualmente disponible de forma EXPERIMENTAL!"
+"IMPORTANTE: Actualmente isto é EXPERIMENTAL!"
+
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
-msgstr "descarga una licencia y guárdala en el directorio \"LICENSES/\""
+msgstr "Descargar unha licenza e gardala na carpeta LICENSES/"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
 "- The current directory if its name is LICENSES.\n"
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
-"Descarga una licencia y guárdala en el directorio LICENSES/.\n"
+"Descargar unha licenza e gardala na carpeta LICENSES/.\n"
 "\n"
-"El directorio LICENSES/ es automáticamente detectado en el siguiente orden:\n"
+"A carpeta LICENSES/ procurase neste orde:\n"
 "\n"
-"- El directorio LICENSES/ en la raíz del repositorio VCS.\n"
+"- a carpeta LICENSES/ na raíz do repositorio VCS.\n"
 "\n"
-"- El directorio actual, si su nombre es LICENSES.\n"
+"- a carpeta actual se o seu nome é LICENSES.\n"
 "\n"
-"- El directorio LICENSES/ en el directorio actual.\n"
+"- a carpeta LICENSES/  no directorio actual.\n"
 "\n"
-"Si el directorio LICENSES/ no fuese encontrado, simplemente se creará uno."
+"Se non se atopa a carpeta LICENSES/ créase unha."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
-msgstr "inicia el proyecto REUSE"
+msgstr "iniciar un proxecto REUSE"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
-msgstr "lista todos los ficheros no compatibles"
+msgstr "listar todos os arquivos que non cumplen os criterios"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -176,768 +193,758 @@
 "the LICENSES/ directory?\n"
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
-"Examina el directorio del proyecto para comprobar su conformidad con la "
-"versión {reuse_version} de la Especificación REUSE. Puedes encontrar la "
-"última versión de la especificación en <https://reuse.software/spec/>\n"
+"Verificar que a carpeta do proxecto cumple coa versión {reuse_version} da "
+"especificación REUSE. Pode atopar a última versión da especificación en "
+"<https://reuse.software/spec/>.\n"
 "\n"
-"Los siguientes criterios son específicamente chequeados:\n"
+"Comprobase específicamente os seguintes criterios:\n"
 "\n"
-"- ¿Hay alguna licencia mala (no reconocida, no compatible con SPDX...) en el "
-"proyecto?\n"
+"- Existen licenzas inapropiadas (non recoñecidas ou que incumplen o SPDX) no "
+"proxecto?\n"
 "\n"
-"- ¿Se hace referencia a alguna licencia dentro del proyecto, pero esta no se "
-"encuentra incluida en el directorio LICENSES/?\n"
+"- Hai algunha licenza mencionada no proxecto que non está incluida na "
+"carpeta LICENSES/?\n"
 "\n"
-"- ¿Existe alguna licencia, de las incluidas en el directorio LICENSES/, que "
-"no esté en uso en el proyecto?\n"
+"- A carpeta LICENSES/ contén licenzas non usadas no proxecto?\n"
 "\n"
-"- ¿Tienen todos los ficheros información válida sobre copyright y licencia?"
+"- Todos os arquivos teñen información correcta de copyright e licenza?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
-msgstr "imprime la lista de materiales del proyecto en formato SPDX"
+msgstr "imprimir a lista de materiales do proxecto en formato SPDX"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
-msgstr "No se pudo procesar '{expression}'"
+msgstr "Non se pode analizar '{expression}'"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
-msgstr "'{}' no es un fichero"
+msgstr "'{}' non é un arquivo"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
-msgstr "'{}' no es un directorio"
+msgstr "'{}' non é un directorio"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
-msgstr "no se puede abrir '{}'"
+msgstr "non se pode abrir '{}'"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
-msgstr "no se pude escribir en el directorio '{}'"
+msgstr "non se pode escribir no directorio '{}'"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
-msgstr "no se puede escribir en '{}'"
+msgstr "non se pode escribir en '{}'"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
-msgstr "no se puede leer o escribir '{}'"
+msgstr "non se pode ler ou escribir en '{}'"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
-msgstr "'{}' no es una expresión SPDX válida; abortando"
+msgstr "'{}' non é unha expresión SPDX válida, cancelando"
+
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' non é un Identificador de Licenza SPDX válido."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Consulte unha lista de Identificadores de Licenza SPDX válidos en <https://"
+"spdx.org/licenses/>."
 
-#: src/reuse/download.py:80
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
-msgstr "Identificador SPDX de la licencia"
+msgstr "Identificador de Licenza SPDX da licenza"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
-msgstr "descargar todas las licencias no disponibles detectadas en el proyecto"
+msgstr "descargar todas as licenzas detectadas mais non atopadas no proxecto"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
-msgstr "Error: {spdx_identifier} ya existe."
+msgstr "Erro: {spdx_identifier} xa existe."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
-msgstr "Error: Fallo al descargar la licencia."
-
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' no es un Identificador SPDX de Licencia válido."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Consulta <https://spdx.org/licenses/> para obtener un listado de los "
-"Identificadores SPDX de Licencia válidos."
+msgstr "Erro: Fallo descargando a licenza."
 
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
-msgstr "¿Está funcionando tu conexión a Internet?"
+msgstr "Está a funcionar a súa conexión a internet?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
-msgstr "{spdx_identifier} descargado con éxito."
+msgstr "Descargouse correctamente o {spdx_identifier}."
 
-#: src/reuse/download.py:136
-msgid "the following arguments are required: license"
-msgstr "se requieren los siguientes parámetros: license"
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
 
 #: src/reuse/download.py:138
+msgid "the following arguments are required: license"
+msgstr "requirense os seguintes argumentos: licenza"
+
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
-msgstr "no se puede utilizar --output con más de una licencia"
+msgstr "non se pode usar --output con máis dunha licenza"
 
-#: src/reuse/header.py:103
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
-"el comentario generado carece del mensaje de copyright o de las frases de "
-"licencia"
+"o comentario xerado non ten liñas de copyright ou expresións de licenza"
 
-#: src/reuse/header.py:293
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
-"explicit-license"
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
 msgstr ""
-"'{path}' carece de una extensión de fichero conocida: por favor, utiliza --"
-"style o --explicit-license"
 
-#: src/reuse/header.py:352
+#: src/reuse/header.py:421
+#, python-brace-format
+msgid ""
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"'{path}' non ten unha extensión de arquivo recoñecida, precisa usar --style "
+"ou --explicit-license"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
+msgstr ""
+
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
-msgstr "Error: No se pudo crear un comentario para '{path}'"
+msgstr "Erro: Non se pode crear un comentario para '{path}'"
 
-#: src/reuse/header.py:359
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
-"Error: La cabecera de comentario generada para '{path}' carece del mensaje "
-"de copyright o de las frases de licencia; la plantilla seguramente es "
-"incorrecta. No se ha escrito una nueva cabecera."
+"Erro: A cabeceira comentada xerada para '{path}' non contén liñas de "
+"copyright ou expresións de licenza. Posibelmente o modelo é incorrecto. Non "
+"se escribiu unha nova cabecereira."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:370
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
-msgstr "Cabecera de {path} correctamente cambiada"
+msgstr "A cabeceira de {path} cambiada con éxito"
 
-#: src/reuse/header.py:383
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
-msgstr "declaración de los derechos de autor, repetible"
+msgstr "declaración de copyright, repetibel"
 
-#: src/reuse/header.py:390
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
-msgstr "Identificador SPDX, repetible"
+msgstr "Identificador SPDX, repetibel"
 
-#: src/reuse/header.py:397
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "Identificador SPDX, repetibel"
+
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
-msgstr "año de la declaración de copyright; opcional"
+msgstr "ano da declaración de copyright, opcional"
 
-#: src/reuse/header.py:405
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
-msgstr "estilo de comentario a utilizar; opcional"
+msgstr "estilo de comentario a usar, opcional"
+
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "estilo de comentario a usar, opcional"
 
-#: src/reuse/header.py:412
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
-msgstr "nombre de la plantilla a utilizar; opcional"
+msgstr "nome do modelo a usar, opcional"
 
-#: src/reuse/header.py:417
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
-msgstr "no incluir el año en la declaración"
+msgstr "non incluir ano na declaración"
+
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "ano da declaración de copyright, opcional"
+
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "estilo de comentario a usar, opcional"
+
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "estilo de comentario a usar, opcional"
 
-#: src/reuse/header.py:422
-msgid "place header in path.license instead of path"
-msgstr "coloca la cabecera en path.license, en lugar de path"
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
+
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
 
-#: src/reuse/header.py:430
-msgid "option --copyright or --license is required"
-msgstr "una de estas opciones es necesaria: --copyright o --license"
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
 
-#: src/reuse/header.py:434
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
+msgstr "precisase a opción --copyright ou --license"
+
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
-msgstr "las opciones -exclude-year y --year son mutuamente excluyentes"
+msgstr "as opcións --exclude-year e --year non se poden usar á vez"
 
-#: src/reuse/header.py:450
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "as opcións --exclude-year e --year non se poden usar á vez"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
-msgstr "no pudo encontrarse la plantilla {template}"
+msgstr "no se atopa o modelo {template}"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
-msgstr ""
-"'{path}' es un fichero binario: en consecuencia, se utiliza '{new_path}' "
-"para la cabecera"
+msgstr "'{path}' é binario, logo úsase '{new_path}' para a cabeceira"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
-"¿Bajo qué licencia se encuentra tu proyecto? Aporta el Identificador SPDX de "
-"Licencia."
+"Baixo que licenza está o seu proxecto? indique o Identificador de Licenza "
+"SPDX."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License "
 "Identifier."
 msgstr ""
-"¿Bajo qué otras licencias se encuentra tu proyecto? Proporciona el "
-"Identificador SPDX de Licencia."
+"Baixo que outra licenza está o seu proxecto? indique o Identificador de "
+"Licenza SPDX."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
-msgstr "Para terminar de añadir licencias pulsa RETORNO."
+msgstr "Para rematar de engadir licenzas, prema ENTER."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
-msgstr "Proyecto ya inicializado"
+msgstr "O proxecto xa está iniciado"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
-msgstr "Inicializando el proyecto para REUSE."
+msgstr "Iniciando o proxecto para REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
-msgstr "¿Cuál es el nombre del proyecto?"
+msgstr "Cal é o nome do proxecto?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
-msgstr "¿Cuál es la dirección de Internet del proyecto?"
+msgstr "Cal é o enderezo en internet do proxecto?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
-msgstr "¿Cuál es el nombre del mantenedor?"
+msgstr "Cal é o nome do mantenedor?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
-msgstr "¿Cuál es la dirección de correo electrónico del mantenedor?"
+msgstr "Cal é o correo electrónico do mantenedor?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
-msgstr "¡Ya hemos terminado! Iniciando."
+msgstr "Rematou todo! iniciando arestora."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
 msgstr "Descargando {}"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
-msgstr "{} ya existe"
+msgstr "{} xa existe"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
-msgstr "No se pudo descargar {}"
+msgstr "Non se pode descargar {}"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
 msgstr "Creando .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
-msgstr "Inicialización completa."
+msgstr "Inicialización completada."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"¡Enhorabuena! Tu proyecto es compatible con la versión {} de la "
-"Especificación REUSE :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
 msgstr ""
-"Desafortunadamente, tu proyecto no es compatible con la versión {} de la "
-"Especificación REUSE :-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
-msgstr "LICENCIAS MALAS"
+msgstr "LICENZAS DEFECTUOSAS"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
-msgstr "'{}' encontrado en:"
+msgstr "'{}' atopado en:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
-msgstr "LICENCIAS OBSOLETAS"
+msgstr "LICENZAS OBSOLETAS"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
-msgstr "Las siguientes licencias han quedado obsoletas según SPDX:"
+msgstr "As seguintes licenzas son obsoletas para SPDX:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
-msgstr "LICENCIAS SIN EXTENSIÓN DE FICHERO"
+msgstr "LICENZAS SEN EXTENSIÓN DE ARQUIVO"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
-msgstr "Las siguientes licencias no tienen extensión de fichero:"
+msgstr "As seguintes licenzas non teñen extesión de arquivo:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
-msgstr "LICENCIAS NO ENCONTRADAS"
+msgstr "LICENZAS NON ATOPADAS"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
-msgstr "LICENCIAS NO UTILIZADAS"
+msgstr "LICENZAS SEN USO"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
-msgstr "Las siguientes licencias no son utilizadas:"
+msgstr "As seguintes licenzas non se usan:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
-msgstr "ERRORES DE LECTURA"
+msgstr "ERROS DE LECTURA"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
-msgstr "No se pudo leer:"
+msgstr "Non se pode ler:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
-msgstr "FALTA INFORMACIÓN SOBRE COPYRIGHT Y LICENCIA"
+msgstr "NON SE ATOPA INFORMACIÓN DE LICENZA OU COPYRIGHT"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
-msgstr "Los siguientes archivos carecen de información de copyright y licencia:"
+msgstr ""
+"Os seguintes arquivos non teñen información de licenza nen de copyright:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
-msgstr "Los siguientes ficheros carecen de información de copyright:"
+msgstr "Os seguintes arquivos non teñen información de copyright:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
-msgstr "Los siguientes ficheros carecen de información de licencia:"
+msgstr "Os seguintes arquivos non teñen información de licenza:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
-msgstr "RESUMEN"
+msgstr "RESUMO"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
-msgstr "Licencias malas:"
+msgstr "Licenzas defectuosas:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
-msgstr "Licencias obsoletas:"
+msgstr "Licenzas obsoletas:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
-msgstr "Licencias sin extensión de fichero:"
+msgstr "Licenzas sen extensión de arquivo:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
-msgstr "Licencias no encontradas:"
+msgstr "Licenzas non atopadas:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
-msgstr "Licencias no utilizadas:"
+msgstr "Licenzas non usadas:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
-msgstr "Licencias utilizadas:"
+msgstr "Licenzas usadas:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
-msgstr "Errores de lectura: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
+msgstr "Erros de lectura: {count}"
+
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
+msgstr "Arquivos con información de copyright: {count} / {total}"
+
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
+msgstr "Arquivos con información de licenza: {count} / {total}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
-msgstr "Ficheros con información sobre copyright: {count} / {total}"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr ""
+"Congratulacións! O seu proxecto cumple coa versión {} da especificación "
+"REUSE :-)"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
-msgstr "Ficheros con información de licencia: {count} / {total}"
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Desgraciadamente o seu proxecto non cumple coa versión {} da especificación "
+"REUSE :-("
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "no se pudo encontrar Git"
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
-msgstr "'{path}' cubierto por .reuse/dep5"
+msgstr "'{path}' cuberto por .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
-"'{path}' posee una expresión SPDX que no puede ser procesada; omitiendo el "
-"archivo"
+"'{path}' inclúe unha expresión SPDX que non se pode analizar, saltando o "
+"arquivo"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
-msgstr ".reuse/dep5 presenta errores de sintaxis"
+msgstr ".reuse/dep5 ten erros de sintaxe"
+
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
-msgstr "determinando el identificador de '{path}'"
+msgstr "resolvendo o identificador de '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
-msgstr "{path} no tiene extensión de fichero"
+msgstr "{path} non ten extensión de arquivo"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
-"No pudo detectarse el Identificador SPDX de Licencia de {path}: detectando "
-"{identifier}. Asegúrate de que la licencia consta en la lista de licencias "
-"alojada en <https://spdx.org/licenses/>, o de que empieza por 'LicenseRef-', "
-"y de que posee una extensión de fichero."
+"Non se pode resolver o Identificador de Licenza SPDX de {path}, resólvese "
+"como {identifier}. Asegúrese que a licenza está na lista publicada en "
+"<https://spdx.org/licenses/> ou que comeza con 'LicenseRef-' e ten unha "
+"extensión de arquivo."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
-"{identifier} es el Identificador SPDX de Licencia, tanto de {path}, como de "
+"{identifier} é o Identificador de Licenza SPDX de ambos os dous {path} e "
 "{other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
-msgstr "No se pudo leer '{path}'"
+msgstr "Non se pode ler '{path}'"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
-msgstr "Se produjo un error inesperado al procesar '{path}'"
+msgstr "Aconteceu un erro inesperado lendo '{path}'"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' no acaba en .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
 msgstr "uso: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
-msgstr ".__call__() no definido"
+msgstr ".__call__() non definido"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
-msgstr ""
-"analizador sintáctico desconocido: %(parser_name)r (alternativas: "
-"%(choices)s)"
+msgstr "analizador descoñecido %(parser_name)r (alternativas: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
-msgstr "parámetro \"-\" con modo %r"
+msgstr "argumento \"-\" con modo %r"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "no se puede abrir '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "non se pode abrir '%(filename)s': %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
-msgstr "no se pueden fusionar las acciones: dos grupos se llaman %r"
+msgstr "non se poden misturar as accións - dous grupos teñen o nome %r"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' es un argumento posicional inválido"
+msgstr "'required' non é un argumento valido para os posicionais"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
-"Opción no válida %(option)r: Debe comenzar con una letra %(prefix_chars)r"
+"cadea de opción non válida %(option)r: precisa comenzar cun carácter "
+"%(prefix_chars)r"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
-msgstr "se requiere dest= para opciones como %r"
+msgstr "requírese dest= para opcións do tipo %r"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
-msgstr "valor no válido de conflict_resolution: %r"
+msgstr "valor non válido para conflict_resolution: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
-msgstr[0] "cadena de opción conflictiva: %s"
-msgstr[1] "cadenas de opción conflictivas: %s"
+msgstr[0] "cadea de opción conflictiva: %s"
+msgstr[1] "cadeas de opción conflictivas: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
-msgstr "los parámetros mutuamente excluyentes deben ser opcionales"
+msgstr "os argumentos mutuamente exclusivos deben ser opcionais"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
-msgstr "parámetros posicionales"
+msgstr "argumentos posicionais"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
-msgstr "parámetros opcionales"
+msgstr "argumentos opcionais"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
-msgstr "mostrar este mensaje de ayuda y salir"
+msgstr "mostrar esta mensaxe de axuda e sair"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
-msgstr "no puede contener múltiples parámetros del subanalizador sintáctico"
+msgstr "non pode haber múltiples argumentos para o subanalizador"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2277
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
-msgstr "parámetros no reconocidos: %s"
+msgstr "argumentos non recoñecidos: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
-msgstr "no permitido con el parámetro %s"
+msgstr "non se permite co argumento %s"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
-msgstr "parámetro explícito ignorado: %r"
+msgstr "argumento explicito %r ignorado"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
-msgstr "los siguientes parámetros son obligatorios: %s"
+msgstr "precísanse os seguintes argumentos: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
-msgstr "se requiere uno de los parámetros %s"
+msgstr "precísase un dos argumentos %s"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
-msgstr "se espera un parámetro"
+msgstr "espérase un argumento"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
-msgstr "se espera un parámetro, como máximo"
+msgstr "espérase un argumento como máximo"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
-msgstr "se espera un parámetro, como mínimo"
+msgstr "espérase un argumento como mínimo"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2098
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
-msgstr[0] "se espera el parámetro %s"
-msgstr[1] "se esperan los parámetros %s"
+msgstr[0] "espérase %s argumento"
+msgstr[1] "espéranse %s argumentos"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2157
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
-msgstr "opción ambigua: %(option)s podría coincidir con %(matches)s"
+msgstr "opción ambigua: %(option)s pode encaixar con %(matches)s"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2220
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
-msgstr "cadena de opción inesperada: %s"
+msgstr "opción de cadea non esperada: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2417
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
-msgstr "%r no se puede invocar"
+msgstr "%r non se pode chamar"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2434
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
-msgstr "valor no válido de %(type)s: %(value)r"
+msgstr "valor non válido %(type)s: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2445
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
-msgstr "opción inválida: %(value)r (opciones: %(choices)s)"
+msgstr "alternativa non válida: %(value)r (elixir entre %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2521
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
-msgstr "%(prog)s: error: %(message)s\n"
-
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "no se puede abrir '%(filename)s': %(error)s"
+msgstr "%(prog)s: erro: %(message)s\n"
 
-#~ msgid "yielding %s"
-#~ msgstr "apuntando a %s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "cadea de opción conflictiva: %s"
 
-#~ msgid "currently walking in %s"
-#~ msgstr "actualmente recorriendo %s"
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "cadea de opción conflictiva: %s"
 
-#~ msgid "ignoring %s"
-#~ msgstr "ignorando %s"
-
-#~ msgid "searching %s for reuse information"
-#~ msgstr "buscando información de reuse en %s"
-
-#~ msgid "%s could not be decoded"
-#~ msgstr "%s no se pudo decodificar"
-
-#~ msgid "%s covered by debian/copyright"
-#~ msgstr "%s cubierto por debian/copyright"
-
-#~ msgid ""
-#~ "{path} is licensed under {identifier}, but its license file could not be "
-#~ "found"
-#~ msgstr ""
-#~ "{path} con licencia {identifier}, pero no se encontró el archivo con la "
-#~ "licencia"
-
-#~ msgid "searching %s for license tags"
-#~ msgstr "buscando etiquetas de licencia en %s"
-
-#~ msgid ""
-#~ "Could not resolve SPDX identifier of {path}, resolving to {identifier}"
-#~ msgstr ""
-#~ "No se pudo resolver el identificador SPDX de {path}, resolviendo a "
-#~ "{identifier}"
-
-#~ msgid "no debian/copyright file, or could not read it"
-#~ msgstr "no existe o no se pudo leer el archivo debian/copyright"
-
-#~ msgid "reuse  Copyright (C) 2017-2018  Free Software Foundation Europe e.V."
-#~ msgstr ""
-#~ "Copyright (C) 2017-2018 de reuse Free Software Foundation Europe e.V."
-
-#~ msgid ""
-#~ "reuse is free software: you can redistribute it and/or modify it under "
-#~ "the terms of the GNU General Public License as published by the Free "
-#~ "Software Foundation, either version 3 of the License, or (at your option) "
-#~ "any later version.\n"
-#~ "\n"
-#~ "reuse is distributed in the hope that it will be useful, but WITHOUT ANY "
-#~ "WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS "
-#~ "FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more "
-#~ "details.\n"
-#~ "\n"
-#~ "You should have received a copy of the GNU General Public License along "
-#~ "with reuse.  If not, see <http://www.gnu.org/licenses/>."
-#~ msgstr ""
-#~ "reuse es software libre: puedes redistribuirlo y/o modificarlo bajo los "
-#~ "términos de la Licencia Pública General GNU (GNU GPL) tal y como está "
-#~ "publicada por la Free Software Foundation, tanto la versión 3 de la "
-#~ "Licencia, o (a tu elección) cualquier versión posterior.\n"
-#~ "\n"
-#~ "reuse se distribuye con la esperanza de ser útil, pero SIN NINGUNA "
-#~ "GARANTIA; ni siquiera la garantia implícita de COMERCIABILIDAD o "
-#~ "ADECUACIÓN PARA UN PROPÓSITO PARTICULAR. Consulta la Licencia Pública "
-#~ "General GNU para más detalles.\n"
-#~ "\n"
-#~ "Deberías haber recibido una copia de la Licencia Pública General GNU con "
-#~ "reuse. Si no es así, consulta <http://www.gnu.org/licenses/>."
-
-#~ msgid "IMPORTANT:"
-#~ msgstr "IMPORTANTE:"
-
-#~ msgid ""
-#~ "You do not have pygit2 installed.  reuse will slow down significantly "
-#~ "because of this.  For better performance, please install your "
-#~ "distribution's version of pygit2."
-#~ msgstr ""
-#~ "No tienes instalado pygit2 por lo que reuse funcionará significativamente "
-#~ "más lento. Por favor, instala la versión de pygit2 de tu distribución "
-#~ "para un mejor rendimiento."
-
-#~ msgid "could not read %s"
-#~ msgstr "no se pudo leer %s"
-
-#~ msgid "none\n"
-#~ msgstr "nada\n"
-
-#~ msgid "do not use debian/copyright to extract reuse information"
-#~ msgstr "no use debian/copyright para extraer información de reuse"
-
-#~ msgid ""
-#~ "List all non-compliant files.\n"
-#~ "\n"
-#~ "A file is non-compliant when:\n"
-#~ "\n"
-#~ "- It has no copyright information.\n"
-#~ "\n"
-#~ "- It has no license (declared as SPDX expression).\n"
-#~ "\n"
-#~ "- Its license could not be found.\n"
-#~ "\n"
-#~ "This prints only the paths of the files that do not comply, each file on "
-#~ "a separate line.\n"
-#~ "\n"
-#~ "Error and warning messages are output to STDERR."
-#~ msgstr ""
-#~ "Lista todos los ficheros no compatibles.\n"
-#~ "\n"
-#~ "Un fichero es no compatible si:\n"
-#~ "\n"
-#~ "- no tiene información de copyright.\n"
-#~ "\n"
-#~ "- no tiene licencia (declarada como una expresión SPDX).\n"
-#~ "\n"
-#~ "- su licencia no se encuentra.\n"
-#~ "\n"
-#~ "Esto imprime únicamente las rutas de los ficheros no compatibles, cada "
-#~ "fichero en una línea separada.\n"
-#~ "\n"
-#~ "Los mensajes de error y aviso se muestran en STDERR."
-
-#~ msgid "SPDX expressions are mandatory for compliance"
-#~ msgstr "Las expresiones SPDX son de obligatorio cumplimiento"
+#~ msgid "can't open '%s': %s"
+#~ msgstr "non se pode abrir '%s': %s"
 
-#~ msgid "copyright notices are mandatory for compliance"
-#~ msgstr "las notas de copyright son de obligatorio cumplimiento"
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "colocar a cabeceira en carpeta.licenza no canto de carpeta"
 
-#~ msgid "print the SPDX expressions of each provided file"
-#~ msgstr "imprime las expresiones SPDX de cada fichero proporcionado"
+#~ msgid "could not find Git"
+#~ msgstr "non se pode atopar o Git"
 
-#~ msgid "reuse, version {}\n"
-#~ msgstr "reuse, versión {}\n"
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' non remata en .spdx"
```

### Comparing `reuse-2.0.0/po/fr.po` & `reuse-2.1.0/po/fr.po`

 * *Files 15% similar despite different names*

```diff
@@ -2,107 +2,126 @@
 # SPDX-FileCopyrightText: 2020 Vincent Lequertier <vincent@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-15 20:23+0100\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: 2023-02-18 10:24+0000\n"
 "Last-Translator: \"J. Lavoie\" <j.lavoie@net-c.ca>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
 "fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.16-dev\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
-"reuse is a tool for compliance with the REUSE recommendations. See <https://reuse."
-"software/> for more information, and <https://reuse.readthedocs.io/> for the "
-"online documentation."
+"reuse is a tool for compliance with the REUSE recommendations. See <https://"
+"reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
+"for the online documentation."
 msgstr ""
 "reuse est un outil pour la conformité aux recommandations de l'initiative "
-"REUSE. Voir <https://reuse.software/> pour plus d'informations, et "
-"<https://reuse.readthedocs.io/> pour la documentation en ligne."
+"REUSE. Voir <https://reuse.software/> pour plus d'informations, et <https://"
+"reuse.readthedocs.io/> pour la documentation en ligne."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
-"This version of reuse is compatible with version {} of the REUSE Specification."
+"This version of reuse is compatible with version {} of the REUSE "
+"Specification."
 msgstr ""
 "Cette version de reuse est compatible avec la version {} de la spécification "
 "REUSE."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
 msgstr "Soutenir le travail de la FSFE :"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
-"Donations are critical to our strength and autonomy. They enable us to continue "
-"working for Free Software wherever necessary. Please consider making a donation "
-"at <https://fsfe.org/donate/>."
+"Donations are critical to our strength and autonomy. They enable us to "
+"continue working for Free Software wherever necessary. Please consider "
+"making a donation at <https://fsfe.org/donate/>."
 msgstr ""
 "Les dons sont cruciaux pour notre force et notre autonomie. Ils nous "
 "permettent de continuer à travailler pour le Logiciel Libre partout où c'est "
 "nécessaire. Merci d'envisager de faire un don <https://fsfe.org/donate/>."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
 msgstr "activer les instructions de débogage"
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
 msgstr "ne pas omettre les sous-modules Git"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "ne pas omettre les sous-modules Git"
+
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
 msgstr "pas de multiprocessing"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
 msgstr "définition de la racine (root) du projet"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
 msgstr "voir la version du programme et quitter"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr "sous-commandes"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
 msgstr ""
 "ajout des informations de droits d'auteur et de licence dans les en-têtes "
 "(header) des fichiers"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
-"By using --copyright and --license, you can specify which copyright holders and "
-"licenses to add to the headers of the given files.\n"
+"By using --copyright and --license, you can specify which copyright holders "
+"and licenses to add to the headers of the given files.\n"
 "\n"
-"The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or override the "
-"comment style to use.\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
 "\n"
-"You can change the template of the header comment by using --template. Place a "
-"Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the template "
-"by specifying '--template mytemplate'. Read the online documentation on how to "
-"use this feature.\n"
+"The comment style should be auto-detected for your files. If a comment style "
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
 "\n"
-"If a binary file is detected, or if --explicit-license is specified, the header "
-"is placed in a .license file.\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
+"\n"
+"You can change the template of the header comment by using --template. Place "
+"a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
+"template by specifying '--template mytemplate'. Read the online "
+"documentation on how to use this feature.\n"
 "\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"If a binary file is detected, or if --explicit-license is specified, the "
+"header is placed in a .license file."
 msgstr ""
 "Ajout des informations de droits d'auteur et de licence dans les en-têtes "
 "d'un ou plusieurs fichiers.\n"
 "\n"
 "En sélectionnant --copyright et --license, vous pouvez spécifier quels "
 "titulaires de droits et licences sont ajoutés aux en-têtes des fichiers "
 "listés.\n"
@@ -116,19 +135,23 @@
 "l'option --template. Placez un modèle Jinja2 dans le répertoire .reuse/"
 "templates/mytemplate.jinja2. Vous pouvez utiliser le modèle en précisant '--"
 "template mytemplate'. Consultez la documentation en ligne pour plus "
 "d'informations sur l'utilisation de cette fonctionnalité.\n"
 "\n"
 "IMPORTANT: cette fonctionnalité est EXPÉRIMENTALE pour le moment !"
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
+
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "télécharger une licence et la placer dans le répertoire LICENSES/"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
@@ -136,50 +159,50 @@
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
 "Téléchargez une licence et placez-la dans le répertoire LICENSES/.\n"
 "\n"
-"Les répertoires LICENSES/ se trouvent automatiquement dans l'ordre suivant :"
-"\n"
+"Les répertoires LICENSES/ se trouvent automatiquement dans l'ordre "
+"suivant :\n"
 "\n"
 "- Le répertoire LICENSES/ à la racine du répertoire VCS.\n"
 "\n"
 "- Le répertoire actuel, si son nom est LICENSES.\n"
 "\n"
 "- Le répertoire LICENSES/ dans le répertoire courant.\n"
 "\n"
 "Si le répertoire LICENSES/ n'est pas trouvé, il sera simplement créé."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
 msgstr "initialiser le projet REUSE"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
 msgstr "lister tous les fichiers non-conformes"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
-"Lint the project directory for compliance with version {reuse_version} of the "
-"REUSE Specification. You can find the latest version of the specification at "
-"<https://reuse.software/spec/>.\n"
+"Lint the project directory for compliance with version {reuse_version} of "
+"the REUSE Specification. You can find the latest version of the "
+"specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
 "\n"
 "- Are there any bad (unrecognised, not compliant with SPDX) licenses in the "
 "project?\n"
 "\n"
-"- Are any licenses referred to inside of the project, but not included in the "
-"LICENSES/ directory?\n"
+"- Are any licenses referred to inside of the project, but not included in "
+"the LICENSES/ directory?\n"
 "\n"
-"- Are any licenses included in the LICENSES/ directory that are not used inside "
-"of the project?\n"
+"- Are any licenses included in the LICENSES/ directory that are not used "
+"inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
 "Vérifiez le répertoire projet pour assurer la conformité à la version "
 "{reuse_version} de la spécification REUSE. Vous pouvez trouver la dernière "
 "version de la spécification à l'adresse <https://reuse.software/spec/>.\n"
 "\n"
@@ -190,578 +213,747 @@
 "\n"
 "- Y a-t-il des licences dans le répertoire LICENSES/ qui sont inutilisées "
 "dans le projet ?\n"
 "\n"
 "- Tous les fichiers disposent-ils d'informations de droits d'auteur et de "
 "licence valides ?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
 msgstr "imprimer la nomenclature du projet au format SPDX"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
 msgstr "Analyse de la syntaxe de '{expression}' impossible"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
 msgstr "'{}' n'est pas un fichier"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
 msgstr "'{}' n'est pas un répertoire"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
 msgstr "'{}' ne peut être ouvert"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
 msgstr "écriture impossible dans le répertoire '{}'"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
 msgstr "écriture impossible dans '{}'"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
 msgstr "lecture ou écriture impossible pour '{}'"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
 msgstr "'{}' n'est pas une expression SPDX valide, abandon"
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' n'est pas un identifiant de licence SPDX valide."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Consultez <https://spdx.org/licenses/> pour une liste des identifiants de "
+"licence SPDX valides."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
 msgstr "Identification de la licence SPDX"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
 msgstr "télécharger toutes les licences manquantes détectées dans le projet"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
 msgstr "Erreur : {spdx_identifier} existe déjà."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
 msgstr "Erreur : échec du téléchargement de licence."
 
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' n'est pas un identifiant de licence SPDX valide."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License Identifiers."
-msgstr ""
-"Consultez <https://spdx.org/licenses/> pour une liste des identifiants de "
-"licence SPDX valides."
-
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
 msgstr "Votre connexion internet fonctionne-t-elle ?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
 msgstr "Téléchargement de {spdx_identifier} terminé."
 
-#: src/reuse/download.py:136
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
+
+#: src/reuse/download.py:138
 msgid "the following arguments are required: license"
 msgstr "les arguments suivants sont nécessaires : license"
 
-#: src/reuse/download.py:138
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
 msgstr "--output ne peut pas être utilisé avec plus d'une licence"
 
-#: src/reuse/header.py:103
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
 "les commentaires générés ne contiennent pas de ligne ou d'expression de "
 "droits d'auteur ou de licence"
 
-#: src/reuse/header.py:293
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
-"explicit-license"
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
+msgstr ""
+
+#: src/reuse/header.py:421
+#, python-brace-format
+msgid ""
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
 msgstr ""
 "'{path}' n'est pas une extension de fichier reconnue, merci d'utiliser --"
 "style ou --explicit-license"
 
-#: src/reuse/header.py:352
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
+msgstr ""
+
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Erreur : les commentaires ne peuvent être créés dans '{path}'"
 
-#: src/reuse/header.py:359
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
-"license expressions. The template is probably incorrect. Did not write new header."
+"license expressions. The template is probably incorrect. Did not write new "
+"header."
 msgstr ""
 "Erreur : l'en-tête de commentaire généré dans '{path}' ne contient pas de "
 "ligne ou d'expression de droits d'auteur ou de licence. Le modèle est "
 "probablement incorrect. Nouvel en-tête non écrit."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:370
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "En-tête de {path} modifié avec succès"
 
-#: src/reuse/header.py:383
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
 msgstr "déclaration de droits d'auteur, répétable"
 
-#: src/reuse/header.py:390
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
 msgstr "Identifiant SPDX, répétable"
 
-#: src/reuse/header.py:397
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "Identifiant SPDX, répétable"
+
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
 msgstr "année de déclaration de droits d'auteur, optionnel"
 
-#: src/reuse/header.py:405
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
 msgstr "style de commentaire à utiliser, optionnel"
 
-#: src/reuse/header.py:412
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "style de commentaire à utiliser, optionnel"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
 msgstr "nom de modèle à utiliser, optionnel"
 
-#: src/reuse/header.py:417
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
 msgstr "ne pas inclure d'année dans la déclaration"
 
-#: src/reuse/header.py:422
-msgid "place header in path.license instead of path"
-msgstr "placez l'en-tête dans path.license au lieu de path"
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "année de déclaration de droits d'auteur, optionnel"
+
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "style de commentaire à utiliser, optionnel"
+
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "style de commentaire à utiliser, optionnel"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
+
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
 
-#: src/reuse/header.py:430
-msgid "option --copyright or --license is required"
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
 msgstr "une des options --copyright ou --license est nécessaire"
 
-#: src/reuse/header.py:434
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
 msgstr "les options --exclude-year et --year sont mutuellement exclusives"
 
-#: src/reuse/header.py:450
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "les options --exclude-year et --year sont mutuellement exclusives"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
 msgstr "le modèle {template} est introuvable"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr ""
 "'{path}' est un fichier binaire, par conséquent le fichier '{new_path}' est "
 "utilisé pour l'en-tête"
 
 #: src/reuse/init.py:25
-msgid "What license is your project under? Provide the SPDX License Identifier."
+msgid ""
+"What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
 "Sous quelle licence est enregistrè votre projet ? Merci de fournir un "
 "identifiant de licence SPDX."
 
 #: src/reuse/init.py:29
 msgid ""
-"What other license is your project under? Provide the SPDX License Identifier."
+"What other license is your project under? Provide the SPDX License "
+"Identifier."
 msgstr ""
 "Sous quelle autre licence est enregistré votre projet ? Merci de fournir un "
 "identifiant de licence SPDX."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
 msgstr "Pour finir l'ajout de licences, presser ENTRÉE."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
 msgstr "Le projet est déjà initialisé"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
 msgstr "Initialisation du projet pour REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
 msgstr "Quel est le nom du projet ?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
 msgstr "Quelle est l'adresse internet du projet ?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
 msgstr "Quel est le nom de la personne chargée de la maintenance ?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
 msgstr ""
 "Quelle est l'adresse électronique de la personne chargée de la maintenance ?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
 msgstr "Tout est prêt ! Maintenant, on initialise."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
 msgstr "Télécharge {}"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
 msgstr "{} existe déjà"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
 msgstr "{} n'a pas pu être téléchargé"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
 msgstr "Création de .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
 msgstr "Initialisation terminée."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"Félicitations ! Votre projet est conforme à la version {} de la "
-"spécification REUSE :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
 msgstr ""
-"Malheureusement, votre projet n'est pas conforme à la version {} de la "
-"spécification REUSE :-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
 msgstr "MAUVAISES LICENCES"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
 msgstr "'{}' trouvé dans :"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
 msgstr "LICENCES OBSOLÈTES"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
 msgstr "Les licences suivantes sont rendues obsolètes par SPDX :"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
 msgstr "LICENCES SANS EXTENSION DE FICHIER"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
 msgstr "Les licences suivantes n'ont pas d'extension de fichier :"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
 msgstr "LICENCES MANQUANTES"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
 msgstr "LICENCES INUTILISÉES"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
 msgstr "Les licences suivantes ne sont pas utilisées :"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
 msgstr "ERREURS DE LECTURE"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
 msgstr "Illisibles :"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "INFORMATION DE DROITS D'AUTEUR ET DE LICENCE MANQUANTE"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
 "Les fichiers suivants ne contiennent pas d'information de droits d'auteurs "
 "et de licence :"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
 msgstr ""
 "Les fichiers suivants ne contiennent pas d'information de droits d'auteurs :"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
 msgstr "Les fichiers suivants ne contiennent pas d'information de licence :"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
 msgstr "RÉSUMÉ"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
 msgstr "Mauvaises licences :"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
 msgstr "Licences obsolètes :"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
 msgstr "Licences sans extension de fichier :"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
 msgstr "Licences manquantes :"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
 msgstr "Licences inutilisées :"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
 msgstr "Licences utilisées :"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
 msgstr "Erreurs de lecture : {count}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
 msgstr ""
 "Fichiers contenant des informations de droits d'auteur : {count} / {total}"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
 msgstr "Fichiers contenant des informations de licence : {count} / {total}"
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "Git ne peut pas être trouvé"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr ""
+"Félicitations ! Votre projet est conforme à la version {} de la "
+"spécification REUSE :-)"
 
-#: src/reuse/project.py:133
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Malheureusement, votre projet n'est pas conforme à la version {} de la "
+"spécification REUSE :-("
+
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
+
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
 msgstr "'{path}' est couvert par .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
-msgid "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
+msgid ""
+"'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
 "'{path}' contient une expression SPDX qui ne peut pas être analysée, le "
 "fichier est ignoré"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 contient des erreurs de syntaxe"
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
+
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
 msgstr "résolution de l'identifiant de '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
 msgstr "{path} n'a pas d'extension de fichier"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
-"Could not resolve SPDX License Identifier of {path}, resolving to {identifier}. "
-"Make sure the license is in the license list found at <https://spdx.org/licenses/"
-"> or that it starts with 'LicenseRef-', and that it has a file extension."
+"Could not resolve SPDX License Identifier of {path}, resolving to "
+"{identifier}. Make sure the license is in the license list found at <https://"
+"spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
+"file extension."
 msgstr ""
 "Impossible de résoudre l'identifiant de licence SPDX de {path}, utilisation "
 "de {identifier}. Merci de vérifier que la licence est dans la liste "
 "trouvable à<https://spdx.org/licenses/> ou qu'elle débute par 'LicenseRef-', "
 "et qu'elle contient une extension de fichier."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
-msgid "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
+msgid ""
+"{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr "{identifier} est l'identifiant de {path} comme de {other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr "Lecture de '{path}' impossible"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
 msgstr "Erreur inattendue lors de l'analyse de '{path}'"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' ne se termine pas en .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.7/argparse.py:297
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
 msgstr "usage : "
 
-#: /usr/lib64/python3.7/argparse.py:845
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
 msgstr ".__call__() est indéfini"
 
-#: /usr/lib64/python3.7/argparse.py:1148
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
 msgstr "analyseur %(parser_name)r inconnu (choix : %(choices)s)"
 
-#: /usr/lib64/python3.7/argparse.py:1202
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "impossible d'ouvrir '%s' : %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "'%(filename)s' ne peut pas être ouvert : %(error)s"
 
-#: /usr/lib64/python3.7/argparse.py:1414
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
-#: /usr/lib64/python3.7/argparse.py:1452
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
 msgstr "'required' est un argument invalide pour les positionnels"
 
-#: /usr/lib64/python3.7/argparse.py:1474
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
-"invalid option string %(option)r: must start with a character %(prefix_chars)r"
+"invalid option string %(option)r: must start with a character "
+"%(prefix_chars)r"
 msgstr ""
 "option de chaîne %(option)r invalide : doit débuter par un caractère "
 "%(prefix_chars)r"
 
-#: /usr/lib64/python3.7/argparse.py:1494
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
 msgstr "dest= est nécessaire pour les options comme %r"
 
-#: /usr/lib64/python3.7/argparse.py:1511
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
 msgstr "valeur de résolution de conflit invalide : %r"
 
-#: /usr/lib64/python3.7/argparse.py:1529
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "chane d'options contradictoire : %s"
 msgstr[1] "chaînes d'options contradictoires : %s"
 
-#: /usr/lib64/python3.7/argparse.py:1595
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
 msgstr "les arguments mutuellement exclusifs doivent être optionnels"
 
-#: /usr/lib64/python3.7/argparse.py:1658
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
 msgstr "arguments positionnels"
 
-#: /usr/lib64/python3.7/argparse.py:1659
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
 msgstr "arguments optionnels"
 
-#: /usr/lib64/python3.7/argparse.py:1674
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
 msgstr "afficher ce message d'aide et quitter"
 
-#: /usr/lib64/python3.7/argparse.py:1705
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible de considérer des arguments de sous-analyse multiples"
 
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
 msgstr "arguments non reconnus : %s"
 
-#: /usr/lib64/python3.7/argparse.py:1854
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
 msgstr "non autorisé avec l'argument %s"
 
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
 msgstr "l'argument explicite %r est ignoré"
 
-#: /usr/lib64/python3.7/argparse.py:2021
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
 msgstr "les arguments suivants sont nécessaires : %s"
 
-#: /usr/lib64/python3.7/argparse.py:2036
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
 msgstr "un des arguments %s est nécessaire"
 
-#: /usr/lib64/python3.7/argparse.py:2079
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
 msgstr "un argument est attendu"
 
-#: /usr/lib64/python3.7/argparse.py:2080
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
 msgstr "au plus un argument est attendu"
 
-#: /usr/lib64/python3.7/argparse.py:2081
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
 msgstr "au moins un argument est attendu"
 
-#: /usr/lib64/python3.7/argparse.py:2083
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "l'argument %s est attendu"
 msgstr[1] "les arguments %s sont attendus"
 
-#: /usr/lib64/python3.7/argparse.py:2143
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "option ambigüe : %(option)s ne correspond pas à %(matches)s"
 
-#: /usr/lib64/python3.7/argparse.py:2206
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
 msgstr "option inattendue : %s"
 
-#: /usr/lib64/python3.7/argparse.py:2403
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
 msgstr "%r ne peut être appelé"
 
-#: /usr/lib64/python3.7/argparse.py:2420
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
 msgstr "valeur %(type)s invalide : %(value)r"
 
-#: /usr/lib64/python3.7/argparse.py:2431
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
 msgstr "choix non valide : %(value)r (choisir parmi %(choices)s)"
 
-#: /usr/lib64/python3.7/argparse.py:2507
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s : erreur : %(message)s\n"
 
-#, python-format
-#~ msgid "can't open '%(filename)s': %(error)s"
-#~ msgstr "'%(filename)s' ne peut pas être ouvert : %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "chane d'options contradictoire : %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "chane d'options contradictoire : %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "impossible d'ouvrir '%s' : %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "placez l'en-tête dans path.license au lieu de path"
+
+#~ msgid "could not find Git"
+#~ msgstr "Git ne peut pas être trouvé"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' ne se termine pas en .spdx"
```

### Comparing `reuse-2.0.0/po/gl.po` & `reuse-2.1.0/po/de.po`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,193 @@
-# SPDX-FileCopyrightText: 2020 pd <eukelade@gmail.com>
+# SPDX-FileCopyrightText: 2020 Max Mehl
+# SPDX-FileCopyrightText: 2020 Thomas Doczkal
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-09 13:51+0100\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: 2023-06-21 09:53+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Galician <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
-"gl/>\n"
-"Language: gl\n"
+"Language-Team: German <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"de/>\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.1\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse é unha ferramenta para o cumprimento das recomendacións REUSE. Ver "
-"<https://reuse.software/> para máis información e <https://reuse.readthedocs."
-"io/> para a documentación en liña."
+"reuse ist ein Werkzeug, um die Empfehlungen von REUSE umzusetzen und zu "
+"überprüfen. Mehr Informationen finden Sie auf <https://reuse.software/> oder "
+"in der Online-Dokumentation auf <https://reuse.readthedocs.io/>."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr ""
-"Esta versión de reuse é compatible coa versión {} da especificación REUSE."
+"Diese Version von reuse ist kompatibel mit Version {} der REUSE-"
+"Spezifikation."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
-msgstr "Apoie o traballo da FSFE:"
+msgstr "Die Arbeit der FSFE unterstützen:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
-"As doazóns son críticas para a nosa forza e autonomía. Permítennos seguir "
-"traballando polo software libre onde sexa necesario. Considere facer unha "
-"doazón a <https://fsfe.org/donate/> ."
+"Spenden sind entscheidend für unsere Leistungsfähigkeit und Autonomie. Sie "
+"ermöglichen es uns, weiterhin für Freie Software zu arbeiten, wo immer es "
+"nötig ist. Bitte erwägen Sie eine Spende unter <https://fsfe.org/donate/>."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
-msgstr "habilitar sentencias de depuración"
+msgstr "Debug-Statements aktivieren"
+
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
-msgstr "non salte os submódulos de Git"
+msgstr "Git-Submodules nicht überspringen"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "Git-Submodules nicht überspringen"
+
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
-msgstr "non empregue multiprocesamento"
+msgstr "kein Multiprocessing verwenden"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
-msgstr "definir a raíz do proxecto"
+msgstr "Stammverzeichnis des Projekts bestimmen"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
-msgstr "mostrar o número de versión do programa e saír"
+msgstr "zeige die Versionsnummer des Programms und beende"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
-msgstr "subcomandos"
+msgstr "Unterkommandos"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
-msgstr "engadir copyright e licenza na cabeceira dos arquivos"
+msgstr ""
+"schreibe Urheberrechts- und Lizenzinformationen in die Kopfzeilen von Dateien"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
-"Engadir copyright e información da licenza na cabeceira de un ou varios "
-"arquivos\n"
+"Schreibe Urheberrechts- und Lizenzinformationen in die Kopfzeilen von einer "
+"oder mehr Dateien.\n"
 "\n"
-"Pódese especificar mediante --license e --copyright a licenza e os donos do "
-"copyright a engadir nas cabeceiras dos arquivos indicados.\n"
+"Mit der Benutzung von --copyright und --license können Sie bestimmen, welche "
+"Urheber und Lizenzen Sie in die Kopfzeilen der jeweiligen Dateien "
+"hinzufügen.\n"
 "\n"
-"O estilo dos comentarios dos arquivos debería detectarse automáticamente, de "
-"non se detectar o proceso abórtase. Pódese usar --style para definir ou "
-"forzar o estilo de comentario a usar.\n"
+"Der Kommentarstil wird normalerweise automatisch erkannt. Wenn das nicht der "
+"Fall ist, endet der Vorgang. Benutzen Sie --style um einen Kommentarstil zu "
+"bestimmen oder zu forcieren.\n"
 "\n"
-"É posible cambiar o modelo do comentario de cabeceira usando --template. Por "
-"exemplo, gardando o modelo Jinja2 na carpeta .reuse/templates/"
-"mytemplate.jinja2 pode usar este modelo indicando  '--template mytemplate'. "
-"Consulte a documentación en liña para máis información sobre esta "
-"característica.\n"
+"Sie können die Vorlage für die Kopfzeilen-Kommentare mit --template ändern. "
+"Erstellen Sie dazu eine Jinja2-Vorlage in .reuse/templates/mytemplate."
+"jinja2. Sie können die Vorlage verwenden mithilfe von '--template "
+"mytemplate'. Mehr Informationen zu dieser Funktion in der Online-"
+"Dokumentation.\n"
 "\n"
-"Se o arquivo é binario ou se especifica --explicit-license, a cabeceira "
-"gárdase nun arquivo .license.\n"
+"Wenn eine Binärdatei erkannt wurde, oder wenn --explicit-license verwendet "
+"wurde, werden die Kopfzeilen in einer .license-Datei gespeichert.\n"
 "\n"
-"IMPORTANTE: Actualmente isto é EXPERIMENTAL!"
+"WICHTIG: Diese Funktion ist momentan EXPERIMENTELL!"
+
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
-msgstr "Descargar unha licenza e gardala na carpeta LICENSES/"
+msgstr "lade eine Datei herunter und speichere sie im Verzeichnis LICENSES/"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
 "- The current directory if its name is LICENSES.\n"
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
-"Descargar unha licenza e gardala na carpeta LICENSES/.\n"
+"Lade eine Datei herunter und speichere sie im Verzeichnis LICENSES/.\n"
 "\n"
-"A carpeta LICENSES/ procurase neste orde:\n"
+"Das LICENSES/-Verzeichnis wird automatisch in dieser Reihenfolge gesucht:\n"
 "\n"
-"- a carpeta LICENSES/ na raíz do repositorio VCS.\n"
+"- Das LICENSES/-Verzeichnis im Wurzelverzeichnis des VCS-Repositorys.\n"
 "\n"
-"- a carpeta actual se o seu nome é LICENSES.\n"
+"- Das aktuelle Verzeichnis wenn dessen Name LICENSES ist.\n"
 "\n"
-"- a carpeta LICENSES/  no directorio actual.\n"
+"- Das LICENSES/-Verzeichnis im aktuellen Verzeichnis.\n"
 "\n"
-"Se non se atopa a carpeta LICENSES/ créase unha."
+"Wenn das LICENSES/-Verzeichnis nicht gefunden werden kann, wird einfach "
+"eines erstellt."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
-msgstr "iniciar un proxecto REUSE"
+msgstr "REUSE-Projekt initialisieren"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
-msgstr "listar todos os arquivos que non cumplen os criterios"
+msgstr "alle nicht-konformen Dateien zeigen"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -172,631 +199,760 @@
 "the LICENSES/ directory?\n"
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
-"Verificar que a carpeta do proxecto cumple coa versión {reuse_version} da "
-"especificación REUSE. Pode atopar a última versión da especificación en "
-"<https://reuse.software/spec/>.\n"
+"Überprüfen Sie das Projektverzeichnis auf die Einhaltung der Version "
+"{reuse_version} der REUSE-Spezifikation. Die neueste Version der "
+"Spezifikation finden Sie unter <https://reuse.software/spec/>.\n"
 "\n"
-"Comprobase específicamente os seguintes criterios:\n"
+"Im Einzelnen werden die folgenden Kriterien geprüft:\n"
 "\n"
-"- Existen licenzas inapropiadas (non recoñecidas ou que incumplen o SPDX) no "
-"proxecto?\n"
+"- Sind im Projekt schlechte (nicht erkannte, nicht SPDX-konforme) Lizenzen "
+"vorhanden?\n"
 "\n"
-"- Hai algunha licenza mencionada no proxecto que non está incluida na "
-"carpeta LICENSES/?\n"
+"- Gibt es Lizenzen, auf die innerhalb des Projekts verwiesen wird, die aber "
+"nicht im Verzeichnis LICENSES/ enthalten sind?\n"
 "\n"
-"- A carpeta LICENSES/ contén licenzas non usadas no proxecto?\n"
+"- Sind Lizenzen im Verzeichnis LICENSES/ enthalten, die nicht innerhalb des "
+"Projekts verwendet werden?\n"
 "\n"
-"- Todos os arquivos teñen información correcta de copyright e licenza?"
+"- Sind alle Dateien mit gültigen Urheberrechts- und Lizenzinformationen "
+"versehen?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
-msgstr "imprimir a lista de materiales do proxecto en formato SPDX"
+msgstr "Komponentenliste im SPDX-Format ausgeben"
+
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
 
-#: src/reuse/_util.py:216
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
-msgstr "Non se pode analizar '{expression}'"
+msgstr "Kann '{expression}' nicht parsen"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
-msgstr "'{}' non é un arquivo"
+msgstr "'{}' ist keine Datei"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
-msgstr "'{}' non é un directorio"
+msgstr "'{}' ist kein Verzeichnis"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
-msgstr "non se pode abrir '{}'"
+msgstr "kann '{}' nicht öffnen"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
-msgstr "non se pode escribir no directorio '{}'"
+msgstr "kann nicht in Verzeichnis '{}' schreiben"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
-msgstr "non se pode escribir en '{}'"
+msgstr "kann nicht in '{}' schreiben"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
-msgstr "non se pode ler ou escribir en '{}'"
+msgstr "kann '{}' nicht lesen oder schreiben"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
-msgstr "'{}' non é unha expresión SPDX válida, cancelando"
+msgstr "'{}' ist kein gültiger SPDX-Ausdruck, breche ab"
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' ist kein gültiger SPDX-Lizenz-Identifikator."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Besuchen Sie <https://spdx.org/licenses/> für eine Liste von gültigen SPDX-"
+"Lizenz-Identifikatoren."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
-msgstr "Identificador de Licenza SPDX da licenza"
+msgstr "SPDX-Lizenz-Identifikator der Lizenz"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
-msgstr "descargar todas as licenzas detectadas mais non atopadas no proxecto"
+msgstr "lade alle fehlenden Lizenzen herunter, die im Projekt gefunden wurden"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
-msgstr "Erro: {spdx_identifier} xa existe."
+msgstr "Fehler: {spdx_identifier} existiert bereits."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
-msgstr "Erro: Fallo descargando a licenza."
-
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' non é un Identificador de Licenza SPDX válido."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Consulte unha lista de Identificadores de Licenza SPDX válidos en "
-"<https://spdx.org/licenses/>."
+msgstr "Fehler: Lizenz konnte nicht heruntergeladen werden."
 
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
-msgstr "Está a funcionar a súa conexión a internet?"
+msgstr "Funktioniert Ihre Internetverbindung?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
-msgstr "Descargouse correctamente o {spdx_identifier}."
+msgstr "{spdx_identifier} erfolgreich heruntergeladen."
 
-#: src/reuse/download.py:136
-msgid "the following arguments are required: license"
-msgstr "requirense os seguintes argumentos: licenza"
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
 
 #: src/reuse/download.py:138
+msgid "the following arguments are required: license"
+msgstr "Die folgenden Argumente sind erforderlich: license"
+
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
-msgstr "non se pode usar --output con máis dunha licenza"
+msgstr "Kann --output nicht mit mehr als einer Lizenz verwenden"
 
-#: src/reuse/header.py:103
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
-msgstr "o comentario xerado non ten liñas de copyright ou expresións de licenza"
+msgstr ""
+"Dem generierten Kommentar fehlen Zeilen zum Urheberrecht oder Lizenzausdrücke"
 
-#: src/reuse/header.py:293
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
+msgstr ""
+
+#: src/reuse/header.py:421
+#, python-brace-format
+msgid ""
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"'{path}' hat keine erkannte Dateiendung, bitte verwenden Sie --style oder --"
 "explicit-license"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
 msgstr ""
-"'{path}' non ten unha extensión de arquivo recoñecida, precisa usar --style "
-"ou --explicit-license"
 
-#: src/reuse/header.py:352
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
-msgstr "Erro: Non se pode crear un comentario para '{path}'"
+msgstr "Fehler: Kann kein Kommentar für '{path}' erstellen"
 
-#: src/reuse/header.py:359
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
-"Erro: A cabeceira comentada xerada para '{path}' non contén liñas de "
-"copyright ou expresións de licenza. Posibelmente o modelo é incorrecto. Non "
-"se escribiu unha nova cabecereira."
+"Fehler: Die generierten Kommentar-Kopfzeilen für '{path}' enthalten fehlende "
+"Urheberrechtszeilen oder Lizenzausdrücke. Die Vorlage ist wahrscheinlich "
+"falsch. Keine neuen Kopfzeile geschrieben."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:370
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
-msgstr "A cabeceira de {path} cambiada con éxito"
+msgstr "Kopfzeilen von {path} erfolgreich geändert"
 
-#: src/reuse/header.py:383
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
-msgstr "declaración de copyright, repetibel"
+msgstr "Urheberrechtsinformation, wiederholbar"
 
-#: src/reuse/header.py:390
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
-msgstr "Identificador SPDX, repetibel"
+msgstr "SPDX-Lizenz-Identifikator, wiederholbar"
+
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "SPDX-Lizenz-Identifikator, wiederholbar"
 
-#: src/reuse/header.py:397
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
-msgstr "ano da declaración de copyright, opcional"
+msgstr "Jahr der Urheberrechtsinformation, optional"
 
-#: src/reuse/header.py:405
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
-msgstr "estilo de comentario a usar, opcional"
+msgstr "zu benutzender Kommentarstil, optional"
 
-#: src/reuse/header.py:412
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "zu benutzender Kommentarstil, optional"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
-msgstr "nome do modelo a usar, opcional"
+msgstr "Name der zu verwendenden Vorlage, optional"
 
-#: src/reuse/header.py:417
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
-msgstr "non incluir ano na declaración"
+msgstr "füge kein Jahr in Angabe hinzu"
+
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "Jahr der Urheberrechtsinformation, optional"
 
-#: src/reuse/header.py:422
-msgid "place header in path.license instead of path"
-msgstr "colocar a cabeceira en carpeta.licenza no canto de carpeta"
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "zu benutzender Kommentarstil, optional"
 
-#: src/reuse/header.py:430
-msgid "option --copyright or --license is required"
-msgstr "precisase a opción --copyright ou --license"
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "zu benutzender Kommentarstil, optional"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
 
-#: src/reuse/header.py:434
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
+msgstr "Option --copyright oder --license ist erforderlich"
+
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
-msgstr "as opcións --exclude-year e --year non se poden usar á vez"
+msgstr "Die Optionen --exclude-year und --year schließen sich gegenseitig aus"
 
-#: src/reuse/header.py:450
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "Die Optionen --exclude-year und --year schließen sich gegenseitig aus"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
-msgstr "no se atopa o modelo {template}"
+msgstr "Vorlage {template} konnte nicht gefunden werden"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
-msgstr "'{path}' é binario, logo úsase '{new_path}' para a cabeceira"
+msgstr ""
+"'{path}' ist im Binärformat, benutze daher '{new_path}' für die Kopfzeilen"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
-"Baixo que licenza está o seu proxecto? indique o Identificador de Licenza "
-"SPDX."
+"Unter welcher Lizenz steht Ihr Projekt? Geben Sie den SPDX-Lizenz-"
+"Identifikator an."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License "
 "Identifier."
 msgstr ""
-"Baixo que outra licenza está o seu proxecto? indique o Identificador de "
-"Licenza SPDX."
+"Unter welcher anderen Lizenz steht Ihr Projekt? Geben Sie den SPDX-Lizenz-"
+"Identifikator an."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
-msgstr "Para rematar de engadir licenzas, prema ENTER."
+msgstr "Um keine weiteren Lizenzen hinzuzufügen, drücken Sie ENTER."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
-msgstr "O proxecto xa está iniciado"
+msgstr "Projekt bereits initialisiert"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
-msgstr "Iniciando o proxecto para REUSE."
+msgstr "Initialisiere Projekt für REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
-msgstr "Cal é o nome do proxecto?"
+msgstr "Was ist der Name des Projekts?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
-msgstr "Cal é o enderezo en internet do proxecto?"
+msgstr "Was ist die Internetadresse des Projekts?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
-msgstr "Cal é o nome do mantenedor?"
+msgstr "Was ist der Name der Betreuenden?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
-msgstr "Cal é o correo electrónico do mantenedor?"
+msgstr "Wie lautet die E-Mail-Adresse der Betreuenden?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
-msgstr "Rematou todo! iniciando arestora."
+msgstr "Alles erledigt! Initialisiere jetzt."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
-msgstr "Descargando {}"
+msgstr "Lade {} herunter"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
-msgstr "{} xa existe"
+msgstr "{} existiert bereits"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
-msgstr "Non se pode descargar {}"
+msgstr "Konnte {} nicht herunterladen"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
-msgstr "Creando .reuse/dep5"
+msgstr "Erstelle .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
-msgstr "Inicialización completada."
+msgstr "Initialisierung vollständig."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"Congratulacións! O seu proxecto cumple coa versión {} da especificación "
-"REUSE :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
 msgstr ""
-"Desgraciadamente o seu proxecto non cumple coa versión {} da especificación "
-"REUSE :-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
-msgstr "LICENZAS DEFECTUOSAS"
+msgstr "FALSCHE LIZENZEN"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
-msgstr "'{}' atopado en:"
+msgstr "'{}' gefunden in:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
-msgstr "LICENZAS OBSOLETAS"
+msgstr "VERALTETE LIZENZEN"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
-msgstr "As seguintes licenzas son obsoletas para SPDX:"
+msgstr "Die folgenden Lizenzen wurden von SPDX als veraltetet gekennzeichnet:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
-msgstr "LICENZAS SEN EXTENSIÓN DE ARQUIVO"
+msgstr "LIZENZEN OHNE DATEIENDUNG"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
-msgstr "As seguintes licenzas non teñen extesión de arquivo:"
+msgstr "Die folgenden Lizenzen haben keine Dateiendung:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
-msgstr "LICENZAS NON ATOPADAS"
+msgstr "FEHLENDE LIZENZEN"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
-msgstr "LICENZAS SEN USO"
+msgstr "NICHT VERWENDETE LIZENZEN"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
-msgstr "As seguintes licenzas non se usan:"
+msgstr "Die folgenden Lizenzen werden nicht benutzt:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
-msgstr "ERROS DE LECTURA"
+msgstr "LESEFEHLER"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
-msgstr "Non se pode ler:"
+msgstr "Unlesbar:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
-msgstr "NON SE ATOPA INFORMACIÓN DE LICENZA OU COPYRIGHT"
+msgstr "FEHLENDE URHEBERRECHTS- UND LIZENZINFORMATIONEN"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
-"Os seguintes arquivos non teñen información de licenza nen de copyright:"
+"Die folgenden Dateien haben keine Urheberrechts- und Lizenzinformationen:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
-msgstr "Os seguintes arquivos non teñen información de copyright:"
+msgstr "Die folgenden Dateien haben keine Urheberrechtsinformationen:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
-msgstr "Os seguintes arquivos non teñen información de licenza:"
+msgstr "Die folgenden Dateien haben keine Lizenzinformationen:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
-msgstr "RESUMO"
+msgstr "ZUSAMMENFASSUNG"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
-msgstr "Licenzas defectuosas:"
+msgstr "Falsche Lizenzen:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
-msgstr "Licenzas obsoletas:"
+msgstr "Veraltete Lizenzen:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
-msgstr "Licenzas sen extensión de arquivo:"
+msgstr "Lizenzen ohne Dateiendung:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
-msgstr "Licenzas non atopadas:"
+msgstr "Fehlende Lizenzen:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
-msgstr "Licenzas non usadas:"
+msgstr "Unbenutzte Lizenzen:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
-msgstr "Licenzas usadas:"
+msgstr "Verwendete Lizenzen:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
-msgstr "Erros de lectura: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
+msgstr "Lesefehler: {count}"
+
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
+msgstr "Dateien mit Urheberrechtsinformationen: {count} / {total}"
+
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
+msgstr "Dateien mit Lizenzinformationen: {count} / {total}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
-msgstr "Arquivos con información de copyright: {count} / {total}"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr ""
+"Herzlichen Glückwunsch! Ihr Projekt ist konform mit Version {} der REUSE-"
+"Spezifikation :-)"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
-msgstr "Arquivos con información de licenza: {count} / {total}"
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Leider ist Ihr Projekt nicht konform mit Version {} der REUSE-"
+"Spezifikation :-("
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "non se pode atopar o Git"
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
-msgstr "'{path}' cuberto por .reuse/dep5"
+msgstr "'{path}' abgedeckt durch .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
-"'{path}' inclúe unha expresión SPDX que non se pode analizar, saltando o "
-"arquivo"
+"'{path}' trägt einen SPDX-Ausdruck, der nicht geparst werden kann. "
+"Überspringe Datei"
+
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
-msgstr ".reuse/dep5 ten erros de sintaxe"
+msgstr ".reuse/dep5 hat Syntaxfehler"
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
+
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
-msgstr "resolvendo o identificador de '{path}'"
+msgstr "erkenne Identifikator von '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
-msgstr "{path} non ten extensión de arquivo"
+msgstr "{path} hat keine Dateiendung"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
-"Non se pode resolver o Identificador de Licenza SPDX de {path}, resólvese "
-"como {identifier}. Asegúrese que a licenza está na lista publicada en "
-"<https://spdx.org/licenses/> ou que comeza con 'LicenseRef-' e ten unha "
-"extensión de arquivo."
+"Konnte SPDX-Lizenz-Identifikator von {path} nicht erkennen, der auf "
+"{identifier} verweist. Stellen Sie sicher, dass die Lizenz in der "
+"Lizenzliste unter <https://spdx.org/licenses/> steht oder mit 'LicenseRef-' "
+"beginnt und eine Dateiendung hat."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
-"{identifier} é o Identificador de Licenza SPDX de ambos os dous {path} e "
-"{other_path}"
+"{identifier} ist der SPDX-Lizenz-Identifikator von {path} und {other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
-msgstr "Non se pode ler '{path}'"
+msgstr "Konnte '{path}' nicht lesen"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
-msgstr "Aconteceu un erro inesperado lendo '{path}'"
+msgstr "Unerwarteter Fehler beim Parsen von '{path}' aufgetreten"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' non remata en .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
-msgstr "uso: "
+msgstr "Benutzung: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
-msgstr ".__call__() non definido"
+msgstr ".__call__() nicht definiert"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
-msgstr "analizador descoñecido %(parser_name)r (alternativas: %(choices)s)"
+msgstr "unbekannter Parser %(parser_name)r (Auswahl: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
-msgstr "argumento \"-\" con modo %r"
+msgstr "Argument \"-\" mit Modus %r"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "non se pode abrir '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "Kann '%(filename)s' nicht öffnen: %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
-msgstr "non se poden misturar as accións - dous grupos teñen o nome %r"
+msgstr "Kann Aktionen nicht zusammenführen - zwei Gruppen heißen %r"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' non é un argumento valido para os posicionais"
+msgstr "'required' ist ein ungültiges Argument für Positionsangaben"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
-"cadea de opción non válida %(option)r: precisa comenzar cun carácter "
-"%(prefix_chars)r"
+"Ungültige Option %(option)r: Muss mit einem Buchstaben %(prefix_chars)r "
+"beginnen"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
-msgstr "requírese dest= para opcións do tipo %r"
+msgstr "dest= ist erforderlich für Optionen wie %r"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
-msgstr "valor non válido para conflict_resolution: %r"
+msgstr "Ungültiger Wert für conflict_resolution: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
-msgstr[0] "cadea de opción conflictiva: %s"
-msgstr[1] "cadeas de opción conflictivas: %s"
+msgstr[0] "Widersprüchliche Option: %s"
+msgstr[1] "Widersprüchliche Optionen: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
-msgstr "os argumentos mutuamente exclusivos deben ser opcionais"
+msgstr "Sich gegenseitig ausschließende Argumente müssen optional sein"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
-msgstr "argumentos posicionais"
+msgstr "Positions-Argumente"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
-msgstr "argumentos opcionais"
+msgstr "Optionale Argumente"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
-msgstr "mostrar esta mensaxe de axuda e sair"
+msgstr "zeige diese Hilfsnachricht und beende"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
-msgstr "non pode haber múltiples argumentos para o subanalizador"
+msgstr "mehrere Subparser-Argumente sind nicht möglich"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2277
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
-msgstr "argumentos non recoñecidos: %s"
+msgstr "unbekannte Argumente: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
-msgstr "non se permite co argumento %s"
+msgstr "nicht erlaubt mit Argument %s"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
-msgstr "argumento explicito %r ignorado"
+msgstr "explizites Argument %r ignoriert"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
-msgstr "precísanse os seguintes argumentos: %s"
+msgstr "die folgenden Argumente sind erforderlich: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
-msgstr "precísase un dos argumentos %s"
+msgstr "eines der Argumente %s ist erforderlich"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
-msgstr "espérase un argumento"
+msgstr "erwartete ein Argument"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
-msgstr "espérase un argumento como máximo"
+msgstr "erwartete höchstens ein Argument"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
-msgstr "espérase un argumento como mínimo"
+msgstr "erwartete mindestens ein Argument"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2098
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
-msgstr[0] "espérase %s argumento"
-msgstr[1] "espéranse %s argumentos"
+msgstr[0] "erwartete %s Argument"
+msgstr[1] "erwartete %s Argumente"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2157
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
-msgstr "opción ambigua: %(option)s pode encaixar con %(matches)s"
+msgstr "mehrdeutige Option: %(option)s könnte %(matches)s bedeuten"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2220
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
-msgstr "opción de cadea non esperada: %s"
+msgstr "unerwarteter Options-String: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2417
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
-msgstr "%r non se pode chamar"
+msgstr "%r ist nicht aufrufbar"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2434
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
-msgstr "valor non válido %(type)s: %(value)r"
+msgstr "ungültiger %(type)s Wert: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2445
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
-msgstr "alternativa non válida: %(value)r (elixir entre %(choices)s)"
+msgstr "ungültige Auswahl: %(value)r (wähle von %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2521
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
-msgstr "%(prog)s: erro: %(message)s\n"
+msgstr "%(prog)s: Fehler: %(message)s\n"
 
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "non se pode abrir '%(filename)s': %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "Widersprüchliche Option: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "Widersprüchliche Option: %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "Kann '%s' nicht öffnen: %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "Speichere Kopfzeilen in path.license anstatt path"
+
+#~ msgid "could not find Git"
+#~ msgstr "konnte Git nicht finden"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' endet nicht mit .spdx"
```

### Comparing `reuse-2.0.0/po/nl.po` & `reuse-2.1.0/po/es.po`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,192 @@
-# SPDX-FileCopyrightText: 2018, 2020 Carmen Bianca Bakker
-# SPDX-FileCopyrightText: 2017, 2020 André Ockers
+# SPDX-FileCopyrightText: 2018 pd <euklade@gmail.com>
+# SPDX-FileCopyrightText: 2018 flow <adolflow@sindominio.net>
+# SPDX-FileCopyrightText: 2020 Roberto Bauglir <bauglir@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: FSFE reuse\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-12-20 12:18+0100\n"
-"PO-Revision-Date: 2023-02-18 10:24+0000\n"
-"Last-Translator: \"J. Lavoie\" <j.lavoie@net-c.ca>\n"
-"Language-Team: Dutch <https://hosted.weblate.org/projects/fsfe/reuse-tool/nl/"
-">\n"
-"Language: nl\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
+"PO-Revision-Date: 2023-02-20 19:38+0000\n"
+"Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/fsfe/reuse-tool/"
+"es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.18.1\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
-"reuse is een tool voor naleving van de REUSE Initiatief aanbevelingen. Zie "
-"<https://reuse.software/> voor meer informatie en <https://reuse.readthedocs."
-"io/> voor de online documentatie."
+"reuse es una herramienta para cumplir con las recomendaciones de la "
+"iniciativa REUSE. Visita <https://reuse.software/> para obtener más "
+"información, y <https://reuse.readthedocs.io/> para acceder a la "
+"documentación en línea."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr ""
-"Deze versie van reuse is compatibel met versie {} van de REUSE Specificatie."
+"Esta versión de reuse es compatible con la versión {} de la Especificación "
+"REUSE."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
-msgstr "Ondersteun het werk van de FSFE:"
+msgstr "Apoya el trabajo de la FSFE:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
-"Donaties zijn belangrijk voor onze sterkte en autonomie. Ze staan ons toe om "
-"verder te werken voor vrije software waar nodig. Overweeg alstublieft om een "
-"donatie te maken bij <https://fsfe.org/donate/>."
+"Las donaciones son esenciales para nuestra fortaleza y autonomía. Estas nos "
+"permiten continuar trabajando por el Software Libre allá donde sea "
+"necesario. Por favor, considera el hacer una donación en <https://fsfe.org/"
+"donate/>."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
-msgstr "zet debug statements aan"
+msgstr "habilita instrucciones de depuración"
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
-msgstr "sla Git-submodules niet over"
+msgstr "no omitas los submódulos de Git"
+
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "no omitas los submódulos de Git"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
-msgstr "gebruik geen multiprocessing"
+msgstr "no utilices multiproceso"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
-msgstr "bepaal de root van het project"
+msgstr "define el origen del proyecto"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
-msgstr "versienummer van het programma laten zien en verlaten"
+msgstr "muestra la versión del programa y sale"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
-msgstr "subcommando's"
+msgstr "subcomandos"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
-msgstr ""
-"voeg auteursrechts- en licentie-informatie toe aan de headers van bestanden"
+msgstr "agrega el copyright y la licencia a la cabecera de los ficheros"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
-"Voeg auteursrechts- en licentie-informatie toe aan de headers van een of "
-"meer bestanden.\n"
+"Añade copyright y licencias en la cabecera de uno o más archivos.\n"
 "\n"
-"Met --copyright en --license kun je de auteursrechthouders en licenties "
-"specificeren die toegevoegd moeten worden aan de headers van de bestanden.\n"
+"Usando --copyright y --license, puede especificar qué titulares de derechos "
+"de autor y licencias añadir a las cabeceras de los archivos dados.\n"
 "\n"
-"De commentstijl wordt automatisch gedetecteerd voor uw bestanden. Als een "
-"commentstijl niet gedetecteerd kan worden, stopt het proces. Gebruik --style "
-"om een commentstijl te bepalen.\n"
+"El estilo de comentario debería detectarse automáticamente para sus "
+"archivos. Si no se puede detectar un estilo de comentario, el proceso se "
+"aborta. Utilice --style para especificar o anular el estilo de comentario a "
+"utilizar.\n"
 "\n"
-"U kunt het sjabloon van de header veranderen met --template. Zet een Jinja2-"
-"sjabloon in .reuse/templates/mijnsjabloon.jinja2. U kunt het sjabloon "
-"gebruiken door '--template mijnsjabloon' te specificeren. Lees de online "
-"documentatie voor meer informatie over deze functionaliteit.\n"
+"Puede cambiar la plantilla del comentario de cabecera usando --template. "
+"Coloque una plantilla Jinja2 en .reuse/templates/mytemplate.jinja2. Puedes "
+"usar la plantilla especificando '--template mytemplate'. Lea la información "
+"en internet sobre cómo utilizar esta función.\n"
 "\n"
-"Als een binary bestand gedetecteerd is, of als --explicit-license gebruikt "
-"wordt, dan wordt de header in een .license bestand geplaatst.\n"
+"Si se detecta un archivo binario, o si se especifica --explicit-license, la "
+"cabecera se coloca en un archivo .license.\n"
 "\n"
-"BELANGRIJK: Dit is momenteel EXPERIMENTEEL!"
+"IMPORTANTE: ¡Esto está actualmente disponible de forma EXPERIMENTAL!"
+
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
-msgstr "download een licentie en plaats het in de LICENSES/-map"
+msgstr "descarga una licencia y guárdala en el directorio \"LICENSES/\""
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
 "- The current directory if its name is LICENSES.\n"
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
-"Download een licentie en plaats het in de LICENSES/-map.\n"
+"Descarga una licencia y guárdala en el directorio LICENSES/.\n"
 "\n"
-"De LICENSES/-map is automatisch gevonden in de volgende volgorde:\n"
+"El directorio LICENSES/ es automáticamente detectado en el siguiente orden:\n"
 "\n"
-"- De LICENSES/-map in de root van de VCS-map.\n"
+"- El directorio LICENSES/ en la raíz del repositorio VCS.\n"
 "\n"
-"- De huidige map als de naam van de huidige map LICENSES/ is.\n"
+"- El directorio actual, si su nombre es LICENSES.\n"
 "\n"
-"- De LICENSES/-map in de huidige map.\n"
+"- El directorio LICENSES/ en el directorio actual.\n"
 "\n"
-"Als de LICENSES/-map niet gevonden kan worden, dan wordt er een gemaakt."
+"Si el directorio LICENSES/ no fuese encontrado, simplemente se creará uno."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
-msgstr "initialiseer REUSE-project"
+msgstr "inicia el proyecto REUSE"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
-msgstr "lijst maken van alle bestanden die tekortschieten"
+msgstr "lista todos los ficheros no compatibles"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -173,680 +198,811 @@
 "the LICENSES/ directory?\n"
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
-"Voer een statische controle op de naleving van versie {reuse_version} van de "
-"REUSE-specificatie uit. U kunt de laatste versie van de specificatie vinden "
-"op <https://reuse.software/spec/>.\n"
+"Examina el directorio del proyecto para comprobar su conformidad con la "
+"versión {reuse_version} de la Especificación REUSE. Puedes encontrar la "
+"última versión de la especificación en <https://reuse.software/spec/>\n"
 "\n"
-"De volgende criteria worden in het bijzonder gecontroleerd:\n"
+"Los siguientes criterios son específicamente chequeados:\n"
 "\n"
-"- Bevat het project slechte (niet-herkende, niet met SPDX in overeenstemming "
-"zijnde) licenties?\n"
+"- ¿Hay alguna licencia mala (no reconocida, no compatible con SPDX...) en el "
+"proyecto?\n"
 "\n"
-"- Bevat het project gerefereerde licenties die zich niet in de LICENSES/ map "
-"bevinden?\n"
+"- ¿Se hace referencia a alguna licencia dentro del proyecto, pero esta no se "
+"encuentra incluida en el directorio LICENSES/?\n"
 "\n"
-"- Bevat de map LICENSES/ licenties die binnen het project niet worden "
-"gebruikt?\n"
+"- ¿Existe alguna licencia, de las incluidas en el directorio LICENSES/, que "
+"no esté en uso en el proyecto?\n"
 "\n"
-"- Bevatten alle bestanden geldige informatie over auteursricht en licenties?"
+"- ¿Tienen todos los ficheros información válida sobre copyright y licencia?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
-msgstr "print de materiaallijst van het project in SPDX-formaat"
+msgstr "imprime la lista de materiales del proyecto en formato SPDX"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
-msgstr "Kon '{expression}' niet parsen"
+msgstr "No se pudo procesar '{expression}'"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
-msgstr "'{}' is geen bestand"
+msgstr "'{}' no es un fichero"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
-msgstr "'{}' is geen map"
+msgstr "'{}' no es un directorio"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
-msgstr "kan '{}' niet openen"
+msgstr "no se puede abrir '{}'"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
-msgstr "kan niet schrijven naar map '{}'"
+msgstr "no se pude escribir en el directorio '{}'"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
-msgstr "kan niet schrijven naar '{}'"
+msgstr "no se puede escribir en '{}'"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
-msgstr "kan '{}' niet lezen of schrijven"
+msgstr "no se puede leer o escribir '{}'"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
-msgstr "'{}' is geen geldige SPDX-uitdrukking, aan het afbreken"
+msgstr "'{}' no es una expresión SPDX válida; abortando"
+
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' no es un Identificador SPDX de Licencia válido."
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Consulta <https://spdx.org/licenses/> para obtener un listado de los "
+"Identificadores SPDX de Licencia válidos."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
-msgstr "SPDX Licentie Identificatie of licentie"
+msgstr "Identificador SPDX de la licencia"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
-msgstr ""
-"download alle ontbrekende licenties die in het project zijn gedetecteerd"
+msgstr "descargar todas las licencias no disponibles detectadas en el proyecto"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
-msgstr "Fout: {spdx_identifier} bestaat al."
+msgstr "Error: {spdx_identifier} ya existe."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
-msgstr "Fout: downloaden van licentie mislukt."
+msgstr "Error: Fallo al descargar la licencia."
 
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' is geen geldige SPDX Licentie Identificatie."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Zie <https://spdx.org/licenses/> voor een lijst met geldige SPDX Licentie "
-"Identificaties."
-
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
-msgstr "Werkt uw internetverbinding?"
+msgstr "¿Está funcionando tu conexión a Internet?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
-msgstr "{spdx_identifier} met succes gedowload."
+msgstr "{spdx_identifier} descargado con éxito."
 
-#: src/reuse/download.py:136
-msgid "the following arguments are required: license"
-msgstr "de volgende argumenten zijn verplicht: licentie"
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
 
 #: src/reuse/download.py:138
+msgid "the following arguments are required: license"
+msgstr "se requieren los siguientes parámetros: license"
+
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
-msgstr "kan --output niet met meer dan een licentie gebruiken"
+msgstr "no se puede utilizar --output con más de una licencia"
 
-#: src/reuse/header.py:101
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
-"gegenereerd commentaar mist auteursrechtregels of licentie-uitdrukkingen"
+"el comentario generado carece del mensaje de copyright o de las frases de "
+"licencia"
+
+#: src/reuse/header.py:414
+#, python-brace-format
+msgid ""
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
+msgstr ""
 
-#: src/reuse/header.py:280
+#: src/reuse/header.py:421
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
-"explicit-license"
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"'{path}' carece de una extensión de fichero conocida: por favor, utiliza --"
+"style o --explicit-license"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
+msgstr ""
+
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
 msgstr ""
-"'{path}' heeft geen erkende bestandsextensie; gebruik alstublieft --style of "
-"--explicit-license"
 
-#: src/reuse/header.py:339
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
-msgstr "Fout: Kon geen commentaar voor '{path}' creëren"
+msgstr "Error: No se pudo crear un comentario para '{path}'"
 
-#: src/reuse/header.py:346
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
-"Fout: de gegenereerde commentaarheader voor '{path}' mist auteursrechtregels "
-"of licentie-uitdrukkingen. Het sjabloon is waarschijnlijk niet correct. "
-"Schreef geen nieuwe header."
+"Error: La cabecera de comentario generada para '{path}' carece del mensaje "
+"de copyright o de las frases de licencia; la plantilla seguramente es "
+"incorrecta. No se ha escrito una nueva cabecera."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:357
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
-msgstr "Succesvolle verandering van de header van {path}"
+msgstr "Cabecera de {path} correctamente cambiada"
 
-#: src/reuse/header.py:370
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
-msgstr "auteursrechtverklaring (herhaalbaar)"
+msgstr "declaración de los derechos de autor, repetible"
 
-#: src/reuse/header.py:377
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
-msgstr "SPDX Identificatie (herhaalbaar)"
+msgstr "Identificador SPDX, repetible"
+
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "Identificador SPDX, repetible"
 
-#: src/reuse/header.py:384
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
-msgstr "jaar van auteursrechtverklaring (optie)"
+msgstr "año de la declaración de copyright; opcional"
 
-#: src/reuse/header.py:392
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
-msgstr "te gebruiken commentaarstijl (optie)"
+msgstr "estilo de comentario a utilizar; opcional"
 
-#: src/reuse/header.py:399
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "estilo de comentario a utilizar; opcional"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
-msgstr "naam van het te gebruiken sjabloon (optie)"
+msgstr "nombre de la plantilla a utilizar; opcional"
 
-#: src/reuse/header.py:404
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
-msgstr "voeg geen jaar toe aan verklaring"
+msgstr "no incluir el año en la declaración"
 
-#: src/reuse/header.py:409
-msgid "place header in path.license instead of path"
-msgstr "plaats header in path.license in plaats van path"
-
-#: src/reuse/header.py:417
-msgid "option --copyright or --license is required"
-msgstr "de optie --copyright of --license is vereist"
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "año de la declaración de copyright; opcional"
 
-#: src/reuse/header.py:421
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "estilo de comentario a utilizar; opcional"
+
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "estilo de comentario a utilizar; opcional"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
+
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
+
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
+msgstr "una de estas opciones es necesaria: --copyright o --license"
+
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
-msgstr "de opties --exclude-year en --year sluiten elkaar uit"
+msgstr "las opciones -exclude-year y --year son mutuamente excluyentes"
+
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "las opciones -exclude-year y --year son mutuamente excluyentes"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
 
-#: src/reuse/header.py:437
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
-msgstr "sjabloon {template} kon niet worden gevonden"
+msgstr "no pudo encontrarse la plantilla {template}"
 
-#: src/reuse/header.py:469
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr ""
-"'{path}' is een binary; daarom wordt '{new_path}' gebruikt voor de header"
+"'{path}' es un fichero binario: en consecuencia, se utiliza '{new_path}' "
+"para la cabecera"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
 msgstr ""
-"Onder welke licentie valt uw project? Voeg de SPDX Licientie Identificatie "
-"toe."
+"¿Bajo qué licencia se encuentra tu proyecto? Aporta el Identificador SPDX de "
+"Licencia."
 
 #: src/reuse/init.py:29
 msgid ""
 "What other license is your project under? Provide the SPDX License "
 "Identifier."
 msgstr ""
-"Onder welke andere licentie valt uw project? Voeg de SPDX Licientie "
-"Identificatie toe."
+"¿Bajo qué otras licencias se encuentra tu proyecto? Proporciona el "
+"Identificador SPDX de Licencia."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
-msgstr "Typ RETURN om te stoppen met het toevoegen van licenties."
+msgstr "Para terminar de añadir licencias pulsa RETORNO."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
-msgstr "Project al geïnitialiseerd"
+msgstr "Proyecto ya inicializado"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
-msgstr "Project voor REUSE initialiseren."
+msgstr "Inicializando el proyecto para REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
-msgstr "Wat is de naam van het project?"
+msgstr "¿Cuál es el nombre del proyecto?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
-msgstr "Wat is het internetadres van het project?"
+msgstr "¿Cuál es la dirección de Internet del proyecto?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
-msgstr "Wat is de naam van de beheerder?"
+msgstr "¿Cuál es el nombre del mantenedor?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
-msgstr "Wat is het e-mailadres van de beheerder?"
+msgstr "¿Cuál es la dirección de correo electrónico del mantenedor?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
-msgstr "Klaar! Nu aan het initialiseren."
+msgstr "¡Ya hemos terminado! Iniciando."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
-msgstr "{} aan het downloaden"
+msgstr "Descargando {}"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
-msgstr "{} bestaat al"
+msgstr "{} ya existe"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
-msgstr "Kon {} niet downloaden"
+msgstr "No se pudo descargar {}"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
-msgstr ".reuse/dep5 aan het creëren"
+msgstr "Creando .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
-msgstr "Initialisatie voltooid."
+msgstr "Inicialización completa."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"Gefeliciteerd! Uw project leeft nu versie {} van de REUSE-specificatie na :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
-msgstr "Helaas leeft uw project versie {} van de REUSE-specificatie niet na :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
+msgstr ""
+
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
+msgstr ""
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
-msgstr "SLECHTE LICENTIES"
+msgstr "LICENCIAS MALAS"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
-msgstr "'{}' gevonden in:"
+msgstr "'{}' encontrado en:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
-msgstr "VEROUDERDE LICENTIES"
+msgstr "LICENCIAS OBSOLETAS"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
-msgstr "De volgende licenties zijn verouderd door SPDX:"
+msgstr "Las siguientes licencias han quedado obsoletas según SPDX:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
-msgstr "LICENTIES ZONDER BESTANDSEXTENSIE"
+msgstr "LICENCIAS SIN EXTENSIÓN DE FICHERO"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
-msgstr "De volgende licenties hebben geen bestandsextensie:"
+msgstr "Las siguientes licencias no tienen extensión de fichero:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
-msgstr "ONTBREKENDE LICENTIES"
+msgstr "LICENCIAS NO ENCONTRADAS"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
-msgstr "ONGEBRUIKTE LICENTIES"
+msgstr "LICENCIAS NO UTILIZADAS"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
-msgstr "De volgende licenties zijn niet gebruikt:"
+msgstr "Las siguientes licencias no son utilizadas:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
-msgstr "LEES FOUTEN"
+msgstr "ERRORES DE LECTURA"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
-msgstr "Kon niet lezen:"
+msgstr "No se pudo leer:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
-msgstr "AUTEURSRECHT- EN LICENTIE-INFORMATIE ONTBREEKT"
+msgstr "FALTA INFORMACIÓN SOBRE COPYRIGHT Y LICENCIA"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
-"De volgende bestanden bevatten geen auteursrecht- en licentie-informatie:"
+"Los siguientes archivos carecen de información de copyright y licencia:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
-msgstr "De volgende bestanden hebben geen auteursrechtinformatie:"
+msgstr "Los siguientes ficheros carecen de información de copyright:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
-msgstr "De volgende bestanden bevatten geen licentie-informatie:"
+msgstr "Los siguientes ficheros carecen de información de licencia:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
-msgstr "SAMENVATTING"
+msgstr "RESUMEN"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
-msgstr "Slechte licenties:"
+msgstr "Licencias malas:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
-msgstr "Verouderde licenties:"
+msgstr "Licencias obsoletas:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
-msgstr "Licenties zonder bestandsextensie:"
+msgstr "Licencias sin extensión de fichero:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
-msgstr "Ontbrekende licenties:"
+msgstr "Licencias no encontradas:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
-msgstr "Ongebruikte licenties:"
+msgstr "Licencias no utilizadas:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
-msgstr "Gebruikte licenties:"
+msgstr "Licencias utilizadas:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
-msgstr "Lees fouten: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
+msgstr "Errores de lectura: {count}"
+
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
+msgstr "Ficheros con información sobre copyright: {count} / {total}"
+
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
+msgstr "Ficheros con información de licencia: {count} / {total}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
-msgstr "Bestanden met auteursrechtinformatie: {count} / {total}"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr ""
+"¡Enhorabuena! Tu proyecto es compatible con la versión {} de la "
+"Especificación REUSE :-)"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
-msgstr "Bestanden met licentie-informatie: {count} / {total}"
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Desafortunadamente, tu proyecto no es compatible con la versión {} de la "
+"Especificación REUSE :-("
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "kon Git niet vinden"
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
-msgstr "'{path}' valt onder .reuse/dep5"
+msgstr "'{path}' cubierto por .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
-"'{path}' bevat een SPDX-uitdrukking die niet geparsed kan worden; sla het "
-"bestand over"
+"'{path}' posee una expresión SPDX que no puede ser procesada; omitiendo el "
+"archivo"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
-msgstr ".reuse/dep5 kent syntaxfouten"
+msgstr ".reuse/dep5 presenta errores de sintaxis"
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
+
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
-msgstr "identificatie van '{path}' bepalen"
+msgstr "determinando el identificador de '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
-msgstr "{path} heeft geen bestandsextensie"
+msgstr "{path} no tiene extensión de fichero"
 
-# Niet helemaal duidelijk hoe resolving hier wordt bedoeld.
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
-"Kon de SPDX Licentie Identificatie van {path} niet bepalen, dus gebruiken we "
-"{identifier}. Zorg ervoor dat de licentie zich in de licentielijst bevind "
-"die gevonden kan worden op <https://spdx.org/licenses/> of dat deze begint "
-"met 'LicenseRef-' en dat deze een bestandsextensie heeft."
+"No pudo detectarse el Identificador SPDX de Licencia de {path}: detectando "
+"{identifier}. Asegúrate de que la licencia consta en la lista de licencias "
+"alojada en <https://spdx.org/licenses/>, o de que empieza por 'LicenseRef-', "
+"y de que posee una extensión de fichero."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
-"{identifier} is de SPDX Licentie Identificatie van zowel {path} als "
+"{identifier} es el Identificador SPDX de Licencia, tanto de {path}, como de "
 "{other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
-msgstr "Kon '{path}' niet lezen"
+msgstr "No se pudo leer '{path}'"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
-msgstr "Onverwachte fout vond plaats tijdens het parsen van '{path}'"
+msgstr "Se produjo un error inesperado al procesar '{path}'"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' eindigt niet met .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
-msgstr "gebruik: "
+msgstr "uso: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
-msgstr ".__call__() is niet gedefinieerd"
+msgstr ".__call__() no definido"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
-msgstr "onbekende parser %(parser_name)r (keuzes: %(choices)s)"
+msgstr ""
+"analizador sintáctico desconocido: %(parser_name)r (alternativas: "
+"%(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
-msgstr "argument \"-\" met mode %r"
+msgstr "parámetro \"-\" con modo %r"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "kan '%s' niet openen: %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "no se puede abrir '%(filename)s': %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
-msgstr "kan acties niet samenvoegen - twee groepen delen de naam %r"
+msgstr "no se pueden fusionar las acciones: dos grupos se llaman %r"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
-msgstr "'required' is een ongeldig argument voor positionele argumenten"
+msgstr "'required' es un argumento posicional inválido"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
-"ongeldige optiestring %(option)r: moet beginnen met een karakter "
-"%(prefix_chars)r"
+"Opción no válida %(option)r: Debe comenzar con una letra %(prefix_chars)r"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
-msgstr "dest= is benodigd voor opties zoals %r"
+msgstr "se requiere dest= para opciones como %r"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
-msgstr "ongeldige conflictresolutiewaarde: %r"
+msgstr "valor no válido de conflict_resolution: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
-msgstr[0] "tegenstrijdige optiestring: %s"
-msgstr[1] "tegenstrijdige optiestrings: %s"
+msgstr[0] "cadena de opción conflictiva: %s"
+msgstr[1] "cadenas de opción conflictivas: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
-msgstr "argumenten die elkaar uitsluiten moeten optioneel zijn"
+msgstr "los parámetros mutuamente excluyentes deben ser opcionales"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
-msgstr "positionele argumenten"
+msgstr "parámetros posicionales"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
-msgstr "optionele argumenten"
+msgstr "parámetros opcionales"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
-msgstr "dit helpbericht laten zien en verlaten"
+msgstr "mostrar este mensaje de ayuda y salir"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
-msgstr "kan niet meerdere subparser-argumenten hebben"
+msgstr "no puede contener múltiples parámetros del subanalizador sintáctico"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2276
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
-msgstr "niet erkende argumenten: %s"
+msgstr "parámetros no reconocidos: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
-msgstr "niet toegestaan met argument %s"
+msgstr "no permitido con el parámetro %s"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
-msgstr "expliciet argument %r genegeerd"
+msgstr "parámetro explícito ignorado: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
-msgstr "de volgende argumenten zijn verplicht: %s"
+msgstr "los siguientes parámetros son obligatorios: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
-msgstr "één van de argumenten %s is benodigd"
+msgstr "se requiere uno de los parámetros %s"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
-msgstr "verwachtte één argument"
+msgstr "se espera un parámetro"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
-msgstr "verwachtte maximaal één argument"
+msgstr "se espera un parámetro, como máximo"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
-msgstr "verwachtte minimaal één argument"
+msgstr "se espera un parámetro, como mínimo"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2096
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
-msgstr[0] "verwachtte %s argument"
-msgstr[1] "verwachtte %s argumenten"
+msgstr[0] "se espera el parámetro %s"
+msgstr[1] "se esperan los parámetros %s"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2156
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
-msgstr ""
-"dubbelzinnige optie: %(option)s zou ook gelijk kunnen zijn aan %(matches)s"
+msgstr "opción ambigua: %(option)s podría coincidir con %(matches)s"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2219
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
-msgstr "onverwachtte optiestring: %s"
+msgstr "cadena de opción inesperada: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2416
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
-msgstr "%r is niet callable"
+msgstr "%r no se puede invocar"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2433
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
-msgstr "ongeldige %(type)s waarde: %(value)r"
+msgstr "valor no válido de %(type)s: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2444
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
-msgstr "ongeldige keuze: %(value)r (kiezen uit %(choices)s)"
+msgstr "opción inválida: %(value)r (opciones: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2520
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
-msgstr "%(prog)s: fout: %(message)s\n"
+msgstr "%(prog)s: error: %(message)s\n"
 
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "kan '%(filename)s' niet openen: %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "cadena de opción conflictiva: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "cadena de opción conflictiva: %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "no se puede abrir '%s': %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "coloca la cabecera en path.license, en lugar de path"
+
+#~ msgid "could not find Git"
+#~ msgstr "no se pudo encontrar Git"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' no acaba en .spdx"
 
 #~ msgid "yielding %s"
-#~ msgstr "%s aan het verwerken"
+#~ msgstr "apuntando a %s"
 
 #~ msgid "currently walking in %s"
-#~ msgstr "aan het lopen door %s"
+#~ msgstr "actualmente recorriendo %s"
 
 #~ msgid "ignoring %s"
-#~ msgstr "%s negeren"
+#~ msgstr "ignorando %s"
 
 #~ msgid "searching %s for reuse information"
-#~ msgstr "%s aan het doorzoeken voor reuse informatie"
+#~ msgstr "buscando información de reuse en %s"
 
 #~ msgid "%s could not be decoded"
-#~ msgstr "%s kon niet gedecodeerd worden"
+#~ msgstr "%s no se pudo decodificar"
 
 #~ msgid "%s covered by debian/copyright"
-#~ msgstr "debian/copyright omvat %s"
+#~ msgstr "%s cubierto por debian/copyright"
 
 #~ msgid ""
 #~ "{path} is licensed under {identifier}, but its license file could not be "
 #~ "found"
 #~ msgstr ""
-#~ "{path} valt onder {identifier}, maar het licentiebestand kon niet "
-#~ "gevonden worden"
+#~ "{path} con licencia {identifier}, pero no se encontró el archivo con la "
+#~ "licencia"
 
 #~ msgid "searching %s for license tags"
-#~ msgstr "%s aan het doorzoeken voor licentie-tags"
+#~ msgstr "buscando etiquetas de licencia en %s"
 
 #~ msgid ""
 #~ "Could not resolve SPDX identifier of {path}, resolving to {identifier}"
-#~ msgstr "Kon SPDX-identifier van {path} niet oplossen, gebruik {identifier}"
+#~ msgstr ""
+#~ "No se pudo resolver el identificador SPDX de {path}, resolviendo a "
+#~ "{identifier}"
 
 #~ msgid "no debian/copyright file, or could not read it"
-#~ msgstr "geen debian/copyright bestand, of kon het niet lezen"
+#~ msgstr "no existe o no se pudo leer el archivo debian/copyright"
 
 #~ msgid "reuse  Copyright (C) 2017-2018  Free Software Foundation Europe e.V."
 #~ msgstr ""
-#~ "reuse  Auteursrecht (C) 2017-2018  Free Software Foundation Europe e.V."
+#~ "Copyright (C) 2017-2018 de reuse Free Software Foundation Europe e.V."
 
 #~ msgid ""
 #~ "reuse is free software: you can redistribute it and/or modify it under "
 #~ "the terms of the GNU General Public License as published by the Free "
 #~ "Software Foundation, either version 3 of the License, or (at your option) "
 #~ "any later version.\n"
 #~ "\n"
@@ -854,48 +1010,47 @@
 #~ "WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS "
 #~ "FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more "
 #~ "details.\n"
 #~ "\n"
 #~ "You should have received a copy of the GNU General Public License along "
 #~ "with reuse.  If not, see <http://www.gnu.org/licenses/>."
 #~ msgstr ""
-#~ "reuse is vrije software: u mag het herdistribueren en/of wijzigen onder "
-#~ "de voorwaarden van de GNU Algemene Publieke Licentie zoals gepubliceerd "
-#~ "door de Free Software Foundation, onder versie 3 van de Licentie of (naar "
-#~ "uw keuze) elke latere versie.\n"
-#~ "\n"
-#~ "reuse is gedistribueerd in de hoop dat het nuttig zal zijn maar ZONDER "
-#~ "ENIGE GARANTIE; zelfs zonder de impliciete garanties die GEBRUIKELIJK "
-#~ "ZIJN IN DE HANDEL of voor BRUIKBAARHEID VOOR EEN SPECIFIEK DOEL.  Zie de "
-#~ "GNU Algemene Publieke Licentie voor meer details.\n"
-#~ "\n"
-#~ "U hoort een kopie van de GNU Algemene Publieke Licentie te hebben "
-#~ "ontvangen samen met reuse.  Als dat niet het geval is, zie <http://www."
-#~ "gnu.org/licenses/>."
+#~ "reuse es software libre: puedes redistribuirlo y/o modificarlo bajo los "
+#~ "términos de la Licencia Pública General GNU (GNU GPL) tal y como está "
+#~ "publicada por la Free Software Foundation, tanto la versión 3 de la "
+#~ "Licencia, o (a tu elección) cualquier versión posterior.\n"
+#~ "\n"
+#~ "reuse se distribuye con la esperanza de ser útil, pero SIN NINGUNA "
+#~ "GARANTIA; ni siquiera la garantia implícita de COMERCIABILIDAD o "
+#~ "ADECUACIÓN PARA UN PROPÓSITO PARTICULAR. Consulta la Licencia Pública "
+#~ "General GNU para más detalles.\n"
+#~ "\n"
+#~ "Deberías haber recibido una copia de la Licencia Pública General GNU con "
+#~ "reuse. Si no es así, consulta <http://www.gnu.org/licenses/>."
 
 #~ msgid "IMPORTANT:"
-#~ msgstr "BELANGRIJK:"
+#~ msgstr "IMPORTANTE:"
 
 #~ msgid ""
 #~ "You do not have pygit2 installed.  reuse will slow down significantly "
 #~ "because of this.  For better performance, please install your "
 #~ "distribution's version of pygit2."
 #~ msgstr ""
-#~ "U heeft pygit2 niet geïnstalleerd.  reuse zal hierdoor significant "
-#~ "langzamer draaien.  Voor betere prestatie, installeer alstublieft uw "
-#~ "distributie's versie van pygit2."
+#~ "No tienes instalado pygit2 por lo que reuse funcionará significativamente "
+#~ "más lento. Por favor, instala la versión de pygit2 de tu distribución "
+#~ "para un mejor rendimiento."
 
 #~ msgid "could not read %s"
-#~ msgstr "kon %s niet lezen"
+#~ msgstr "no se pudo leer %s"
 
 #~ msgid "none\n"
-#~ msgstr "geen\n"
+#~ msgstr "nada\n"
 
 #~ msgid "do not use debian/copyright to extract reuse information"
-#~ msgstr "debian/copyright niet gebruiken om reuse informatie te extraheren"
+#~ msgstr "no use debian/copyright para extraer información de reuse"
 
 #~ msgid ""
 #~ "List all non-compliant files.\n"
 #~ "\n"
 #~ "A file is non-compliant when:\n"
 #~ "\n"
 #~ "- It has no copyright information.\n"
@@ -905,33 +1060,33 @@
 #~ "- Its license could not be found.\n"
 #~ "\n"
 #~ "This prints only the paths of the files that do not comply, each file on "
 #~ "a separate line.\n"
 #~ "\n"
 #~ "Error and warning messages are output to STDERR."
 #~ msgstr ""
-#~ "Lijst maken van niet-voldoenende bestanden.\n"
+#~ "Lista todos los ficheros no compatibles.\n"
 #~ "\n"
-#~ "Een bestand voldoet niet als:\n"
+#~ "Un fichero es no compatible si:\n"
 #~ "\n"
-#~ "- Het geen auteursrechtinformatie heeft.\n"
+#~ "- no tiene información de copyright.\n"
 #~ "\n"
-#~ "- Het geen licentie heeft (gegeven als SPDX-uitdrukking).\n"
+#~ "- no tiene licencia (declarada como una expresión SPDX).\n"
 #~ "\n"
-#~ "- Zijn licentie niet gevonden kan worden.\n"
+#~ "- su licencia no se encuentra.\n"
 #~ "\n"
-#~ "Dit print enkel de paden van de bestanden die niet voldoen.  Elk bestand "
-#~ "heeft zijn eigen regel.\n"
+#~ "Esto imprime únicamente las rutas de los ficheros no compatibles, cada "
+#~ "fichero en una línea separada.\n"
 #~ "\n"
-#~ "Fout- en waarschuwingsmeldingen worden geprint naar STDERR."
+#~ "Los mensajes de error y aviso se muestran en STDERR."
 
 #~ msgid "SPDX expressions are mandatory for compliance"
-#~ msgstr "SPDX-uitdrukkingen zijn verplicht voor voldoening"
+#~ msgstr "Las expresiones SPDX son de obligatorio cumplimiento"
 
 #~ msgid "copyright notices are mandatory for compliance"
-#~ msgstr "auteursrechtnotities zijn verplicht voor voldoening"
+#~ msgstr "las notas de copyright son de obligatorio cumplimiento"
 
 #~ msgid "print the SPDX expressions of each provided file"
-#~ msgstr "de SPDX-uitdrukkingen van elke gegeven file printen"
+#~ msgstr "imprime las expresiones SPDX de cada fichero proporcionado"
 
 #~ msgid "reuse, version {}\n"
-#~ msgstr "reuse, versie {}\n"
+#~ msgstr "reuse, versión {}\n"
```

### Comparing `reuse-2.0.0/po/pt.po` & `reuse-2.1.0/po/pt.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,123 @@
 # SPDX-FileCopyrightText: 2020 José Vieira <jvieira33@sapo.pt>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-01-09 13:51+0100\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: 2023-06-21 09:53+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Portuguese <https://hosted.weblate.org/projects/fsfe/"
-"reuse-tool/pt/>\n"
+"Language-Team: Portuguese <https://hosted.weblate.org/projects/fsfe/reuse-"
+"tool/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.18.1\n"
 
-#: src/reuse/_main.py:30
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
 "O reuse é uma ferramenta para observância das recomendações REUSE. Ver "
 "<https://reuse.software/> para mais informação e <https://reuse.readthedocs."
 "io/> para documentação em linha."
 
-#: src/reuse/_main.py:36
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr ""
 "Esta versão do reuse é compatível com a versão {} da especificação REUSE."
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
 msgstr "Apoiar o trabalho da FSFE:"
 
-#: src/reuse/_main.py:43
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
 "Os donativos são cruciais para a nossa força e autonomia. Permitem-nos "
 "continuar a trabalhar em prol do Sotware Livre sempre que necessário. "
 "Considere fazer um donativo em <https://fsfe.org/donate/>."
 
-#: src/reuse/_main.py:66
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
 msgstr "activar expressões de depuração"
 
-#: src/reuse/_main.py:71
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
 msgstr "não ignorar sub-módulos do Git"
 
-#: src/reuse/_main.py:76
+#: src/reuse/_main.py:85
+#, fuzzy
+msgid "do not skip over Meson subprojects"
+msgstr "não ignorar sub-módulos do Git"
+
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
 msgstr "não usar multi-processamento"
 
-#: src/reuse/_main.py:83
+#: src/reuse/_main.py:97
 msgid "define root of project"
 msgstr "definir a raíz do projecto"
 
-#: src/reuse/_main.py:88
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
 msgstr "mostrar o número de versão do programa e sair"
 
-#: src/reuse/_main.py:92
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr "sub-comandos"
 
-#: src/reuse/_main.py:99
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
 msgstr "adicionar direitos de autor e licenciamento ao cabeçalho dos ficheiros"
 
-#: src/reuse/_main.py:102
+#: src/reuse/_main.py:116
+#, fuzzy
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
+"By using --contributor, you can specify people or entity that contributed "
+"but are not copyright holder of the given files.\n"
+"The first comment is replaced with a new header containing the new copyright "
+"and licensing information and its former copyright and licensing. If you "
+"want to keep the first comment intact, use --no-replace.\n"
+"\n"
 "The comment style should be auto-detected for your files. If a comment style "
-"could not be detected, the process aborts. Use --style to specify or "
-"override the comment style to use.\n"
+"could not be detected and --skip-unrecognised is not specified, the process "
+"aborts. Use --style to specify or override the comment style to use.\n"
+"\n"
+"A single-line comment style is used when it is available. If no single-line "
+"comment style is available, a multi-line comment style is used. You can "
+"force a certain comment style using --single-line or --multi-line.\n"
 "\n"
 "You can change the template of the header comment by using --template. Place "
 "a Jinja2 template in .reuse/templates/mytemplate.jinja2. You can use the "
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
-"header is placed in a .license file.\n"
-"\n"
-"IMPORTANT: This is currently EXPERIMENTAL!"
+"header is placed in a .license file."
 msgstr ""
 "Adicionar direitos de autor e licenciamento ao cabeçalho de um ou mais "
 "ficheiros.\n"
 "\n"
 "Usando --copyright e --license, pode-se especificar que detentores de "
 "direitos de autor e que licenças adicionar aos cabeçalhos dos ficheiros em "
 "causa.\n"
@@ -115,19 +133,23 @@
 "documentação em linha para informação adicional sobre esta funcionalidade.\n"
 "\n"
 "Se for detectado um ficheiro binário ou se for especificado --explicit-"
 "license, o cabeçalho é colocado num ficheiro .license\n"
 "\n"
 "IMPORTANTE: Presentemente esta funcionalidade é EXPERIMENTAL!"
 
-#: src/reuse/_main.py:135
+#: src/reuse/_main.py:159
+msgid "deprecated in favor of annotate"
+msgstr ""
+
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr "descarregar uma licença e guardá-la na pasta LICENSES/"
 
-#: src/reuse/_main.py:138
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
@@ -145,23 +167,23 @@
 "\n"
 "- Pasta actual se o nome for LICENSES.\n"
 "\n"
 "- Pasta LICENSES/ na pasta actual.\n"
 "\n"
 "Se não for encontrada, a pasta LICENSES/ será criada."
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
 msgstr "iniciar um projecto REUSE"
 
-#: src/reuse/_main.py:169
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
 msgstr "listar todos os ficheiros não conformes"
 
-#: src/reuse/_main.py:172
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -191,176 +213,270 @@
 "\n"
 "- Há alguma licença incluída na pasta LICENSES/ que não seja usada no "
 "projecto?\n"
 "\n"
 "- Todos os ficheiros têm informação válida de direitos de autor e de "
 "licenciamento?"
 
-#: src/reuse/_main.py:199
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
 msgstr "imprimir a lista de materiais do projecto em formato SPDX"
 
-#: src/reuse/_util.py:216
+#: src/reuse/_main.py:239
+msgid "list all supported SPDX licenses"
+msgstr ""
+
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
 msgstr "Não foi possível executar parse '{expression}'"
 
-#: src/reuse/_util.py:289
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
 msgstr "'{}' não é um ficheiro"
 
-#: src/reuse/_util.py:293
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
 msgstr "'{}' não é uma pasta"
 
-#: src/reuse/_util.py:296
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
 msgstr "não é possível abrir '{}'"
 
-#: src/reuse/_util.py:300
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
 msgstr "não é possível escrever no directório '{}'"
 
-#: src/reuse/_util.py:306
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
 msgstr "não é possível escrever em '{}'"
 
-#: src/reuse/_util.py:308
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
 msgstr "não é possível ler ou escrever em '{}'"
 
-#: src/reuse/_util.py:317
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
 msgstr "'{}' não é uma expressão SPDX válida; a abortar"
 
-#: src/reuse/download.py:80
+#: src/reuse/_util.py:544
+msgid "'{}' is not a valid SPDX License Identifier."
+msgstr "'{}' não é um Identificador de Licença SPDX válido."
+
+#: src/reuse/_util.py:551
+msgid "Did you mean:"
+msgstr ""
+
+#: src/reuse/_util.py:558
+msgid ""
+"See <https://spdx.org/licenses/> for a list of valid SPDX License "
+"Identifiers."
+msgstr ""
+"Consultar uma lista de Identificadores de Licença SPDX válidos em <https://"
+"spdx.org/licenses/>."
+
+#: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
 msgstr "Identificador de Licença SPDX da licença"
 
-#: src/reuse/download.py:85
+#: src/reuse/download.py:93
 msgid "download all missing licenses detected in the project"
 msgstr "descarregar todas as licenças detectadas como em falta no projecto"
 
-#: src/reuse/download.py:97
+#: src/reuse/download.py:105
 #, python-brace-format
 msgid "Error: {spdx_identifier} already exists."
 msgstr "Erro: {spdx_identifier} já existe."
 
-#: src/reuse/download.py:104
+#: src/reuse/download.py:112
 msgid "Error: Failed to download license."
 msgstr "Erro: Falha ao descarregar a licença."
 
-#: src/reuse/download.py:108 src/reuse/init.py:48
-msgid "'{}' is not a valid SPDX License Identifier."
-msgstr "'{}' não é um Identificador de Licença SPDX válido."
-
-#: src/reuse/download.py:115 src/reuse/init.py:55
-msgid ""
-"See <https://spdx.org/licenses/> for a list of valid SPDX License "
-"Identifiers."
-msgstr ""
-"Consultar uma lista de Identificadores de Licença SPDX válidos em "
-"<https://spdx.org/licenses/>."
-
-#: src/reuse/download.py:120
+#: src/reuse/download.py:117
 msgid "Is your internet connection working?"
 msgstr "A ligação à Internet está a funcionar?"
 
-#: src/reuse/download.py:125
+#: src/reuse/download.py:122
 #, python-brace-format
 msgid "Successfully downloaded {spdx_identifier}."
 msgstr "{spdx_identifier} transferido com êxito."
 
-#: src/reuse/download.py:136
+#: src/reuse/download.py:134
+msgid "--output has no effect when used together with --all"
+msgstr ""
+
+#: src/reuse/download.py:138
 msgid "the following arguments are required: license"
 msgstr "são requeridos os seguintes argumentos: licença"
 
-#: src/reuse/download.py:138
+#: src/reuse/download.py:140
 msgid "cannot use --output with more than one license"
 msgstr "não se pode usar --output com mais do que uma licença"
 
-#: src/reuse/header.py:103
+#: src/reuse/header.py:132
 msgid "generated comment is missing copyright lines or license expressions"
 msgstr ""
 "o comentário gerado não tem linhas de direitos de autor ou expressões de "
 "licenciamento"
 
-#: src/reuse/header.py:293
+#: src/reuse/header.py:414
 #, python-brace-format
 msgid ""
-"'{path}' does not have a recognised file extension, please use --style or --"
+"'{path}' does not support single-line comments, please do not use --single-"
+"line"
+msgstr ""
+
+#: src/reuse/header.py:421
+#, python-brace-format
+msgid ""
+"'{path}' does not support multi-line comments, please do not use --multi-line"
+msgstr ""
+
+#: src/reuse/header.py:444
+#, fuzzy
+msgid ""
+"The following files do not have a recognised file extension. Please use --"
+"style, --force-dot-license or --skip-unrecognised:"
+msgstr ""
+"'{path}' não têm uma extensão de ficheiro reconhecida; usar --style ou --"
 "explicit-license"
+
+#: src/reuse/header.py:497
+#, python-brace-format
+msgid "Skipped unrecognised file {path}"
+msgstr ""
+
+#: src/reuse/header.py:509
+#, python-brace-format
+msgid "Skipped file '{path}' already containing REUSE information"
 msgstr ""
-"'{path}' não têm uma extensão de ficheiro reconhecida; usar --style ou "
-"--explicit-license"
 
-#: src/reuse/header.py:352
+#: src/reuse/header.py:543
 #, python-brace-format
 msgid "Error: Could not create comment for '{path}'"
 msgstr "Erro: Não foi possível criar um comentário para '{path}'"
 
-#: src/reuse/header.py:359
+#: src/reuse/header.py:550
 #, python-brace-format
 msgid ""
 "Error: Generated comment header for '{path}' is missing copyright lines or "
 "license expressions. The template is probably incorrect. Did not write new "
 "header."
 msgstr ""
 "Erro: O cabeçalho de comentário gerado para '{path}' não contém linhas de "
 "direitos de autor ou expressões de licenciamento. Provavelmente o modelo não "
 "está correcto. Não foi escrito nenhum novo cabeçalho."
 
 #. TODO: This may need to be rephrased more elegantly.
-#: src/reuse/header.py:370
+#: src/reuse/header.py:561
 #, python-brace-format
 msgid "Successfully changed header of {path}"
 msgstr "O cabeçalho de {path} foi alterado com êxito"
 
-#: src/reuse/header.py:383
+#: src/reuse/header.py:586
 msgid "copyright statement, repeatable"
 msgstr "declaração de direitos de autor (repetível)"
 
-#: src/reuse/header.py:390
+#: src/reuse/header.py:593
 msgid "SPDX Identifier, repeatable"
 msgstr "Identificador SPDX (repetível)"
 
-#: src/reuse/header.py:397
+#: src/reuse/header.py:599
+#, fuzzy
+msgid "file contributor, repeatable"
+msgstr "Identificador SPDX (repetível)"
+
+#: src/reuse/header.py:606
 msgid "year of copyright statement, optional"
 msgstr "ano da declaração de direitos de autor (opcional)"
 
-#: src/reuse/header.py:405
+#: src/reuse/header.py:614
 msgid "comment style to use, optional"
 msgstr "estilo de comentário a usar (opcional)"
 
-#: src/reuse/header.py:412
+#: src/reuse/header.py:620
+#, fuzzy
+msgid "copyright style to use, optional"
+msgstr "estilo de comentário a usar (opcional)"
+
+#: src/reuse/header.py:627
 msgid "name of template to use, optional"
 msgstr "nome do modelo a usar (opcional)"
 
-#: src/reuse/header.py:417
+#: src/reuse/header.py:632
 msgid "do not include year in statement"
 msgstr "não incluir o ano na declaração"
 
-#: src/reuse/header.py:422
-msgid "place header in path.license instead of path"
-msgstr "colocar o cabeçalho em path.license em vez de em path"
+#: src/reuse/header.py:637
+#, fuzzy
+msgid "merge copyright lines if copyright statements are identical"
+msgstr "ano da declaração de direitos de autor (opcional)"
+
+#: src/reuse/header.py:642
+#, fuzzy
+msgid "force single-line comment style, optional"
+msgstr "estilo de comentário a usar (opcional)"
+
+#: src/reuse/header.py:647
+#, fuzzy
+msgid "force multi-line comment style, optional"
+msgstr "estilo de comentário a usar (opcional)"
+
+#: src/reuse/header.py:657
+msgid "write a .license file instead of a header inside the file"
+msgstr ""
+
+#: src/reuse/header.py:664
+msgid "add headers to all files under specified directories recursively"
+msgstr ""
+
+#: src/reuse/header.py:671
+msgid "do not replace the first header in the file; just add a new one"
+msgstr ""
+
+#: src/reuse/header.py:677
+msgid "skip files with unrecognised comment styles"
+msgstr ""
+
+#: src/reuse/header.py:682
+msgid "skip files that already contain REUSE information"
+msgstr ""
 
-#: src/reuse/header.py:430
-msgid "option --copyright or --license is required"
+#: src/reuse/header.py:693
+msgid "'reuse addheader' has been deprecated in favour of 'reuse annotate'"
+msgstr ""
+
+#: src/reuse/header.py:700
+#, fuzzy
+msgid "option --contributor, --copyright or --license is required"
 msgstr "é requerida uma das opções --copyright ou --license"
 
-#: src/reuse/header.py:434
+#: src/reuse/header.py:705
 msgid "option --exclude-year and --year are mutually exclusive"
 msgstr "as opções --exclude-year e --year são mutuamente exclusivas"
 
-#: src/reuse/header.py:450
+#: src/reuse/header.py:710
+#, fuzzy
+msgid "option --single-line and --multi-line are mutually exclusive"
+msgstr "as opções --exclude-year e --year são mutuamente exclusivas"
+
+#: src/reuse/header.py:716
+msgid "--skip-unrecognised has no effect when used together with --style"
+msgstr ""
+
+#: src/reuse/header.py:723
+msgid "--explicit-license has been deprecated in favour of --force-dot-license"
+msgstr ""
+
+#: src/reuse/header.py:767
 #, python-brace-format
 msgid "template {template} could not be found"
 msgstr "o modelo {template} não foi encontrado"
 
-#: src/reuse/header.py:482
+#: src/reuse/header.py:819
 #, python-brace-format
 msgid "'{path}' is a binary, therefore using '{new_path}' for the header"
 msgstr "'{path}' é binário, por isso é usado '{new_path}' para o cabeçalho"
 
 #: src/reuse/init.py:25
 msgid ""
 "What license is your project under? Provide the SPDX License Identifier."
@@ -375,430 +491,463 @@
 "Sob que outra licença está o projecto? Indicar o Identificador de Licença "
 "SPDX."
 
 #: src/reuse/init.py:40
 msgid "To stop adding licenses, hit RETURN."
 msgstr "Para parar a agregação de licenças, premir INTRODUZIR/ENTER."
 
-#: src/reuse/init.py:85
+#: src/reuse/init.py:78
 msgid "Project already initialized"
 msgstr "Projecto já iniciado"
 
-#: src/reuse/init.py:89
+#: src/reuse/init.py:82
 msgid "Initializing project for REUSE."
 msgstr "A iniciar o projecto para REUSE."
 
-#: src/reuse/init.py:94
+#: src/reuse/init.py:87
 msgid "What is the name of the project?"
 msgstr "Qual é o nome do projecto?"
 
-#: src/reuse/init.py:100
+#: src/reuse/init.py:93
 msgid "What is the internet address of the project?"
 msgstr "Qual é o endereço do projecto na internet?"
 
-#: src/reuse/init.py:106
+#: src/reuse/init.py:99
 msgid "What is the name of the maintainer?"
 msgstr "Qual é o nome do responsável (maintainer)?"
 
-#: src/reuse/init.py:112
+#: src/reuse/init.py:105
 msgid "What is the e-mail address of the maintainer?"
 msgstr "Qual é o endereço electrónico do responsável?"
 
-#: src/reuse/init.py:118
+#: src/reuse/init.py:111
 msgid "All done! Initializing now."
 msgstr "Pronto! A iniciar."
 
-#: src/reuse/init.py:126
+#: src/reuse/init.py:119
 msgid "Downloading {}"
 msgstr "A descarregar {}"
 
-#: src/reuse/init.py:131
+#: src/reuse/init.py:124
 msgid "{} already exists"
 msgstr "{} já existe"
 
-#: src/reuse/init.py:134
+#: src/reuse/init.py:127
 msgid "Could not download {}"
 msgstr "Não foi possível descarregar {}"
 
-#: src/reuse/init.py:139
+#: src/reuse/init.py:132
 msgid "Creating .reuse/dep5"
 msgstr "A criar .reuse/dep5"
 
-#: src/reuse/init.py:162
+#: src/reuse/init.py:155
 msgid "Initialization complete."
 msgstr "Iniciação completada."
 
-#: src/reuse/lint.py:55
-msgid ""
-"Congratulations! Your project is compliant with version {} of the REUSE "
-"Specification :-)"
+#: src/reuse/lint.py:27
+msgid "prevents output"
 msgstr ""
-"Parabéns! O projecto está conforme com a versão {} da especificação REUSE :-)"
 
-#: src/reuse/lint.py:62
-msgid ""
-"Unfortunately, your project is not compliant with version {} of the REUSE "
-"Specification :-("
+#: src/reuse/lint.py:30
+msgid "formats output as JSON"
 msgstr ""
-"Infelizmente, o projecto não está conforme com a versão {} da especificação "
-"REUSE :-("
 
-#: src/reuse/lint.py:79
+#: src/reuse/lint.py:36
+msgid "formats output as plain text"
+msgstr ""
+
+#: src/reuse/lint.py:52
 msgid "BAD LICENSES"
 msgstr "LICENÇAS IRREGULARES"
 
-#: src/reuse/lint.py:83 src/reuse/lint.py:148
+#: src/reuse/lint.py:54 src/reuse/lint.py:83
 msgid "'{}' found in:"
 msgstr "'{}' encontrado em:"
 
-#: src/reuse/lint.py:101
+#: src/reuse/lint.py:61
 msgid "DEPRECATED LICENSES"
 msgstr "LICENÇAS DESCONTINUADAS"
 
-#: src/reuse/lint.py:103
+#: src/reuse/lint.py:63
 msgid "The following licenses are deprecated by SPDX:"
 msgstr "As seguintes licenças foram descontinuadas pelo SPDX:"
 
-#: src/reuse/lint.py:121
+#: src/reuse/lint.py:71
 msgid "LICENSES WITHOUT FILE EXTENSION"
 msgstr "LICENÇAS SEM EXTENSÃO DE FICHEIRO"
 
-#: src/reuse/lint.py:123
+#: src/reuse/lint.py:73
 msgid "The following licenses have no file extension:"
 msgstr "As seguintes licenças não têm extensão de ficheiro:"
 
-#: src/reuse/lint.py:143
+#: src/reuse/lint.py:81
 msgid "MISSING LICENSES"
 msgstr "LICENÇAS EM FALTA"
 
-#: src/reuse/lint.py:166
+#: src/reuse/lint.py:90
 msgid "UNUSED LICENSES"
 msgstr "LICENÇAS NÃO USADAS"
 
-#: src/reuse/lint.py:168
+#: src/reuse/lint.py:91
 msgid "The following licenses are not used:"
 msgstr "As seguintes licenças não estão a ser usadas:"
 
-#: src/reuse/lint.py:184
+#: src/reuse/lint.py:98
 msgid "READ ERRORS"
 msgstr "ERROS DE LEITURA"
 
-#: src/reuse/lint.py:186
+#: src/reuse/lint.py:99
 msgid "Could not read:"
 msgstr "Não foi possível ler:"
 
-#: src/reuse/lint.py:209
+#: src/reuse/lint.py:120
 msgid "MISSING COPYRIGHT AND LICENSING INFORMATION"
 msgstr "INFORMAÇÃO EM FALTA SOBRE DIREITOS DE AUTOR E LICENCIAMENTO"
 
-#: src/reuse/lint.py:214
+#: src/reuse/lint.py:126
 msgid "The following files have no copyright and licensing information:"
 msgstr ""
 "Os seguintes ficheiros não contêm informação de direitos de autor nem de "
 "licenciamento:"
 
-#: src/reuse/lint.py:223
+#: src/reuse/lint.py:137
 msgid "The following files have no copyright information:"
 msgstr "Os seguintes ficheiros não contêm informação de direitos de autor:"
 
-#: src/reuse/lint.py:229
+#: src/reuse/lint.py:146
 msgid "The following files have no licensing information:"
 msgstr "Os seguintes ficheiros não contêm informação de licenciamento:"
 
-#: src/reuse/lint.py:243
+#: src/reuse/lint.py:154
 msgid "SUMMARY"
 msgstr "RESUMO"
 
-#: src/reuse/lint.py:249
+#: src/reuse/lint.py:159
 msgid "Bad licenses:"
 msgstr "Licenças irregulares:"
 
-#: src/reuse/lint.py:258
+#: src/reuse/lint.py:160
 msgid "Deprecated licenses:"
 msgstr "Licenças descontinuadas:"
 
-#: src/reuse/lint.py:267
+#: src/reuse/lint.py:161
 msgid "Licenses without file extension:"
 msgstr "Licenças sem extensão de ficheiro:"
 
-#: src/reuse/lint.py:276
+#: src/reuse/lint.py:164
 msgid "Missing licenses:"
 msgstr "Licenças em falta:"
 
-#: src/reuse/lint.py:285
+#: src/reuse/lint.py:165
 msgid "Unused licenses:"
 msgstr "Licenças não usadas:"
 
-#: src/reuse/lint.py:294
+#: src/reuse/lint.py:166
 msgid "Used licenses:"
 msgstr "Licenças usadas:"
 
-#: src/reuse/lint.py:303
-#, python-brace-format
-msgid "Read errors: {count}"
+#: src/reuse/lint.py:167
+#, fuzzy
+msgid "Read errors:"
 msgstr "Erros de leitura: {count}"
 
-#: src/reuse/lint.py:308
-#, python-brace-format
-msgid "Files with copyright information: {count} / {total}"
+#: src/reuse/lint.py:169
+#, fuzzy
+msgid "files with copyright information:"
 msgstr "Ficheiros com informação de direitos de autor: {count} / {total}"
 
-#: src/reuse/lint.py:317
-#, python-brace-format
-msgid "Files with license information: {count} / {total}"
+#: src/reuse/lint.py:173
+#, fuzzy
+msgid "files with license information:"
 msgstr "Ficheiros com informação de licenciamento: {count} / {total}"
 
-#: src/reuse/project.py:59
-msgid "could not find Git"
-msgstr "não foi encontrado o Git"
+#: src/reuse/lint.py:190
+msgid ""
+"Congratulations! Your project is compliant with version {} of the REUSE "
+"Specification :-)"
+msgstr ""
+"Parabéns! O projecto está conforme com a versão {} da especificação REUSE :-)"
+
+#: src/reuse/lint.py:197
+msgid ""
+"Unfortunately, your project is not compliant with version {} of the REUSE "
+"Specification :-("
+msgstr ""
+"Infelizmente, o projecto não está conforme com a versão {} da especificação "
+"REUSE :-("
+
+#: src/reuse/project.py:77
+msgid ""
+"project is not a VCS repository or required VCS software is not installed"
+msgstr ""
 
-#: src/reuse/project.py:133
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
 msgstr "'{path}' abrangido por .reuse/dep5"
 
-#: src/reuse/project.py:145
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
 "'{path}' inclui uma expressão SPDX que não pode ser analisada (parsed); "
 "ficheiro ignorado"
 
-#: src/reuse/project.py:231
+#: src/reuse/project.py:226
+#, python-brace-format
+msgid ""
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
+msgstr ""
+
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
 msgstr ".reuse/dep5 tem erros de sintaxe"
 
-#: src/reuse/project.py:257
+#: src/reuse/project.py:315
+msgid ".reuse/dep5 could not be parsed as utf-8"
+msgstr ""
+
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
 msgstr "a determinar o identificador de '{path}'"
 
-#: src/reuse/project.py:265
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
 msgstr "{path} não tem extensão de ficheiro"
 
-#: src/reuse/project.py:275
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
 "Não foi possível determinar o Identificador de Licença SPDX de {path}; a "
 "determinar como {identifier}. Confirmar que a licença está na lista "
 "publicada em <https://spdx.org/licenses/> ou que começa por 'LicenseRef-' e "
 "tem uma extensão de ficheiro."
 
-#: src/reuse/project.py:287
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
-msgstr "{identifier} é o Identificador de Licença SPDX de {path} e {other_path}"
+msgstr ""
+"{identifier} é o Identificador de Licença SPDX de {path} e {other_path}"
 
-#: src/reuse/report.py:206
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr "Não foi possível ler '{path}'"
 
-#: src/reuse/report.py:213
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
 msgstr "Ocorreu um erro inesperado ao analisar (parse) '{path}'"
 
 #: src/reuse/spdx.py:32
+msgid ""
+"populate the LicenseConcluded field; note that reuse cannot guarantee the "
+"field is accurate"
+msgstr ""
+
+#: src/reuse/spdx.py:39
+msgid "name of the person signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:44
+msgid "name of the organization signing off on the SPDX report"
+msgstr ""
+
+#: src/reuse/spdx.py:60
+msgid ""
+"error: --creator-person=NAME or --creator-organization=NAME required when --"
+"add-license-concluded is provided"
+msgstr ""
+
+#: src/reuse/spdx.py:75
 #, python-brace-format
-msgid "'{path}' does not end with .spdx"
-msgstr "'{path}' não termina em .spdx"
+msgid ""
+"'{path}' does not match a common SPDX file pattern. Find the suggested "
+"naming conventions here: https://spdx.github.io/spdx-spec/conformance/#44-"
+"standard-data-format-requirements"
+msgstr ""
 
-#: /usr/lib64/python3.5/argparse.py:291 /usr/lib64/python3.6/argparse.py:295
-#: /usr/lib64/python3.7/argparse.py:297 /usr/lib64/python3.8/argparse.py:295
+#: /usr/lib/python3.8/argparse.py:307
 msgid "usage: "
 msgstr "uso: "
 
-#: /usr/lib64/python3.5/argparse.py:822 /usr/lib64/python3.6/argparse.py:830
-#: /usr/lib64/python3.7/argparse.py:845 /usr/lib64/python3.8/argparse.py:846
+#: /usr/lib/python3.8/argparse.py:858
 msgid ".__call__() not defined"
 msgstr ".__call__() não definido"
 
-#: /usr/lib64/python3.5/argparse.py:1119 /usr/lib64/python3.6/argparse.py:1127
-#: /usr/lib64/python3.7/argparse.py:1148 /usr/lib64/python3.8/argparse.py:1149
+#: /usr/lib/python3.8/argparse.py:1161
 #, python-format
 msgid "unknown parser %(parser_name)r (choices: %(choices)s)"
 msgstr "analisador desconhecido %(parser_name)r (alternativas: %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:1173 /usr/lib64/python3.6/argparse.py:1181
-#: /usr/lib64/python3.7/argparse.py:1202 /usr/lib64/python3.8/argparse.py:1209
+#: /usr/lib/python3.8/argparse.py:1221
 #, python-format
 msgid "argument \"-\" with mode %r"
 msgstr "argumento \"-\" com modo %r"
 
-#: /usr/lib64/python3.5/argparse.py:1181 /usr/lib64/python3.6/argparse.py:1189
-#: /usr/lib64/python3.7/argparse.py:1210
+#: /usr/lib/python3.8/argparse.py:1230
 #, python-format
-msgid "can't open '%s': %s"
-msgstr "não é possível abrir '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
+msgstr "não é possível abrir '%(filename)s': %(error)s"
 
-#: /usr/lib64/python3.5/argparse.py:1385 /usr/lib64/python3.6/argparse.py:1393
-#: /usr/lib64/python3.7/argparse.py:1414 /usr/lib64/python3.8/argparse.py:1427
+#: /usr/lib/python3.8/argparse.py:1439
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
 msgstr "não é possível combinar as acções - há dois grupos com o nome %r"
 
-#: /usr/lib64/python3.5/argparse.py:1423 /usr/lib64/python3.6/argparse.py:1431
-#: /usr/lib64/python3.7/argparse.py:1452 /usr/lib64/python3.8/argparse.py:1465
+#: /usr/lib/python3.8/argparse.py:1477
 msgid "'required' is an invalid argument for positionals"
 msgstr "'required' não é um argumento válido para posicionais"
 
-#: /usr/lib64/python3.5/argparse.py:1445 /usr/lib64/python3.6/argparse.py:1453
-#: /usr/lib64/python3.7/argparse.py:1474 /usr/lib64/python3.8/argparse.py:1487
+#: /usr/lib/python3.8/argparse.py:1499
 #, python-format
 msgid ""
 "invalid option string %(option)r: must start with a character "
 "%(prefix_chars)r"
 msgstr ""
 "linha de opções %(option)r inválida: tem que começar com um carácter "
 "%(prefix_chars)r"
 
-#: /usr/lib64/python3.5/argparse.py:1465 /usr/lib64/python3.6/argparse.py:1473
-#: /usr/lib64/python3.7/argparse.py:1494 /usr/lib64/python3.8/argparse.py:1507
+#: /usr/lib/python3.8/argparse.py:1519
 #, python-format
 msgid "dest= is required for options like %r"
 msgstr "é requerido dest= para opções do tipo %r"
 
-#: /usr/lib64/python3.5/argparse.py:1482 /usr/lib64/python3.6/argparse.py:1490
-#: /usr/lib64/python3.7/argparse.py:1511 /usr/lib64/python3.8/argparse.py:1524
+#: /usr/lib/python3.8/argparse.py:1536
 #, python-format
 msgid "invalid conflict_resolution value: %r"
 msgstr "valor de conflict_resolution inválido: %r"
 
-#: /usr/lib64/python3.5/argparse.py:1500 /usr/lib64/python3.6/argparse.py:1508
-#: /usr/lib64/python3.7/argparse.py:1529 /usr/lib64/python3.8/argparse.py:1542
+#: /usr/lib/python3.8/argparse.py:1554
 #, python-format
 msgid "conflicting option string: %s"
 msgid_plural "conflicting option strings: %s"
 msgstr[0] "linha de opções conflituante: %s"
 msgstr[1] "linhas de opções conflituantes: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1566 /usr/lib64/python3.6/argparse.py:1574
-#: /usr/lib64/python3.7/argparse.py:1595 /usr/lib64/python3.8/argparse.py:1608
+#: /usr/lib/python3.8/argparse.py:1620
 msgid "mutually exclusive arguments must be optional"
 msgstr "argumentos mutuamente exclusivos têm que ser opcionais"
 
-#: /usr/lib64/python3.5/argparse.py:1629 /usr/lib64/python3.6/argparse.py:1637
-#: /usr/lib64/python3.7/argparse.py:1658 /usr/lib64/python3.8/argparse.py:1671
+#: /usr/lib/python3.8/argparse.py:1683
 msgid "positional arguments"
 msgstr "argumentos posicionais"
 
-#: /usr/lib64/python3.5/argparse.py:1630 /usr/lib64/python3.6/argparse.py:1638
-#: /usr/lib64/python3.7/argparse.py:1659 /usr/lib64/python3.8/argparse.py:1672
+#: /usr/lib/python3.8/argparse.py:1684
 msgid "optional arguments"
 msgstr "argumentos opcionais"
 
-#: /usr/lib64/python3.5/argparse.py:1645 /usr/lib64/python3.6/argparse.py:1653
-#: /usr/lib64/python3.7/argparse.py:1674 /usr/lib64/python3.8/argparse.py:1687
+#: /usr/lib/python3.8/argparse.py:1699
 msgid "show this help message and exit"
 msgstr "mostrar esta mensagem de ajuda e sair"
 
-#: /usr/lib64/python3.5/argparse.py:1676 /usr/lib64/python3.6/argparse.py:1684
-#: /usr/lib64/python3.7/argparse.py:1705 /usr/lib64/python3.8/argparse.py:1718
+#: /usr/lib/python3.8/argparse.py:1730
 msgid "cannot have multiple subparser arguments"
 msgstr "não pode haver argumentos múltiplos de sub-análise (subparser)"
 
-#: /usr/lib64/python3.5/argparse.py:1728 /usr/lib64/python3.6/argparse.py:1736
-#: /usr/lib64/python3.7/argparse.py:1757 /usr/lib64/python3.7/argparse.py:2263
-#: /usr/lib64/python3.8/argparse.py:1770 /usr/lib64/python3.8/argparse.py:2277
+#: /usr/lib/python3.8/argparse.py:1782 /usr/lib/python3.8/argparse.py:2289
 #, python-format
 msgid "unrecognized arguments: %s"
 msgstr "argumentos não reconhecidos: %s"
 
-#: /usr/lib64/python3.5/argparse.py:1825 /usr/lib64/python3.6/argparse.py:1833
-#: /usr/lib64/python3.7/argparse.py:1854 /usr/lib64/python3.8/argparse.py:1867
+#: /usr/lib/python3.8/argparse.py:1879
 #, python-format
 msgid "not allowed with argument %s"
 msgstr "não permitido com o argumento %s"
 
-#: /usr/lib64/python3.5/argparse.py:1871 /usr/lib64/python3.5/argparse.py:1885
-#: /usr/lib64/python3.6/argparse.py:1879 /usr/lib64/python3.6/argparse.py:1893
-#: /usr/lib64/python3.7/argparse.py:1900 /usr/lib64/python3.7/argparse.py:1914
-#: /usr/lib64/python3.8/argparse.py:1913 /usr/lib64/python3.8/argparse.py:1927
+#: /usr/lib/python3.8/argparse.py:1925 /usr/lib/python3.8/argparse.py:1939
 #, python-format
 msgid "ignored explicit argument %r"
 msgstr "argumento explícito %r ignorado"
 
-#: /usr/lib64/python3.5/argparse.py:1992 /usr/lib64/python3.6/argparse.py:2000
-#: /usr/lib64/python3.7/argparse.py:2021 /usr/lib64/python3.8/argparse.py:2034
+#: /usr/lib/python3.8/argparse.py:2046
 #, python-format
 msgid "the following arguments are required: %s"
 msgstr "são requeridos os seguintes argumentos: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2007 /usr/lib64/python3.6/argparse.py:2015
-#: /usr/lib64/python3.7/argparse.py:2036 /usr/lib64/python3.8/argparse.py:2049
+#: /usr/lib/python3.8/argparse.py:2061
 #, python-format
 msgid "one of the arguments %s is required"
 msgstr "é requerido um dos argumentos %s"
 
-#: /usr/lib64/python3.5/argparse.py:2050 /usr/lib64/python3.6/argparse.py:2058
-#: /usr/lib64/python3.7/argparse.py:2079 /usr/lib64/python3.8/argparse.py:2092
+#: /usr/lib/python3.8/argparse.py:2104
 msgid "expected one argument"
 msgstr "é esperado um argumento"
 
-#: /usr/lib64/python3.5/argparse.py:2051 /usr/lib64/python3.6/argparse.py:2059
-#: /usr/lib64/python3.7/argparse.py:2080 /usr/lib64/python3.8/argparse.py:2093
+#: /usr/lib/python3.8/argparse.py:2105
 msgid "expected at most one argument"
 msgstr "é esperado um argumento, no máximo"
 
-#: /usr/lib64/python3.5/argparse.py:2052 /usr/lib64/python3.6/argparse.py:2060
-#: /usr/lib64/python3.7/argparse.py:2081 /usr/lib64/python3.8/argparse.py:2094
+#: /usr/lib/python3.8/argparse.py:2106
 msgid "expected at least one argument"
 msgstr "é esperado um argumento, no mínimo"
 
-#: /usr/lib64/python3.5/argparse.py:2054 /usr/lib64/python3.6/argparse.py:2062
-#: /usr/lib64/python3.7/argparse.py:2083 /usr/lib64/python3.8/argparse.py:2098
+#: /usr/lib/python3.8/argparse.py:2110
 #, python-format
 msgid "expected %s argument"
 msgid_plural "expected %s arguments"
 msgstr[0] "é esperado %s argumento"
 msgstr[1] "são esperados %s argumentos"
 
-#: /usr/lib64/python3.5/argparse.py:2114 /usr/lib64/python3.6/argparse.py:2122
-#: /usr/lib64/python3.7/argparse.py:2143 /usr/lib64/python3.8/argparse.py:2157
+#: /usr/lib/python3.8/argparse.py:2168
 #, python-format
 msgid "ambiguous option: %(option)s could match %(matches)s"
 msgstr "opção ambígua: %(option)s pode ser igual a %(matches)s"
 
-#: /usr/lib64/python3.5/argparse.py:2177 /usr/lib64/python3.6/argparse.py:2185
-#: /usr/lib64/python3.7/argparse.py:2206 /usr/lib64/python3.8/argparse.py:2220
+#: /usr/lib/python3.8/argparse.py:2232
 #, python-format
 msgid "unexpected option string: %s"
 msgstr "linha de opções não esperada: %s"
 
-#: /usr/lib64/python3.5/argparse.py:2281 /usr/lib64/python3.6/argparse.py:2289
-#: /usr/lib64/python3.7/argparse.py:2403 /usr/lib64/python3.8/argparse.py:2417
+#: /usr/lib/python3.8/argparse.py:2429
 #, python-format
 msgid "%r is not callable"
 msgstr "%r não é invocável"
 
-#: /usr/lib64/python3.5/argparse.py:2298 /usr/lib64/python3.6/argparse.py:2306
-#: /usr/lib64/python3.7/argparse.py:2420 /usr/lib64/python3.8/argparse.py:2434
+#: /usr/lib/python3.8/argparse.py:2446
 #, python-format
 msgid "invalid %(type)s value: %(value)r"
 msgstr "valor %(type)s inválido: %(value)r"
 
-#: /usr/lib64/python3.5/argparse.py:2309 /usr/lib64/python3.6/argparse.py:2317
-#: /usr/lib64/python3.7/argparse.py:2431 /usr/lib64/python3.8/argparse.py:2445
+#: /usr/lib/python3.8/argparse.py:2457
 #, python-format
 msgid "invalid choice: %(value)r (choose from %(choices)s)"
 msgstr "alternativa inválida: %(value)r (escolher de %(choices)s)"
 
-#: /usr/lib64/python3.5/argparse.py:2385 /usr/lib64/python3.6/argparse.py:2393
-#: /usr/lib64/python3.7/argparse.py:2507 /usr/lib64/python3.8/argparse.py:2521
+#: /usr/lib/python3.8/argparse.py:2533
 #, python-format
 msgid "%(prog)s: error: %(message)s\n"
 msgstr "%(prog)s: erro: %(message)s\n"
 
-#: /usr/lib64/python3.8/argparse.py:1218
-#, python-format
-msgid "can't open '%(filename)s': %(error)s"
-msgstr "não é possível abrir '%(filename)s': %(error)s"
+#, fuzzy
+#~ msgid "conflicting subparser: %s"
+#~ msgstr "linha de opções conflituante: %s"
+
+#, fuzzy
+#~ msgid "conflicting subparser alias: %s"
+#~ msgstr "linha de opções conflituante: %s"
+
+#~ msgid "can't open '%s': %s"
+#~ msgstr "não é possível abrir '%s': %s"
+
+#~ msgid "place header in path.license instead of path"
+#~ msgstr "colocar o cabeçalho em path.license em vez de em path"
+
+#~ msgid "could not find Git"
+#~ msgstr "não foi encontrado o Git"
+
+#~ msgid "'{path}' does not end with .spdx"
+#~ msgstr "'{path}' não termina em .spdx"
```

### Comparing `reuse-2.0.0/po/reuse.pot` & `reuse-2.1.0/po/reuse.pot`

 * *Files 2% similar despite different names*

```diff
@@ -5,92 +5,96 @@
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "#-#-#-#-#  reuse.pot (PACKAGE VERSION)  #-#-#-#-#\n"
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 08:20+0000\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 "#-#-#-#-#  argparse.pot (PACKAGE VERSION)  #-#-#-#-#\n"
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-06-19 08:20+0000\n"
+"POT-Creation-Date: 2023-07-18 08:51+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
 
-#: src/reuse/_main.py:33
+#: src/reuse/_main.py:34
 msgid ""
 "reuse is a tool for compliance with the REUSE recommendations. See <https://"
 "reuse.software/> for more information, and <https://reuse.readthedocs.io/> "
 "for the online documentation."
 msgstr ""
 
-#: src/reuse/_main.py:39
+#: src/reuse/_main.py:40
 msgid ""
 "This version of reuse is compatible with version {} of the REUSE "
 "Specification."
 msgstr ""
 
-#: src/reuse/_main.py:42
+#: src/reuse/_main.py:43
 msgid "Support the FSFE's work:"
 msgstr ""
 
-#: src/reuse/_main.py:46
+#: src/reuse/_main.py:47
 msgid ""
 "Donations are critical to our strength and autonomy. They enable us to "
 "continue working for Free Software wherever necessary. Please consider "
 "making a donation at <https://fsfe.org/donate/>."
 msgstr ""
 
-#: src/reuse/_main.py:69
+#: src/reuse/_main.py:70
 msgid "enable debug statements"
 msgstr ""
 
-#: src/reuse/_main.py:74
+#: src/reuse/_main.py:75
+msgid "hide deprecation warnings"
+msgstr ""
+
+#: src/reuse/_main.py:80
 msgid "do not skip over Git submodules"
 msgstr ""
 
-#: src/reuse/_main.py:79
+#: src/reuse/_main.py:85
 msgid "do not skip over Meson subprojects"
 msgstr ""
 
-#: src/reuse/_main.py:84
+#: src/reuse/_main.py:90
 msgid "do not use multiprocessing"
 msgstr ""
 
-#: src/reuse/_main.py:91
+#: src/reuse/_main.py:97
 msgid "define root of project"
 msgstr ""
 
-#: src/reuse/_main.py:96
+#: src/reuse/_main.py:102
 msgid "show program's version number and exit"
 msgstr ""
 
-#: src/reuse/_main.py:100
+#: src/reuse/_main.py:106
 msgid "subcommands"
 msgstr ""
 
-#: src/reuse/_main.py:107
+#: src/reuse/_main.py:113
 msgid "add copyright and licensing into the header of files"
 msgstr ""
 
-#: src/reuse/_main.py:110
+#: src/reuse/_main.py:116
 msgid ""
 "Add copyright and licensing into the header of one or more files.\n"
 "\n"
 "By using --copyright and --license, you can specify which copyright holders "
 "and licenses to add to the headers of the given files.\n"
 "\n"
 "By using --contributor, you can specify people or entity that contributed "
@@ -112,46 +116,46 @@
 "template by specifying '--template mytemplate'. Read the online "
 "documentation on how to use this feature.\n"
 "\n"
 "If a binary file is detected, or if --explicit-license is specified, the "
 "header is placed in a .license file."
 msgstr ""
 
-#: src/reuse/_main.py:153
+#: src/reuse/_main.py:159
 msgid "deprecated in favor of annotate"
 msgstr ""
 
-#: src/reuse/_main.py:161
+#: src/reuse/_main.py:167
 msgid "download a license and place it in the LICENSES/ directory"
 msgstr ""
 
-#: src/reuse/_main.py:164
+#: src/reuse/_main.py:170
 msgid ""
 "Download a license and place it in the LICENSES/ directory.\n"
 "\n"
 "The LICENSES/ directory is automatically found in the following order:\n"
 "\n"
 "- The LICENSES/ directory in the root of the VCS repository.\n"
 "\n"
 "- The current directory if its name is LICENSES.\n"
 "\n"
 "- The LICENSES/ directory in the current directory.\n"
 "\n"
 "If the LICENSES/ directory cannot be found, one is simply created."
 msgstr ""
 
-#: src/reuse/_main.py:187
+#: src/reuse/_main.py:193
 msgid "initialize REUSE project"
 msgstr ""
 
-#: src/reuse/_main.py:195
+#: src/reuse/_main.py:201
 msgid "list all non-compliant files"
 msgstr ""
 
-#: src/reuse/_main.py:198
+#: src/reuse/_main.py:204
 #, python-brace-format
 msgid ""
 "Lint the project directory for compliance with version {reuse_version} of "
 "the REUSE Specification. You can find the latest version of the "
 "specification at <https://reuse.software/spec/>.\n"
 "\n"
 "Specifically, the following criteria are checked:\n"
@@ -164,64 +168,64 @@
 "\n"
 "- Are any licenses included in the LICENSES/ directory that are not used "
 "inside of the project?\n"
 "\n"
 "- Do all files have valid copyright and licensing information?"
 msgstr ""
 
-#: src/reuse/_main.py:225
+#: src/reuse/_main.py:231
 msgid "print the project's bill of materials in SPDX format"
 msgstr ""
 
-#: src/reuse/_main.py:233
+#: src/reuse/_main.py:239
 msgid "list all supported SPDX licenses"
 msgstr ""
 
-#: src/reuse/_util.py:339
+#: src/reuse/_util.py:342
 #, python-brace-format
 msgid "Could not parse '{expression}'"
 msgstr ""
 
-#: src/reuse/_util.py:473
+#: src/reuse/_util.py:476
 msgid "'{}' is not a file"
 msgstr ""
 
-#: src/reuse/_util.py:476
+#: src/reuse/_util.py:479
 msgid "'{}' is not a directory"
 msgstr ""
 
-#: src/reuse/_util.py:479
+#: src/reuse/_util.py:482
 msgid "can't open '{}'"
 msgstr ""
 
-#: src/reuse/_util.py:484
+#: src/reuse/_util.py:487
 msgid "can't write to directory '{}'"
 msgstr ""
 
-#: src/reuse/_util.py:490 src/reuse/header.py:575
+#: src/reuse/_util.py:493 src/reuse/header.py:575
 msgid "can't write to '{}'"
 msgstr ""
 
-#: src/reuse/_util.py:503
+#: src/reuse/_util.py:506
 msgid "can't read or write '{}'"
 msgstr ""
 
-#: src/reuse/_util.py:513
+#: src/reuse/_util.py:516
 msgid "'{}' is not a valid SPDX expression, aborting"
 msgstr ""
 
-#: src/reuse/_util.py:541
+#: src/reuse/_util.py:544
 msgid "'{}' is not a valid SPDX License Identifier."
 msgstr ""
 
-#: src/reuse/_util.py:548
+#: src/reuse/_util.py:551
 msgid "Did you mean:"
 msgstr ""
 
-#: src/reuse/_util.py:555
+#: src/reuse/_util.py:558
 msgid ""
 "See <https://spdx.org/licenses/> for a list of valid SPDX License "
 "Identifiers."
 msgstr ""
 
 #: src/reuse/download.py:88
 msgid "SPDX License Identifier of license"
@@ -594,77 +598,80 @@
 
 #: src/reuse/lint.py:197
 msgid ""
 "Unfortunately, your project is not compliant with version {} of the REUSE "
 "Specification :-("
 msgstr ""
 
-#: src/reuse/project.py:75
+#: src/reuse/project.py:77
 msgid ""
 "project is not a VCS repository or required VCS software is not installed"
 msgstr ""
 
-#: src/reuse/project.py:179
+#: src/reuse/project.py:184
 #, python-brace-format
 msgid "'{path}' covered by .reuse/dep5"
 msgstr ""
 
-#: src/reuse/project.py:210
+#: src/reuse/project.py:217
 #, python-brace-format
 msgid ""
 "'{path}' holds an SPDX expression that cannot be parsed, skipping the file"
 msgstr ""
 
-#: src/reuse/project.py:222
+#: src/reuse/project.py:226
 #, python-brace-format
 msgid ""
-"Copyright and licensing information for '{original_path}' have been found in "
-"'{path}' and the DEP5 file located at '{dep5_path}'. The information in the "
-"DEP5 file has been overridden. Please ensure that this is correct."
+"Copyright and licensing information for '{original_path}' has been found in "
+"both '{path}' and in the DEP5 file located at '{dep5_path}'. The information "
+"for these two sources has been aggregated. In the future this behaviour will "
+"change, and you will need to explicitly enable aggregation. See <https://"
+"github.com/fsfe/reuse-tool/issues/779>. You need do nothing yet. Run with `--"
+"suppress-deprecation` to hide this warning."
 msgstr ""
 
-#: src/reuse/project.py:305
+#: src/reuse/project.py:313
 msgid ".reuse/dep5 has syntax errors"
 msgstr ""
 
-#: src/reuse/project.py:307
+#: src/reuse/project.py:315
 msgid ".reuse/dep5 could not be parsed as utf-8"
 msgstr ""
 
-#: src/reuse/project.py:333
+#: src/reuse/project.py:341
 #, python-brace-format
 msgid "determining identifier of '{path}'"
 msgstr ""
 
-#: src/reuse/project.py:341
+#: src/reuse/project.py:349
 #, python-brace-format
 msgid "{path} does not have a file extension"
 msgstr ""
 
-#: src/reuse/project.py:351
+#: src/reuse/project.py:359
 #, python-brace-format
 msgid ""
 "Could not resolve SPDX License Identifier of {path}, resolving to "
 "{identifier}. Make sure the license is in the license list found at <https://"
 "spdx.org/licenses/> or that it starts with 'LicenseRef-', and that it has a "
 "file extension."
 msgstr ""
 
-#: src/reuse/project.py:363
+#: src/reuse/project.py:371
 #, python-brace-format
 msgid ""
 "{identifier} is the SPDX License Identifier of both {path} and {other_path}"
 msgstr ""
 
-#: src/reuse/report.py:265
+#: src/reuse/report.py:263
 #, python-brace-format
 msgid "Could not read '{path}'"
 msgstr ""
 
-#: src/reuse/report.py:272
+#: src/reuse/report.py:270
 #, python-brace-format
 msgid "Unexpected error occurred while parsing '{path}'"
 msgstr ""
 
 #: src/reuse/spdx.py:32
 msgid ""
 "populate the LicenseConcluded field; note that reuse cannot guarantee the "
```

### Comparing `reuse-2.0.0/pyproject.toml` & `reuse-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-FileCopyrightText: 2022 Carmen Bianca Bakker <carmenbianca@fsfe.org>
 # SPDX-FileCopyrightText: 2023 DB Systel GmbH
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 [tool.poetry]
 name = "reuse"
-version = "2.0.0"
+version = "2.1.0"
 description = "reuse is a tool for compliance with the REUSE recommendations."
 authors = [
     "Free Software Foundation Europe <contact@fsfe.org>",
 ]
 maintainers = [
     "Carmen Bianca Bakker <carmenbianca@fsfe.org>",
     "Max Mehl <max.mehl@fsfe.org>",
@@ -53,38 +53,43 @@
 python = "^3.8"
 Jinja2 = "^3.0.0"
 binaryornot = "^0.4.4"
 "boolean.py" = ">=3.8"
 license-expression = ">=1.0"
 python-debian = "^0.1.38,!=0.1.45,!=0.1.46,!=0.1.47"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test.dependencies]
+pytest = ">=6.0.0"
+pytest-cov = ">=2.10.0"
+
+[tool.poetry.group.docs.dependencies]
 Sphinx = ">=4.0.0"
 recommonmark = "^0.7.1"
 sphinx-autodoc-typehints = "^1.12.0"
 sphinxcontrib-apidoc = "^0.3.0"
 furo = "^2023.3.27"
+
+[tool.poetry.group.dev.dependencies]
 black = ">=20"
 isort = "^5.6.0"
-bump2version = "^1.0.0"
 pre-commit = "^2.9.0"
+bump2version = "^1.0.0"
 pylint = "^2.12.2"
-pytest = ">=6.0.0"
-pytest-cov = ">=2.10.0"
 mypy = "^1.0"
+GitPython = "^3.0"
 
 [tool.poetry.scripts]
 reuse = 'reuse._main:main'
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "_build.py"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 80
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `reuse-2.0.0/src/reuse/__init__.py` & `reuse-2.1.0/src/reuse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2021 Alliander N.V.
+# SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmenbianca@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """reuse is a tool for compliance with the REUSE recommendations.
 
 Although the API is documented, it is **NOT** guaranteed stable between minor or
 even patch releases. The semantic versioning of this program pertains
@@ -26,20 +27,20 @@
 
 from boolean.boolean import Expression
 
 try:
     __version__ = version("reuse")
 except PackageNotFoundError:
     # package is not installed
-    __version__ = "2.0.0"
+    __version__ = "2.1.0"
 
 __author__ = "Carmen Bianca Bakker"
 __email__ = "carmenbianca@fsfe.org"
 __license__ = "Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later"
-__REUSE_version__ = "3.1"
+__REUSE_version__ = "3.0"
 
 _LOGGER = logging.getLogger(__name__)
 
 _PACKAGE_PATH = os.path.dirname(__file__)
 _LOCALE_DIR = os.path.join(_PACKAGE_PATH, "locale")
 
 if gettext.find("reuse", localedir=_LOCALE_DIR):
@@ -87,29 +88,30 @@
 
 class SourceType(Enum):
     """
     An enumeration representing the types of sources for license information.
     """
 
     #: A .license file containing license information.
-    DOT_LICENSE_FILE = ".license file"
+    DOT_LICENSE = "dot-license"
     #: A file header containing license information.
-    FILE_HEADER = "file header"
+    FILE_HEADER = "file-header"
     #: A .reuse/dep5 file containing license information.
-    DEP5_FILE = ".reuse/dep5 file"
+    DEP5 = "dep5"
 
 
 # TODO: In Python 3.10+, add kw_only=True
 @dataclass(frozen=True)
 class ReuseInfo:
     """Simple dataclass holding licensing and copyright information"""
 
     spdx_expressions: Set[Expression] = field(default_factory=set)
     copyright_lines: Set[str] = field(default_factory=set)
     contributor_lines: Set[str] = field(default_factory=set)
+    path: Optional[str] = None
     source_path: Optional[str] = None
     source_type: Optional[SourceType] = None
 
     def _check_nonexistent(self, **kwargs: Any) -> None:
         nonexistent_attributes = set(kwargs) - set(self.__dict__)
         if nonexistent_attributes:
             raise KeyError(
@@ -149,14 +151,25 @@
                 new_kwargs[key] = attr_val
         return self.__class__(**new_kwargs)  # type: ignore
 
     def contains_copyright_or_licensing(self) -> bool:
         """Either *spdx_expressions* or *copyright_lines* is non-empty."""
         return bool(self.spdx_expressions or self.copyright_lines)
 
+    def contains_info(self) -> bool:
+        """Any field except *path*, *source_path* and *source_type* is
+        non-empty.
+        """
+        keys = {
+            key
+            for key in self.__dict__
+            if key not in ("path", "source_path", "source_type")
+        }
+        return any(self.__dict__[key] for key in keys)
+
     def __bool__(self) -> bool:
         return any(self.__dict__.values())
 
     def __or__(self, value: "ReuseInfo") -> "ReuseInfo":
         return self.union(value)
```

### Comparing `reuse-2.0.0/src/reuse/_format.py` & `reuse-2.1.0/src/reuse/_format.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/_licenses.py` & `reuse-2.1.0/src/reuse/_licenses.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/_main.py` & `reuse-2.1.0/src/reuse/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Entry functions for reuse."""
 
 import argparse
 import logging
 import sys
+import warnings
 from gettext import gettext as _
 from typing import IO, Callable, List, Optional, Type, cast
 
 from . import (
     __REUSE_version__,
     __version__,
     download,
@@ -65,14 +66,19 @@
         description=_DESCRIPTION_TEXT,
         epilog=_EPILOG_TEXT,
     )
     parser.add_argument(
         "--debug", action="store_true", help=_("enable debug statements")
     )
     parser.add_argument(
+        "--suppress-deprecation",
+        action="store_true",
+        help=_("hide deprecation warnings"),
+    )
+    parser.add_argument(
         "--include-submodules",
         action="store_true",
         help=_("do not skip over Git submodules"),
     )
     parser.add_argument(
         "--include-meson-subprojects",
         action="store_true",
@@ -267,14 +273,17 @@
     if args is None:
         args = cast(List[str], sys.argv[1:])
 
     main_parser = parser()
     parsed_args = main_parser.parse_args(args)
 
     setup_logging(level=logging.DEBUG if parsed_args.debug else logging.WARNING)
+    # Show all warnings raised by ourselves.
+    if not parsed_args.suppress_deprecation:
+        warnings.filterwarnings("default", module="reuse")
 
     if parsed_args.version:
         out.write(f"reuse {__version__}\n")
         return 0
 
     if parsed_args.root:
         project = Project(parsed_args.root)
@@ -283,8 +292,8 @@
     project.include_submodules = parsed_args.include_submodules
     project.include_meson_subprojects = parsed_args.include_meson_subprojects
 
     return parsed_args.func(parsed_args, project, out)
 
 
 if __name__ == "__main__":
-    main()
+    sys.exit(main())
```

### Comparing `reuse-2.0.0/src/reuse/_util.py` & `reuse-2.1.0/src/reuse/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from argparse import ArgumentTypeError
 from collections import Counter
 from difflib import SequenceMatcher
 from gettext import gettext as _
 from hashlib import sha1
 from itertools import chain
 from os import PathLike
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import IO, Any, BinaryIO, Dict, Iterator, List, Optional, Set, Union
 
 from boolean.boolean import Expression, ParseError
 from debian.copyright import Copyright
 from license_expression import ExpressionError, Licensing
 
 from . import ReuseInfo, SourceType
@@ -221,27 +221,30 @@
     if path.suffix == ".license":
         return path
     return Path(f"{path}.license")
 
 
 def _copyright_from_dep5(path: StrPath, dep5_copyright: Copyright) -> ReuseInfo:
     """Find the reuse information of *path* in the dep5 Copyright object."""
-    result = dep5_copyright.find_files_paragraph(Path(path).as_posix())
+    path = PurePath(path).as_posix()
+    result = dep5_copyright.find_files_paragraph(path)
 
     if result is None:
         return ReuseInfo()
 
     return ReuseInfo(
         spdx_expressions=set(
             map(_LICENSING.parse, [result.license.synopsis])  # type: ignore
         ),
         copyright_lines=set(
             map(str.strip, result.copyright.splitlines())  # type: ignore
         ),
-        source_type=SourceType.DEP5_FILE,
+        path=path,
+        source_type=SourceType.DEP5,
+        source_path=".reuse/dep5",
     )
 
 
 def _parse_copyright_year(year: str) -> list:
     """Parse copyright years and return list."""
     if not year:
         ret = []
```

### Comparing `reuse-2.0.0/src/reuse/comment.py` & `reuse-2.1.0/src/reuse/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,14 +682,15 @@
     ".tfvars": PythonCommentStyle,
     ".thy": MlCommentStyle,
     ".toc": TexCommentStyle,
     ".toml": PythonCommentStyle,
     ".ts": CCommentStyle,
     ".tsx": CCommentStyle,
     ".ttl": PythonCommentStyle,  # Turtle/RDF
+    ".typ": CCommentStyle,  # typst files
     ".ui": UncommentableCommentStyle,
     ".v": CCommentStyle,  # V-Lang source code
     ".vala": CCommentStyle,
     ".vim": VimCommentStyle,
     ".vm": VelocityCommentStyle,
     ".vsh": CCommentStyle,  # V-Lang script
     ".vtl": VelocityCommentStyle,
```

### Comparing `reuse-2.0.0/src/reuse/download.py` & `reuse-2.1.0/src/reuse/download.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/header.py` & `reuse-2.1.0/src/reuse/header.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/init.py` & `reuse-2.1.0/src/reuse/init.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/lint.py` & `reuse-2.1.0/src/reuse/lint.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/project.py` & `reuse-2.1.0/src/reuse/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 # SPDX-FileCopyrightText: 2023 DB Systel GmbH
+# SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmenbianca@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module that contains the central Project class."""
 
 import contextlib
 import glob
 import logging
 import os
+import warnings
 from gettext import gettext as _
 from pathlib import Path
-from typing import Dict, Iterator, Optional, Union, cast
+from typing import Dict, Iterator, List, Optional, Union, cast
 
 from boolean.boolean import ParseError
 from debian.copyright import Copyright
 from debian.copyright import Error as DebianError
 from license_expression import ExpressionError
 
 from . import (
@@ -143,47 +145,48 @@
                     if the_file.stat().st_size == 0:
                         _LOGGER.debug("skipping 0-sized file '%s'", the_file)
                         continue
 
                 _LOGGER.debug("yielding '%s'", the_file)
                 yield the_file
 
-    def reuse_info_of(self, path: StrPath) -> ReuseInfo:
+    def reuse_info_of(self, path: StrPath) -> List[ReuseInfo]:
         """Return REUSE info of *path*.
 
-        This function will return any REUSE information that it can find, both
-        from within the file, the .license file and from the .reuse/dep5 file.
+        This function will return any REUSE information that it can find: from
+        within the file, the .license file and/or from the .reuse/dep5 file.
 
-        It also returns a single primary source path of the license/copyright
-        information, where 'primary' means '.license file' > 'header' > 'dep5'
+        The presence of a .license file always means that the file itself will
+        not be parsed for REUSE information.
+
+        When the .reuse/dep5 file covers a file and there is also REUSE
+        information within that file (or within its .license file), then two
+        :class:`ReuseInfo` objects are returned in the set, each with respective
+        discovered REUSE information and information about the source.
         """
         original_path = path
         path = _determine_license_path(path)
-        dep5_path: Optional[str] = None
-        source_path = ""
-        source_type = None
 
         _LOGGER.debug(f"searching '{path}' for REUSE information")
 
         # This means that only one 'source' of licensing/copyright information
         # is captured in ReuseInfo
         dep5_result = ReuseInfo()
         file_result = ReuseInfo()
+        result = []
 
         # Search the .reuse/dep5 file for REUSE information.
         if self._copyright:
             dep5_result = _copyright_from_dep5(
                 self.relative_from_root(path), self._copyright
             )
             if dep5_result.contains_copyright_or_licensing():
                 _LOGGER.info(
                     _("'{path}' covered by .reuse/dep5").format(path=path)
                 )
-                source_path = str(self.root / ".reuse/dep5")
-                dep5_path = source_path
 
         # Search the file for REUSE information.
         with path.open("rb") as fp:
             try:
                 # Completely read the file once to search for possible snippets
                 if _contains_snippet(fp):
                     _LOGGER.debug(f"'{path}' seems to contain a SPDX Snippet")
@@ -193,54 +196,59 @@
                 # Reset read position
                 fp.seek(0)
                 # Scan the file for REUSE info, possible limiting the read
                 # length
                 file_result = extract_reuse_info(
                     decoded_text_from_binary(fp, size=read_limit)
                 )
-                if file_result:
-                    source_path = str(path)
+                if file_result.contains_copyright_or_licensing():
                     if path.suffix == ".license":
-                        source_type = SourceType.DOT_LICENSE_FILE
+                        source_type = SourceType.DOT_LICENSE
                     else:
                         source_type = SourceType.FILE_HEADER
+                    file_result = file_result.copy(
+                        path=self.relative_from_root(original_path).as_posix(),
+                        source_path=self.relative_from_root(path).as_posix(),
+                        source_type=source_type,
+                    )
 
             except (ExpressionError, ParseError):
                 _LOGGER.error(
                     _(
                         "'{path}' holds an SPDX expression that cannot be"
                         " parsed, skipping the file"
                     ).format(path=path)
                 )
 
         # There is both information in a .dep5 file and in the file header
-        if (
-            dep5_result.contains_copyright_or_licensing()
-            and file_result.contains_copyright_or_licensing()
-        ):
-            _LOGGER.warning(
+        if dep5_result.contains_info() and file_result.contains_info():
+            warnings.warn(
                 _(
-                    "Copyright and licensing information for '{original_path}'"
-                    " have been found in '{path}' and the DEP5 file located at"
-                    " '{dep5_path}'. The information in the DEP5 file has been"
-                    " overridden. Please ensure that this is correct."
+                    "Copyright and licensing information for"
+                    " '{original_path}' has been found in both '{path}' and"
+                    " in the DEP5 file located at '{dep5_path}'. The"
+                    " information for these two sources has been"
+                    " aggregated. In the future this behaviour will change,"
+                    " and you will need to explicitly enable aggregation."
+                    " See"
+                    " <https://github.com/fsfe/reuse-tool/issues/779>. You"
+                    " need do nothing yet. Run with"
+                    " `--suppress-deprecation` to hide this warning."
                 ).format(
-                    original_path=original_path, path=path, dep5_path=dep5_path
-                )
+                    original_path=original_path,
+                    path=path,
+                    dep5_path=dep5_result.source_path,
+                ),
+                PendingDeprecationWarning,
             )
-        # Information is only found in a DEP5 file
-        elif (
-            dep5_result.contains_copyright_or_licensing()
-            and not file_result.contains_copyright_or_licensing()
-        ):
-            return dep5_result.copy(source_path=source_path)
-        # There is a file header or a .license file
-        return file_result.copy(
-            source_path=source_path, source_type=source_type
-        )
+        if dep5_result.contains_info():
+            result.append(dep5_result)
+        if file_result.contains_info():
+            result.append(file_result)
+        return result
 
     def relative_from_root(self, path: StrPath) -> Path:
         """If the project root is /tmp/project, and *path* is
         /tmp/project/src/file, then return src/file.
         """
         path = Path(path)
         try:
```

### Comparing `reuse-2.0.0/src/reuse/report.py` & `reuse-2.1.0/src/reuse/report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
 # SPDX-FileCopyrightText: 2022 Pietro Albini <pietro.albini@ferrous-systems.com>
+# SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmenbianca@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Module that contains reports about files and projects for linting."""
 
 import datetime
 import logging
 import multiprocessing as mp
 import random
 from gettext import gettext as _
 from hashlib import md5
 from io import StringIO
 from os import cpu_count
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, cast
 from uuid import uuid4
 
 from . import __REUSE_version__, __version__
 from ._util import _LICENSING, StrPath, _checksum
 from .project import Project, ReuseInfo
 
@@ -186,37 +187,34 @@
         out.write(f"Created: {now.isoformat()}Z\n")
         out.write(
             "CreatorComment: <text>This document was created automatically"
             " using available reuse information consistent with"
             " REUSE.</text>\n"
         )
 
-        reports = sorted(self.file_reports, key=lambda x: x.spdxfile.name)
+        reports = sorted(self.file_reports, key=lambda x: x.name)
 
         for report in reports:
             out.write(
                 "Relationship: SPDXRef-DOCUMENT describes"
-                f" {report.spdxfile.spdx_id}\n"
+                f" {report.spdx_id}\n"
             )
 
         for report in reports:
             out.write("\n")
-            out.write(f"FileName: {report.spdxfile.name}\n")
-            out.write(f"SPDXID: {report.spdxfile.spdx_id}\n")
-            out.write(f"FileChecksum: SHA1: {report.spdxfile.chk_sum}\n")
-            out.write(
-                f"LicenseConcluded: {report.spdxfile.license_concluded}\n"
-            )
+            out.write(f"FileName: {report.name}\n")
+            out.write(f"SPDXID: {report.spdx_id}\n")
+            out.write(f"FileChecksum: SHA1: {report.chk_sum}\n")
+            out.write(f"LicenseConcluded: {report.license_concluded}\n")
 
-            for lic in sorted(report.spdxfile.licenses_in_file):
+            for lic in sorted(report.licenses_in_file):
                 out.write(f"LicenseInfoInFile: {lic}\n")
-            if report.spdxfile.copyright:
+            if report.copyright:
                 out.write(
-                    "FileCopyrightText:"
-                    f" <text>{report.spdxfile.copyright}</text>\n"
+                    "FileCopyrightText:" f" <text>{report.copyright}</text>\n"
                 )
             else:
                 out.write("FileCopyrightText: NONE\n")
 
         # Licenses
         for lic, path in sorted(self.licenses.items()):
             if lic.startswith("LicenseRef-"):
@@ -306,15 +304,15 @@
         """Set of license identifiers that are found in file reports."""
         if self._used_licenses is not None:
             return self._used_licenses
 
         self._used_licenses = {
             lic
             for file_report in self.file_reports
-            for lic in file_report.spdxfile.licenses_in_file
+            for lic in file_report.licenses_in_file
         }
         return self._used_licenses
 
     @property
     def unused_licenses(self) -> Set[str]:
         """Set of license identifiers that are not found in any file report."""
         if self._unused_licenses is not None:
@@ -337,29 +335,29 @@
         """Set of paths that have no license information."""
         if self._files_without_licenses is not None:
             return self._files_without_licenses
 
         self._files_without_licenses = {
             file_report.path
             for file_report in self.file_reports
-            if not file_report.spdxfile.licenses_in_file
+            if not file_report.licenses_in_file
         }
 
         return self._files_without_licenses
 
     @property
     def files_without_copyright(self) -> Set[Path]:
         """Set of paths that have no copyright information."""
         if self._files_without_copyright is not None:
             return self._files_without_copyright
 
         self._files_without_copyright = {
             file_report.path
             for file_report in self.file_reports
-            if not file_report.spdxfile.copyright
+            if not file_report.copyright
         }
 
         return self._files_without_copyright
 
     @property
     def is_compliant(self) -> bool:
         """Whether the report is compliant with the REUSE Spec."""
@@ -378,64 +376,62 @@
                 self.read_errors,
             )
         )
 
         return self._is_compliant
 
 
-class _File:  # pylint: disable=too-few-public-methods
-    """Represent an SPDX file. Sufficiently enough for our purposes, in any
-    case.
-    """
+class FileReport:  # pylint: disable=too-many-instance-attributes
+    """Object that holds a linting report about a single file."""
 
-    def __init__(
-        self,
-        name: str,
-        spdx_id: Optional[str] = None,
-        chk_sum: Optional[str] = None,
-    ):
-        self.name: str = name
-        self.spdx_id: Optional[str] = spdx_id
-        self.chk_sum: Optional[str] = chk_sum
+    def __init__(self, name: str, path: StrPath, do_checksum: bool = True):
+        self.name = name
+        self.path = Path(path)
+        self.do_checksum = do_checksum
+
+        self.reuse_infos: List[ReuseInfo] = []
+
+        self.spdx_id: Optional[str] = None
+        self.chk_sum: Optional[str] = None
         self.licenses_in_file: List[str] = []
         self.license_concluded: str = ""
         self.copyright: str = ""
-        self.info: ReuseInfo = ReuseInfo()
-
-
-class FileReport:
-    """Object that holds a linting report about a single file. Importantly,
-    it also contains SPDX File information in :attr:`spdxfile`.
-    """
-
-    def __init__(self, name: StrPath, path: StrPath, do_checksum: bool = True):
-        self.spdxfile = _File(str(name))
-        self.path = Path(path)
-        self.do_checksum = do_checksum
 
         self.bad_licenses: Set[str] = set()
         self.missing_licenses: Set[str] = set()
 
     def to_dict_lint(self) -> Dict[str, Any]:
         """Turn the report into a json-like dictionary with exclusively
         information relevant for linting.
         """
         return {
-            "path": str(Path(self.path).resolve()),
-            # TODO: Why does every copyright line have the same source?
+            # This gets rid of the './' prefix. In Python 3.9, use
+            # str.removeprefix.
+            "path": PurePath(self.name).as_posix(),
             "copyrights": [
-                {"value": copyright_, "source": self.spdxfile.info.source_path}
-                for copyright_ in self.spdxfile.copyright.split("\n")
-                if copyright_
+                {
+                    "value": line,
+                    "source": reuse_info.source_path,
+                    "source_type": reuse_info.source_type.value
+                    if reuse_info.source_type
+                    else None,
+                }
+                for reuse_info in self.reuse_infos
+                for line in reuse_info.copyright_lines
             ],
-            # TODO: Why does every license expression have the same source?
-            "licenses": [
-                {"value": license_, "source": self.spdxfile.info.source_path}
-                for license_ in self.spdxfile.licenses_in_file
-                if license_
+            "spdx_expressions": [
+                {
+                    "value": str(expression),
+                    "source": reuse_info.source_path,
+                    "source_type": reuse_info.source_type.value
+                    if reuse_info.source_type
+                    else None,
+                }
+                for reuse_info in self.reuse_infos
+                for expression in reuse_info.spdx_expressions
             ],
         }
 
     @classmethod
     def generate(
         cls,
         project: Project,
@@ -445,78 +441,84 @@
     ) -> "FileReport":
         """Generate a FileReport from a path in a Project."""
         path = Path(path)
         if not path.is_file():
             raise OSError(f"{path} is not a file")
 
         relative = project.relative_from_root(path)
-        report = cls("./" + str(relative), path, do_checksum=do_checksum)
+        report = cls(f"./{relative}", path, do_checksum=do_checksum)
 
         # Checksum and ID
         if report.do_checksum:
-            report.spdxfile.chk_sum = _checksum(path)
+            report.chk_sum = _checksum(path)
         else:
             # This path avoids a lot of heavy computation, which is handy for
             # scenarios where you only need a unique hash, not a consistent
             # hash.
-            report.spdxfile.chk_sum = f"{random.getrandbits(160):040x}"
+            report.chk_sum = f"{random.getrandbits(160):040x}"
         spdx_id = md5()
-        spdx_id.update(str(relative).encode("utf-8"))
-        spdx_id.update(report.spdxfile.chk_sum.encode("utf-8"))
-        report.spdxfile.spdx_id = f"SPDXRef-{spdx_id.hexdigest()}"
-
-        reuse_info = project.reuse_info_of(path)
-        for expression in reuse_info.spdx_expressions:
-            for identifier in _LICENSING.license_keys(expression):
-                # A license expression akin to Apache-1.0+ should register
-                # correctly if LICENSES/Apache-1.0.txt exists.
-                identifiers = {identifier}
-                if identifier.endswith("+"):
-                    identifiers.add(identifier[:-1])
-                # Bad license
-                if not identifiers.intersection(project.license_map):
-                    report.bad_licenses.add(identifier)
-                # Missing license
-                if not identifiers.intersection(project.licenses):
-                    report.missing_licenses.add(identifier)
+        spdx_id.update(report.name.encode("utf-8"))
+        spdx_id.update(report.chk_sum.encode("utf-8"))
+        report.spdx_id = f"SPDXRef-{spdx_id.hexdigest()}"
+
+        reuse_infos = project.reuse_info_of(path)
+        for reuse_info in reuse_infos:
+            for expression in reuse_info.spdx_expressions:
+                for identifier in _LICENSING.license_keys(expression):
+                    # A license expression akin to Apache-1.0+ should register
+                    # correctly if LICENSES/Apache-1.0.txt exists.
+                    identifiers = {identifier}
+                    if identifier.endswith("+"):
+                        identifiers.add(identifier[:-1])
+                    # Bad license
+                    if not identifiers.intersection(project.license_map):
+                        report.bad_licenses.add(identifier)
+                    # Missing license
+                    if not identifiers.intersection(project.licenses):
+                        report.missing_licenses.add(identifier)
 
-                # Add license to report.
-                report.spdxfile.licenses_in_file.append(identifier)
+                    # Add license to report.
+                    report.licenses_in_file.append(identifier)
 
         if not add_license_concluded:
-            report.spdxfile.license_concluded = "NOASSERTION"
-        elif not reuse_info.spdx_expressions:
-            report.spdxfile.license_concluded = "NONE"
+            report.license_concluded = "NOASSERTION"
+        elif not any(reuse_info.spdx_expressions for reuse_info in reuse_infos):
+            report.license_concluded = "NONE"
         else:
             # Merge all the license expressions together, wrapping them in
             # parentheses to make sure an expression doesn't spill into another
             # one. The extra parentheses will be removed by the roundtrip
             # through parse() -> simplify() -> render().
-            report.spdxfile.license_concluded = (
+            report.license_concluded = (
                 _LICENSING.parse(
                     " AND ".join(
                         f"({expression})"
+                        for reuse_info in reuse_infos
                         for expression in reuse_info.spdx_expressions
                     ),
                 )
                 .simplify()
                 .render()
             )
 
         # Copyright text
-        report.spdxfile.copyright = "\n".join(
-            sorted(reuse_info.copyright_lines)
+        report.copyright = "\n".join(
+            sorted(
+                line
+                for reuse_info in reuse_infos
+                for line in reuse_info.copyright_lines
+            )
         )
         # Source of licensing and copyright info
-        report.spdxfile.info = reuse_info
+        report.reuse_infos = reuse_infos
         return report
 
     def __hash__(self) -> int:
-        if self.spdxfile.chk_sum is not None:
-            return hash(self.spdxfile.name + self.spdxfile.chk_sum)
+        if self.chk_sum is not None:
+            return hash(self.name + self.chk_sum)
         return super().__hash__()
 
 
 def format_creator(creator: Optional[str]) -> str:
     """Render the creator field based on the provided flag"""
     if creator is None:
         return "Anonymous ()"
```

### Comparing `reuse-2.0.0/src/reuse/resources/exceptions.json` & `reuse-2.1.0/src/reuse/resources/exceptions.json`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/resources/licenses.json` & `reuse-2.1.0/src/reuse/resources/licenses.json`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/spdx.py` & `reuse-2.1.0/src/reuse/spdx.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/supported_licenses.py` & `reuse-2.1.0/src/reuse/supported_licenses.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/src/reuse/vcs.py` & `reuse-2.1.0/src/reuse/vcs.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/conftest.py` & `reuse-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/resources/fsfe.png` & `reuse-2.1.0/tests/resources/fsfe.png`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_comment.py` & `reuse-2.1.0/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_core.py` & `reuse-2.1.0/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for some core components."""
 
 import pytest
 
-from reuse import ReuseInfo
+from reuse import ReuseInfo, SourceType
 
 # REUSE-IgnoreStart
 
 
 def test_reuse_info_contains_copyright_or_licensing():
     """If either spdx_expressions or copyright_lines is truthy, expect True."""
     arguments = [
@@ -31,14 +31,37 @@
 
 def test_reuse_info_contains_copyright_or_licensing_other_truthy():
     """If another attribute is truthy, still expect False."""
     info = ReuseInfo(contributor_lines={"SPDX-FileContributor: 2017 Jane Doe"})
     assert not info.contains_copyright_or_licensing()
 
 
+def test_reuse_info_contains_info_simple():
+    """If any of the non-source files are truthy, expect True."""
+    assert ReuseInfo(spdx_expressions={"MIT"}).contains_info()
+    assert ReuseInfo(
+        copyright_lines={"SPDX-FileCopyrightText: 2017 Jane Doe"}
+    ).contains_info()
+    assert ReuseInfo(
+        contributor_lines={"SPDX-FileContributor: 2017 John Doe"}
+    ).contains_info()
+
+
+def test_reuse_info_contains_info_empty():
+    """If the ReuseInfo object is empty, expect False."""
+    info = ReuseInfo()
+    assert not info.contains_info()
+
+
+def test_reuse_info_contains_info_source_truthy():
+    """If any of the source information is truthy, still expect False."""
+    assert not ReuseInfo(source_path="foo.py").contains_info()
+    assert not ReuseInfo(source_type=SourceType.FILE_HEADER).contains_info()
+
+
 def test_reuse_info_copy_simple():
     """Get a copy of ReuseInfo with one field replaced."""
     info = ReuseInfo(
         spdx_expressions={"GPL-3.0-or-later"},
         copyright_lines={"2017 Jane Doe"},
         source_path="foo",
     )
```

### Comparing `reuse-2.0.0/tests/test_download.py` & `reuse-2.1.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_header.py` & `reuse-2.1.0/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_lint.py` & `reuse-2.1.0/tests/test_lint.py`

 * *Files 18% similar despite different names*

```diff
@@ -187,37 +187,8 @@
         if test_file["path"].startswith(str(fake_repository / "doc")):
             assert test_file["licenses"][0]["value"] == "CC0-1.0"
             assert test_file["licenses"][0]["source"] == str(
                 fake_repository / ".reuse/dep5"
             )
 
 
-def test_lint_json_output_precedence(fake_repository):
-    """Test for lint with JSON output with focus on precedence."""
-    (fake_repository / "doc/differently_licensed_docs.rst").write_text(
-        "SPDX-License-Identifier: MIT"
-    )
-    project = Project(fake_repository)
-    report = ProjectReport.generate(project)
-
-    json_result = report.to_dict_lint()
-
-    assert json_result
-    # Test result
-    assert json_result["summary"]["compliant"] is False
-    # Test license path precedence
-    for test_file in json_result["files"]:
-        if test_file["path"].startswith(
-            str(fake_repository / "doc/differently_licensed_docs.rst")
-        ):
-            assert test_file["licenses"][0]["value"] == "MIT"
-            assert test_file["licenses"][0]["source"] == str(
-                fake_repository / "doc/differently_licensed_docs.rst"
-            )
-        if test_file["path"].startswith(str(fake_repository / "doc/index.rst")):
-            assert test_file["licenses"][0]["value"] == "CC0-1.0"
-            assert test_file["licenses"][0]["source"] == str(
-                fake_repository / ".reuse/dep5"
-            )
-
-
 # REUSE-IgnoreEnd
```

### Comparing `reuse-2.0.0/tests/test_main.py` & `reuse-2.1.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_main_annotate.py` & `reuse-2.1.0/tests/test_main_annotate.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_main_annotate_merge.py` & `reuse-2.1.0/tests/test_main_annotate_merge.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_project.py` & `reuse-2.1.0/tests/test_project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # SPDX-FileCopyrightText: 2017 Free Software Foundation Europe e.V. <https://fsfe.org>
 # SPDX-FileCopyrightText: © 2020 Liferay, Inc. <https://liferay.com>
 # SPDX-FileCopyrightText: 2022 Florian Snow <florian@familysnow.net>
+# SPDX-FileCopyrightText: 2023 Carmen Bianca BAKKER <carmenbianca@fsfe.org>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for reuse.project."""
 
 import os
 import shutil
+import warnings
 from importlib import import_module
 from inspect import cleandoc
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 from license_expression import LicenseSymbol
 
+from reuse import SourceType
 from reuse.project import Project
 
 try:
     IS_POSIX = bool(import_module("posix"))
 except ImportError:
     IS_POSIX = False
 
@@ -217,86 +220,94 @@
 
     project = Project(empty_directory)
     with pytest.raises((IsADirectoryError, PermissionError)):
         project.reuse_info_of(empty_directory / "src")
 
 
 def test_reuse_info_of_unlicensed_file(fake_repository):
-    """Return an empty ReuseInfo object when asking for the REUSE information
-    of a file that has no REUSE information.
+    """Return an empty set when asking for the REUSE information of a file that
+    has no REUSE information.
+
     """
     (fake_repository / "foo.py").write_text("foo")
     project = Project(fake_repository)
     assert not bool(project.reuse_info_of("foo.py"))
 
 
 def test_reuse_info_of_only_copyright(fake_repository):
     """A file contains only a copyright line. Test whether it correctly picks
     up on that.
     """
     (fake_repository / "foo.py").write_text(
         "SPDX-FileCopyrightText: 2017 Jane Doe"
     )
     project = Project(fake_repository)
-    reuse_info = project.reuse_info_of("foo.py")
+    reuse_info = project.reuse_info_of("foo.py")[0]
     assert not any(reuse_info.spdx_expressions)
     assert len(reuse_info.copyright_lines) == 1
     assert (
         reuse_info.copyright_lines.pop()
         == "SPDX-FileCopyrightText: 2017 Jane Doe"
     )
-
-
-def test_reuse_info_of_only_copyright_also_covered_by_debian(fake_repository):
-    """A file contains only a copyright line, but debian/copyright also has
-    information on this file. Use only the information from file header.
-    """
-    (fake_repository / "doc/foo.py").write_text(
-        "SPDX-FileCopyrightText: in file"
-    )
-    project = Project(fake_repository)
-    reuse_info = project.reuse_info_of("doc/foo.py")
-
-    assert len(reuse_info.copyright_lines) == 1
-    assert "SPDX-FileCopyrightText: in file" in reuse_info.copyright_lines
+    assert reuse_info.source_type == SourceType.FILE_HEADER
+    assert reuse_info.source_path == "foo.py"
+    assert reuse_info.path == "foo.py"
 
 
 def test_reuse_info_of_also_covered_by_dep5(fake_repository):
     """A file contains all REUSE information, but .reuse/dep5 also
-    provides information on this file. Use only the information
-    from the file header.
+    provides information on this file. Aggregate the information (for now), and
+    expect a PendingDeprecationWarning.
     """
     (fake_repository / "doc/foo.py").write_text(
         dedent(
             """
             SPDX-License-Identifier: MIT
             SPDX-FileCopyrightText: in file"""
         )
     )
     project = Project(fake_repository)
-    reuse_info = project.reuse_info_of("doc/foo.py")
-    assert LicenseSymbol("MIT") in reuse_info.spdx_expressions
-    assert LicenseSymbol("CC0-1.0") not in reuse_info.spdx_expressions
-    assert "SPDX-FileCopyrightText: in file" in reuse_info.copyright_lines
-    assert "2017 Jane Doe" not in reuse_info.copyright_lines
+    with warnings.catch_warnings(record=True) as caught_warnings:
+        reuse_infos = project.reuse_info_of("doc/foo.py")
+        assert len(reuse_infos) == 2
+        assert reuse_infos[0].source_type != reuse_infos[1].source_type
+        for reuse_info in reuse_infos:
+            if reuse_info.source_type == SourceType.DEP5:
+                assert LicenseSymbol("CC0-1.0") in reuse_info.spdx_expressions
+                assert "2017 Jane Doe" in reuse_info.copyright_lines
+                assert reuse_info.path == "doc/foo.py"
+                assert reuse_info.source_path == ".reuse/dep5"
+            elif reuse_info.source_type == SourceType.FILE_HEADER:
+                assert LicenseSymbol("MIT") in reuse_info.spdx_expressions
+                assert (
+                    "SPDX-FileCopyrightText: in file"
+                    in reuse_info.copyright_lines
+                )
+                assert reuse_info.path == "doc/foo.py"
+                assert reuse_info.source_path == "doc/foo.py"
+
+        assert len(caught_warnings) == 1
+        assert issubclass(
+            caught_warnings[0].category, PendingDeprecationWarning
+        )
 
 
 def test_reuse_info_of_no_duplicates(empty_directory):
     """A file contains the same lines twice. The ReuseInfo only contains those
     lines once.
     """
     spdx_line = "SPDX-License-Identifier: GPL-3.0-or-later\n"
     copyright_line = (
         "SPDX-FileCopyrightText: 2017 Free Software Foundation Europe\n"
     )
     text = spdx_line + copyright_line
 
     (empty_directory / "foo.py").write_text(text * 2)
     project = Project(empty_directory)
-    reuse_info = project.reuse_info_of("foo.py")
+    reuse_info = project.reuse_info_of("foo.py")[0]
     assert len(reuse_info.spdx_expressions) == 1
     assert LicenseSymbol("GPL-3.0-or-later") in reuse_info.spdx_expressions
     assert len(reuse_info.copyright_lines) == 1
     assert (
         "SPDX-FileCopyrightText: 2017 Free Software Foundation Europe"
         in reuse_info.copyright_lines
     )
@@ -305,32 +316,37 @@
 def test_reuse_info_of_binary_succeeds(fake_repository):
     """reuse_info_of succeeds when the target is covered by dep5."""
     shutil.copy(
         RESOURCES_DIRECTORY / "fsfe.png", fake_repository / "doc/fsfe.png"
     )
 
     project = Project(fake_repository)
-    reuse_info = project.reuse_info_of("doc/fsfe.png")
+    reuse_info = project.reuse_info_of("doc/fsfe.png")[0]
     assert LicenseSymbol("CC0-1.0") in reuse_info.spdx_expressions
+    assert reuse_info.source_type == SourceType.DEP5
+    assert reuse_info.path == "doc/fsfe.png"
 
 
 def test_license_file_detected(empty_directory):
     """Test whether---when given a file and a license file---the license file
     is detected and read.
     """
     (empty_directory / "foo.py").write_text("foo")
     (empty_directory / "foo.py.license").write_text(
         "SPDX-FileCopyrightText: 2017 Jane Doe\nSPDX-License-Identifier: MIT\n"
     )
 
     project = Project(empty_directory)
-    reuse_info = project.reuse_info_of("foo.py")
+    reuse_info = project.reuse_info_of("foo.py")[0]
 
     assert "SPDX-FileCopyrightText: 2017 Jane Doe" in reuse_info.copyright_lines
     assert LicenseSymbol("MIT") in reuse_info.spdx_expressions
+    assert reuse_info.source_type == SourceType.DOT_LICENSE
+    assert reuse_info.path == "foo.py"
+    assert reuse_info.source_path == "foo.py.license"
 
 
 def test_licenses_filename(empty_directory):
     """Detect the license identifier of a license from its stem."""
     (empty_directory / "LICENSES").mkdir()
     (empty_directory / "LICENSES/foo.txt").write_text("foo")
     project = Project(empty_directory)
```

### Comparing `reuse-2.0.0/tests/test_report.py` & `reuse-2.1.0/tests/test_report.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 """Tests for reuse.report"""
 
 
 import os
 import sys
 from importlib import import_module
+from textwrap import dedent
 
 import pytest
 
+from reuse import SourceType
 from reuse.project import Project
 from reuse.report import FileReport, ProjectReport
 
 try:
     IS_POSIX = bool(import_module("posix"))
 except ImportError:
     IS_POSIX = False
@@ -39,21 +41,21 @@
     project = Project(fake_repository)
     result = FileReport.generate(
         project,
         "src/source_code.py",
         add_license_concluded=add_license_concluded,
     )
 
-    assert result.spdxfile.licenses_in_file == ["GPL-3.0-or-later"]
+    assert result.licenses_in_file == ["GPL-3.0-or-later"]
     assert (
-        result.spdxfile.license_concluded == "GPL-3.0-or-later"
+        result.license_concluded == "GPL-3.0-or-later"
         if add_license_concluded
         else "NOASSERTION"
     )
-    assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
+    assert result.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
 def test_generate_file_report_file_from_different_cwd(
     fake_repository, add_license_concluded
 ):
@@ -61,21 +63,21 @@
     os.chdir("/")
     project = Project(fake_repository)
     result = FileReport.generate(
         project,
         fake_repository / "src/source_code.py",
         add_license_concluded=add_license_concluded,
     )
-    assert result.spdxfile.licenses_in_file == ["GPL-3.0-or-later"]
+    assert result.licenses_in_file == ["GPL-3.0-or-later"]
     assert (
-        result.spdxfile.license_concluded == "GPL-3.0-or-later"
+        result.license_concluded == "GPL-3.0-or-later"
         if add_license_concluded
         else "NOASSERTION"
     )
-    assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
+    assert result.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
 def test_generate_file_report_file_missing_license(
     fake_repository, add_license_concluded
 ):
@@ -84,18 +86,18 @@
         "SPDX-License-Identifier: BSD-3-Clause"
     )
     project = Project(fake_repository)
     result = FileReport.generate(
         project, "foo.py", add_license_concluded=add_license_concluded
     )
 
-    assert result.spdxfile.copyright == ""
-    assert result.spdxfile.licenses_in_file == ["BSD-3-Clause"]
+    assert result.copyright == ""
+    assert result.licenses_in_file == ["BSD-3-Clause"]
     assert (
-        result.spdxfile.license_concluded == "BSD-3-Clause"
+        result.license_concluded == "BSD-3-Clause"
         if add_license_concluded
         else "NOASSERTION"
     )
     assert result.missing_licenses == {"BSD-3-Clause"}
     assert not result.bad_licenses
 
 
@@ -107,18 +109,18 @@
         "SPDX-License-Identifier: fakelicense"
     )
     project = Project(fake_repository)
     result = FileReport.generate(
         project, "foo.py", add_license_concluded=add_license_concluded
     )
 
-    assert result.spdxfile.copyright == ""
-    assert result.spdxfile.licenses_in_file == ["fakelicense"]
+    assert result.copyright == ""
+    assert result.licenses_in_file == ["fakelicense"]
     assert (
-        result.spdxfile.license_concluded == "fakelicense"
+        result.license_concluded == "fakelicense"
         if add_license_concluded
         else "NOASSERTION"
     )
     assert result.bad_licenses == {"fakelicense"}
     assert result.missing_licenses == {"fakelicense"}
 
 
@@ -133,61 +135,61 @@
     )
     (fake_repository / "LICENSES/Apache-1.0.txt").touch()
     project = Project(fake_repository)
     result = FileReport.generate(
         project, "foo.py", add_license_concluded=add_license_concluded
     )
 
-    assert result.spdxfile.copyright == ""
-    assert result.spdxfile.licenses_in_file == ["Apache-1.0+"]
+    assert result.copyright == ""
+    assert result.licenses_in_file == ["Apache-1.0+"]
     assert (
-        result.spdxfile.license_concluded == "Apache-1.0+"
+        result.license_concluded == "Apache-1.0+"
         if add_license_concluded
         else "NOASSERTION"
     )
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
 def test_generate_file_report_exception(fake_repository, add_license_concluded):
     """Simple generate test to test if the exception is detected."""
     project = Project(fake_repository)
     result = FileReport.generate(
         project, "src/exception.py", add_license_concluded=add_license_concluded
     )
 
-    assert set(result.spdxfile.licenses_in_file) == {
+    assert set(result.licenses_in_file) == {
         "GPL-3.0-or-later",
         "Autoconf-exception-3.0",
     }
     assert (
-        result.spdxfile.license_concluded
+        result.license_concluded
         == "GPL-3.0-or-later WITH Autoconf-exception-3.0"
         if add_license_concluded
         else "NOASSERTION"
     )
-    assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
+    assert result.copyright == "SPDX-FileCopyrightText: 2017 Jane Doe"
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
 def test_generate_file_report_no_licenses(
     fake_repository, add_license_concluded
 ):
     """Test behavior when no license information is present in the file"""
     (fake_repository / "foo.py").write_text("")
     project = Project(fake_repository)
     result = FileReport.generate(
         project, "foo.py", add_license_concluded=add_license_concluded
     )
 
-    assert result.spdxfile.copyright == ""
-    assert not result.spdxfile.licenses_in_file
+    assert result.copyright == ""
+    assert not result.licenses_in_file
     assert (
-        result.spdxfile.license_concluded == "NONE"
+        result.license_concluded == "NONE"
         if add_license_concluded
         else "NOASSERTION"
     )
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
@@ -198,32 +200,77 @@
     project = Project(fake_repository)
     result = FileReport.generate(
         project,
         "src/multiple_licenses.rs",
         add_license_concluded=add_license_concluded,
     )
 
-    assert result.spdxfile.copyright == "SPDX-FileCopyrightText: 2022 Jane Doe"
-    assert set(result.spdxfile.licenses_in_file) == {
+    assert result.copyright == "SPDX-FileCopyrightText: 2022 Jane Doe"
+    assert set(result.licenses_in_file) == {
         "GPL-3.0-or-later",
         "Apache-2.0",
         "CC0-1.0",
         "Autoconf-exception-3.0",
     }
     assert (
-        result.spdxfile.license_concluded
+        result.license_concluded
         == "GPL-3.0-or-later AND (Apache-2.0 OR CC0-1.0"
         " WITH Autoconf-exception-3.0)"
         if add_license_concluded
         else "NOASSERTION"
     )
     assert not result.bad_licenses
     assert not result.missing_licenses
 
 
+def test_generate_file_report_to_dict_lint_source_information(fake_repository):
+    """When a file is covered both by DEP5 and its file header, the lint dict
+    should correctly convey the source information.
+    """
+    (fake_repository / "doc/foo.py").write_text(
+        dedent(
+            """
+            SPDX-License-Identifier: MIT OR 0BSD
+            SPDX-FileCopyrightText: in file"""
+        )
+    )
+    project = Project(fake_repository)
+    report = FileReport.generate(
+        project,
+        "doc/foo.py",
+    )
+    result = report.to_dict_lint()
+    assert result["path"] == "doc/foo.py"
+    assert len(result["copyrights"]) == 2
+    assert (
+        result["copyrights"][0]["source_type"]
+        != result["copyrights"][1]["source_type"]
+    )
+    for copyright_ in result["copyrights"]:
+        if copyright_["source_type"] == SourceType.DEP5.value:
+            assert copyright_["source"] == ".reuse/dep5"
+            assert copyright_["value"] == "2017 Jane Doe"
+        elif copyright_["source_type"] == SourceType.FILE_HEADER.value:
+            assert copyright_["source"] == "doc/foo.py"
+            assert copyright_["value"] == "SPDX-FileCopyrightText: in file"
+
+    assert len(result["spdx_expressions"]) == 2
+    assert (
+        result["spdx_expressions"][0]["source_type"]
+        != result["spdx_expressions"][1]["source_type"]
+    )
+    for expression in result["spdx_expressions"]:
+        if expression["source_type"] == SourceType.DEP5.value:
+            assert expression["source"] == ".reuse/dep5"
+            assert expression["value"] == "CC0-1.0"
+        elif expression["source_type"] == SourceType.FILE_HEADER.value:
+            assert expression["source"] == "doc/foo.py"
+            assert expression["value"] == "MIT OR 0BSD"
+
+
 def test_generate_project_report_simple(fake_repository, multiprocessing):
     """Simple generate test, just to see if it sort of works."""
     project = Project(fake_repository)
     result = ProjectReport.generate(project, multiprocessing=multiprocessing)
 
     assert not result.bad_licenses
     assert not result.licenses_without_extension
```

### Comparing `reuse-2.0.0/tests/test_util.py` & `reuse-2.1.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/tests/test_vcs.py` & `reuse-2.1.0/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `reuse-2.0.0/PKG-INFO` & `reuse-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reuse
-Version: 2.0.0
+Version: 2.1.0
 Summary: reuse is a tool for compliance with the REUSE recommendations.
 Home-page: https://reuse.software/
 License: Apache-2.0 AND CC0-1.0 AND CC-BY-SA-4.0 AND GPL-3.0-or-later
 Author: Free Software Foundation Europe
 Author-email: contact@fsfe.org
 Maintainer: Carmen Bianca Bakker
 Maintainer-email: carmenbianca@fsfe.org
@@ -272,15 +272,15 @@
 Git. This uses [pre-commit](https://pre-commit.com/). Once you
 [have it installed](https://pre-commit.com/#install), add this to the
 `.pre-commit-config.yaml` in your repository:
 
 ```yaml
 repos:
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v2.0.0
+    rev: v2.1.0
     hooks:
       - id: reuse
 ```
 
 Then run `pre-commit install`. Now, every time you commit, `reuse lint` is run
 in the background, and will prevent your commit from going through if there was
 an error.
```

