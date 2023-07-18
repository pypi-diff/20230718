# Comparing `tmp/i18ndude-6.0.0a1.tar.gz` & `tmp/i18ndude-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i18ndude-6.0.0a1.tar", last modified: Mon May  8 20:57:57 2023, max compression
+gzip compressed data, was "i18ndude-6.1.0.tar", last modified: Tue Jul 18 15:49:05 2023, max compression
```

## Comparing `i18ndude-6.0.0a1.tar` & `i18ndude-6.1.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655965 i18ndude-6.0.0a1/
--rw-r--r--   0 maurits    (501) staff       (20)    14343 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      136 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.656198 i18ndude-6.0.0a1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.637197 i18ndude-6.0.0a1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      825 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/COPYRIGHT
--rw-r--r--   0 maurits    (501) staff       (20)    15880 2023-05-08 20:57:56.000000 i18ndude-6.0.0a1/docs/ChangeLog
--rw-r--r--   0 maurits    (501) staff       (20)    12296 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      439 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)    10185 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/docs/command.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-08 20:57:57.656996 i18ndude-6.0.0a1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.631591 i18ndude-6.0.0a1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.643047 i18ndude-6.0.0a1/src/i18ndude/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    32873 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    20834 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/extract.py
--rw-r--r--   0 maurits    (501) staff       (20)    10947 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/generator.py
--rw-r--r--   0 maurits    (501) staff       (20)     2985 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/gsextract.py
--rw-r--r--   0 maurits    (501) staff       (20)     1831 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    22287 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/pygettext.py
--rwxr-xr-x   0 maurits    (501) staff       (20)    28016 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/script.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.632302 i18ndude-6.0.0a1/src/i18ndude/testdata/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652132 i18ndude-6.0.0a1/src/i18ndude/testdata/input/
--rw-r--r--   0 maurits    (501) staff       (20)      522 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/empty-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po
--rw-r--r--   0 maurits    (501) staff       (20)      820 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot
--rw-r--r--   0 maurits    (501) staff       (20)     2361 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2779 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt
--rw-r--r--   0 maurits    (501) staff       (20)      916 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      392 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2.py
--rw-r--r--   0 maurits    (501) staff       (20)      893 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt
--rw-r--r--   0 maurits    (501) staff       (20)      510 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test4.pt
--rw-r--r--   0 maurits    (501) staff       (20)      882 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.652604 i18ndude-6.0.0a1/src/i18ndude/testdata/output/
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/testdata/output/README.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.655631 i18ndude-6.0.0a1/src/i18ndude/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    34684 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)      252 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_extract.py
--rw-r--r--   0 maurits    (501) staff       (20)     7921 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)     5558 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py
--rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     9723 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/untranslated.py
--rw-r--r--   0 maurits    (501) staff       (20)    11122 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     6119 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/visualisation.py
--rw-r--r--   0 maurits    (501) staff       (20)     3237 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 20:57:57.646149 i18ndude-6.0.0a1/src/i18ndude.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    27562 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1572 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      142 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       85 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        9 2023-05-08 20:57:57.000000 i18ndude-6.0.0a1/src/i18ndude.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.550879 i18ndude-6.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    14676 2023-07-18 15:49:05.000000 i18ndude-6.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      136 2023-07-18 15:49:05.000000 i18ndude-6.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    27895 2023-07-18 15:49:05.551122 i18ndude-6.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-07-18 15:49:05.000000 i18ndude-6.1.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.539116 i18ndude-6.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      825 2023-07-18 15:49:05.000000 i18ndude-6.1.0/docs/COPYRIGHT
+-rw-r--r--   0 maurits    (501) staff       (20)    15880 2023-07-18 15:49:05.000000 i18ndude-6.1.0/docs/ChangeLog
+-rw-r--r--   0 maurits    (501) staff       (20)    12296 2023-07-18 15:49:05.000000 i18ndude-6.1.0/docs/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2023-07-18 15:49:05.000000 i18ndude-6.1.0/docs/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    10185 2023-07-18 15:49:05.000000 i18ndude-6.1.0/docs/command.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      429 2023-07-18 15:49:05.000000 i18ndude-6.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-07-18 15:49:05.551540 i18ndude-6.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2140 2023-07-18 15:49:05.000000 i18ndude-6.1.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.535842 i18ndude-6.1.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.543249 i18ndude-6.1.0/src/i18ndude/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    30870 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3738 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20403 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10692 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2899 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/gsextract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1780 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      479 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/messages.pot
+-rw-r--r--   0 maurits    (501) staff       (20)    22492 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/pygettext.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)    28000 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/script.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.536154 i18ndude-6.1.0/src/i18ndude/testdata/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.548667 i18ndude-6.1.0/src/i18ndude/testdata/input/
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/chameleon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/empty-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/synctest-de.po
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/synctest.pot
+-rw-r--r--   0 maurits    (501) staff       (20)     2338 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1917 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2779 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test1.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      916 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test2-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      316 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      893 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test2_expected-en.po
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test3.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test4.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      882 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/input/test5.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.548879 i18ndude-6.1.0/src/i18ndude/testdata/output/
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/testdata/output/README.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.550630 i18ndude-6.1.0/src/i18ndude/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    35946 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/test_catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      240 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/test_extract.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7592 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/test_untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5474 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/test_utils.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)     1524 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/tox-check-i18ndude-command.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      832 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10089 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/untranslated.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11131 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6250 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/visualisation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3197 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude/zcmlextract.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-18 15:49:05.545055 i18ndude-6.1.0/src/i18ndude.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    27895 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1598 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2023-07-18 15:49:05.000000 i18ndude-6.1.0/src/i18ndude.egg-info/top_level.txt
```

### Comparing `i18ndude-6.0.0a1/CHANGES.rst` & `i18ndude-6.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,40 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.0 (2023-07-18)
+------------------
+
+New features:
+
+
+- Let i18n:ignore ignore all translatable strings in its scope. (#109)
+
+
+Bug fixes:
+
+
+- Remove Python 2 support code.  Use pyupgrade, isort, black, flake8.
+  [maurits] (#23)
+
+
+6.0.0 (2023-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix pre-commit integration.
+  [gforcada] (#1)
+
+
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0a1/PKG-INFO` & `i18ndude-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18ndude
-Version: 6.0.0a1
+Version: 6.1.0
 Summary: i18ndude performs various tasks related to ZPT's, Python Scripts and i18n.
 Home-page: https://github.com/collective/i18ndude
 Author: Daniel Nouri
 Author-email: plone-i18n@lists.sourceforge.net
 Maintainer: Maurits van Rees
 Maintainer-email: maurits@vanrees.org
 License: GPL
@@ -78,14 +78,15 @@
     -   repo: https://github.com/collective/i18ndude
         rev: "master"
         hooks:
         -   id: i18ndude
 
 For now it only finds the strings not marked for translation.
 
+
 Command line interface
 ======================
 
 These are the various command line options.
 
 .. ### AUTOGENERATED FROM HERE ###
 
@@ -376,24 +377,51 @@
     --width NUMBER      Set output page width. Default is 79.
     -i, --ignore-extra  Ignore extra messages: do not add msgids that are not in
                         the original po-file. Only update translations for
                         existing msgids.
     --no-override       Do not override translations, only add missing
                         translations.
 
+
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.0 (2023-07-18)
+------------------
+
+New features:
+
+
+- Let i18n:ignore ignore all translatable strings in its scope. (#109)
+
+
+Bug fixes:
+
+
+- Remove Python 2 support code.  Use pyupgrade, isort, black, flake8.
+  [maurits] (#23)
+
+
+6.0.0 (2023-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix pre-commit integration.
+  [gforcada] (#1)
+
+
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0a1/README.rst` & `i18ndude-6.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/docs/COPYRIGHT` & `i18ndude-6.1.0/docs/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/docs/ChangeLog` & `i18ndude-6.1.0/docs/ChangeLog`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/docs/LICENSE` & `i18ndude-6.1.0/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/docs/command.rst` & `i18ndude-6.1.0/docs/command.rst`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/catalog.py` & `i18ndude-6.1.0/src/i18ndude/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-# -*- coding: utf-8 -*-
+from collections import OrderedDict
 from i18ndude.utils import quote
+from i18ndude.utils import undouble_unicode_escape
 from i18ndude.utils import wrapAndQuoteString
 from i18ndude.utils import wrapString
-from i18ndude.utils import undouble_unicode_escape
-from collections import OrderedDict
 from zope.i18nmessageid import Message
+
 import os
 import re
 import sys
 import time
 
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
 
 DEFAULT_PO_HEADER = [
-    '--- PLEASE EDIT THE LINES BELOW CORRECTLY ---',
-    'SOME DESCRIPTIVE TITLE.',
-    'FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.']
-
-DEFAULT_PO_MIME = (('Project-Id-Version', 'PACKAGE VERSION'),
-                   ('POT-Creation-Date', 'YEAR-MO-DA HO:MI +ZONE'),
-                   ('PO-Revision-Date', 'YEAR-MO-DA HO:MI +ZONE'),
-                   ('Last-Translator', 'FULL NAME <EMAIL@ADDRESS>'),
-                   ('Language-Team', 'LANGUAGE <LL@li.org>'),
-                   ('MIME-Version', '1.0'),
-                   ('Content-Type', 'text/plain; charset=utf-8'),
-                   ('Content-Transfer-Encoding', '8bit'),
-                   ('Plural-Forms', 'nplurals=1; plural=0'),
-                   ('Language-Code', 'en'),
-                   ('Language-Name', 'English'),
-                   ('Preferred-Encodings', 'utf-8 latin1'),
-                   ('Domain', 'DOMAIN'))
+    "--- PLEASE EDIT THE LINES BELOW CORRECTLY ---",
+    "SOME DESCRIPTIVE TITLE.",
+    "FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.",
+]
+
+DEFAULT_PO_MIME = (
+    ("Project-Id-Version", "PACKAGE VERSION"),
+    ("POT-Creation-Date", "YEAR-MO-DA HO:MI +ZONE"),
+    ("PO-Revision-Date", "YEAR-MO-DA HO:MI +ZONE"),
+    ("Last-Translator", "FULL NAME <EMAIL@ADDRESS>"),
+    ("Language-Team", "LANGUAGE <LL@li.org>"),
+    ("MIME-Version", "1.0"),
+    ("Content-Type", "text/plain; charset=utf-8"),
+    ("Content-Transfer-Encoding", "8bit"),
+    ("Plural-Forms", "nplurals=1; plural=0"),
+    ("Language-Code", "en"),
+    ("Language-Name", "English"),
+    ("Preferred-Encodings", "utf-8 latin1"),
+    ("Domain", "DOMAIN"),
+)
 
 MAX_OCCUR = 3  # maximum number of occurrences listed
 # Set it to None to list all occurences
 
 
-ORIGINAL_COMMENT = ' Original: '
-DEFAULT_COMMENT = ' Default: '
+ORIGINAL_COMMENT = " Original: "
+DEFAULT_COMMENT = " Default: "
 
 
 def now():
-    fmt = '%Y-%m-%d %H:%M+0000'
+    fmt = "%Y-%m-%d %H:%M+0000"
     return time.strftime(fmt, time.gmtime())
 
 
 def is_literal_id(msgid):
-    if '_' in msgid and ' ' not in msgid:
+    if "_" in msgid and " " not in msgid:
         return False
     else:
         return True
 
 
 class MessageEntry:
-    """ MessageEntry is class representing one msgid with its accompanying
+    """MessageEntry is class representing one msgid with its accompanying
     msgstr and optional positional information and comments.
     """
 
     def __init__(
-            self, msgid, msgstr='',
-            references=[], automatic_comments=[], comments=[]):
-        """Build a MessageEntry.
-        """
+        self, msgid, msgstr="", references=[], automatic_comments=[], comments=[]
+    ):
+        """Build a MessageEntry."""
         self.msgid = msgid
         self.msgstr = undouble_unicode_escape(msgstr)
         self.references = references
         self.automatic_comments = automatic_comments
         self.comments = comments
 
     def __repr__(self):
-        """Textual representation of a MessageEntry.
-        """
-        return ', '.join([
-            self.msgid,
-            self.msgstr,
-            repr(self.references),
-            repr(self.automatic_comments),
-            repr(self.comments)
-        ])
+        """Textual representation of a MessageEntry."""
+        return ", ".join(
+            [
+                self.msgid,
+                self.msgstr,
+                repr(self.references),
+                repr(self.automatic_comments),
+                repr(self.comments),
+            ]
+        )
 
     def __eq__(self, other):
-        """ Compare a MessageEntry to another one"""
+        """Compare a MessageEntry to another one"""
         assert isinstance(other, MessageEntry)
         if (
-                self.msgid == other.msgid and
-                self.msgstr == other.msgstr and
-                self.references == other.references and
-                self.automatic_comments == other.automatic_comments and
-                self.comments == other.comments
+            self.msgid == other.msgid
+            and self.msgstr == other.msgstr
+            and self.references == other.references
+            and self.automatic_comments == other.automatic_comments
+            and self.comments == other.comments
         ):
             return True
         return False
 
     def __ne__(self, other):
-        """ Compare a MessageEntry to another one"""
+        """Compare a MessageEntry to another one"""
         assert isinstance(other, MessageEntry)
         if self.__eq__(other):
             return False
         return True
 
     def getDefaultComment(self, multiple=False):
-        """Returns the automatic comment starting with Default: """
+        """Returns the automatic comment starting with Default:"""
         defaults = []
         for c in self.automatic_comments:
             if c.startswith(DEFAULT_COMMENT):
                 defaults.append(c)
         if len(defaults) == 0:
             return None
         if multiple:
             return defaults
         return defaults[0]
 
     def getDefault(self):
         """Returns the text of the default comment"""
         comment = self.getDefaultComment()
         if comment is not None:
-            default = comment.replace(DEFAULT_COMMENT + '\"', '')
+            default = comment.replace(DEFAULT_COMMENT + '"', "")
             return default[:-1]
         return None
 
     def getDefaults(self):
         """Returns the text of the default comments"""
         comments = self.getDefaultComment(multiple=True)
         defaults = []
         if comments is None:
             return None
         for dc in comments:
-            default = dc.replace(DEFAULT_COMMENT + '\"', '')
+            default = dc.replace(DEFAULT_COMMENT + '"', "")
             defaults.append(default[:-1])
         return defaults
 
     def getOriginalComment(self):
-        """Returns the comment line starting with Original: """
+        """Returns the comment line starting with Original:"""
         for c in self.comments:
             if c.startswith(ORIGINAL_COMMENT):
                 return c
         return None
 
     def getOriginal(self):
         """Returns the text of the original comment"""
         comment = self.getOriginalComment()
         if comment is not None:
-            orig = comment.replace(ORIGINAL_COMMENT + '\"', '')
+            orig = comment.replace(ORIGINAL_COMMENT + '"', "")
             return orig[:-1]
         return None
 
 
 class MessageCatalog(OrderedDict):
     """MessageCatalog is a collection of MessageEntries
 
@@ -170,20 +170,20 @@
         self.commentary_header = DEFAULT_PO_HEADER
         self.mime_header = OrderedDict()
         for key, value in DEFAULT_PO_MIME:
             self.mime_header[key] = value
 
         self.filename = filename
         self.domain = domain
-        self.encoding = 'utf-8'
+        self.encoding = "utf-8"
 
         if filename:
             self._initialize_with(filename)
         elif domain:
-            self.mime_header['Domain'] = domain
+            self.mime_header["Domain"] = domain
 
     def getComments(self, msgid):
         """Returns the commentary lines that I have for a msgid."""
         assert msgid in self
         return self[msgid].comments
 
     def getOriginalComment(self, msgid):
@@ -205,125 +205,137 @@
         """Returns the original text for a msgid."""
         assert msgid in self
         return self[msgid].getDefault()
 
     def update(self, dict=None):
         if dict is None:
             return
-        for (key, val) in dict.items():
-            if getattr(val, 'msgid', None) is not None \
-               and not isinstance(val.msgid, unicode):
+        for key, val in dict.items():
+            if getattr(val, "msgid", None) is not None and not isinstance(
+                val.msgid, str
+            ):
                 val.msgid = val.msgid.decode(self.encoding)
-            if getattr(val, 'msgstr', None) is not None \
-               and not isinstance(val.msgstr, unicode):
+            if getattr(val, "msgstr", None) is not None and not isinstance(
+                val.msgstr, str
+            ):
                 val.msgstr = val.msgstr.decode(self.encoding)
-            if isinstance(key, unicode):
+            if isinstance(key, str):
                 self[key] = val
             else:
                 self[key.decode(self.encoding)] = val
 
-    def add(self, msgid, msgstr='',
-            comments=[], references=[], automatic_comments=[]):
+    def add(self, msgid, msgstr="", comments=[], references=[], automatic_comments=[]):
         """Add an entry to the catalog.
 
         If the msgid already exists in the catalog, we only add comments,
         references and automatic comments to the entry."""
         if isinstance(msgid, MessageEntry):
             msgstr = msgid.msgstr
             references = msgid.references
             automatic_comments = msgid.automatic_comments
             comments = msgid.comments
             msgid = msgid.msgid
-        if not isinstance(msgid, unicode):
+        if not isinstance(msgid, str):
             msgid = msgid.decode(self.encoding)
-        if not isinstance(msgstr, unicode):
+        if not isinstance(msgstr, str):
             msgstr = msgstr.decode(self.encoding)
         if msgid not in self:
-            self[msgid] = MessageEntry(msgid, msgstr=msgstr, comments=comments,
-                                       references=references,
-                                       automatic_comments=automatic_comments)
+            self[msgid] = MessageEntry(
+                msgid,
+                msgstr=msgstr,
+                comments=comments,
+                references=references,
+                automatic_comments=automatic_comments,
+            )
         else:
             # We can have a msgid with an associated default in a page
             # template, and the same msgid with a different default in a Python
             # file
             if msgstr != self[msgid].msgstr:
                 # XXX this does not appear to have any test coverage
                 # the actual warnings are emitted by zope.tal
-                msg = u"Warning: msgid '%s' in %s already exists " \
-                      u"with a different default (bad: %s, should be: %s)\n" \
-                      u"The references for the existent value are:\n%s\n"
-                msg = msg % (msgid,
-                             u'\n'.join(references),
-                             msgstr,
-                             self[msgid].msgstr,
-                             u'\n'.join(self[msgid].references))
-                if not PY3:
-                    msg = msg.encode('utf-8')
+                msg = (
+                    "Warning: msgid '%s' in %s already exists "
+                    "with a different default (bad: %s, should be: %s)\n"
+                    "The references for the existent value are:\n%s\n"
+                )
+                msg = msg % (
+                    msgid,
+                    "\n".join(references),
+                    msgstr,
+                    self[msgid].msgstr,
+                    "\n".join(self[msgid].references),
+                )
                 sys.stderr.write(msg)
             if comments:
-                comments = [
-                    c for c in comments if c not in self[msgid].comments]
+                comments = [c for c in comments if c not in self[msgid].comments]
                 self[msgid].comments.extend(comments)
             if references:
-                references = [ref for ref in references
-                              if ref not in self[msgid].references]
+                references = [
+                    ref for ref in references if ref not in self[msgid].references
+                ]
                 self[msgid].references.extend(references)
             if automatic_comments:
-                automatic_comments = [ac for ac in automatic_comments if ac
-                                      not in self[msgid].automatic_comments]
+                automatic_comments = [
+                    ac
+                    for ac in automatic_comments
+                    if ac not in self[msgid].automatic_comments
+                ]
                 self[msgid].automatic_comments.extend(automatic_comments)
 
-    def add_missing(self, msgctl, defaultmsgstr='', mergewarn=None):
+    def add_missing(self, msgctl, defaultmsgstr="", mergewarn=None):
         """Each msgid that I miss and ``msgctl`` contains will be included in
         my catalog, including contextual information.
 
         Returns the ids that were added."""
         ids = []
         for key in msgctl:
             if key not in self:
                 entry = msgctl[key]
                 msgstr = defaultmsgstr or entry.msgstr
                 if isinstance(key, Message):
                     msgstr = key.default or msgstr
-                self.add(key, msgstr=msgstr, comments=entry.comments,
-                         references=entry.references,
-                         automatic_comments=entry.automatic_comments)
+                self.add(
+                    key,
+                    msgstr=msgstr,
+                    comments=entry.comments,
+                    references=entry.references,
+                    automatic_comments=entry.automatic_comments,
+                )
                 ids.append(key)
             elif mergewarn:
-                message = 'Merge-Warning: Key is already in target-catalog: %s'\
-                    % key
-                if not PY3:
-                    message = message.encode('utf-8')
+                message = "Merge-Warning: Key is already in target-catalog: %s" % key
                 sys.stderr.write(message)
 
         return ids
 
     def merge(self, msgctl):
         """Each msgid that I miss and ``msgctl`` contains will be included in
         my catalog."""
         for key in msgctl:
             entry = msgctl[key]
-            self.add(key, msgstr=entry.msgstr, comments=entry.comments,
-                     references=entry.references,
-                     automatic_comments=entry.automatic_comments)
+            self.add(
+                key,
+                msgstr=entry.msgstr,
+                comments=entry.comments,
+                references=entry.references,
+                automatic_comments=entry.automatic_comments,
+            )
 
     def sync(self, msgctl):
         """Syncronize the catalog with the given one. This removes all messages
         which are not found anymore in the new catalog, adds additional ones
         and overwrites the comments with the ones from the given catalog. This
         is used in the sync command.
         """
-        removed_msgids = [quote(msgid)
-                          for msgid in self.accept_ids(msgctl.keys())]
+        removed_msgids = [quote(msgid) for msgid in self.accept_ids(msgctl.keys())]
         self.overwrite_context(msgctl)
-        added_msgids = [quote(msgid)
-                        for msgid in self.add_missing(msgctl)]
+        added_msgids = [quote(msgid) for msgid in self.add_missing(msgctl)]
 
-        self.mime_header[
-            'POT-Creation-Date'] = msgctl.mime_header['POT-Creation-Date']
+        self.mime_header["POT-Creation-Date"] = msgctl.mime_header["POT-Creation-Date"]
 
         return (added_msgids, removed_msgids)
 
     def overwrite_context(self, msgctl):
         """For each message in the given message catalog that I know of,
         I will overwrite my contextual information with the given catalog's
         one."""
@@ -361,53 +373,54 @@
 
     def _initialize_with(self, filename):
         # reading in text mode, but likely to contain bytes
         file = open(filename)
         parser = POParser(file)
         parser.read()
         file.close()
-        header = parser.msgdict.get('')
+        header = parser.msgdict.get("")
         if header is None:
             sys.stderr.write(
                 "%s misses 'msgid \"\"' and 'msgstr \"\"' "
-                "near the top. Will be fixed." % filename)
+                "near the top. Will be fixed." % filename
+            )
         else:
             try:
                 self.commentary_header = header.comments
                 self._parse_mime_header(header.msgstr)
-                del parser.msgdict['']
+                del parser.msgdict[""]
             except KeyError:
                 sys.stderr.write("%s lacks MIME header." % filename)
         # Update the file after the header has been read.
         self.update(parser.msgdict)
 
     def _parse_mime_header(self, msgstr):
-        pairs = [line.split(':', 1) for line in msgstr.split(r'\n') if line]
+        pairs = [line.split(":", 1) for line in msgstr.split(r"\n") if line]
         for key, value in pairs:
             self.mime_header[key.strip()] = value.strip()
-            if key.lower() == 'domain':
+            if key.lower() == "domain":
                 self.domain = value.strip()
-            if key.lower() == 'content-type':
-                self.encoding = value.strip().lower().split('=')[-1]
+            if key.lower() == "content-type":
+                self.encoding = value.strip().lower().split("=")[-1]
 
 
 class POParser:
 
     """Parses an existing po- file and builds a dictionary according to
     MessageCatalog. POParser is the deserializer, POWriter the serializer.
     """
 
     def __init__(self, file):
         self._file = file
         self._in_paren = re.compile(r'"(.*)"')
         self.msgdict = OrderedDict()  # see MessageCatalog for structure
-        self.line = ''
+        self.line = ""
         self.sameMessageEntry = True
-        self.msgid = ''
-        self.msgstr = ''
+        self.msgid = ""
+        self.msgstr = ""
         self.references = []
         self.automatic_comments = []
         self.comments = []
 
     def read(self):
         """Start reading from file.
 
@@ -429,32 +442,32 @@
                 if newstatus:
                     self._readSameMessage()
                 else:
                     self._readNewMessage()
 
         # last msg
         if self.msgid not in self.msgdict:
-            self.line = '#:'
+            self.line = "#:"
             self._readNewMessage()
 
     def _readSameMessage(self):
         """We're reading a comment or msgid."""
         line = self.line
-        if line.startswith('msgstr'):
+        if line.startswith("msgstr"):
             self.sameMessageEntry = False
-        elif line.startswith('#:'):
+        elif line.startswith("#:"):
             self.references.append(line[2:].strip())
-        elif line.startswith('#.'):
+        elif line.startswith("#."):
             line = line[2:].rstrip()
             ls = line.startswith
             if ls(ORIGINAL_COMMENT):
                 line = line.replace(ORIGINAL_COMMENT, DEFAULT_COMMENT)
             if line not in self.automatic_comments:
                 self.automatic_comments.append(line)
-        elif line.startswith('#'):
+        elif line.startswith("#"):
             line = line[1:].rstrip()
             ls = line.startswith
             if ls(ORIGINAL_COMMENT) or ls(DEFAULT_COMMENT):
                 line = line.replace(ORIGINAL_COMMENT, DEFAULT_COMMENT)
                 if line not in self.automatic_comments:
                     self.automatic_comments.append(line)
             else:
@@ -463,107 +476,79 @@
             search = self._in_paren.search(line)
             if search:
                 self.msgid += search.groups()[0]
 
     def _readNewMessage(self):
         """We're reading msgstr."""
         sw = self.line.startswith
-        if sw('#') or sw('msgid'):
+        if sw("#") or sw("msgid"):
             self.sameMessageEntry = True
             self.msgdict[self.msgid] = MessageEntry(
-                self.msgid, msgstr=self.msgstr, references=self.references,
+                self.msgid,
+                msgstr=self.msgstr,
+                references=self.references,
                 automatic_comments=self.automatic_comments,
-                comments=self.comments)
+                comments=self.comments,
+            )
             # reset variables
-            self.msgid = self.msgstr = ''
+            self.msgid = self.msgstr = ""
             self.references = []
             self.automatic_comments = []
             self.comments = []
         else:
             search = self._in_paren.search(self.line)
             if search:
                 self.msgstr += search.groups()[0]
 
 
 class POWriter:
-
     def __init__(self, file, catalog):
-        """Initialize a POWriter with a filelike object that I am to write to.
-        """
+        """Initialize a POWriter with a filelike object that I am to write to."""
         self._file = file
         self._msgctl = catalog
 
-    def _encode(self, line, input_encoding=None, output_encoding=None):
-        """encode a given unicode type or string type to string type
-        in encoding output_encoding
-        """
-        if PY3:
-            return line
-        # all of the below is a python2-only unicode hack
-        # just goes to show why python3 was needed
-
-        content_type = self._msgctl.mime_header.get(
-            'Content-Type', 'text/plain; charset=utf-8')
-        charset = content_type.split('=')
-        encoding = charset[-1]
-
-        # check if input is not type unicode
-        if not isinstance(line, unicode):
-            if input_encoding is None:
-                # get input encoding from message catalog
-                input_encoding = encoding
-            line = unicode(line, input_encoding)
-
-        if output_encoding is None:
-            # get output encoding from message catalog
-            output_encoding = encoding
-
-        return line.encode(output_encoding)
-
     def _printToFile(self, file, string):
-        """ Print wrapper which allows to specifiy an output encoding"""
+        """Print wrapper which allows to specifiy an output encoding"""
         if string:
             string = string.strip()
-            file.write(self._encode(string))
-        file.write('\n')
+            file.write(string)
+        file.write("\n")
 
     def write(self, sort=True, msgstrToComment=False, sync=False):
         """Start writing to file."""
         self._write_header()
-        self._write_messages(
-            sort=sort, msgstrToComment=msgstrToComment, sync=sync)
+        self._write_messages(sort=sort, msgstrToComment=msgstrToComment, sync=sync)
 
     def _write_header(self):
         """Writes out commentary and mime headers."""
         ctl = self._msgctl
         f = self._file
 
         # header
         for line in ctl.commentary_header:
-            self._printToFile(f, '#%s' % line)
+            self._printToFile(f, "#%s" % line)
 
         if not ctl.mime_header:  # mime-header n/a
             self._printToFile(f, False)
             return
 
         # write out mime:
         self._printToFile(f, 'msgid ""')
         self._printToFile(f, 'msgstr ""')
 
         for key in ctl.mime_header.keys():
-            self._printToFile(f, '"%s: %s\\n"' % (key, ctl.mime_header[key]))
+            self._printToFile(f, f'"{key}: {ctl.mime_header[key]}\\n"')
 
     def _write_messages(self, sort, msgstrToComment, sync):
         """Writes the messages out."""
         f = self._file
         ids = sorted(self._msgctl.keys())
         for id in ids:
             entry = self._msgctl[id]
-            self._print_entry(
-                f, id, entry, msgstrToComment=msgstrToComment, sync=sync)
+            self._print_entry(f, id, entry, msgstrToComment=msgstrToComment, sync=sync)
 
     def _create_msgid(self, value):
         # Wrap over multiple lines if needed.
         values = wrapString(value)
         # Quote all lines and separate them by newlines.
         return 'msgid "%s"' % '"\n"'.join(values)
 
@@ -581,169 +566,164 @@
         comments = entry.comments
         automatic_comments = entry.automatic_comments
 
         msg_changed = False
         fuzzy = False
 
         for comment in comments:
-            if not comment.startswith(', fuzzy')\
-                    and not comment.startswith(' , fuzzy'):
-                self._printToFile(f, '#%s' % comment)
+            if not comment.startswith(", fuzzy") and not comment.startswith(" , fuzzy"):
+                self._printToFile(f, "#%s" % comment)
             else:
                 fuzzy = True
 
         # used in pot methods
         if msgstrToComment and msgstr:
             # no html markup in the default comments as these are not
             # allowed in msgstr's either
-            msgstr = msgstr.replace('"', '\\\"')
-            msgstr = msgstr.replace('\n', '\\n')
-            msgstr = msgstr.replace('&quot;', '\\\"')
-            msgstr = msgstr.replace('&#xa0;', ' ')
-            msgstr = msgstr.replace('&amp;', '&')
-            msgstr = msgstr.replace('&hellip;', u'\u2026')
-            msgstr = msgstr.replace('&#8230;', u'\u2026')
-            msgstr = msgstr.replace('&mdash;', u'\u2014')
-            msgstr = msgstr.replace('&#9632;', u'\u25A0')
-            msgstr = msgstr.replace('&#9675;', u'\u25CB')
-            msgstr = msgstr.replace('&#9679;', u'\u25CF')
-            self._printToFile(f, '#.%s"%s"' % (DEFAULT_COMMENT, msgstr))
-            msgstr = ''
+            msgstr = msgstr.replace('"', '\\"')
+            msgstr = msgstr.replace("\n", "\\n")
+            msgstr = msgstr.replace("&quot;", '\\"')
+            msgstr = msgstr.replace("&#xa0;", " ")
+            msgstr = msgstr.replace("&amp;", "&")
+            msgstr = msgstr.replace("&hellip;", "\u2026")
+            msgstr = msgstr.replace("&#8230;", "\u2026")
+            msgstr = msgstr.replace("&mdash;", "\u2014")
+            msgstr = msgstr.replace("&#9632;", "\u25A0")
+            msgstr = msgstr.replace("&#9675;", "\u25CB")
+            msgstr = msgstr.replace("&#9679;", "\u25CF")
+            self._printToFile(f, f'#.{DEFAULT_COMMENT}"{msgstr}"')
+            msgstr = ""
 
         # used in sync to filter duplicate default comments
         if sync:
             default_comments = [
-                o for o in automatic_comments if o.startswith(DEFAULT_COMMENT)]
+                o for o in automatic_comments if o.startswith(DEFAULT_COMMENT)
+            ]
             if len(default_comments) > 1:
                 msg_changed = True
                 # the first element is the old comment, the second the new one
                 automatic_comments.remove(default_comments[0])
 
         for ac in automatic_comments:
-            self._printToFile(f, '#.%s' % ac)
+            self._printToFile(f, "#.%s" % ac)
 
         # key is the filename, value is the filename or filename:lineno
         refs = {}
         for ref in entry.references:
-            pparts = ref.split('Products%s' % os.sep)
-            p2parts = ref.split('products%s' % os.sep)
-            sparts = ref.split('src%s' % os.sep, 1)
+            pparts = ref.split("Products%s" % os.sep)
+            p2parts = ref.split("products%s" % os.sep)
+            sparts = ref.split("src%s" % os.sep, 1)
             if len(pparts) > 1:
                 ref = pparts[1]
             elif len(p2parts) > 1:
                 ref = p2parts[1]
             elif len(sparts) > 1:
                 ref = sparts[1]
             # Normalize path separators to unix-style
-            ref.replace(os.sep, '/')
+            ref.replace(os.sep, "/")
 
             # We can have two references to the same file
             # but with different line number. We only include
             # the reference once.
-            filename = ref.split(':')[0]
+            filename = ref.split(":")[0]
             if filename not in refs:
                 refs[filename] = ref
 
         # Support for max number of references
         refs_values = sorted(refs.values())
-#        include_ellipsis = MAX_OCCUR is not None and \
-#                           len(refs_values[MAX_OCCUR:])
+        #        include_ellipsis = MAX_OCCUR is not None and \
+        #                           len(refs_values[MAX_OCCUR:])
         for idx, ref in enumerate(refs_values[:MAX_OCCUR]):
-            self._printToFile(f, '#: %s' % ref)
-#            if include_ellipsis and idx == MAX_OCCUR - 1:
-# self._printToFile(f, '#: %s' % ref)
-# self._printToFile(f, '#: ...')
+            self._printToFile(f, "#: %s" % ref)
+        #            if include_ellipsis and idx == MAX_OCCUR - 1:
+        # self._printToFile(f, '#: %s' % ref)
+        # self._printToFile(f, '#: ...')
 
         if msgstr and (msg_changed or fuzzy):
-            self._printToFile(f, '#, fuzzy')
+            self._printToFile(f, "#, fuzzy")
 
         # Add backslash escape to id.
-        if '"' in id and u'\\"' not in id:
+        if '"' in id and '\\"' not in id:
             id = id.replace('"', '\\"')
 
         self._printToFile(f, self._create_msgid(id))
-        if '\\n' not in msgstr:
+        if "\\n" not in msgstr:
             self._printToFile(f, self._create_msgstr(msgstr))
         else:
             self._printToFile(f, 'msgstr ""')
-            lines = msgstr.split('\\n')
+            lines = msgstr.split("\\n")
             for line in lines[:-1]:
                 # Restore the literal backslash-n at the end
-                line += '\\n'
+                line += "\\n"
                 # Wrap over multiple lines if needed.
                 newline = wrapAndQuoteString(line)
                 self._printToFile(f, newline)
             if lines[-1]:
                 # This is the part after the last literal backslash-n
                 newline = wrapAndQuoteString(lines[-1])
                 self._printToFile(f, newline)
 
 
 class PTReader:
-    """Reads in a list of page templates.
-    """
-
-    def __init__(self, path, domain='none', exclude=(), include_line_numbers=True):
+    """Reads in a list of page templates."""
 
+    def __init__(self, path, domain="none", exclude=(), include_line_numbers=True):
         self.domain = domain
         self.catalogs = {}  # keyed by domain name
         self.path = path
         self.exclude = exclude
         self.include_line_numbers = include_line_numbers
 
     def read(self):
         """Reads in from all given ZPTs and builds up MessageCatalogs accordingly.
 
         The MessageCatalogs can after this call be accessed through attribute
         ``catalogs``, which indexes the MessageCatalogs by their domain.
         """
         from .extract import tal_strings
-        tal = tal_strings(self.path, domain=self.domain,
-                          exclude=self.exclude + ('tests', 'docs'))
 
-        for msgid in tal:
+        tal = tal_strings(
+            self.path, domain=self.domain, exclude=self.exclude + ("tests", "docs")
+        )
 
-            msgstr = msgid.default or ''
+        for msgid in tal:
+            msgstr = msgid.default or ""
 
-            if msgid and msgid != '${DYNAMIC_CONTENT}':
+            if msgid and msgid != "${DYNAMIC_CONTENT}":
                 if self.include_line_numbers:
-                    filenames = [l[0] + ':' + str(l[1]) for l in tal[msgid]]
+                    filenames = [line[0] + ":" + str(line[1]) for line in tal[msgid]]
                 else:
-                    filenames = sorted(set([l[0] for l in tal[msgid]]))
-                self._add_msg(msgid,
-                              msgstr,
-                              [],
-                              filenames,
-                              [],
-                              self.domain)
+                    filenames = sorted({line[0] for line in tal[msgid]})
+                self._add_msg(msgid, msgstr, [], filenames, [], self.domain)
 
         return []
 
-    def _add_msg(self, msgid, msgstr, comments, filename, automatic_comments,
-                 domain):
-
+    def _add_msg(self, msgid, msgstr, comments, filename, automatic_comments, domain):
         if not domain:
-            sys.stderr.write('No domain name for msgid "%s" in %s\n' %
-                             (msgid, filename))
+            sys.stderr.write(
+                'No domain name for msgid "%s" in %s\n' % (msgid, filename)
+            )
             return
 
         if domain not in self.catalogs:
             self.catalogs[domain] = MessageCatalog(domain=domain)
 
-        self.catalogs[domain].add(msgid, msgstr=msgstr, comments=comments,
-                                  references=filename,
-                                  automatic_comments=automatic_comments)
+        self.catalogs[domain].add(
+            msgid,
+            msgstr=msgstr,
+            comments=comments,
+            references=filename,
+            automatic_comments=automatic_comments,
+        )
 
 
 class PYReader:
-    """Reads in a list of python scripts.
-    """
+    """Reads in a list of python scripts."""
 
     def __init__(self, path, domain, exclude=(), include_line_numbers=True):
-
         self.domain = domain
         self.catalogs = {}  # keyed by domain name
         self.path = path
         self.exclude = exclude
         self.include_line_numbers = include_line_numbers
 
     def read(self):
@@ -755,48 +735,46 @@
 
         read returns the list of tuples (filename, errormsg), where filename
         is the name of the file that could not be read and errormsg a human
         readable error message.
         """
 
         from .extract import py_strings
-        py = py_strings(self.path, self.domain,
-                        exclude=self.exclude + ('tests', ))
+
+        py = py_strings(self.path, self.domain, exclude=self.exclude + ("tests",))
 
         for msgid in py:
             if self.include_line_numbers:
-                filenames = [l[0] + ':' + str(l[1]) for l in py[msgid]]
+                filenames = [line[0] + ":" + str(line[1]) for line in py[msgid]]
             else:
-                filenames = sorted(set([l[0] for l in py[msgid]]))
-            self._add_msg(msgid,
-                          msgid.default or '',
-                          [],
-                          filenames,
-                          [],
-                          self.domain)
+                filenames = sorted({line[0] for line in py[msgid]})
+            self._add_msg(msgid, msgid.default or "", [], filenames, [], self.domain)
         return []
 
-    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments,
-                 domain):
+    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments, domain):
         if not domain:
-            sys.stderr.write('No domain name for msgid "%s" in %s\n' %
-                             (msgid, references))
+            sys.stderr.write(
+                'No domain name for msgid "%s" in %s\n' % (msgid, references)
+            )
             return
 
         if domain not in self.catalogs:
             self.catalogs[domain] = MessageCatalog(domain=domain)
 
-        self.catalogs[domain].add(msgid, msgstr=msgstr, comments=comments,
-                                  references=references,
-                                  automatic_comments=automatic_comments)
+        self.catalogs[domain].add(
+            msgid,
+            msgstr=msgstr,
+            comments=comments,
+            references=references,
+            automatic_comments=automatic_comments,
+        )
 
 
-class GSReader(object):
-    """Reads in a list of GenericSetup profile files.
-    """
+class GSReader:
+    """Reads in a list of GenericSetup profile files."""
 
     def __init__(self, path, domain, exclude=(), include_line_numbers=True):
         self.domain = domain
         self.catalogs = {}  # keyed by domain name
         self.path = path
         self.exclude = exclude
         # Note: the current extractor does not give us line numbers at all.
@@ -811,45 +789,43 @@
 
         read returns the list of tuples (filename, errormsg), where filename
         is the name of the file that could not be read and errormsg a human
         readable error message.
         """
 
         from .gsextract import gs_strings
-        gs = gs_strings(self.path, self.domain,
-                        exclude=self.exclude + ('tests', ))
+
+        gs = gs_strings(self.path, self.domain, exclude=self.exclude + ("tests",))
 
         for domain in gs:
             for msgid in gs[domain]:
-                self._add_msg(msgid[0],
-                              msgid[1],
-                              [],
-                              [msgid[2]],
-                              [],
-                              domain)
+                self._add_msg(msgid[0], msgid[1], [], [msgid[2]], [], domain)
         return []
 
-    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments,
-                 domain):
+    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments, domain):
         if not domain:
-            sys.stderr.write('No domain name for msgid "%s" in %s\n' %
-                             (msgid, references))
+            sys.stderr.write(
+                'No domain name for msgid "%s" in %s\n' % (msgid, references)
+            )
             return
 
         if domain not in self.catalogs:
             self.catalogs[domain] = MessageCatalog(domain=domain)
 
-        self.catalogs[domain].add(msgid, msgstr=msgstr, comments=comments,
-                                  references=references,
-                                  automatic_comments=automatic_comments)
+        self.catalogs[domain].add(
+            msgid,
+            msgstr=msgstr,
+            comments=comments,
+            references=references,
+            automatic_comments=automatic_comments,
+        )
 
 
-class ZCMLReader(object):
-    """Reads in a list of ZCML files.
-    """
+class ZCMLReader:
+    """Reads in a list of ZCML files."""
 
     def __init__(self, path, domain, exclude=(), include_line_numbers=True):
         self.domain = domain
         self.catalogs = {}  # keyed by domain name
         self.path = path
         self.exclude = exclude
         self.include_line_numbers = include_line_numbers
@@ -863,37 +839,36 @@
 
         read returns the list of tuples (filename, errormsg), where filename
         is the name of the file that could not be read and errormsg a human
         readable error message.
         """
 
         from .zcmlextract import zcml_strings
-        zcml = zcml_strings(self.path, self.domain,
-                            exclude=self.exclude + ('tests', ))
+
+        zcml = zcml_strings(self.path, self.domain, exclude=self.exclude + ("tests",))
 
         for domain in zcml:
             for msgid in zcml[domain]:
                 # We only have one filename.
                 filename = msgid[2]
                 if not self.include_line_numbers:
                     filename = filename.split(":")[0]
-                self._add_msg(msgid[0],
-                              msgid[1],
-                              [],
-                              [filename],
-                              [],
-                              domain)
+                self._add_msg(msgid[0], msgid[1], [], [filename], [], domain)
         return []
 
-    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments,
-                 domain):
+    def _add_msg(self, msgid, msgstr, comments, references, automatic_comments, domain):
         if not domain:
-            sys.stderr.write('No domain name for msgid "%s" in %s\n' %
-                             (msgid, references))
+            sys.stderr.write(
+                'No domain name for msgid "%s" in %s\n' % (msgid, references)
+            )
             return
 
         if domain not in self.catalogs:
             self.catalogs[domain] = MessageCatalog(domain=domain)
 
-        self.catalogs[domain].add(msgid, msgstr=msgstr, comments=comments,
-                                  references=references,
-                                  automatic_comments=automatic_comments)
+        self.catalogs[domain].add(
+            msgid,
+            msgstr=msgstr,
+            comments=comments,
+            references=references,
+            automatic_comments=automatic_comments,
+        )
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/common.py` & `i18ndude-6.1.0/src/i18ndude/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,73 @@
-from lxml import etree
 from io import StringIO
+from lxml import etree
+
 import re
 
-import sys
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
 
 # These are included in the file if missing.
 DEFAULT_DECL = {
-    '<!DOCTYPE':
-    '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" '
+    "<!DOCTYPE": '<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" '
     '"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">',
-
-    '<?xml': '<?xml version="1.0" encoding="utf-8"?>'
+    "<?xml": '<?xml version="1.0" encoding="utf-8"?>',
 }
 HTML_PARSER = etree.HTMLParser()
 
 
 def prepare_xml(file):
     """Tidies up things within the zpts."""
 
-    content = ''.join(file.readlines())
+    content = "".join(file.readlines())
 
-    for el in ['<!DOCTYPE', '<?xml']:
+    for el in ["<!DOCTYPE", "<?xml"]:
         idx = content.find(el)
         if idx >= 0:
             if content[0:idx].strip():
-                idx2 = content.find('>', idx + 1)
-                extraction = content[idx:idx2 + 1]
-                content = extraction + content[:idx] + content[idx2 + 1:]
+                idx2 = content.find(">", idx + 1)
+                extraction = content[idx : idx2 + 1]
+                content = extraction + content[:idx] + content[idx2 + 1 :]
                 # mispositioned element fixed at this point
         else:  # element was not found, replace with default
             content = DEFAULT_DECL[el] + content
 
     # We want namespace declarations for tal, metal and i18n.
     # http://sf.net/tracker/?func=detail&atid=516339&aid=982527&group_id=66950
-    mobj = re.search(r'<([a-zA-Z]+)', content)
+    mobj = re.search(r"<([a-zA-Z]+)", content)
     if mobj:
-        if mobj.group(1) == 'html':
+        if mobj.group(1) == "html":
             m = mobj.end()
-            extra = ''
-            if 'xmlns:i18n=' not in content:
+            extra = ""
+            if "xmlns:i18n=" not in content:
                 extra += 'xmlns:i18n="http://xml.zope.org/namespaces/i18n" '
-            if 'xmlns:metal=' not in content:
+            if "xmlns:metal=" not in content:
                 extra += 'xmlns:metal="http://xml.zope.org/namespaces/metal" '
-            if 'xmlns:tal=' not in content:
+            if "xmlns:tal=" not in content:
                 extra += 'xmlns:tal="http://xml.zope.org/namespaces/tal">'
             if extra:
-                content = content[:m] + ' ' + extra + content[m:]
+                content = content[:m] + " " + extra + content[m:]
         else:
             m = mobj.start()
             content = (
-                content[:m] +
-                '<html ' +
-                'xmlns:i18n="http://xml.zope.org/namespaces/i18n" '
-                'xmlns:metal="http://xml.zope.org/namespaces/metal" ' +
-                'xmlns:tal="http://xml.zope.org/namespaces/tal">' +
-                '<head><title></title></head><body>' +
-                content[m:] +
-                '</body></html>')
+                content[:m]
+                + "<html "
+                + 'xmlns:i18n="http://xml.zope.org/namespaces/i18n" '
+                'xmlns:metal="http://xml.zope.org/namespaces/metal" '
+                + 'xmlns:tal="http://xml.zope.org/namespaces/tal">'
+                + "<head><title></title></head><body>"
+                + content[m:]
+                + "</body></html>"
+            )
 
     content = content.strip()
-    if not isinstance(content, unicode):
+    if not isinstance(content, str):
         try:
-            content = content.decode('utf-8')
+            content = content.decode("utf-8")
         except UnicodeDecodeError:
-            print('ERROR: {} not decodable as utf-8'.format(file.name))
-            content = u''
+            print(f"ERROR: {file.name} not decodable as utf-8")
+            content = ""
     return StringIO(content)
 
 
 def tree_content(tree):
     content = etree.tostring(tree)
     if content is None:
         return
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/extract.py` & `i18ndude-6.1.0/src/i18ndude/extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python2.4
-# -*- coding: utf-8 -*-
 ##############################################################################
 #
 # Copyright (c) 2003 Zope Corporation and Contributors.
 # All Rights Reserved.
 #
 # This software is subject to the provisions of the Zope Public License,
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
@@ -12,47 +11,42 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Extract message strings from python modules, page template files
 and ZCML files.
 """
-__docformat__ = 'restructuredtext'
+__docformat__ = "restructuredtext"
 
 # INFO: This is a modified copy of zope3's zope.app.locales.extract (r71023).
 
-from .pygettext import safe_eval, normalize, make_escapes
+from .pygettext import make_escapes
+from .pygettext import normalize
+from .pygettext import safe_eval
+from i18ndude.generator import DudeGenerator
+
+# Modified, as we don't want a dependency on zope.app.locales
+# from zope.app.locales.interfaces import IPOTEntry, IPOTMaker, ITokenEater
+from i18ndude.interfaces import IPOTEntry
+from i18ndude.interfaces import IPOTMaker
+from i18ndude.interfaces import ITokenEater
 from zope.i18nmessageid import Message
 from zope.interface import implementer
+
 import fnmatch
 import os
 import sys
 import time
 import tokenize
 import traceback
 
-# Modified, as we don't want a dependency on zope.app.locales
-# from zope.app.locales.interfaces import IPOTEntry, IPOTMaker, ITokenEater
-from i18ndude.interfaces import IPOTEntry, IPOTMaker, ITokenEater
-from i18ndude.generator import DudeGenerator
 
-DEFAULT_CHARSET = 'utf-8'
-DEFAULT_ENCODING = '8bit'
-PY3 = sys.version_info > (3,)
-
-# Sigh. The `tokenize.tokenize()` API deprecated in py22 is actually the
-# py36 API, but not in a py27 backward compatible way. And the py27 API
-# `tokenize.generate_tokens()` apparently exists, but is undocumented and
-# chokes in py36 in a forward incompatible way.
-
-if PY3:
-    unicode = str
-    py2orpy3_tokenize = tokenize.tokenize
-else:
-    py2orpy3_tokenize = tokenize.generate_tokens
+DEFAULT_CHARSET = "utf-8"
+DEFAULT_ENCODING = "8bit"
+
 
 # Modified header, which is more suitable for any project
 
 # pot_header = '''\
 # ##############################################################################
 # #
 # # Copyright (c) 2003-2004 Zope Corporation and Contributors.
@@ -76,33 +70,33 @@
 # "MIME-Version: 1.0\\n"
 # "Content-Type: text/plain; charset=%(charset)s\\n"
 # "Content-Transfer-Encoding: %(encoding)s\\n"
 # "Generated-By: zope/app/locales/extract.py\\n"
 #
 # '''
 
-pot_header = '''\
+pot_header = """\
 msgid ""
 msgstr ""
 "Project-Id-Version: %(version)s\\n"
 "POT-Creation-Date: %(time)s\\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\\n"
 "Language-Team: LANGUAGE <LL@li.org>\\n"
 "MIME-Version: 1.0\\n"
 "Content-Type: text/plain; charset=%(charset)s\\n"
 "Content-Transfer-Encoding: %(encoding)s\\n"
 "Plural-Forms: nplurals=1; plural=0\\n",
 "Generated-By: i18ndude\\n"
 
-'''
+"""
 
 
 @implementer(IPOTEntry)
-class POTEntry(object):
+class POTEntry:
     r"""This class represents a single message entry in the POT file.
 
     >>> import sys
     >>> make_escapes(0)
     >>> class FakeFile(object):
     ...     def write(self, data):
     ...         sys.stdout.write(data)
@@ -141,97 +135,96 @@
     msgid "send"
     msgstr ""
     <BLANKLINE>
     """
 
     def __init__(self, msgid, comments=None):
         self.msgid = msgid
-        self.comments = comments or ''
+        self.comments = comments or ""
 
     def addComment(self, comment):
-        self.comments += comment + '\n'
+        self.comments += comment + "\n"
 
     def addLocationComment(self, filename, line):
-        self.comments += '#: %s:%s\n' % (
-            filename.replace(os.sep, '/'), line)
+        self.comments += "#: {}:{}\n".format(filename.replace(os.sep, "/"), line)
 
     def write(self, file):
         if self.comments:
             file.write(self.comments)
-        if (isinstance(self.msgid, Message) and
-                self.msgid.default is not None):
+        if isinstance(self.msgid, Message) and self.msgid.default is not None:
             default = self.msgid.default.strip()
             lines = normalize(default).split("\n")
             lines[0] = "#. Default: %s\n" % lines[0]
             for i in range(1, len(lines)):
                 lines[i] = "#.  %s\n" % lines[i]
             file.write("".join(lines))
-        file.write('msgid %s\n' % normalize(self.msgid))
+        file.write("msgid %s\n" % normalize(self.msgid))
         file.write('msgstr ""\n')
-        file.write('\n')
-
-    def __cmp__(self, other):
-        return cmp(self.comments, other.comments)
+        file.write("\n")
 
 
 @implementer(IPOTMaker)
-class POTMaker(object):
-    """This class inserts sets of strings into a POT file.
-    """
+class POTMaker:
+    """This class inserts sets of strings into a POT file."""
 
     def __init__(self, output_fn, path):
         self._output_filename = output_fn
         self.path = path
         self.catalog = {}
 
     def add(self, strings, base_dir=None):
         for msgid, locations in strings.items():
-            if msgid == '':
+            if msgid == "":
                 continue
             if msgid not in self.catalog:
                 self.catalog[msgid] = POTEntry(msgid)
 
             for filename, lineno in locations:
                 if base_dir is not None:
-                    filename = filename.replace(base_dir, '')
+                    filename = filename.replace(base_dir, "")
                 self.catalog[msgid].addLocationComment(filename, lineno)
 
     def _getProductVersion(self):
         # First, try to get the product version
-        fn = os.path.join(self.path, 'version.txt')
+        fn = os.path.join(self.path, "version.txt")
         if os.path.exists(fn):
-            return open(fn, 'r').read().strip()
+            return open(fn).read().strip()
 
         # Do not fall back to the Zope version, as this makes no sense for the
         # general project.
 
         # # Second, try to find a Zope version
         # from zope.app.applicationcontrol.zopeversion import ZopeVersionUtility  # noqa
         # return ZopeVersionUtility.getZopeVersion()
-        return 'PACKAGE VERSION'
+        return "PACKAGE VERSION"
 
     def write(self):
-        file = open(self._output_filename, 'w')
-        file.write(pot_header % {'time': time.ctime(),
-                                 'version': self._getProductVersion(),
-                                 'charset': DEFAULT_CHARSET,
-                                 'encoding': DEFAULT_ENCODING})
+        file = open(self._output_filename, "w")
+        file.write(
+            pot_header
+            % {
+                "time": time.ctime(),
+                "version": self._getProductVersion(),
+                "charset": DEFAULT_CHARSET,
+                "encoding": DEFAULT_ENCODING,
+            }
+        )
 
         # Sort the catalog entries by filename
         catalog = sorted(self.catalog.values())
 
         # Write each entry to the file
         for entry in catalog:
             entry.write(file)
 
         file.close()
 
 
 @implementer(ITokenEater)
-class TokenEater(object):
+class TokenEater:
     """This is almost 100% taken from `pygettext.py`, except that I
     removed all option handling and output a dictionary.
 
     >>> eater = TokenEater()
     >>> make_escapes(0)
 
     TokenEater eats tokens generated by the standard python module
@@ -242,109 +235,109 @@
 
     We feed it a (fake) file:
 
     >>> file = BytesIO((
     ...     "_(u'hello ${name}', u'buenos dias', {'name': 'Bob'}); "
     ...     "_(u'hi ${name}', mapping={'name': 'Bob'})"
     ...     ).encode('utf-8'))
-    >>> g = py2orpy3_tokenize(file.readline)
+    >>> g = tokenize.tokenize(file.readline)
     >>> for ttype, tstring, stup, etup, line in g:
     ...     eater(ttype, tstring, stup, etup, line)
 
     The catalog of collected message ids contains our example
 
     >>> catalog = eater.getCatalog()
     >>> items = sorted(list(catalog.items()))
     >>> expect = [(u'hello ${name}', [(None, 1)]),
     ...           (u'hi ${name}', [(None, 1)])]
     >>> items == expect
     True
 
-    The key in the catalog is not a unicode string, it's a real
+    The key in the catalog is not a string, it's a real
     message id with a default value:
 
     >>> msgid = items.pop(0)[0]
     >>> msgid == u'hello ${name}'
     True
     >>> msgid.default == u'buenos dias'
     True
 
     >>> msgid = items.pop(0)[0]
     >>> msgid == u'hi ${name}'
     True
     >>> msgid.default == u''
     True
 
-    Note that everything gets converted to unicode.
+    Note that everything gets converted to string.
     """
 
     def __init__(self):
         self.__messages = {}
         self.__state = self.__waiting
         self.__data = []
         self.__lineno = -1
         self.__freshmodule = 1
         self.__curfile = None
 
     def __call__(self, ttype, tstring, stup, etup, line):
         self.__state(ttype, tstring, stup[0])
 
     def __waiting(self, ttype, tstring, lineno):
-        if ttype == tokenize.NAME and tstring in ['_']:
+        if ttype == tokenize.NAME and tstring in ["_"]:
             self.__state = self.__keywordseen
 
     def __suiteseen(self, ttype, tstring, lineno):
         # ignore anything until we see the colon
-        if ttype == tokenize.OP and tstring == ':':
+        if ttype == tokenize.OP and tstring == ":":
             self.__state = self.__suitedocstring
 
     def __suitedocstring(self, ttype, tstring, lineno):
         # ignore any intervening noise
         if ttype == tokenize.STRING:
             self.__addentry(safe_eval(tstring), lineno, isdocstring=1)
             self.__state = self.__waiting
-        elif ttype not in (tokenize.NEWLINE, tokenize.INDENT,
-                           tokenize.COMMENT):
+        elif ttype not in (tokenize.NEWLINE, tokenize.INDENT, tokenize.COMMENT):
             # there was no class docstring
             self.__state = self.__waiting
 
     def __keywordseen(self, ttype, tstring, lineno):
-        if ttype == tokenize.OP and tstring == '(':
+        if ttype == tokenize.OP and tstring == "(":
             self.__data = []
-            self.__msgid = ''
-            self.__default = ''
+            self.__msgid = ""
+            self.__default = ""
             self.__lineno = lineno
             self.__state = self.__openseen
         else:
             self.__state = self.__waiting
 
     def __openseen(self, ttype, tstring, lineno):
-        if ((ttype == tokenize.OP and tstring == ')') or
-                (ttype == tokenize.NAME and tstring == 'mapping')):
+        if (ttype == tokenize.OP and tstring == ")") or (
+            ttype == tokenize.NAME and tstring == "mapping"
+        ):
             # We've seen the last of the translatable strings.  Record the
             # line number of the first line of the strings and update the list
             # of messages seen.  Reset state for the next batch.  If there
             # were no strings inside _(), then just ignore this entry.
             if self.__data or self.__msgid:
                 if self.__default:
                     msgid = self.__msgid
                     default = self.__default
                 elif self.__msgid:
                     msgid = self.__msgid
-                    default = ''.join(self.__data)
+                    default = "".join(self.__data)
                 else:
-                    msgid = ''.join(self.__data)
+                    msgid = "".join(self.__data)
                     default = None
                 self.__addentry(msgid, default)
             self.__state = self.__waiting
-        elif ttype == tokenize.OP and tstring == ',':
+        elif ttype == tokenize.OP and tstring == ",":
             if not self.__msgid:
-                self.__msgid = ''.join(self.__data)
+                self.__msgid = "".join(self.__data)
             elif not self.__default:
-                self.__default = ''.join(self.__data)
+                self.__default = "".join(self.__data)
             self.__data = []
         elif ttype == tokenize.STRING:
             self.__data.append(safe_eval(tstring))
 
     # XXX: This is the original method from pystrings... maybe we need some
     #      of these changes.
 
@@ -376,33 +369,41 @@
     #         self.__state = self.__waiting
 
     def __addentry(self, msg, default=None, lineno=None, isdocstring=0):
         if lineno is None:
             lineno = self.__lineno
 
         if default is not None:
-            default = unicode(default)
+            default = str(default)
         msg = Message(msg, default=default)
         if msg in self.__messages:
             messages = list(self.__messages.keys())
             idx = messages.index(msg)
             existing_msg = messages[idx]
             if msg.default != existing_msg.default:
-                references = '\n'.join([
-                    location[0] + ':' + str(location[1])
-                    for location in self.__messages[msg].keys()
-                ])
+                references = "\n".join(
+                    [
+                        location[0] + ":" + str(location[1])
+                        for location in self.__messages[msg].keys()
+                    ]
+                )
                 # XXX this does not appear to have any test coverage
                 # the actual warnings are emitted by zope.tal
                 sys.stderr.write(
                     "Warning: msgid '%s' in %s already exists "
                     "with a different default (bad: %s, should be: %s)\n"
-                    "The references for the existent value are:\n%s\n" %
-                    (msg, self.__curfile + ':' + str(lineno),
-                     msg.default, existing_msg.default, references))
+                    "The references for the existent value are:\n%s\n"
+                    % (
+                        msg,
+                        self.__curfile + ":" + str(lineno),
+                        msg.default,
+                        existing_msg.default,
+                        references,
+                    )
+                )
         entry = (self.__curfile, lineno)
         self.__messages.setdefault(msg, {})[entry] = isdocstring
 
     def set_filename(self, filename):
         self.__curfile = filename
         self.__freshmodule = 1
 
@@ -429,143 +430,147 @@
 
 
 def find_files(dir, pattern, exclude=()):
     files = []
     folders = dir
 
     if isinstance(dir, str):
-        folders = (dir, )
+        folders = (dir,)
 
     def visit(files, dirpath, names):
         # exclude dirnames
         dirnames = dirpath.split(os.path.sep)
         for ex in exclude:
             if ex in dirnames:
                 return
         # exclude filenames and regexps for those
         for ex in exclude:
             names[:] = [x for x in names if not fnmatch.fnmatch(x, ex)]
-        files += [os.path.join(dirpath, name)
-                  for name in fnmatch.filter(names, pattern)]
+        files += [
+            os.path.join(dirpath, name) for name in fnmatch.filter(names, pattern)
+        ]
 
     for folder in folders:
         if os.path.isdir(folder):
             for dirpath, dirnames, filenames in os.walk(folder):
                 visit(files, dirpath, filenames)
         else:
             if fnmatch.filter([folder], pattern):
                 files.append(folder)
     return sorted(files)
 
+
 # We don't want to assume a default domain of Zope
 # def py_strings(dir, domain="zope", exclude=()):
 
 
 def py_strings(dir, domain="none", exclude=()):
-    """Retrieve all Python messages from `dir` that are in the `domain`.
-    """
+    """Retrieve all Python messages from `dir` that are in the `domain`."""
     eater = TokenEater()
     make_escapes(0)
     for filename in find_files(
-            # We want to include cpy and vpy scripts as well
-            # dir, '*.py', exclude=('extract.py', 'pygettext.py')+tuple(exclude)):  # noqa
-            dir,
-            '*.*py',
-            exclude=('extract.py', 'pygettext.py') + tuple(exclude)
-        ):
-        fp = open(filename, 'rb')  # tokenize expects bytes
+        # We want to include cpy and vpy scripts as well
+        # dir, '*.py', exclude=('extract.py', 'pygettext.py')+tuple(exclude)):  # noqa
+        dir,
+        "*.*py",
+        exclude=("extract.py", "pygettext.py") + tuple(exclude),
+    ):
+        fp = open(filename, "rb")  # tokenize expects bytes
         try:
             eater.set_filename(filename)
             try:
-                g = py2orpy3_tokenize(fp.readline)
+                g = tokenize.tokenize(fp.readline)
                 for ttype, tstring, stup, etup, line in g:
                     eater(ttype, tstring, stup, etup, line)
             except tokenize.TokenError as e:
-                sys.stderr.write('%s: %s, line %d, column %d' % (
-                    e[0], filename, e[1][0], e[1][1]))
+                sys.stderr.write(
+                    "%s: %s, line %d, column %d" % (e[0], filename, e[1][0], e[1][1])
+                )
         finally:
             fp.close()
     # One limitation of the Python message extractor is that it cannot
     # determine the domain of the string, since it is not contained anywhere
     # directly. The only way this could be done is by loading the module and
     # inspect the '_' function. For now we simply assume that all the found
     # strings have the domain the user specified.
     return eater.getCatalog()
 
 
 def zcml_strings(dir, domain="zope", site_zcml=None):
-    """Retrieve all ZCML messages from `dir` that are in the `domain`.
-    """
+    """Retrieve all ZCML messages from `dir` that are in the `domain`."""
     from zope.app.appsetup import config
+
     import zope
+
     dirpath = os.path.dirpath
     if site_zcml is None:
         # TODO this assumes a checkout directory structure
-        site_zcml = os.path.join(dirpath(dirpath(dirpath(zope.__file__))),
-                                 "site.zcml")
+        site_zcml = os.path.join(dirpath(dirpath(dirpath(zope.__file__))), "site.zcml")
     context = config(site_zcml, features=("devmode",), execute=False)
     return context.i18n_strings.get(domain, {})
 
 
 def tal_strings(dir, domain="zope", include_default_domain=False, exclude=()):
-    """Retrieve all TAL messages from `dir` that are in the `domain`.
-    """
+    """Retrieve all TAL messages from `dir` that are in the `domain`."""
     # We import zope.tal.talgettext here because we can't rely on the
     # right sys path until app_dir has run
-    from zope.tal.talgettext import POEngine, POTALInterpreter
     from zope.tal.htmltalparser import HTMLTALParser
+    from zope.tal.talgettext import POEngine
+    from zope.tal.talgettext import POTALInterpreter
     from zope.tal.talparser import TALParser
-    engine = POEngine()
 
-    class Devnull(object):
+    engine = POEngine()
 
+    class Devnull:
         def write(self, s):
             pass
 
-    for filename in (find_files(dir, '*.*pt', exclude=tuple(exclude)) +
-                     find_files(dir, '*.html', exclude=tuple(exclude)) +
-                     find_files(dir, '*.kupu', exclude=tuple(exclude)) +
-                     find_files(dir, '*.pox', exclude=tuple(exclude)) +
-                     find_files(dir, '*.xsl', exclude=tuple(exclude))):
+    for filename in (
+        find_files(dir, "*.*pt", exclude=tuple(exclude))
+        + find_files(dir, "*.html", exclude=tuple(exclude))
+        + find_files(dir, "*.kupu", exclude=tuple(exclude))
+        + find_files(dir, "*.pox", exclude=tuple(exclude))
+        + find_files(dir, "*.xsl", exclude=tuple(exclude))
+    ):
         engine.file = filename
         name, ext = os.path.splitext(filename)
         # First try with standard zope.tal parsers.
-        if ext == '.html' or ext.endswith('pt'):
+        if ext == ".html" or ext.endswith("pt"):
             parser = HTMLTALParser()
         else:
             parser = TALParser()
         try:
             parser.parseFile(filename)
             program, macros = parser.getCode()
-            POTALInterpreter(program, macros, engine, stream=Devnull(),
-                             metal=False)()
+            POTALInterpreter(program, macros, engine, stream=Devnull(), metal=False)()
         except KeyboardInterrupt:
             raise
-        except:  # Hee hee, I love bare excepts!
-            if ext == '.html' or ext.endswith('pt'):
+        except Exception:
+            if ext == ".html" or ext.endswith("pt"):
                 # We can have one retry with our own generator.
                 gen = DudeGenerator(xml=0)
                 parser = HTMLTALParser(gen=gen)
                 try:
                     parser.parseFile(filename)
                     program, macros = parser.getCode()
-                    POTALInterpreter(program, macros, engine, stream=Devnull(),
-                                     metal=False)()
-                except:  # Hee hee, I love bare excepts!
-                    print('There was an error processing', filename)
+                    POTALInterpreter(
+                        program, macros, engine, stream=Devnull(), metal=False
+                    )()
+                except Exception:
+                    print("There was an error processing", filename)
                     traceback.print_exc()
             else:
-                print('There was an error processing', filename)
+                print("There was an error processing", filename)
                 traceback.print_exc()
 
     # See whether anything in the domain was found
     if domain not in engine.catalog:
         return {}
     # We do not want column numbers.
     catalog = engine.catalog[domain].copy()
     # When the Domain is 'default', then this means that none was found;
     # Include these strings; yes or no?
     if include_default_domain:
-        catalog.update(engine.catalog['default'])
+        catalog.update(engine.catalog["default"])
     for msgid, locations in catalog.items():
-        catalog[msgid] = [(l[0], l[1][0]) for l in locations]
+        catalog[msgid] = [(loc[0], loc[1][0]) for loc in locations]
     return catalog
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/generator.py` & `i18ndude-6.1.0/src/i18ndude/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 from zope.tal import taldefs
 from zope.tal.taldefs import I18NError
 from zope.tal.taldefs import TAL_VERSION
 from zope.tal.taldefs import TALError
 from zope.tal.talgenerator import _parseI18nAttributes
 from zope.tal.talgenerator import TALGenerator
 from zope.tal.translationcontext import DEFAULT_DOMAIN
 from zope.tal.translationcontext import TranslationContext
 
 import re
 
 
-NOT_ALLOWED_IN_NAME = re.compile(r'[^\w-]')
+NOT_ALLOWED_IN_NAME = re.compile(r"[^\w-]")
 
 
 class DudeGenerator(TALGenerator):
 
     """Custom Generator that does not raise template errors.
 
     We have simply removed any TALErrors and METALErrors that would be
@@ -23,16 +22,24 @@
     of your template.  It needs to know just enough to be able to
     extract i18n information from it.
 
     Main use case: support default tal attributes plus
     chameleon-specific ones.
     """
 
-    def emitStartElement(self, name, attrlist, taldict, metaldict, i18ndict,
-                         position=(None, None), isend=0):
+    def emitStartElement(
+        self,
+        name,
+        attrlist,
+        taldict,
+        metaldict,
+        i18ndict,
+        position=(None, None),
+        isend=0,
+    ):
         if not taldict and not metaldict and not i18ndict:
             # Handle the simple, common case
             self.emitStartTag(name, attrlist, isend)
             self.todoPush({})
             if isend:
                 self.emitEndElement(name, isend)
             return
@@ -44,16 +51,17 @@
             taldict["content"] = taldict.pop("replace")
             replaced = True
 
         for key, value in i18ndict.items():
             if key not in taldefs.KNOWN_I18N_ATTRIBUTES:
                 raise I18NError("bad i18n attribute: " + repr(key), position)
             if not value and key in ("attributes", "data", "id"):
-                raise I18NError("missing value for i18n attribute: " +
-                                repr(key), position)
+                raise I18NError(
+                    "missing value for i18n attribute: " + repr(key), position
+                )
 
         todo = {}
         defineMacro = metaldict.get("define-macro")
         extendMacro = metaldict.get("extend-macro")
         useMacro = metaldict.get("use-macro")
         defineSlot = metaldict.get("define-slot")
         fillSlot = metaldict.get("fill-slot")
@@ -67,38 +75,38 @@
         omitTag = taldict.get("omit-tag")
         TALtag = taldict.get("tal tag")
         i18nattrs = i18ndict.get("attributes")
         # Preserve empty string if implicit msgids are used.  We'll generate
         # code with the msgid='' and calculate the right implicit msgid during
         # interpretation phase.
         msgid = i18ndict.get("translate")
-        varname = i18ndict.get('name')
-        i18ndata = i18ndict.get('data')
+        varname = i18ndict.get("name")
+        i18ndata = i18ndict.get("data")
 
         if varname and not self.i18nLevel:
             raise I18NError(
-                "i18n:name can only occur inside a translation unit",
-                position)
+                "i18n:name can only occur inside a translation unit", position
+            )
 
         if varname and NOT_ALLOWED_IN_NAME.search(varname):
             raise I18NError(
-                "i18n:name cannot contain non-word characters "
-                "(spaces, punctuation)", position)
+                "i18n:name cannot contain non-word characters " "(spaces, punctuation)",
+                position,
+            )
 
         if i18ndata and not msgid:
-            raise I18NError("i18n:data must be accompanied by i18n:translate",
-                            position)
+            raise I18NError("i18n:data must be accompanied by i18n:translate", position)
 
         if defineMacro or extendMacro or useMacro:
             useMacro = useMacro or extendMacro
 
         if content and msgid:
             raise I18NError(
-                "explicit message id and tal:content can't be used together",
-                position)
+                "explicit message id and tal:content can't be used together", position
+            )
 
         repeatWhitespace = None
         if repeat:
             # Hack to include preceding whitespace in the loop program
             repeatWhitespace = self.unEmitNewlineWhitespace()
         if position != (None, None):
             # TODO: at some point we should insist on a non-trivial position
@@ -131,28 +139,25 @@
                 todo["useMacro"] = useMacro
                 self.inMacroUse = 1
             if defineSlot:
                 self.pushProgram()
                 todo["defineSlot"] = defineSlot
 
         if defineSlot or i18ndict:
-
             domain = i18ndict.get("domain") or self.i18nContext.domain
             source = i18ndict.get("source") or self.i18nContext.source
             target = i18ndict.get("target") or self.i18nContext.target
-            if (domain != DEFAULT_DOMAIN
-                    or source is not None
-                    or target is not None):
-                self.i18nContext = TranslationContext(self.i18nContext,
-                                                      domain=domain,
-                                                      source=source,
-                                                      target=target)
-                self.emit("beginI18nContext",
-                          {"domain": domain, "source": source,
-                           "target": target})
+            if domain != DEFAULT_DOMAIN or source is not None or target is not None:
+                self.i18nContext = TranslationContext(
+                    self.i18nContext, domain=domain, source=source, target=target
+                )
+                self.emit(
+                    "beginI18nContext",
+                    {"domain": domain, "source": source, "target": target},
+                )
                 todo["i18ncontext"] = 1
         if taldict or i18ndict:
             dict = {}
             for item in attrlist:
                 key, value = item[:2]
                 dict[key] = value
             self.emit("beginScope", dict)
@@ -175,55 +180,54 @@
         if repeat:
             todo["repeat"] = repeat
             self.pushProgram()
             if repeatWhitespace:
                 self.emitText(repeatWhitespace)
         if content:
             if varname:
-                todo['i18nvar'] = varname
+                todo["i18nvar"] = varname
                 todo["content"] = content
                 self.pushProgram()
             else:
                 todo["content"] = content
         # i18n:name w/o tal:replace uses the content as the interpolation
         # dictionary values
         elif varname:
-            todo['i18nvar'] = varname
+            todo["i18nvar"] = varname
             self.pushProgram()
         if msgid is not None:
             self.i18nLevel += 1
-            todo['msgid'] = msgid
+            todo["msgid"] = msgid
         if i18ndata:
-            todo['i18ndata'] = i18ndata
+            todo["i18ndata"] = i18ndata
         optTag = omitTag is not None or TALtag
         if optTag:
             todo["optional tag"] = omitTag, TALtag
             self.pushProgram()
         if attrsubst or i18nattrs:
             if attrsubst:
                 try:
-                    repldict = taldefs.parseAttributeReplacements(
-                        attrsubst, self.xml)
+                    repldict = taldefs.parseAttributeReplacements(attrsubst, self.xml)
                 except TALError:
                     repldict = {}
             else:
                 repldict = {}
             if i18nattrs:
-                i18nattrs = _parseI18nAttributes(i18nattrs, self.position,
-                                                 self.xml)
+                i18nattrs = _parseI18nAttributes(i18nattrs, self.position, self.xml)
             else:
                 i18nattrs = {}
             # Convert repldict's name-->expr mapping to a
             # name-->(compiled_expr, translate) mapping
             for key, value in sorted(repldict.items()):
                 if i18nattrs.get(key, None):
                     raise I18NError(
                         "attribute [%s] cannot both be part of tal:attributes"
                         " and have a msgid in i18n:attributes" % key,
-                        position)
+                        position,
+                    )
                 ce = self.compileExpression(value)
                 repldict[key] = ce, key in i18nattrs, i18nattrs.get(key)
             for key in sorted(i18nattrs):
                 if key not in repldict:
                     repldict[key] = None, 1, i18nattrs.get(key)
         else:
             repldict = {}
@@ -247,25 +251,24 @@
             todo["position"] = position
         self.todoPush(todo)
         if isend:
             self.emitEndElement(name, isend, position=position)
 
     def emitRepeat(self, arg):
         try:
-            super(DudeGenerator, self).emitRepeat(arg)
+            super().emitRepeat(arg)
         except TALError:
             # Could be Chameleon syntax.
             # It might be okay to simply return, as we are not really
             # interested in compiling everything.  But we can try.
             # We look for tal:repeat="   (a,b,c) python:something"
             # in a way similar to zope.tal.
             m = re.match(r"(?s)\s*(\(.+\))\s+(.*)\Z", arg)
             if not m:
-                raise TALError("invalid repeat syntax: " + repr(arg),
-                               self.position)
+                raise TALError("invalid repeat syntax: " + repr(arg), self.position)
             name, expr = m.group(1, 2)
             cexpr = self.compileExpression(expr)
             program = self.popProgram()
             self.emit("loop", name, cexpr, program)
 
     def emitDefines(self, defines):
         # Originally we did not have this method, so the one from zope.tal was used.
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/gsextract.py` & `i18ndude-6.1.0/src/i18ndude/gsextract.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import sys
-
+from i18ndude.extract import find_files
 from lxml import etree
 
-from i18ndude.extract import find_files
+import sys
+
 
-I18N_NS = 'http://xml.zope.org/namespaces/i18n'
-I18N_DOMAIN = '{%s}domain' % I18N_NS
-I18N_TRANSLATE = '{%s}translate' % I18N_NS
-I18N_ATTRIBUTES = '{%s}attributes' % I18N_NS
+I18N_NS = "http://xml.zope.org/namespaces/i18n"
+I18N_DOMAIN = "{%s}domain" % I18N_NS
+I18N_TRANSLATE = "{%s}translate" % I18N_NS
+I18N_ATTRIBUTES = "{%s}attributes" % I18N_NS
 
 
-class GSParser(object):
-    """GenericSetup profile i18n parser.
-    """
+class GSParser:
+    """GenericSetup profile i18n parser."""
 
     def __init__(self):
         self.catalogs = {}
         self.filename = None
 
     def parse(self, filename):
         self.filename = filename
         try:
             tree = etree.parse(filename)
         except Exception as e:
-            print(u"There was an error in parsing %s: %s" % (filename, e))
+            print(f"There was an error in parsing {filename}: {e}")
             sys.exit(0)
         elem = tree.getroot()
         domain = elem.get(I18N_DOMAIN, None)
         self.parseNode(elem, domain)
         self.parseChildren(elem, domain)
 
     def parseChildren(self, elem, domain):
@@ -48,44 +47,41 @@
                 if text is not None:
                     text = text.strip()
                 if text:
                     msgid = msgstr = text
                     if translate:
                         msgid = translate
                     else:
-                        msgstr = u""
+                        msgstr = ""
                     if msgid:
-                        self.catalogs[domain].append(
-                            (msgid, msgstr, self.filename))
+                        self.catalogs[domain].append((msgid, msgstr, self.filename))
             if attributes is not None:
-                attributes = attributes.strip().split(';')
+                attributes = attributes.strip().split(";")
                 for attr in attributes:
                     parts = attr.split()
                     if len(parts) == 2:
                         attr, msgid = parts
                     else:
                         attr = parts[0]
-                        msgid = u""
+                        msgid = ""
                     text = elem.get(attr)
                     if text is not None:
                         text = text.strip()
                     if text:
                         if msgid:
                             msgstr = text
                         else:
                             msgid = text
-                            msgstr = u""
-                        self.catalogs[domain].append(
-                            (msgid, msgstr, self.filename))
+                            msgstr = ""
+                        self.catalogs[domain].append((msgid, msgstr, self.filename))
 
     def getCatalogs(self):
         return self.catalogs
 
 
 def gs_strings(dir, domain="none", exclude=()):
-    """Retrieve all messages from `dir` that are in the `domain`.
-    """
+    """Retrieve all messages from `dir` that are in the `domain`."""
     parser = GSParser()
-    for filename in find_files(dir, '*.xml', exclude=tuple(exclude)):
+    for filename in find_files(dir, "*.xml", exclude=tuple(exclude)):
         parser.parse(filename)
 
     return parser.getCatalogs()
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/interfaces.py` & `i18ndude-6.1.0/src/i18ndude/interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,55 +9,48 @@
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Abstract objects for the i18n extraction machinery
 """
-__docformat__ = 'restructuredtext'
+__docformat__ = "restructuredtext"
 
 # INFO: This is a modified copy of zope3's zope.app.locales.interfaces (r71023)
 
 from zope.interface import Interface
 
 
 class IPOTEntry(Interface):
-    """Represents a single message entry in a POT file
-    """
+    """Represents a single message entry in a POT file"""
 
     def addComment(comment):
-        """Add a comment to the entry
-        """
+        """Add a comment to the entry"""
 
     def addLocationComment(filename, line):
         """Add a comment regarding the location where this message id
         entry can be found
         """
 
     def write(file):
-        """Write the entry to the file
-        """
+        """Write the entry to the file"""
 
 
 class IPOTMaker(Interface):
-    """Writes POT entries to a POT file
-    """
+    """Writes POT entries to a POT file"""
 
     def add(strings, base_dir=None):
-        """Add `strings` to the internal catalog.
-        """
+        """Add `strings` to the internal catalog."""
 
     def write():
-        """Write strings to the POT file
-        """
+        """Write strings to the POT file"""
 
 
 class ITokenEater(Interface):
-    """Eats tokens from the python tokenizer
-    """
+    """Eats tokens from the python tokenizer"""
 
     def getCatalog():
         """Return the catalog of collected message ids as keys of a
         dictionary. The values are a tuple consisting the of the
         filename and the line number at which the message id was
         found.
         """
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/pygettext.py` & `i18ndude-6.1.0/src/i18ndude/pygettext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #! /usr/bin/env python
-# -*- coding: utf-8 -*-
 # Originally written by Barry Warsaw <barry@zope.com>
 #
 # Minimally patched to make it even more xgettext compatible
 # by Peter Funk <pf@artcom-gmbh.de>
 #
 # 2002-11-22 Jürgen Hermann <jh@web.de>
 # Added checks that _() only contains string literals, and
@@ -12,19 +11,24 @@
 # directory (including globbing chars, important for Win32).
 # Made docstring fit in 80 chars wide displays using pydoc.
 #
 
 # for selftesting
 try:
     import fintl
+
     _ = fintl.gettext
 except ImportError:
-    _ = lambda s: s
 
-__doc__ = _("""pygettext -- Python equivalent of xgettext(1)
+    def _(s):
+        return s
+
+
+__doc__ = _(
+    """pygettext -- Python equivalent of xgettext(1)
 
 Many systems (Solaris, Linux, Gnu) provide extensive tools that ease the
 internationalization of C programs. Most of these tools are independent of
 the programming language and can be used from within Python programs.
 Martin von Loewis' work[1] helps considerably in this regard.
 
 There's one problem though; xgettext is the program that scans source code
@@ -149,38 +153,42 @@
     -X filename
     --no-docstrings=filename
         Specify a file that contains a list of files (one per line) that
         should not have their docstrings extracted.  This is only useful in
         conjunction with the -D option above.
 
 If `inputfile' is -, standard input is read.
-""")
+"""
+)
 
-import os
+from functools import reduce
+
+import getopt
+import glob
 import imp
+import operator
+import os
 import sys
-import glob
 import time
-import getopt
 import token
 import tokenize
-import operator
-from functools import reduce
 
-__version__ = '1.5'
 
-default_keywords = ['_']
-DEFAULTKEYWORDS = ', '.join(default_keywords)
+__version__ = "1.5"
 
-EMPTYSTRING = ''
+default_keywords = ["_"]
+DEFAULTKEYWORDS = ", ".join(default_keywords)
+
+EMPTYSTRING = ""
 
 
 # The normal pot-file header. msgmerge and Emacs's po-mode work better if it's
 # there.
-pot_header = _('''\
+pot_header = _(
+    """\
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR ORGANIZATION
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\\n"
@@ -189,18 +197,19 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\\n"
 "Language-Team: LANGUAGE <LL@li.org>\\n"
 "MIME-Version: 1.0\\n"
 "Content-Type: text/plain; charset=CHARSET\\n"
 "Content-Transfer-Encoding: ENCODING\\n"
 "Generated-By: pygettext.py %(version)s\\n"
 
-''')
+"""
+)
 
 
-def usage(code, msg=''):
+def usage(code, msg=""):
     sys.stderr.write(__doc__ % globals())
     if msg:
         sys.stderr.write(msg)
     sys.exit(code)
 
 
 escapes = []
@@ -216,19 +225,19 @@
     else:
         mod = 256
     for i in range(256):
         if 32 <= (i % mod) <= 126:
             escapes.append(chr(i))
         else:
             escapes.append("\\%03o" % i)
-    escapes[ord('\\')] = '\\\\'
-    escapes[ord('\t')] = '\\t'
-    escapes[ord('\r')] = '\\r'
-    escapes[ord('\n')] = '\\n'
-    escapes[ord('\"')] = '\\"'
+    escapes[ord("\\")] = "\\\\"
+    escapes[ord("\t")] = "\\t"
+    escapes[ord("\r")] = "\\r"
+    escapes[ord("\n")] = "\\n"
+    escapes[ord('"')] = '\\"'
 
 
 def escape(s):
     global escapes
     s = list(s)
     for i in range(len(s)):
         try:
@@ -236,69 +245,73 @@
         except IndexError:
             s[i] = s[i]
     return EMPTYSTRING.join(s)
 
 
 def safe_eval(s):
     # unwrap quotes, safely
-    return eval(s, {'__builtins__': {}}, {})
+    return eval(s, {"__builtins__": {}}, {})
 
 
 def normalize(s):
     # This converts the various Python string types into a format that is
     # appropriate for .po files, namely much closer to C style.
-    lines = s.split('\n')
+    lines = s.split("\n")
     if len(lines) == 1:
         s = '"' + escape(s) + '"'
     else:
         if not lines[-1]:
             del lines[-1]
-            lines[-1] = lines[-1] + '\n'
+            lines[-1] = lines[-1] + "\n"
         for i in range(len(lines)):
             lines[i] = escape(lines[i])
         lineterm = '\\n"\n"'
         s = '""\n"' + lineterm.join(lines) + '"'
     if not isinstance(s, str):
-        s = s.encode('utf-8')
+        s = s.encode("utf-8")
     return s
 
 
 def containsAny(str, set):
     """Check whether 'str' contains ANY of the chars in 'set'"""
     return 1 in [c in str for c in set]
 
 
 def _visit_pyfiles(list, dirname, names):
     """Helper for getFilesForName()."""
     # get extension for python source files
-    if '_py_ext' not in globals():
+    if "_py_ext" not in globals():
         global _py_ext
-        _py_ext = [triple[0] for triple in imp.get_suffixes()
-                   if triple[2] == imp.PY_SOURCE][0]
+        _py_ext = [
+            triple[0] for triple in imp.get_suffixes() if triple[2] == imp.PY_SOURCE
+        ][0]
 
     # don't recurse into CVS directories
-    if 'CVS' in names:
-        names.remove('CVS')
+    if "CVS" in names:
+        names.remove("CVS")
 
     # add all *.py files to list
     list.extend(
-        [os.path.join(dirname, file) for file in names
-         if os.path.splitext(file)[1] == _py_ext]
+        [
+            os.path.join(dirname, file)
+            for file in names
+            if os.path.splitext(file)[1] == _py_ext
+        ]
     )
 
 
 def _get_modpkg_path(dotted_name, pathlist=None):
     """Get the filesystem path for a module or a package.
 
     Return the file system path to a file for a module, and to a directory for
     a package. Return None if the name is not found, or is a builtin or
     extension module.
     """
     # split off top-most name
-    parts = dotted_name.split('.', 1)
+    parts = dotted_name.split(".", 1)
 
     if len(parts) > 1:
         # we have a dotted path, import top-level package
         try:
             file, pathname, description = imp.find_module(parts[0], pathlist)
             if file:
                 file.close()
@@ -310,16 +323,15 @@
             # recursively handle the remaining name parts
             pathname = _get_modpkg_path(parts[1], [pathname])
         else:
             pathname = None
     else:
         # plain name
         try:
-            file, pathname, description = imp.find_module(
-                dotted_name, pathlist)
+            file, pathname, description = imp.find_module(dotted_name, pathlist)
             if file:
                 file.close()
             if description[2] not in [imp.PY_SOURCE, imp.PKG_DIRECTORY]:
                 pathname = None
         except ImportError:
             pathname = None
 
@@ -353,15 +365,14 @@
         # a single file
         return [name]
 
     return []
 
 
 class TokenEater:
-
     def __init__(self, options):
         self.__options = options
         self.__messages = {}
         self.__state = self.__waiting
         self.__data = []
         self.__lineno = -1
         self.__freshmodule = 1
@@ -383,64 +394,65 @@
                 if ttype == tokenize.STRING:
                     self.__addentry(safe_eval(tstring), lineno, isdocstring=1)
                     self.__freshmodule = 0
                 elif ttype not in (tokenize.COMMENT, tokenize.NL):
                     self.__freshmodule = 0
                 return
             # class docstring?
-            if ttype == tokenize.NAME and tstring in ('class', 'def'):
+            if ttype == tokenize.NAME and tstring in ("class", "def"):
                 self.__state = self.__suiteseen
                 return
         if ttype == tokenize.NAME and tstring in opts.keywords:
             self.__state = self.__keywordseen
 
     def __suiteseen(self, ttype, tstring, lineno):
         # ignore anything until we see the colon
-        if ttype == tokenize.OP and tstring == ':':
+        if ttype == tokenize.OP and tstring == ":":
             self.__state = self.__suitedocstring
 
     def __suitedocstring(self, ttype, tstring, lineno):
         # ignore any intervening noise
         if ttype == tokenize.STRING:
             self.__addentry(safe_eval(tstring), lineno, isdocstring=1)
             self.__state = self.__waiting
-        elif ttype not in (tokenize.NEWLINE, tokenize.INDENT,
-                           tokenize.COMMENT):
+        elif ttype not in (tokenize.NEWLINE, tokenize.INDENT, tokenize.COMMENT):
             # there was no class docstring
             self.__state = self.__waiting
 
     def __keywordseen(self, ttype, tstring, lineno):
-        if ttype == tokenize.OP and tstring == '(':
+        if ttype == tokenize.OP and tstring == "(":
             self.__data = []
             self.__lineno = lineno
             self.__state = self.__openseen
         else:
             self.__state = self.__waiting
 
     def __openseen(self, ttype, tstring, lineno):
-        if ttype == tokenize.OP and tstring == ')':
+        if ttype == tokenize.OP and tstring == ")":
             # We've seen the last of the translatable strings.  Record the
             # line number of the first line of the strings and update the list
             # of messages seen.  Reset state for the next batch.  If there
             # were no strings inside _(), then just ignore this entry.
             if self.__data:
                 self.__addentry(EMPTYSTRING.join(self.__data))
             self.__state = self.__waiting
         elif ttype == tokenize.STRING:
             self.__data.append(safe_eval(tstring))
-        elif ttype not in [tokenize.COMMENT, token.INDENT, token.DEDENT,
-                           token.NEWLINE, tokenize.NL]:
+        elif ttype not in [
+            tokenize.COMMENT,
+            token.INDENT,
+            token.DEDENT,
+            token.NEWLINE,
+            tokenize.NL,
+        ]:
             # warn if we see anything else than STRING or whitespace
-            sys.stderr.write(_(
-                '*** %(file)s:%(lineno)s: Seen unexpected token "%(token)s"'
-            ) % {
-                'token': tstring,
-                'file': self.__curfile,
-                'lineno': self.__lineno
-            })
+            sys.stderr.write(
+                _('*** %(file)s:%(lineno)s: Seen unexpected token "%(token)s"')
+                % {"token": tstring, "file": self.__curfile, "lineno": self.__lineno}
+            )
             self.__state = self.__waiting
 
     def __addentry(self, msg, lineno=None, isdocstring=0):
         if lineno is None:
             lineno = self.__lineno
         if msg not in self.__options.toexclude:
             entry = (self.__curfile, lineno)
@@ -448,19 +460,18 @@
 
     def set_filename(self, filename):
         self.__curfile = filename
         self.__freshmodule = 1
 
     def write(self, fp):
         options = self.__options
-        timestamp = time.strftime('%Y-%m-%d %H:%M+%Z')
+        timestamp = time.strftime("%Y-%m-%d %H:%M+%Z")
         # The time stamp in the header doesn't have the same format as that
         # generated by xgettext...
-        fp.write(
-            pot_header % {'time': timestamp, 'version': __version__})
+        fp.write(pot_header % {"time": timestamp, "version": __version__})
         # Sort the entries.  First sort each particular entry's keys, then
         # sort all the entries by their first item.
         reverse = {}
         for k, v in self.__messages.items():
             keys = sorted(v.keys())
             reverse.setdefault(tuple(keys), []).append((k, v))
         rkeys = sorted(reverse.keys())
@@ -478,118 +489,131 @@
                 # file name and then by line number.
                 v = sorted(v.keys())
                 if not options.writelocations:
                     pass
                 # location comments are different b/w Solaris and GNU:
                 elif options.locationstyle == options.SOLARIS:
                     for filename, lineno in v:
-                        d = {'filename': filename, 'lineno': lineno}
-                        fp.write(_(
-                            '# File: %(filename)s, line: %(lineno)d') % d)
+                        d = {"filename": filename, "lineno": lineno}
+                        fp.write(_("# File: %(filename)s, line: %(lineno)d") % d)
                 elif options.locationstyle == options.GNU:
                     # fit as many locations on one line, as long as the
                     # resulting line length doesn't exceeds 'options.width'
-                    locline = '#:'
+                    locline = "#:"
                     for filename, lineno in v:
-                        d = {'filename': filename, 'lineno': lineno}
-                        s = _(' %(filename)s:%(lineno)d') % d
+                        d = {"filename": filename, "lineno": lineno}
+                        s = _(" %(filename)s:%(lineno)d") % d
                         if len(locline) + len(s) <= options.width:
                             locline = locline + s
                         else:
                             fp.write(locline)
                             locline = "#:" + s
                     if len(locline) > 2:
                         fp.write(locline)
                 if isdocstring:
-                    fp.write('#, docstring')
-                fp.write('msgid', normalize(k))
+                    fp.write("#, docstring")
+                fp.write("msgid", normalize(k))
                 fp.write('msgstr ""\n')
 
 
 def main():
     global default_keywords
     try:
         opts, args = getopt.getopt(
             sys.argv[1:],
-            'ad:DEhk:Kno:p:S:Vvw:x:X:',
-            ['extract-all', 'default-domain=', 'escape', 'help',
-             'keyword=', 'no-default-keywords',
-             'add-location', 'no-location', 'output=', 'output-dir=',
-             'style=', 'verbose', 'version', 'width=', 'exclude-file=',
-             'docstrings', 'no-docstrings',
-             ])
+            "ad:DEhk:Kno:p:S:Vvw:x:X:",
+            [
+                "extract-all",
+                "default-domain=",
+                "escape",
+                "help",
+                "keyword=",
+                "no-default-keywords",
+                "add-location",
+                "no-location",
+                "output=",
+                "output-dir=",
+                "style=",
+                "verbose",
+                "version",
+                "width=",
+                "exclude-file=",
+                "docstrings",
+                "no-docstrings",
+            ],
+        )
     except getopt.error as msg:
         usage(1, msg)
 
     # for holding option values
     class Options:
         # constants
         GNU = 1
         SOLARIS = 2
         # defaults
         extractall = 0  # FIXME: currently this option has no effect at all.
         escape = 0
         keywords = []
-        outpath = ''
-        outfile = 'messages.pot'
+        outpath = ""
+        outfile = "messages.pot"
         writelocations = 1
         locationstyle = GNU
         verbose = 0
         width = 78
-        excludefilename = ''
+        excludefilename = ""
         docstrings = 0
         nodocstrings = {}
 
     options = Options()
     locations = {
-        'gnu': options.GNU,
-        'solaris': options.SOLARIS,
+        "gnu": options.GNU,
+        "solaris": options.SOLARIS,
     }
 
     # parse options
     for opt, arg in opts:
-        if opt in ('-h', '--help'):
+        if opt in ("-h", "--help"):
             usage(0)
-        elif opt in ('-a', '--extract-all'):
+        elif opt in ("-a", "--extract-all"):
             options.extractall = 1
-        elif opt in ('-d', '--default-domain'):
-            options.outfile = arg + '.pot'
-        elif opt in ('-E', '--escape'):
+        elif opt in ("-d", "--default-domain"):
+            options.outfile = arg + ".pot"
+        elif opt in ("-E", "--escape"):
             options.escape = 1
-        elif opt in ('-D', '--docstrings'):
+        elif opt in ("-D", "--docstrings"):
             options.docstrings = 1
-        elif opt in ('-k', '--keyword'):
+        elif opt in ("-k", "--keyword"):
             options.keywords.append(arg)
-        elif opt in ('-K', '--no-default-keywords'):
+        elif opt in ("-K", "--no-default-keywords"):
             default_keywords = []
-        elif opt in ('-n', '--add-location'):
+        elif opt in ("-n", "--add-location"):
             options.writelocations = 1
-        elif opt in ('--no-location',):
+        elif opt in ("--no-location",):
             options.writelocations = 0
-        elif opt in ('-S', '--style'):
+        elif opt in ("-S", "--style"):
             options.locationstyle = locations.get(arg.lower())
             if options.locationstyle is None:
-                usage(1, _('Invalid value for --style: %s') % arg)
-        elif opt in ('-o', '--output'):
+                usage(1, _("Invalid value for --style: %s") % arg)
+        elif opt in ("-o", "--output"):
             options.outfile = arg
-        elif opt in ('-p', '--output-dir'):
+        elif opt in ("-p", "--output-dir"):
             options.outpath = arg
-        elif opt in ('-v', '--verbose'):
+        elif opt in ("-v", "--verbose"):
             options.verbose = 1
-        elif opt in ('-V', '--version'):
-            print(_('pygettext.py (xgettext for Python) %s') % __version__)
+        elif opt in ("-V", "--version"):
+            print(_("pygettext.py (xgettext for Python) %s") % __version__)
             sys.exit(0)
-        elif opt in ('-w', '--width'):
+        elif opt in ("-w", "--width"):
             try:
                 options.width = int(arg)
             except ValueError:
-                usage(1, _('--width argument must be an integer: %s') % arg)
-        elif opt in ('-x', '--exclude-file'):
+                usage(1, _("--width argument must be an integer: %s") % arg)
+        elif opt in ("-x", "--exclude-file"):
             options.excludefilename = arg
-        elif opt in ('-X', '--no-docstrings'):
+        elif opt in ("-X", "--no-docstrings"):
             fp = open(arg)
             try:
                 while True:
                     line = fp.readline()
                     if not line:
                         break
                     options.nodocstrings[line[:-1]] = 1
@@ -604,72 +628,74 @@
 
     # initialize list of strings to exclude
     if options.excludefilename:
         try:
             fp = open(options.excludefilename)
             options.toexclude = fp.readlines()
             fp.close()
-        except IOError:
-            sys.stderr.write(_(
-                "Can't read --exclude-file: %s") % options.excludefilename)
+        except OSError:
+            sys.stderr.write(
+                _("Can't read --exclude-file: %s") % options.excludefilename
+            )
             sys.exit(1)
     else:
         options.toexclude = []
 
     # resolve args to module lists
     expanded = []
     for arg in args:
-        if arg == '-':
+        if arg == "-":
             expanded.append(arg)
         else:
             expanded.extend(getFilesForName(arg))
     args = expanded
 
     # slurp through all the files
     eater = TokenEater(options)
     for filename in args:
-        if filename == '-':
+        if filename == "-":
             if options.verbose:
-                print(_('Reading standard input'))
+                print(_("Reading standard input"))
             fp = sys.stdin
             closep = 0
         else:
             if options.verbose:
-                print(_('Working on %s') % filename)
+                print(_("Working on %s") % filename)
             fp = open(filename)
             closep = 1
         try:
             eater.set_filename(filename)
             try:
                 g = tokenize.generate_tokens(fp.readline)
                 for ttype, tstring, stup, etup, line in g:
                     eater(ttype, tstring, stup, etup, line)
             except tokenize.TokenError as e:
-                sys.stderr.write('%s: %s, line %d, column %d' % (
-                    e[0], filename, e[1][0], e[1][1]))
+                sys.stderr.write(
+                    "%s: %s, line %d, column %d" % (e[0], filename, e[1][0], e[1][1])
+                )
         finally:
             if closep:
                 fp.close()
 
     # write the output
-    if options.outfile == '-':
+    if options.outfile == "-":
         fp = sys.stdout
         closep = 0
     else:
         if options.outpath:
             options.outfile = os.path.join(options.outpath, options.outfile)
-        fp = open(options.outfile, 'w')
+        fp = open(options.outfile, "w")
         closep = 1
     try:
         eater.write(fp)
     finally:
         if closep:
             fp.close()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
     # some more test strings
-    _(u'a unicode string')
+    _("a string")
     # this one creates a warning
-    _('*** Seen unexpected token "%(token)s"') % {'token': 'test'}
-    _('more' 'than' 'one' 'string')
+    _('*** Seen unexpected token "%(token)s"') % {"token": "test"}
+    _("more" "than" "one" "string")
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/script.py` & `i18ndude-6.1.0/src/i18ndude/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,83 +17,86 @@
 
 #    You should have received a copy of the GNU General Public License
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307, USA
 
 # -----------------------------------------------------------------------------
 
+from i18ndude import catalog
+from i18ndude import common
+from i18ndude import untranslated
+from i18ndude import utils
+from i18ndude import visualisation
+
 import argparse
 import os
 import sys
 import textwrap
 import xml.sax
 
-from i18ndude import common, untranslated, catalog, visualisation, utils
-
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
 
 # Define a parent parser for the wrapping arguments.  This is shared
 # by a few commands.  Note: if you use this parser, you need to call
 # the parse_wrapping_arguments function somewhere in the handling of
 # your command.
 wrapper_parser = argparse.ArgumentParser(add_help=False)
 wrapping_group = wrapper_parser.add_mutually_exclusive_group()
+wrapping_group.add_argument("--wrap", action="store_true", help="Wrap long lines.")
 wrapping_group.add_argument(
-    '--wrap', action='store_true', help="Wrap long lines.")
-wrapping_group.add_argument(
-    '--no-wrap', action='store_true',
-    help="Do not wrap long lines. This is the default.")
+    "--no-wrap",
+    action="store_true",
+    help="Do not wrap long lines. This is the default.",
+)
 wrapper_parser.add_argument(
-    '--width', metavar='NUMBER', type=int,
-    help="Set output page width. Default is %d." % utils.MAX_WIDTH)
+    "--width",
+    metavar="NUMBER",
+    type=int,
+    help="Set output page width. Default is %d." % utils.MAX_WIDTH,
+)
 
 
 def parse_wrapping_arguments(arguments):
     """Parse the arguments that handle wrapping.
 
     Based on the arguments we can store the result in utils.MAX_WIDTH
     and utils.WRAP.  If the arguments are not set, we do nothing: the
     default values of those variables are used.
     """
-    if 'width' in arguments and arguments.width:
+    if "width" in arguments and arguments.width:
         utils.MAX_WIDTH = arguments.width
-    if 'wrap' in arguments and arguments.wrap:
+    if "wrap" in arguments and arguments.wrap:
         utils.WRAP = True
-    elif 'no_wrap' in arguments and arguments.no_wrap:
+    elif "no_wrap" in arguments and arguments.no_wrap:
         utils.WRAP = False
 
 
-def short_usage(code, msg=''):
+def short_usage(code, msg=""):
     if msg:
         sys.stderr.write(msg)
-    sys.stderr.write(u"Type i18ndude -h<Enter> to see the help.")
+    sys.stderr.write("Type i18ndude -h<Enter> to see the help.")
     sys.exit(code)
 
 
 def filter_isfile(files):
     result = []
     for name in files:  # parse file by file
         name = name.strip()
         if os.path.isdir(name):  # descend recursively
             subdirs = []
             for subpath in os.listdir(name):
-                if subpath.startswith('.'):
+                if subpath.startswith("."):
                     # ignore hidden file
                     continue
                 path = os.path.join(name, subpath)
-                if (os.path.isdir(path) or
-                        os.path.splitext(subpath)[1].endswith('pt')):
+                if os.path.isdir(path) or os.path.splitext(subpath)[1].endswith("pt"):
                     subdirs.append(path)
             result += filter_isfile(subdirs)
 
         elif not os.path.isfile(name):
-            sys.stderr.write(
-                'Warning: %s is not a file or is ignored.' % name)
+            sys.stderr.write("Warning: %s is not a file or is ignored." % name)
 
         else:
             result.append(name)
     return result
 
 
 def find_untranslated_parser(subparsers):
@@ -116,30 +119,40 @@
     setting the "i18n:ignore" attribute on the tag. Same for
     attributes with "i18n:ignore-attributes". Note that i18ndude may
     be happy with this, but your template engine may fail when trying
     to render a template containing those ignore hints.  You need
     Chameleon 2.23 or higher, or the to be released zope.tal 4.1.2.
     """
     parser = subparsers.add_parser(
-        'find-untranslated',
+        "find-untranslated",
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
+    )
+    parser.add_argument(
+        "-s",
+        "--silent",
+        action="store_true",
+        help=(
+            "The report will only contain a summary of errors and warnings for "
+            "each file (or no output if there are no errors or warnings)."
+        ),
+    )
+    parser.add_argument(
+        "-n",
+        "--nosummary",
+        action="store_true",
+        help=("The report will contain only the errors for each file."),
     )
-    parser.add_argument('-s', '--silent', action='store_true', help=(
-        "The report will only contain a summary of errors and warnings for "
-        "each file (or no output if there are no errors or warnings)."))
-    parser.add_argument('-n', '--nosummary', action='store_true', help=(
-        "The report will contain only the errors for each file."))
-    parser.add_argument('files', nargs='*', help="list of ZPT filenames")
+    parser.add_argument("files", nargs="*", help="list of ZPT filenames")
     parser.set_defaults(func=find_untranslated)
     return parser
 
 
 def find_untranslated(arguments):
-    parser = xml.sax.make_parser(['expat'])
+    parser = xml.sax.make_parser(["expat"])
     # disable external validation to make it work without network access
     parser.setFeature(xml.sax.handler.feature_external_ges, False)
     parser.setFeature(xml.sax.handler.feature_external_pes, False)
     handler = untranslated.VerboseHandler(parser)  # default
 
     if arguments.silent:
         handler = untranslated.SilentHandler(parser)
@@ -150,16 +163,15 @@
     errors = 0
     for filename in filter_isfile(arguments.files):  # parse file by file
         with open(filename) as myfile:
             try:
                 if not myfile.read().strip():
                     continue
             except UnicodeDecodeError:
-                print('ERROR: UnicodeDecodeError while reading {}'.format(
-                    filename))
+                print("ERROR: UnicodeDecodeError while reading {}".format(filename))
                 continue
         # Reinitialize the handler, resetting errors.
         handler.set_filename(filename)
         file_errors = []
         success = False
         for content in common.present_file_contents(filename):
             if content is None:
@@ -169,15 +181,15 @@
                 file_errors.extend(content)
                 continue
             # Reinitialize the handler, resetting errors.
             handler.set_filename(filename)
             try:
                 parser.parse(content)
             except KeyboardInterrupt:
-                sys.stderr.write('Interrupted by user.')
+                sys.stderr.write("Interrupted by user.")
                 sys.exit(1)
             except xml.sax.SAXException as error:
                 file_errors.append(error)
                 continue
             except Exception as error:
                 file_errors.append(error)
                 continue
@@ -197,18 +209,18 @@
             # So some untranslated strings were found.
             errors += 1
         if success:
             # next file
             continue
         if file_errors:
             errors += 1
-            report = 'ERRORs found trying to parse document in various ways:\n'
+            report = "ERRORs found trying to parse document in various ways:\n"
             for error in file_errors:
-                report += '%s\n' % error
-            handler.log(report, 'FATAL')
+                report += "%s\n" % error
+            handler.log(report, "FATAL")
     return errors
 
 
 def rebuild_pot_parser(subparsers):
     """Argument parser for rebuild-pot command.
 
     rebuild-pot --pot <filename> --create <domain>
@@ -258,35 +270,42 @@
 
     You can suppress the line numbers by using the --no-line-numbers option.
     The default might change in the future.  If you love line numbers, you can
     add --line-numbers to be sure you keep them when you get a newer version
     of i18ndude.  If you specify both options, the last one wins.
     """
     parser = subparsers.add_parser(
-        'rebuild-pot',
+        "rebuild-pot",
         parents=[wrapper_parser],
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
     )
-    parser.add_argument('-p', '--pot', metavar='filename',
-                        dest='pot_fn', required=True)
-    parser.add_argument('-c', '--create', metavar='domain',
-                        dest='create_domain', required=False)
-    parser.add_argument('-m', '--merge', metavar='filename', dest='merge_fn')
-    parser.add_argument('--merge2', metavar='filename', dest='merge2_fn')
+    parser.add_argument("-p", "--pot", metavar="filename", dest="pot_fn", required=True)
     parser.add_argument(
-        '--exclude', metavar='"<ignore1> <ignore2> ..."', default='')
+        "-c", "--create", metavar="domain", dest="create_domain", required=False
+    )
+    parser.add_argument("-m", "--merge", metavar="filename", dest="merge_fn")
+    parser.add_argument("--merge2", metavar="filename", dest="merge2_fn")
+    parser.add_argument("--exclude", metavar='"<ignore1> <ignore2> ..."', default="")
     # You can switch line numbers on or off.  Both options store their value
     # in include_line_numbers.  The order is important:
     # the last one here wins, both in this file and on the command line.
-    parser.add_argument('--no-line-numbers', action="store_false",
-                        dest='include_line_numbers', required=False)
-    parser.add_argument('--line-numbers', action="store_true",
-                        dest='include_line_numbers', required=False)
-    parser.add_argument('path', nargs='*')
+    parser.add_argument(
+        "--no-line-numbers",
+        action="store_false",
+        dest="include_line_numbers",
+        required=False,
+    )
+    parser.add_argument(
+        "--line-numbers",
+        action="store_true",
+        dest="include_line_numbers",
+        required=False,
+    )
+    parser.add_argument("path", nargs="*")
     parser.set_defaults(func=rebuild_pot)
     return parser
 
 
 def rebuild_pot(arguments):
     merge_ctl = None
 
@@ -316,16 +335,16 @@
             "exclude": exclude,
             "include_line_numbers": include_line_numbers,
         }
         ptreader = catalog.PTReader(*reader_args, **reader_kwargs)
         pyreader = catalog.PYReader(*reader_args, **reader_kwargs)
         gsreader = catalog.GSReader(*reader_args, **reader_kwargs)
         zcmlreader = catalog.ZCMLReader(*reader_args, **reader_kwargs)
-    except IOError as e:
-        short_usage(0, 'I/O Error: %s' % e)
+    except OSError as e:
+        short_usage(0, "I/O Error: %s" % e)
 
     # Read the data.
     ptreader.read()
     pyreader.read()
     gsreader.read()
     zcmlreader.read()
 
@@ -333,24 +352,22 @@
 
     ptctl = pyctl = gsctl = zcmlctl = {}
     if domain in ptreader.catalogs:
         ptctl = ptreader.catalogs[domain]
         for key in orig_ctl.keys():
             if key in ptctl:
                 # preserve comments
-                ptctl[key].comments = ptctl[
-                    key].comments + orig_ctl.getComments(key)
+                ptctl[key].comments = ptctl[key].comments + orig_ctl.getComments(key)
 
     if domain in pyreader.catalogs:
         pyctl = pyreader.catalogs[domain]
         for key in orig_ctl.keys():
             if key in pyctl:
                 # preserve comments
-                pyctl[key].comments = pyctl[
-                    key].comments + orig_ctl.getComments(key)
+                pyctl[key].comments = pyctl[key].comments + orig_ctl.getComments(key)
 
     if domain in gsreader.catalogs:
         gsctl = gsreader.catalogs[domain]
         # XXX Preserve comments?
 
     if domain in zcmlreader.catalogs:
         zcmlctl = zcmlreader.catalogs[domain]
@@ -377,16 +394,16 @@
         # use headers from orig-catalog
         ctl.commentary_header = orig_ctl.commentary_header
         ctl.mime_header = orig_ctl.mime_header
 
     if merge2_fn:
         ctl.add_missing(merge2_ctl, mergewarn=True)
 
-    ctl.mime_header['POT-Creation-Date'] = catalog.now()
-    file = open(pot_fn, 'w')
+    ctl.mime_header["POT-Creation-Date"] = catalog.now()
+    file = open(pot_fn, "w")
     writer = catalog.POWriter(file, ctl)
     writer.write(msgstrToComment=True)
 
 
 def merge_parser(subparsers):
     """Argument parser for merge command.
 
@@ -399,55 +416,55 @@
     these msgids into the target-pot file. If a msgid already
     exists, I'll warn you and ignore that msgid.
 
     If you provide a --merge2 <filename> I'll first merge this one
     in addition to the first one.
     """
     parser = subparsers.add_parser(
-        'merge',
+        "merge",
         parents=[wrapper_parser],
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
     )
-    parser.add_argument('-p', '--pot', metavar='filename',
-                        dest='pot_fn', required=True)
-    parser.add_argument('-m', '--merge', metavar='filename', dest='merge_fn',
-                        required=True)
-    parser.add_argument('--merge2', metavar='filename', dest='merge2_fn')
+    parser.add_argument("-p", "--pot", metavar="filename", dest="pot_fn", required=True)
+    parser.add_argument(
+        "-m", "--merge", metavar="filename", dest="merge_fn", required=True
+    )
+    parser.add_argument("--merge2", metavar="filename", dest="merge2_fn")
     parser.set_defaults(func=merge)
     return parser
 
 
 def merge(arguments):
     # Determine final argument values.
     pot_fn = arguments.pot_fn
     merge_fn = arguments.merge_fn
     merge2_fn = arguments.merge2_fn
     if merge2_fn == merge_fn:
         merge2_fn = False
 
     if not pot_fn:
-        short_usage(1, u"No pot file specified as target with --pot.")
+        short_usage(1, "No pot file specified as target with --pot.")
     if not merge_fn:
-        short_usage(1, u"No potfile specified as source with --merge.")
+        short_usage(1, "No potfile specified as source with --merge.")
 
     try:
         orig_ctl = catalog.MessageCatalog(filename=pot_fn)
         merge_ctl = catalog.MessageCatalog(filename=merge_fn)
         if merge2_fn:
             merge2_ctl = catalog.MessageCatalog(filename=merge2_fn)
-    except IOError as e:
-        short_usage(0, 'I/O Error: %s' % e)
+    except OSError as e:
+        short_usage(0, "I/O Error: %s" % e)
 
     # merge
-    orig_ctl.add_missing(merge_ctl, '', 1)
+    orig_ctl.add_missing(merge_ctl, "", 1)
     if merge2_fn:
-        orig_ctl.add_missing(merge2_ctl, '', 1)
-    orig_ctl.mime_header['POT-Creation-Date'] = catalog.now()
-    file = open(pot_fn, 'w')
+        orig_ctl.add_missing(merge2_ctl, "", 1)
+    orig_ctl.mime_header["POT-Creation-Date"] = catalog.now()
+    file = open(pot_fn, "w")
     writer = catalog.POWriter(file, orig_ctl)
     writer.write(msgstrToComment=True)
 
 
 def sync_parser(subparsers):
     """Argument parser for sync command.
 
@@ -457,80 +474,83 @@
     description = """
     Given a pot-file with the --pot option and a list of po-files I'll
     remove from the po files those message translations of which the
     msgids are not in the pot-file and add messages that the pot-file has
     but the po-file doesn't.
     """
     parser = subparsers.add_parser(
-        'sync',
+        "sync",
         parents=[wrapper_parser],
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
+    )
+    parser.add_argument(
+        "-p", "--pot", metavar="potfilename", dest="pot_fn", required=True
     )
-    parser.add_argument('-p', '--pot', metavar='potfilename',
-                        dest='pot_fn', required=True)
-    parser.add_argument('files', nargs='+', metavar='pofilename')
+    parser.add_argument("files", nargs="+", metavar="pofilename")
     parser.set_defaults(func=sync)
     return parser
 
 
 def sync(arguments):
     pot_fn = arguments.pot_fn
     if not pot_fn:
-        short_usage(1, u"No pot file specified as target with --pot.")
+        short_usage(1, "No pot file specified as target with --pot.")
 
     files = filter_isfile(arguments.files)
 
     try:
         pot_ctl = catalog.MessageCatalog(filename=pot_fn)
         po_ctls = [catalog.MessageCatalog(filename=fn) for fn in files]
-    except IOError as e:
-        short_usage(1, 'I/O Error: %s' % e)
+    except OSError as e:
+        short_usage(1, "I/O Error: %s" % e)
 
     for po in po_ctls:
         added_msgids, removed_msgids = po.sync(pot_ctl)
 
-        file = open(po.filename, 'w')
+        file = open(po.filename, "w")
         writer = catalog.POWriter(file, po)
         writer.write(msgstrToComment=False, sync=True)
 
-        print('%s: %s added, %s removed' % (po.filename,
-                                            len(added_msgids),
-                                            len(removed_msgids)))
+        print(
+            "{}: {} added, {} removed".format(
+                po.filename, len(added_msgids), len(removed_msgids)
+            )
+        )
         file.close()
 
 
 def two_file_parser(subparsers, cmd, description):
     """Argument parser for command that takes two files.
 
     filter, admix and trmerge all accept two files as arguments.
     """
 
     parser = subparsers.add_parser(
         cmd,
         parents=[wrapper_parser],
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
     )
-    parser.add_argument('file1')
-    parser.add_argument('file2')
+    parser.add_argument("file1")
+    parser.add_argument("file2")
     return parser
 
 
 def filter_parser(subparsers):
     """Argument parser for filter command.
 
     filter <file1> <file2>
     """
 
     description = """
     Given two pot-files I will write a copy of file1 to stdout with all
     messages removed that are also in file2, i.e. where msgids match.
     """
-    parser = two_file_parser(subparsers, 'filter', description)
+    parser = two_file_parser(subparsers, "filter", description)
     parser.set_defaults(func=filter)
     return parser
 
 
 def filter(arguments):
     f1_ctl = catalog.MessageCatalog(filename=arguments.file1)
     f2_ctl = catalog.MessageCatalog(filename=arguments.file2)
@@ -557,15 +577,15 @@
 
     description = """
     Given two po-files I will look for translated entries in file2 that
     are untranslated in file1. I add these translations (msgstrs) to
     file1. Note that this will not affect the number of entries in file1.
     The result will be on stdout.
     """
-    parser = two_file_parser(subparsers, 'admix', description)
+    parser = two_file_parser(subparsers, "admix", description)
     parser.set_defaults(func=admix)
     return parser
 
 
 def admix(arguments):
     base_ctl = catalog.MessageCatalog(filename=arguments.file1)
     mixin_ctl = catalog.MessageCatalog(filename=arguments.file2)
@@ -598,20 +618,29 @@
     Fuzzy translations in file2 are ignored.
 
     The result will be on stdout.  If you want to update the first
     file in place, use a temporary file, something like this:
 
       i18ndude trmerge file1.po file2.po > tmp_merge && mv tmp_merge file1.po
     """
-    parser = two_file_parser(subparsers, 'trmerge', description)
-    parser.add_argument('-i', '--ignore-extra', action='store_true', help=(
-        "Ignore extra messages: do not add msgids that are not in the "
-        "original po-file. Only update translations for existing msgids."))
-    parser.add_argument('--no-override', action='store_true', help=(
-        "Do not override translations, only add missing translations."))
+    parser = two_file_parser(subparsers, "trmerge", description)
+    parser.add_argument(
+        "-i",
+        "--ignore-extra",
+        action="store_true",
+        help=(
+            "Ignore extra messages: do not add msgids that are not in the "
+            "original po-file. Only update translations for existing msgids."
+        ),
+    )
+    parser.add_argument(
+        "--no-override",
+        action="store_true",
+        help=("Do not override translations, only add missing translations."),
+    )
     parser.set_defaults(func=trmerge)
     return parser
 
 
 def trmerge(arguments):
     base_ctl = catalog.MessageCatalog(filename=arguments.file1)
     mixin_ctl = catalog.MessageCatalog(filename=arguments.file2)
@@ -623,31 +652,33 @@
             # has chosen to ignore it.
             continue
         mixin_entry = mixin_ctl[msgid]
         mixin_msgstr = mixin_entry.msgstr
         if not mixin_msgstr:
             # The mixin translation is empty.
             continue
-        if ', fuzzy' in mixin_entry.comments:
+        if ", fuzzy" in mixin_entry.comments:
             # The mixin translation is fuzzy.
             continue
-        if (arguments.no_override
-                and base_entry is not None
-                and base_entry.msgstr
-                and ', fuzzy' not in base_entry.comments):
+        if (
+            arguments.no_override
+            and base_entry is not None
+            and base_entry.msgstr
+            and ", fuzzy" not in base_entry.comments
+        ):
             # The user does not want to override and we have an
             # existing, non-fuzzy translation.
             continue
         # Okay, we have a fine new translation.
         entry = base_entry or mixin_entry
         entry.msgstr = mixin_msgstr
-        if ', fuzzy' in entry.comments:
+        if ", fuzzy" in entry.comments:
             # The base entry was fuzzy, but the mixin has a different
             # or non-fuzzy translation.
-            entry.comments.remove(', fuzzy')
+            entry.comments.remove(", fuzzy")
         # Finally store the new entry
         base_ctl[msgid] = entry
 
     writer = catalog.POWriter(sys.stdout, base_ctl)
     writer.write(sort=False)
 
 
@@ -668,26 +699,25 @@
 
     With the --tiered option, we split the languages in three tiers or groups,
     the first two with languages that Plone was traditionally translated in,
     in a hardcoded order, followed by other languages.
     This was the default output for years.
     """
     parser = subparsers.add_parser(
-        'list',
+        "list",
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=description
+        description=description,
     )
-    parser.add_argument('-p', '--products', metavar='product', nargs='+',
-                        required=True)
+    parser.add_argument("-p", "--products", metavar="product", nargs="+", required=True)
     parser.add_argument(
-        '-t', '--table', action='store_true',
-        help="Output as html table")
+        "-t", "--table", action="store_true", help="Output as html table"
+    )
     parser.add_argument(
-        '--tiered', action='store_true',
-        help="Show in traditional three-tiered order")
+        "--tiered", action="store_true", help="Show in traditional three-tiered order"
+    )
     parser.set_defaults(func=arg_list)
     return parser
 
 
 def arg_list(arguments):
     table = arguments.table
     products = arguments.products
@@ -711,38 +741,37 @@
             ctl = catalog.MessageCatalog(filename=file)
             if pot_ctl is None:
                 pot_ctl = ctl
             else:
                 pot_ctl.merge(ctl)
 
     if not pot_ctl:
-        short_usage(1, 'Error: No pot files found.')
+        short_usage(1, "Error: No pot files found.")
 
     po_ctls = {}
     for product in pos:
         for file in pos[product]:
             ctl = catalog.MessageCatalog(filename=file)
             language = utils.getLanguage(product, file)
             lang_ctl = po_ctls.get(language, None)
             if lang_ctl is None:
                 po_ctls[language] = ctl
             else:
                 po_ctls[language].merge(ctl)
 
     if not po_ctls:
-        short_usage(1, 'Error: No po files found.')
+        short_usage(1, "Error: No po files found.")
 
     po_catalogs = []
     # flatten to list and sort
     keys = sorted(po_ctls.keys())
     for key in keys:
         po_catalogs.append(po_ctls[key])
 
-    visualisation.make_listing(
-        pot_ctl, po_catalogs, table=table, tiered=tiered)
+    visualisation.make_listing(pot_ctl, po_catalogs, table=table, tiered=tiered)
 
 
 def main():
     description = """
     i18ndude performs various tasks related to ZPT's, Python Scripts
     and i18n.
 
@@ -751,16 +780,17 @@
     with .po files (with the 'sync' command).
 
     Call i18ndude with one of the listed subcommands followed by
     --help to get help for that subcommand.
     """
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        description=textwrap.dedent(description))
-    subparsers = parser.add_subparsers(title='subcommands')
+        description=textwrap.dedent(description),
+    )
+    subparsers = parser.add_subparsers(title="subcommands")
     # Add subparsers.
     find_untranslated_parser(subparsers)
     rebuild_pot_parser(subparsers)
     merge_parser(subparsers)
     sync_parser(subparsers)
     filter_parser(subparsers)
     admix_parser(subparsers)
@@ -769,18 +799,19 @@
     # Parse the arguments.
     sys_args = sys.argv[1:]
     if not sys_args:
         # Plain 'bin/i18ndude' may fail in some Python versions.
         # See https://github.com/collective/i18ndude/issues/68
         # Pretend that 'bin/i18ndude --help' was called.
         # This makes sense in general anyway.
-        sys_args = ['--help']
+        sys_args = ["--help"]
     arguments = parser.parse_args(sys_args)
     # Special handling for the wrapping arguments, if any.
     parse_wrapping_arguments(arguments)
     # Call the function of the chosen command with the arguments.
     errors = arguments.func(arguments)
     if errors:
         sys.exit(1)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/chameleon.pt` & `i18ndude-6.1.0/src/i18ndude/testdata/input/chameleon.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest-de.po` & `i18ndude-6.1.0/src/i18ndude/testdata/input/synctest-de.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/synctest.pot` & `i18ndude-6.1.0/src/i18ndude/testdata/input/synctest.pot`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test-en.po` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test-en.po`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 "Its quite annoying that all translation editors wrap translations strings at "
 "80 characters, but then when you update the po files with i18ndude they are "
 "unwrapped and kept as huge lines. Can we fix that?"
 msgstr ""
 "Of course we can fix that. After all: i18ndude is awesome, as I am sure you "
 "all agree."
 
+msgid "msgid for standard text"
+msgstr "msgstr ···"
+
+#. Default: [···]
+#: ./folder/file_unicode
+msgid "msgid for text with comment"
+msgstr "msgstr ···"
+
 msgid "msgid for text with german umlaut"
 msgstr "äöüß text"
 
 msgid "msgid for text with html-entity"
 msgstr "&quot;this&nbsp;is&laquo;&auml;&amp;&ouml;&raquo;&quot;"
 
-msgid "msgid for unicode text"
-msgstr "unicode msgstr ···"
-
-#. Default: [···]
-#: ./folder/file_unicode
-msgid "msgid for unicode text with comment"
-msgstr "unicode msgstr ···"
-
 ## I am a dead comment
 msgid "msgid has spaces"
 msgstr "msgstr has spaces"
 
 # comment1
 #. Default: "msgstr1"
 #: file1
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.xml` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test.xml`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test.zcml` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test.zcml`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test1.pt` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test1.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2-en.po` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test2-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test2_expected-en.po` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test2_expected-en.po`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test3.pt` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test3.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/testdata/input/test5.pt` & `i18ndude-6.1.0/src/i18ndude/testdata/input/test5.pt`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/tests/test_catalog.py` & `i18ndude-6.1.0/src/i18ndude/tests/test_catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,783 +1,907 @@
-# -*- coding: utf-8 -*-
+from .utils import TESTDATA_DIR
 from i18ndude import catalog
 from i18ndude import utils
-from .utils import TESTDATA_DIR
+
 import os
-import sys
 import unittest
 import warnings
 
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
-
 
 class TestGlobal(unittest.TestCase):
-
     def test_isLiteralId(self):
         i = catalog.is_literal_id
-        errortext = 'False literal msgid recognition'
-        self.assertFalse(i('label_yes'), errortext)
-        self.assertFalse(i('_'), errortext)
-        self.assertTrue(i(' '), errortext)
-        self.assertTrue(i(' _'), errortext)
-        self.assertTrue(i('text'), errortext)
-        self.assertTrue(i('This is a text.'), errortext)
+        errortext = "False literal msgid recognition"
+        self.assertFalse(i("label_yes"), errortext)
+        self.assertFalse(i("_"), errortext)
+        self.assertTrue(i(" "), errortext)
+        self.assertTrue(i(" _"), errortext)
+        self.assertTrue(i("text"), errortext)
+        self.assertTrue(i("This is a text."), errortext)
 
     def test_originalComment(self):
         self.assertEqual(
-            catalog.ORIGINAL_COMMENT,
-            ' Original: ',
-            'Wrong original comment constant'
+            catalog.ORIGINAL_COMMENT, " Original: ", "Wrong original comment constant"
         )
 
     def test_defaultComment(self):
         self.assertEqual(
-            catalog.DEFAULT_COMMENT,
-            ' Default: ',
-            'Wrong default comment constant'
+            catalog.DEFAULT_COMMENT, " Default: ", "Wrong default comment constant"
         )
 
 
 class TestMessageEntry(unittest.TestCase):
-
     def setUp(self):
         self.me = catalog.MessageEntry
-        self.msgid = 'test msgid'
-        self.msgstr = 'test text'
-        self.references = ['test1.pt', 'test2.pt']
-        self.default_text = 'test default'
-        self.default_comment = '%s"%s"' % (catalog.DEFAULT_COMMENT, self.default_text)  # noqa
-        self.automatic_comments = ['first line', 'second line', self.default_comment]  # noqa
-        self.orig_text = 'test original'
-        self.orig_comment = '%s"%s"' % (catalog.ORIGINAL_COMMENT, self.orig_text)  # noqa
-        self.comments = ['A comment', self.orig_comment]
+        self.msgid = "test msgid"
+        self.msgstr = "test text"
+        self.references = ["test1.pt", "test2.pt"]
+        self.default_text = "test default"
+        self.default_comment = f'{catalog.DEFAULT_COMMENT}"{self.default_text}"'  # noqa
+        self.automatic_comments = [
+            "first line",
+            "second line",
+            self.default_comment,
+        ]  # noqa
+        self.orig_text = "test original"
+        self.orig_comment = f'{catalog.ORIGINAL_COMMENT}"{self.orig_text}"'  # noqa
+        self.comments = ["A comment", self.orig_comment]
 
     def test_init(self):
         me = self.me
         me1 = me(self.msgid)
-        self.assertEqual(me1.msgid, self.msgid, 'msgid not set correctly')
+        self.assertEqual(me1.msgid, self.msgid, "msgid not set correctly")
         me1 = me(self.msgid, msgstr=self.msgstr)
-        self.assertEqual(me1.msgid, self.msgid, 'msgid not set correctly')
-        self.assertEqual(me1.msgstr, self.msgstr, 'msgstr not set correctly')
+        self.assertEqual(me1.msgid, self.msgid, "msgid not set correctly")
+        self.assertEqual(me1.msgstr, self.msgstr, "msgstr not set correctly")
 
         me1 = me(self.msgid, msgstr=self.msgstr, references=self.references)
-        self.assertEqual(me1.msgid, self.msgid, 'msgid not set correctly')
-        self.assertEqual(me1.msgstr, self.msgstr, 'msgstr not set correctly')
-        self.assertEqual(me1.references, self.references, 'references not set correctly')  # noqa
+        self.assertEqual(me1.msgid, self.msgid, "msgid not set correctly")
+        self.assertEqual(me1.msgstr, self.msgstr, "msgstr not set correctly")
+        self.assertEqual(
+            me1.references, self.references, "references not set correctly"
+        )  # noqa
 
         me1 = me(self.msgid, msgstr=self.msgstr, comments=self.comments)
-        self.assertEqual(me1.msgid, self.msgid, 'msgid not set correctly')
-        self.assertEqual(me1.msgstr, self.msgstr, 'msgstr not set correctly')
-        self.assertEqual(me1.comments, self.comments, 'comments not set correctly')  # noqa
-        self.assertEqual(me1.getOriginalComment(), self.orig_comment, 'Original comment not set correctly')  # noqa
-        self.assertEqual(me1.getOriginal(), self.orig_text, 'Original text not set correctly')  # noqa
-
-        me2 = me(self.msgid, msgstr=self.msgstr, automatic_comments=self.automatic_comments)  # noqa
-        self.assertEqual(me2.msgid, self.msgid, 'msgid not set correctly')
-        self.assertEqual(me2.msgstr, self.msgstr, 'msgstr not set correctly')
-        self.assertEqual(me2.automatic_comments, self.automatic_comments, 'comments not set correctly')  # noqa
-        self.assertEqual(me2.getDefaultComment(), self.default_comment, 'Default comment not set correctly')  # noqa
-        self.assertEqual(me2.getDefault(), self.default_text, 'Default text not set correctly')  # noqa
+        self.assertEqual(me1.msgid, self.msgid, "msgid not set correctly")
+        self.assertEqual(me1.msgstr, self.msgstr, "msgstr not set correctly")
+        self.assertEqual(
+            me1.comments, self.comments, "comments not set correctly"
+        )  # noqa
+        self.assertEqual(
+            me1.getOriginalComment(),
+            self.orig_comment,
+            "Original comment not set correctly",
+        )  # noqa
+        self.assertEqual(
+            me1.getOriginal(), self.orig_text, "Original text not set correctly"
+        )  # noqa
+
+        me2 = me(
+            self.msgid, msgstr=self.msgstr, automatic_comments=self.automatic_comments
+        )  # noqa
+        self.assertEqual(me2.msgid, self.msgid, "msgid not set correctly")
+        self.assertEqual(me2.msgstr, self.msgstr, "msgstr not set correctly")
+        self.assertEqual(
+            me2.automatic_comments,
+            self.automatic_comments,
+            "comments not set correctly",
+        )  # noqa
+        self.assertEqual(
+            me2.getDefaultComment(),
+            self.default_comment,
+            "Default comment not set correctly",
+        )  # noqa
+        self.assertEqual(
+            me2.getDefault(), self.default_text, "Default text not set correctly"
+        )  # noqa
 
 
 class TestMessageCatalogInit(unittest.TestCase):
-
     def setUp(self):
         self.mc = catalog.MessageCatalog
         self.me = catalog.MessageEntry
-        self.file = os.path.join(TESTDATA_DIR, 'input', 'test-en.po')
-        self.emptyfile = os.path.join(TESTDATA_DIR, 'input', 'empty-en.po')
+        self.file = os.path.join(TESTDATA_DIR, "input", "test-en.po")
+        self.emptyfile = os.path.join(TESTDATA_DIR, "input", "empty-en.po")
 
         self.commentary_header = [
-            ' Translation of test.pot to English',
-            ' Hanno Schlichting <schlichting@bakb.net>, 2005']
+            " Translation of test.pot to English",
+            " Hanno Schlichting <schlichting@bakb.net>, 2005",
+        ]
 
         self.mimeheader = {
-            'Language-Code': 'en',
-            'Domain': 'testing',
-            'PO-Revision-Date': '2005-08-10 21:15+0000',
-            'Content-Transfer-Encoding': '8bit',
-            'Language-Name': 'English',
-            'Plural-Forms': 'nplurals=1; plural=0;',
-            'Project-Id-Version': 'i18ndude',
-            'Preferred-Encodings': 'utf-8 latin1',
-            'Last-Translator': u'Unicödé Guy',
-            'Language-Team': 'Plone i18n <plone-i18n@lists.sourceforge.net>',
-            'POT-Creation-Date': '2005-08-01 12:00+0000',
-            'Content-Type': 'text/plain; charset=utf-8', 'MIME-Version': '1.0'
+            "Language-Code": "en",
+            "Domain": "testing",
+            "PO-Revision-Date": "2005-08-10 21:15+0000",
+            "Content-Transfer-Encoding": "8bit",
+            "Language-Name": "English",
+            "Plural-Forms": "nplurals=1; plural=0;",
+            "Project-Id-Version": "i18ndude",
+            "Preferred-Encodings": "utf-8 latin1",
+            "Last-Translator": "Unicödé Guy",
+            "Language-Team": "Plone i18n <plone-i18n@lists.sourceforge.net>",
+            "POT-Creation-Date": "2005-08-01 12:00+0000",
+            "Content-Type": "text/plain; charset=utf-8",
+            "MIME-Version": "1.0",
         }
 
         self.msgids = {
-            u'msgid1': self.me(
-                'msgid1',
-                msgstr='msgstr1',
-                references=['file1', 'file2'],
+            "msgid1": self.me(
+                "msgid1",
+                msgstr="msgstr1",
+                references=["file1", "file2"],
                 automatic_comments=[' Default: "msgstr1"'],
-                comments=[' comment1']),
-
-            u'msgid2': self.me(
-                'msgid2',
-                msgstr='msgstr2',
-                references=['file2']),
-
-            u'msgid3': self.me(
-                'msgid3',
-                msgstr='\\n\\nmsgstr\\n3',
-                references=['file3'],
-                comments=[' comment3']),
-
-            u'msgid4': self.me(
-                'msgid4',
-                msgstr='msgstr4',
-                references=['file4']),
-
-            u'msgid5': self.me(
-                'msgid5',
-                msgstr='msgstr5',
-                comments=[' comment5']),
-
-            u'msgid6': self.me(
-                'msgid6',
-                msgstr='msgstr6'),
-
-            u'msgid7': self.me(
-                'msgid7',
-                msgstr='msgstr7',
-                comments=[', fuzzy']),
-
-            u'msgid8': self.me(
-                'msgid8'),
-
-            u'msgid has spaces': self.me(
-                'msgid has spaces',
-                msgstr='msgstr has spaces',
-                comments=['# I am a dead comment']),
-
-            u'msgid_has_underlines': self.me(
-                'msgid_has_underlines',
-                msgstr='msgstr_has_underlines'),
-
-            u'msgid_has_underlines and spaces': self.me(
-                'msgid_has_underlines and spaces',
-                msgstr='msgstr_has_underlines and spaces'),
-
-            u'msgid for unicode text': self.me(
-                'msgid for unicode text',
-                msgstr=u'unicode msgstr \xb7\xb7\xb7'),
-
-            u'msgid for unicode text with comment': self.me(
-                'msgid for unicode text with comment',
-                msgstr=u'unicode msgstr \xb7\xb7\xb7',
-                references=['./folder/file_unicode'],
-                automatic_comments=[' Default: [···]']),
-
-            u'msgid for text with german umlaut': self.me(
-                'msgid for text with german umlaut',
-                msgstr=u'\xe4\xf6\xfc\xdf text'),
-
-            u'msgid for text with html-entity': self.me(
-                'msgid for text with html-entity',
-                msgstr='&quot;this&nbsp;is&laquo;&auml;&amp;&ouml;&raquo;&quot;'),  # noqa
-
-            (u"Its quite annoying that all translation editors wrap "
-             "translations strings at 80 characters, but then when you "
-             "update the po files with i18ndude they are unwrapped and "
-             "kept as huge lines. Can we fix that?"): self.me(
-                 u"Its quite annoying that all translation editors wrap "
-                 "translations strings at 80 characters, but then when you "
-                 "update the po files with i18ndude they are unwrapped and "
-                 "kept as huge lines. Can we fix that?",
-                 msgstr=("Of course we can fix that. After all: i18ndude is "
-                         "awesome, as I am sure you all agree."),
-                 comments=[
-                     (" https://github.com/collective/i18ndude/issues/3 "
-                      "complains about long lines. But long comment lines "
-                      "should be left intact."),
-                     (" Note that the unix msgattrib command can wrap or "
-                      "unwrap long lines in po files.")]),
-
-            u'msgid_with_long_lines_including_backslash_n.': self.me(
-                'msgid_with_long_lines_including_backslash_n.',
-                msgstr=("Falls aktiv wird der entsprechende \\nLinkcycle einen"
-                        " Button haben, mit dem man durch ihn blaettern kann. "
-                        "mit dem man durch ihn blaettern kann. mit dem man "
-                        "durch ihn blaettern kann. mit dem man durch ihn "
-                        "blaettern kann.")),  # XXX
-
+                comments=[" comment1"],
+            ),
+            "msgid2": self.me("msgid2", msgstr="msgstr2", references=["file2"]),
+            "msgid3": self.me(
+                "msgid3",
+                msgstr="\\n\\nmsgstr\\n3",
+                references=["file3"],
+                comments=[" comment3"],
+            ),
+            "msgid4": self.me("msgid4", msgstr="msgstr4", references=["file4"]),
+            "msgid5": self.me("msgid5", msgstr="msgstr5", comments=[" comment5"]),
+            "msgid6": self.me("msgid6", msgstr="msgstr6"),
+            "msgid7": self.me("msgid7", msgstr="msgstr7", comments=[", fuzzy"]),
+            "msgid8": self.me("msgid8"),
+            "msgid has spaces": self.me(
+                "msgid has spaces",
+                msgstr="msgstr has spaces",
+                comments=["# I am a dead comment"],
+            ),
+            "msgid_has_underlines": self.me(
+                "msgid_has_underlines", msgstr="msgstr_has_underlines"
+            ),
+            "msgid_has_underlines and spaces": self.me(
+                "msgid_has_underlines and spaces",
+                msgstr="msgstr_has_underlines and spaces",
+            ),
+            "msgid for standard text": self.me(
+                "msgid for standard text", msgstr="msgstr \xb7\xb7\xb7"
+            ),
+            "msgid for text with comment": self.me(
+                "msgid for text with comment",
+                msgstr="msgstr \xb7\xb7\xb7",
+                references=["./folder/file_unicode"],
+                automatic_comments=[" Default: [···]"],
+            ),
+            "msgid for text with german umlaut": self.me(
+                "msgid for text with german umlaut", msgstr="\xe4\xf6\xfc\xdf text"
+            ),
+            "msgid for text with html-entity": self.me(
+                "msgid for text with html-entity",
+                msgstr="&quot;this&nbsp;is&laquo;&auml;&amp;&ouml;&raquo;&quot;",
+            ),  # noqa
+            (
+                "Its quite annoying that all translation editors wrap "
+                "translations strings at 80 characters, but then when you "
+                "update the po files with i18ndude they are unwrapped and "
+                "kept as huge lines. Can we fix that?"
+            ): self.me(
+                "Its quite annoying that all translation editors wrap "
+                "translations strings at 80 characters, but then when you "
+                "update the po files with i18ndude they are unwrapped and "
+                "kept as huge lines. Can we fix that?",
+                msgstr=(
+                    "Of course we can fix that. After all: i18ndude is "
+                    "awesome, as I am sure you all agree."
+                ),
+                comments=[
+                    (
+                        " https://github.com/collective/i18ndude/issues/3 "
+                        "complains about long lines. But long comment lines "
+                        "should be left intact."
+                    ),
+                    (
+                        " Note that the unix msgattrib command can wrap or "
+                        "unwrap long lines in po files."
+                    ),
+                ],
+            ),
+            "msgid_with_long_lines_including_backslash_n.": self.me(
+                "msgid_with_long_lines_including_backslash_n.",
+                msgstr=(
+                    "Falls aktiv wird der entsprechende \\nLinkcycle einen"
+                    " Button haben, mit dem man durch ihn blaettern kann. "
+                    "mit dem man durch ihn blaettern kann. mit dem man "
+                    "durch ihn blaettern kann. mit dem man durch ihn "
+                    "blaettern kann."
+                ),
+            ),  # XXX
         }
 
     def test_init(self):
         failing = False
         try:
             catalog.MessageCatalog()
         except AssertionError:
             failing = True
-        self.assertTrue(
-            failing, 'Init without parameters should not be allowed.')
+        self.assertTrue(failing, "Init without parameters should not be allowed.")
 
     def test_initWithDomain(self):
-        domain = 'testing'
+        domain = "testing"
         test = self.mc(domain=domain)
         mime = catalog.DEFAULT_PO_MIME
         for key, value in mime:
-            if key != 'Domain':
+            if key != "Domain":
                 self.assertEqual(
-                    value,
-                    test.mime_header[key],
-                    'header mismatch on %s' % key
+                    value, test.mime_header[key], "header mismatch on %s" % key
                 )
             else:
-                self.assertEqual(
-                    domain,
-                    test.mime_header['Domain'],
-                    'Domain mismatch'
-                )
+                self.assertEqual(domain, test.mime_header["Domain"], "Domain mismatch")
         self.assertEqual(
             catalog.DEFAULT_PO_HEADER,
             test.commentary_header,
-            'commentary header mismatch'
+            "commentary header mismatch",
         )
-        self.assertEqual(len(test), 0, 'Non-empty catalog')
+        self.assertEqual(len(test), 0, "Non-empty catalog")
 
     def test_initWithEmptyFile(self):
         test = self.mc(filename=self.emptyfile)
         mime = catalog.DEFAULT_PO_MIME
         for key, value in mime:
             self.assertEqual(
-                value,
-                test.mime_header[key],
-                'header mismatch on %s' % key
+                value, test.mime_header[key], "header mismatch on %s" % key
             )
 
     def test_initWithEmptyFileAndDomain(self):
         failing = False
         try:
-            self.mc(domain='testing', filename=self.emptyfile)
+            self.mc(domain="testing", filename=self.emptyfile)
         except AssertionError:
             failing = True
         self.assertTrue(
-            failing,
-            'Init with filename and domain parameters is not allowed.'
+            failing, "Init with filename and domain parameters is not allowed."
         )
 
     def test_initWithFile(self):
         test = self.mc(filename=self.file)
         for key in test.mime_header:
             self.assertEqual(
                 test.mime_header[key],
                 self.mimeheader[key],
-                'wrong mime header parsing:\nGot: %s !=\nExpected: %s'
-                % (test.mime_header[key], self.mimeheader[key])
+                "wrong mime header parsing:\nGot: %s !=\nExpected: %s"
+                % (test.mime_header[key], self.mimeheader[key]),
             )
         for value in test.commentary_header:
             self.assertTrue(
-                value in self.commentary_header,
-                'wrong commentary header parsing'
+                value in self.commentary_header, "wrong commentary header parsing"
             )
         if not test == self.msgids:
             for key in test:
                 self.assertTrue(
                     test[key] == self.msgids[key],
-                    'error in po parsing:\nGot:      %s !=\nExpected: %s'
-                    % (test[key], self.msgids[key])
+                    "error in po parsing:\nGot:      %s !=\nExpected: %s"
+                    % (test[key], self.msgids[key]),
                 )
 
 
 class TestMessageCatalog(unittest.TestCase):
-
     def setUp(self):
-        self.domain = 'testing'
+        self.domain = "testing"
         self.mc = catalog.MessageCatalog(domain=self.domain)
-        self.msgid = 'test msgid'
-        self.msgstr = 'test text'
-        self.references = ['test1.pt', 'test2.pt']
-        self.default_text = 'test default'
-        self.default_comment = '%s"%s"' % (catalog.DEFAULT_COMMENT, self.default_text)  # noqa
-        self.automatic_comments = ['first line', 'second line', self.default_comment]  # noqa
-        self.orig_text = 'test original'
-        self.orig_comment = '%s"%s"' % (catalog.ORIGINAL_COMMENT, self.orig_text)  # noqa
-        self.comments = ['A comment', self.orig_comment]
+        self.msgid = "test msgid"
+        self.msgstr = "test text"
+        self.references = ["test1.pt", "test2.pt"]
+        self.default_text = "test default"
+        self.default_comment = f'{catalog.DEFAULT_COMMENT}"{self.default_text}"'  # noqa
+        self.automatic_comments = [
+            "first line",
+            "second line",
+            self.default_comment,
+        ]  # noqa
+        self.orig_text = "test original"
+        self.orig_comment = f'{catalog.ORIGINAL_COMMENT}"{self.orig_text}"'  # noqa
+        self.comments = ["A comment", self.orig_comment]
 
     def test_add(self):
         msgid = self.msgid
         msgstr = self.msgstr
         references = self.references
         automatic_comments = self.automatic_comments
 
         # add with msgid
         self.mc.add(msgid)
-        self.assertTrue(msgid in self.mc, 'msgid not found in catalog')
+        self.assertTrue(msgid in self.mc, "msgid not found in catalog")
         del self.mc[msgid]
-        self.assertFalse(msgid in self.mc, 'msgid found in catalog')
+        self.assertFalse(msgid in self.mc, "msgid found in catalog")
         # add with msgid and msgstr
         self.mc.add(msgid, msgstr=msgstr)
-        self.assertEqual(self.mc[msgid].msgstr, msgstr, 'msgstr not found in catalog.')  # noqa
+        self.assertEqual(
+            self.mc[msgid].msgstr, msgstr, "msgstr not found in catalog."
+        )  # noqa
         del self.mc[msgid]
-        self.assertFalse(msgid in self.mc, 'msgid found in catalog')
+        self.assertFalse(msgid in self.mc, "msgid found in catalog")
         # add with msgid, msgstr and filename
         self.mc.add(msgid, msgstr=msgstr, references=references)
-        self.assertEqual(self.mc[msgid].references, references, 'references not found in catalog.')  # noqa
+        self.assertEqual(
+            self.mc[msgid].references, references, "references not found in catalog."
+        )  # noqa
         del self.mc[msgid]
-        self.assertFalse(msgid in self.mc, 'msgid found in catalog')
+        self.assertFalse(msgid in self.mc, "msgid found in catalog")
         # add with msgid, msgstr, filename and excerpt
-        self.mc.add(msgid, msgstr=msgstr, references=references, automatic_comments=automatic_comments)  # noqa
-        self.assertEqual(self.mc[msgid].automatic_comments, automatic_comments, 'automatic_comments not found in catalog.')  # noqa
+        self.mc.add(
+            msgid,
+            msgstr=msgstr,
+            references=references,
+            automatic_comments=automatic_comments,
+        )  # noqa
+        self.assertEqual(
+            self.mc[msgid].automatic_comments,
+            automatic_comments,
+            "automatic_comments not found in catalog.",
+        )  # noqa
         del self.mc[msgid]
-        self.assertFalse(msgid in self.mc, 'msgid found in catalog')
+        self.assertFalse(msgid in self.mc, "msgid found in catalog")
 
     def test_multipleAdd(self):
         msgid = self.msgid
         msgstr = self.msgstr
         references = self.references
         automatic_comments = self.automatic_comments
 
-        self.mc.add(msgid, msgstr=msgstr, references=references, automatic_comments=automatic_comments)  # noqa
-        self.mc.add(msgid, msgstr=msgstr, references=references, automatic_comments=automatic_comments)  # noqa
-        self.assertTrue(len(self.mc) == 1, 'duplicate msgid')
-        self.assertTrue(len(self.mc[msgid].references) == 2, 'references missing')  # noqa
+        self.mc.add(
+            msgid,
+            msgstr=msgstr,
+            references=references,
+            automatic_comments=automatic_comments,
+        )  # noqa
+        self.mc.add(
+            msgid,
+            msgstr=msgstr,
+            references=references,
+            automatic_comments=automatic_comments,
+        )  # noqa
+        self.assertTrue(len(self.mc) == 1, "duplicate msgid")
+        self.assertTrue(
+            len(self.mc[msgid].references) == 2, "references missing"
+        )  # noqa
 
     def test_originalComment(self):
-        self.mc.add(self.msgid, msgstr=self.msgstr, references=self.references, automatic_comments=self.automatic_comments)  # noqa
+        self.mc.add(
+            self.msgid,
+            msgstr=self.msgstr,
+            references=self.references,
+            automatic_comments=self.automatic_comments,
+        )  # noqa
         self.mc[self.msgid].comments.extend(self.comments)
-        self.assertEqual(self.mc.getComments(self.msgid), self.comments, 'wrong comments')  # noqa
-        self.assertEqual(self.mc.getOriginalComment(self.msgid), self.orig_comment, 'wrong original comment line')  # noqa
-        self.assertEqual(self.mc.getOriginal(self.msgid), self.orig_text, 'wrong original comment text')  # noqa
-        self.assertEqual(self.mc.getDefaultComment(self.msgid), self.default_comment, 'wrong default comment line')  # noqa
-        self.assertEqual(self.mc.getDefault(self.msgid), self.default_text, 'wrong default comment text')  # noqa
+        self.assertEqual(
+            self.mc.getComments(self.msgid), self.comments, "wrong comments"
+        )  # noqa
+        self.assertEqual(
+            self.mc.getOriginalComment(self.msgid),
+            self.orig_comment,
+            "wrong original comment line",
+        )  # noqa
+        self.assertEqual(
+            self.mc.getOriginal(self.msgid),
+            self.orig_text,
+            "wrong original comment text",
+        )  # noqa
+        self.assertEqual(
+            self.mc.getDefaultComment(self.msgid),
+            self.default_comment,
+            "wrong default comment line",
+        )  # noqa
+        self.assertEqual(
+            self.mc.getDefault(self.msgid),
+            self.default_text,
+            "wrong default comment text",
+        )  # noqa
 
 
 class TestMessageCatalogSync(unittest.TestCase):
-
     def setUp(self):
         mc = catalog.MessageCatalog
-        self.potfile = os.path.join(TESTDATA_DIR, 'input', 'synctest.pot')
-        self.pofile = os.path.join(TESTDATA_DIR, 'input', 'synctest-de.po')
+        self.potfile = os.path.join(TESTDATA_DIR, "input", "synctest.pot")
+        self.pofile = os.path.join(TESTDATA_DIR, "input", "synctest-de.po")
         self.pot = mc(filename=self.potfile)
         self.po = mc(filename=self.pofile)
 
     def test_sync(self):
         old_defaults = {}
         for id in self.po:
             old_defaults[id] = self.po[id].getDefault()
         self.po.sync(self.pot)
-        self.assertTrue(len(self.pot) == len(self.po), 'number of messages does not match')  # noqa
+        self.assertTrue(
+            len(self.pot) == len(self.po), "number of messages does not match"
+        )  # noqa
         for msgid in self.pot:
-            self.assertTrue(msgid in self.po, 'msgid %s could not be found' % self.pot[msgid])  # noqa
-            self.assertTrue(self.po[msgid].references == self.pot[msgid].references)  # noqa
+            self.assertTrue(
+                msgid in self.po, "msgid %s could not be found" % self.pot[msgid]
+            )  # noqa
+            self.assertTrue(
+                self.po[msgid].references == self.pot[msgid].references
+            )  # noqa
             defaults = self.po[msgid].getDefaults()
             if defaults is not None:
                 for dc in defaults:
                     self.assertTrue(
-                        dc == self.pot[msgid].getDefault() or
-                        dc == old_defaults[msgid],
-                        'Either old or new default comment is missing on msgid: %s' % msgid  # noqa
+                        dc == self.pot[msgid].getDefault() or dc == old_defaults[msgid],
+                        "Either old or new default comment is missing on msgid: %s"
+                        % msgid,  # noqa
                     )
 
 
 class TestMessagePoWriter(unittest.TestCase):
-
     def setUp(self):
         mc = catalog.MessageCatalog
-        self.input = os.path.join(TESTDATA_DIR, 'input', 'test-en.po')
-        self.output = os.path.join(TESTDATA_DIR, 'output', 'test-en.po')
-        self.input2 = os.path.join(TESTDATA_DIR, 'input', 'test2-en.po')
-        self.expectedOutput2 = os.path.join(TESTDATA_DIR, 'input', 'test2_expected-en.po')  # noqa
-        self.output2 = os.path.join(TESTDATA_DIR, 'output', 'test2-en.po')
+        self.input = os.path.join(TESTDATA_DIR, "input", "test-en.po")
+        self.output = os.path.join(TESTDATA_DIR, "output", "test-en.po")
+        self.input2 = os.path.join(TESTDATA_DIR, "input", "test2-en.po")
+        self.expectedOutput2 = os.path.join(
+            TESTDATA_DIR, "input", "test2_expected-en.po"
+        )  # noqa
+        self.output2 = os.path.join(TESTDATA_DIR, "output", "test2-en.po")
         self.catalog = mc(filename=self.input)
         self.catalog2 = mc(filename=self.input2)
         if os.path.exists(self.output):
             os.remove(self.output)
         if os.path.exists(self.output2):
             os.remove(self.output2)
 
     def test_write(self):
         # Explicitly enable wrapping here, as that is what we did in
         # the test po file.
         orig_wrap = utils.WRAP
         utils.WRAP = True
-        fd = open(self.output, 'w')
+        fd = open(self.output, "w")
         pow = catalog.POWriter(fd, self.catalog)
         pow.write(sort=True)
         fd.close()
         # Restore original value.
         utils.WRAP = orig_wrap
 
-        input_ = open(self.input, 'r')
-        output = open(self.output, 'r')
+        input_ = open(self.input)
+        output = open(self.output)
 
         # compare line by line
         inlines = input_.readlines()
         outlines = enumerate(output.readlines())
 
         input_.close()
         output.close()
 
         for i, result in outlines:
             orig = inlines[i]
             self.assertEqual(
-                orig,
-                result,
-                'difference in line %s, \'%s\' != \'%s\''
-                % (i, orig, result)
+                orig, result, "difference in line %s, '%s' != '%s'" % (i, orig, result)
             )
 
     def test_writeSpecialComments(self):
-        fd = open(self.output2, 'w')
+        fd = open(self.output2, "w")
         pow = catalog.POWriter(fd, self.catalog2)
         pow.write(sort=True)
         fd.close()
 
-        output = open(self.output2, 'r')
-        expected = open(self.expectedOutput2, 'r')
+        output = open(self.output2)
+        expected = open(self.expectedOutput2)
 
         # compare line by line
         outlines = output.readlines()
         explines = enumerate(expected.readlines())
 
         output.close()
         expected.close()
 
         for i, result in explines:
             orig = outlines[i]
             self.assertEqual(
                 orig,
                 result,
-                'difference in line %s, Got: \'%s\' != Expected: \'%s\''
-                % (i, orig, result)
+                "difference in line %s, Got: '%s' != Expected: '%s'"
+                % (i, orig, result),
             )
 
     def tearDown(self):
         if os.path.exists(self.output):
             os.remove(self.output)
         if os.path.exists(self.output2):
             os.remove(self.output2)
 
 
 class TestMessagePTReader(unittest.TestCase):
-
     def test_read_no_line_numbers(self):
         me = catalog.MessageEntry
-        input_ = os.path.join(TESTDATA_DIR, 'input')
-        filename = input_ + os.sep + 'test1.pt'
-        filename3 = input_ + os.sep + 'test3.pt'
-        filename5 = input_ + os.sep + 'test5.pt'
+        input_ = os.path.join(TESTDATA_DIR, "input")
+        filename = input_ + os.sep + "test1.pt"
+        filename3 = input_ + os.sep + "test3.pt"
+        filename5 = input_ + os.sep + "test5.pt"
         output = {
-            u'Buzz': me(u'Buzz', references=[filename]),
-            u'${foo} ${with-dash-and_underscore}': me(u'${foo} ${with-dash-and_underscore}', references=[filename]),  # noqa
-            u'dig_this': me(u'dig_this', msgstr=u'Dig this', references=[filename]),  # noqa
-            u'text_buzz': me(u'text_buzz', msgstr=u'Buzz', references=[filename]),  # noqa
-            u'some_alt': me(u'some_alt', msgstr=u'Some alt', references=[filename, filename3]),  # noqa
-            u'title_some_alt': me(u'title_some_alt', msgstr=u'Some title', references=[filename]),  # noqa
-            u'Job started at ${datetime} by user ${userid}.': me(u'Job started at ${datetime} by user ${userid}.', references=[filename]),  # noqa
-            u'spacing': me(u'spacing', msgstr=u'Space <br /> before and after.', references=[filename]),  # noqa
-            u'spacing_strong': me(u'spacing_strong', msgstr=u'Please press your browser\'s <strong>Back</strong> button to try again.', references=[filename]),  # noqa
-            u'<tt>domain</tt> is one of the <em>local domains</em>:': me(u'<tt>domain</tt> is one of the <em>local domains</em>:', references=[filename]),  # noqa
-            u'odd': me(u'odd', references=[filename]),
-            u'even': me(u'even', references=[filename]),
-            u'Test for issue 15, html5 attributes without value': me(u'Test for issue 15, html5 attributes without value', references=[filename]),  # noqa
-            u'rebuild-pot should not complain about Chameleon repeat syntax.': me(u'rebuild-pot should not complain about Chameleon repeat syntax.', references=[filename5]),  # noqa
-            u'rebuild-pot should not complain about Chameleon define syntax.': me(u'rebuild-pot should not complain about Chameleon define syntax.', references=[filename5]),  # noqa
+            "Buzz": me("Buzz", references=[filename]),
+            "${foo} ${with-dash-and_underscore}": me(
+                "${foo} ${with-dash-and_underscore}", references=[filename]
+            ),  # noqa
+            "dig_this": me(
+                "dig_this", msgstr="Dig this", references=[filename]
+            ),  # noqa
+            "text_buzz": me("text_buzz", msgstr="Buzz", references=[filename]),  # noqa
+            "some_alt": me(
+                "some_alt", msgstr="Some alt", references=[filename, filename3]
+            ),  # noqa
+            "title_some_alt": me(
+                "title_some_alt", msgstr="Some title", references=[filename]
+            ),  # noqa
+            "Job started at ${datetime} by user ${userid}.": me(
+                "Job started at ${datetime} by user ${userid}.", references=[filename]
+            ),  # noqa
+            "spacing": me(
+                "spacing",
+                msgstr="Space <br /> before and after.",
+                references=[filename],
+            ),  # noqa
+            "spacing_strong": me(
+                "spacing_strong",
+                msgstr="Please press your browser's <strong>Back</strong> button to try again.",
+                references=[filename],
+            ),  # noqa
+            "<tt>domain</tt> is one of the <em>local domains</em>:": me(
+                "<tt>domain</tt> is one of the <em>local domains</em>:",
+                references=[filename],
+            ),  # noqa
+            "odd": me("odd", references=[filename]),
+            "even": me("even", references=[filename]),
+            "Test for issue 15, html5 attributes without value": me(
+                "Test for issue 15, html5 attributes without value",
+                references=[filename],
+            ),  # noqa
+            "rebuild-pot should not complain about Chameleon repeat syntax.": me(
+                "rebuild-pot should not complain about Chameleon repeat syntax.",
+                references=[filename5],
+            ),  # noqa
+            "rebuild-pot should not complain about Chameleon define syntax.": me(
+                "rebuild-pot should not complain about Chameleon define syntax.",
+                references=[filename5],
+            ),  # noqa
         }
 
-        ptr = catalog.PTReader(input_, domain='testing', include_line_numbers = False)
+        ptr = catalog.PTReader(input_, domain="testing", include_line_numbers=False)
         with warnings.catch_warnings(record=True) as log:
             warnings.simplefilter("always")
             # This call will give a warning from zope.tal.
             ptr.read()
             self.assertGreaterEqual(len(log), 1, log)
-            contents = '\n'.join([str(x.message) for x in log])
+            contents = "\n".join([str(x.message) for x in log])
             # Check that a few key elements are in the
             # warning, without wanting to check the exact
             # wording, as this can easily change.
-            self.assertTrue("already exists with a different default"
-                            in contents, 'missing "already exists"')
-            self.assertTrue("bad: b'Buzzer', should be: b'Buzz'"  # py36
-                            in contents or
-                            "bad: Buzzer, should be: Buzz"  # py27
-                            in contents,
-                            u'bad Buzzer not in contents: {}'.format(contents))
+            self.assertTrue(
+                "already exists with a different default" in contents,
+                'missing "already exists"',
+            )
+            self.assertTrue(
+                "bad: b'Buzzer', should be: b'Buzz'" in contents  # py36
+                or "bad: Buzzer, should be: Buzz" in contents,  # py27
+                f"bad Buzzer not in contents: {contents}",
+            )
 
-        out = ptr.catalogs['testing']
+        out = ptr.catalogs["testing"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in pt parsing.\nUnexpected msgid: %s' % key
+                key in output, "Failure in pt parsing.\nUnexpected msgid: %s" % key
             )
         for key in output:
-            self.assertTrue(out[key] == output[key],
-                            'Failure in pt parsing.\nGot:%s\nExpected:%s' %
-                            (out[key], output[key]))
+            self.assertTrue(
+                out[key] == output[key],
+                "Failure in pt parsing.\nGot:%s\nExpected:%s" % (out[key], output[key]),
+            )
         self.assertEqual(len(out), len(output))
 
     def test_read_include_line_numbers(self):
         me = catalog.MessageEntry
-        input_ = os.path.join(TESTDATA_DIR, 'input')
-        filename = input_ + os.sep + 'test1.pt'
-        filename3 = input_ + os.sep + 'test3.pt'
-        filename5 = input_ + os.sep + 'test5.pt'
+        input_ = os.path.join(TESTDATA_DIR, "input")
+        filename = input_ + os.sep + "test1.pt"
+        filename3 = input_ + os.sep + "test3.pt"
+        filename5 = input_ + os.sep + "test5.pt"
         output = {
-            u'Buzz': me(u'Buzz', references=[filename + ':21']),
-            u'${foo} ${with-dash-and_underscore}': me(u'${foo} ${with-dash-and_underscore}', references=[filename + ':26']),  # noqa
-            u'dig_this': me(u'dig_this', msgstr=u'Dig this', references=[filename + ':52']),  # noqa
-            u'text_buzz': me(u'text_buzz', msgstr=u'Buzz', references=[filename + ':29', filename + ':31']),  # noqa
-            u'some_alt': me(u'some_alt', msgstr=u'Some alt', references=[filename + ':15', filename3 + ':15']),  # noqa
-            u'title_some_alt': me(u'title_some_alt', msgstr=u'Some title', references=[filename + ':15']),  # noqa
-            u'Job started at ${datetime} by user ${userid}.': me(u'Job started at ${datetime} by user ${userid}.', references=[filename + ':46']),  # noqa
-            u'spacing': me(u'spacing', msgstr=u'Space <br /> before and after.', references=[filename + ':37']),  # noqa
-            u'spacing_strong': me(u'spacing_strong', msgstr=u'Please press your browser\'s <strong>Back</strong> button to try again.', references=[filename + ':41']),  # noqa
-            u'<tt>domain</tt> is one of the <em>local domains</em>:': me(u'<tt>domain</tt> is one of the <em>local domains</em>:', references=[filename + ':49']),  # noqa
-            u'odd': me(u'odd', references=[filename + ':58']),
-            u'even': me(u'even', references=[filename + ':59']),
-            u'Test for issue 15, html5 attributes without value': me(u'Test for issue 15, html5 attributes without value', references=[filename + ':62']),  # noqa
-            u'rebuild-pot should not complain about Chameleon repeat syntax.': me(u'rebuild-pot should not complain about Chameleon repeat syntax.', references=[filename5 + ':16']),  # noqa
-            u'rebuild-pot should not complain about Chameleon define syntax.': me(u'rebuild-pot should not complain about Chameleon define syntax.', references=[filename5 + ':19']),  # noqa
+            "Buzz": me("Buzz", references=[filename + ":21"]),
+            "${foo} ${with-dash-and_underscore}": me(
+                "${foo} ${with-dash-and_underscore}", references=[filename + ":26"]
+            ),  # noqa
+            "dig_this": me(
+                "dig_this", msgstr="Dig this", references=[filename + ":52"]
+            ),  # noqa
+            "text_buzz": me(
+                "text_buzz",
+                msgstr="Buzz",
+                references=[filename + ":29", filename + ":31"],
+            ),  # noqa
+            "some_alt": me(
+                "some_alt",
+                msgstr="Some alt",
+                references=[filename + ":15", filename3 + ":15"],
+            ),  # noqa
+            "title_some_alt": me(
+                "title_some_alt", msgstr="Some title", references=[filename + ":15"]
+            ),  # noqa
+            "Job started at ${datetime} by user ${userid}.": me(
+                "Job started at ${datetime} by user ${userid}.",
+                references=[filename + ":46"],
+            ),  # noqa
+            "spacing": me(
+                "spacing",
+                msgstr="Space <br /> before and after.",
+                references=[filename + ":37"],
+            ),  # noqa
+            "spacing_strong": me(
+                "spacing_strong",
+                msgstr="Please press your browser's <strong>Back</strong> button to try again.",
+                references=[filename + ":41"],
+            ),  # noqa
+            "<tt>domain</tt> is one of the <em>local domains</em>:": me(
+                "<tt>domain</tt> is one of the <em>local domains</em>:",
+                references=[filename + ":49"],
+            ),  # noqa
+            "odd": me("odd", references=[filename + ":58"]),
+            "even": me("even", references=[filename + ":59"]),
+            "Test for issue 15, html5 attributes without value": me(
+                "Test for issue 15, html5 attributes without value",
+                references=[filename + ":62"],
+            ),  # noqa
+            "rebuild-pot should not complain about Chameleon repeat syntax.": me(
+                "rebuild-pot should not complain about Chameleon repeat syntax.",
+                references=[filename5 + ":16"],
+            ),  # noqa
+            "rebuild-pot should not complain about Chameleon define syntax.": me(
+                "rebuild-pot should not complain about Chameleon define syntax.",
+                references=[filename5 + ":19"],
+            ),  # noqa
         }
 
-        ptr = catalog.PTReader(input_, domain='testing')
+        ptr = catalog.PTReader(input_, domain="testing")
         with warnings.catch_warnings(record=True) as log:
             warnings.simplefilter("always")
             # This call will give a warning from zope.tal.
             ptr.read()
             self.assertGreaterEqual(len(log), 1, log)
-            contents = '\n'.join([str(x.message) for x in log])
+            contents = "\n".join([str(x.message) for x in log])
             # Check that a few key elements are in the
             # warning, without wanting to check the exact
             # wording, as this can easily change.
-            self.assertTrue("already exists with a different default"
-                            in contents, 'missing "already exists"')
-            self.assertTrue("bad: b'Buzzer', should be: b'Buzz'"  # py36
-                            in contents or
-                            "bad: Buzzer, should be: Buzz"  # py27
-                            in contents,
-                            u'bad Buzzer not in contents: {}'.format(contents))
+            self.assertTrue(
+                "already exists with a different default" in contents,
+                'missing "already exists"',
+            )
+            self.assertTrue(
+                "bad: b'Buzzer', should be: b'Buzz'" in contents  # py36
+                or "bad: Buzzer, should be: Buzz" in contents,  # py27
+                f"bad Buzzer not in contents: {contents}",
+            )
 
-        out = ptr.catalogs['testing']
+        out = ptr.catalogs["testing"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in pt parsing.\nUnexpected msgid: %s' % key
+                key in output, "Failure in pt parsing.\nUnexpected msgid: %s" % key
             )
         for key in output:
-            self.assertTrue(out[key] == output[key],
-                            'Failure in pt parsing.\nGot:%s\nExpected:%s' %
-                            (out[key], output[key]))
+            self.assertTrue(
+                out[key] == output[key],
+                "Failure in pt parsing.\nGot:%s\nExpected:%s" % (out[key], output[key]),
+            )
         self.assertEqual(len(out), len(output))
 
 
 class TestMessagePYReader(unittest.TestCase):
-
     def test_read_py_no_line_numbers(self):
         me = catalog.MessageEntry
-        dirpath = os.path.join(TESTDATA_DIR, 'input')
-        filepath = os.path.join(dirpath, 'test2.py')
+        dirpath = os.path.join(TESTDATA_DIR, "input")
+        filepath = os.path.join(dirpath, "test2.py")
         input_ = dirpath
         output = {
-            u'Zero': me(u'Zero', references=[filepath]),
-            u'One': me(u'One', references=[filepath]),
-            u'msgid_three': me(u'msgid_three', msgstr='Three', references=[filepath]),  # noqa
-            u'msgid_four': me(u'msgid_four', msgstr='Four ${map}', references=[filepath]),  # noqa
-            u'msgid_five': me(u'msgid_five', msgstr=u"五番目", references=[filepath]),  # noqa
-            u'msgid_six': me(u'msgid_six', msgstr=u"\nLine 1\nLine 2\nLine 3\n", references=[filepath]),  # noqa
-            # XXX This should not be found as it's in a different domain
-            # instead it recognizes the domain as a msgstr now
-            u'Out1': me(u'Out1', msgstr='running', references=[filepath])  # noqa
+            "Zero": me("Zero", references=[filepath]),
+            "One": me("One", references=[filepath]),
+            "msgid_three": me(
+                "msgid_three", msgstr="Three", references=[filepath]
+            ),  # noqa
+            "msgid_four": me(
+                "msgid_four", msgstr="Four ${map}", references=[filepath]
+            ),  # noqa
+            "msgid_five": me("msgid_five", msgstr="五番目", references=[filepath]),  # noqa
+            "msgid_six": me(
+                "msgid_six", msgstr="\nLine 1\nLine 2\nLine 3\n", references=[filepath]
+            ),  # noqa
         }
 
-        pyr = catalog.PYReader(input_, 'testing', include_line_numbers = False)
+        pyr = catalog.PYReader(input_, "testing", include_line_numbers=False)
         pyr.read()
-        out = pyr.catalogs['testing']
+        out = pyr.catalogs["testing"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in py parsing.\nUnexpected msgid: %s' % key)
+                key in output, "Failure in py parsing.\nUnexpected msgid: %s" % key
+            )
         for key in output:
             self.assertTrue(
                 out.get(key, False),
-                'Failure in py parsing.\nMissing:%s' % output.get(key))
+                "Failure in py parsing.\nMissing:%s" % output.get(key),
+            )
             self.assertTrue(
                 out.get(key) == output.get(key),
-                'Failure in py parsing.\nGot:%s\nExpected:%s' %
-                (out.get(key), output.get(key))
+                "Failure in py parsing.\nGot:%s\nExpected:%s"
+                % (out.get(key), output.get(key)),
             )
         self.assertEqual(len(out), len(output))
 
     def test_read_py_include_line_numbers(self):
         me = catalog.MessageEntry
-        dirpath = os.path.join(TESTDATA_DIR, 'input')
-        filepath = os.path.join(dirpath, 'test2.py')
+        dirpath = os.path.join(TESTDATA_DIR, "input")
+        filepath = os.path.join(dirpath, "test2.py")
         input_ = dirpath
         output = {
-            u'Zero': me(u'Zero', references=[filepath + ':4']),
-            u'One': me(u'One', references=[filepath + ':5']),
-            u'msgid_three': me(u'msgid_three', msgstr='Three', references=[filepath + ':10']),  # noqa
-            u'msgid_four': me(u'msgid_four', msgstr='Four ${map}', references=[filepath + ':13']),  # noqa
-            u'msgid_five': me(u'msgid_five', msgstr=u"五番目", references=[filepath + ':17']),  # noqa
-            u'msgid_six': me(u'msgid_six', msgstr=u"\nLine 1\nLine 2\nLine 3\n", references=[filepath + ':19']),  # noqa
-            # XXX This should not be found as it's in a different domain
-            # instead it recognizes the domain as a msgstr now
-            u'Out1': me(u'Out1', msgstr='running', references=[filepath + ':7'])  # noqa
+            "Zero": me("Zero", references=[filepath + ":6"]),
+            "One": me("One", references=[filepath + ":7"]),
+            "msgid_three": me(
+                "msgid_three", msgstr="Three", references=[filepath + ":9"]
+            ),  # noqa
+            "msgid_four": me(
+                "msgid_four", msgstr="Four ${map}", references=[filepath + ":11"]
+            ),  # noqa
+            "msgid_five": me(
+                "msgid_five", msgstr="五番目", references=[filepath + ":13"]
+            ),  # noqa
+            "msgid_six": me(
+                "msgid_six",
+                msgstr="\nLine 1\nLine 2\nLine 3\n",
+                references=[filepath + ":15"],
+            ),  # noqa
         }
 
-        pyr = catalog.PYReader(input_, 'testing')
+        pyr = catalog.PYReader(input_, "testing")
         pyr.read()
-        out = pyr.catalogs['testing']
+        out = pyr.catalogs["testing"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in py parsing.\nUnexpected msgid: %s' % key)
+                key in output, "Failure in py parsing.\nUnexpected msgid: %s" % key
+            )
         for key in output:
             self.assertTrue(
                 out.get(key, False),
-                'Failure in py parsing.\nMissing:%s' % output.get(key))
+                "Failure in py parsing.\nMissing:%s" % output.get(key),
+            )
             self.assertTrue(
                 out.get(key) == output.get(key),
-                'Failure in py parsing.\nGot:%s\nExpected:%s' %
-                (out.get(key), output.get(key))
+                "Failure in py parsing.\nGot:%s\nExpected:%s"
+                % (out.get(key), output.get(key)),
             )
         self.assertEqual(len(out), len(output))
 
 
 class TestMessageGSReader(unittest.TestCase):
-
     def test_read_no_line_numbers(self):
         # GSReader has actually never supported line numbers.
         me = catalog.MessageEntry
-        dirpath = os.path.join(TESTDATA_DIR, 'input')
-        filepath = os.path.join(dirpath, 'test.xml')
+        dirpath = os.path.join(TESTDATA_DIR, "input")
+        filepath = os.path.join(dirpath, "test.xml")
         input_ = dirpath
         output = {
-            u'RSS feed':
-                me(u'RSS feed',
-                        references=[filepath]),
-            u'Print this':
-                me(u'Print this',
-                        references=[filepath]),
+            "RSS feed": me("RSS feed", references=[filepath]),
+            "Print this": me("Print this", references=[filepath]),
         }
 
-        reader = catalog.GSReader(input_, 'plone')
+        reader = catalog.GSReader(input_, "plone")
         reader.read()
-        out = reader.catalogs['plone']
+        out = reader.catalogs["plone"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in gs parsing.\nUnexpected msgid: %s' % key)
+                key in output, "Failure in gs parsing.\nUnexpected msgid: %s" % key
+            )
         for key in output:
             self.assertTrue(
                 out.get(key, False),
-                'Failure in gs parsing.\nMissing:%s' % output.get(key))
+                "Failure in gs parsing.\nMissing:%s" % output.get(key),
+            )
             self.assertTrue(
                 out.get(key) == output.get(key),
-                'Failure in gs parsing.\nGot:%s\nExpected:%s' %
-                (out.get(key), output.get(key))
+                "Failure in gs parsing.\nGot:%s\nExpected:%s"
+                % (out.get(key), output.get(key)),
             )
         self.assertEqual(len(out), len(output))
 
 
 class TestMessageZCMLReader(unittest.TestCase):
-
     def test_read_no_line_numbers(self):
         me = catalog.MessageEntry
-        dirpath = os.path.join(TESTDATA_DIR, 'input')
-        filepath = os.path.join(dirpath, 'test.zcml')
+        dirpath = os.path.join(TESTDATA_DIR, "input")
+        filepath = os.path.join(dirpath, "test.zcml")
         input_ = dirpath
         output = {
-            u'Plone Site':
-                me(u'Plone Site',
-                        references=[filepath]),
-            u'Profile for a default Plone.':
-                me(u'Profile for a default Plone.',
-                        references=[filepath]),
-            u'Mandatory dependencies for a Plone site':
-                me(u'Mandatory dependencies for a Plone site',
-                        references=[filepath]),
-            u'Adds title and description fields.':
-                me(u'Adds title and description fields.',
-                        references=[filepath]),
-            u'Basic metadata':
-                me(u'Basic metadata',
-                        references=[filepath]),
-            u'Content rule names should be translated.':
-                me(u'Content rule names should be translated.',
-                        references=[filepath]),
+            "Plone Site": me("Plone Site", references=[filepath]),
+            "Profile for a default Plone.": me(
+                "Profile for a default Plone.", references=[filepath]
+            ),
+            "Mandatory dependencies for a Plone site": me(
+                "Mandatory dependencies for a Plone site", references=[filepath]
+            ),
+            "Adds title and description fields.": me(
+                "Adds title and description fields.", references=[filepath]
+            ),
+            "Basic metadata": me("Basic metadata", references=[filepath]),
+            "Content rule names should be translated.": me(
+                "Content rule names should be translated.", references=[filepath]
+            ),
         }
 
-        reader = catalog.ZCMLReader(input_, 'plone', include_line_numbers = False)
+        reader = catalog.ZCMLReader(input_, "plone", include_line_numbers=False)
         reader.read()
-        out = reader.catalogs['plone']
+        out = reader.catalogs["plone"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in zcml parsing.\nUnexpected msgid: %s' % key)
+                key in output, "Failure in zcml parsing.\nUnexpected msgid: %s" % key
+            )
         for key in output:
             self.assertTrue(
                 out.get(key, False),
-                'Failure in zcml parsing.\nMissing:%s' % output.get(key))
+                "Failure in zcml parsing.\nMissing:%s" % output.get(key),
+            )
             self.assertTrue(
                 out.get(key) == output.get(key),
-                'Failure in zcml parsing.\nGot:%s\nExpected:%s' %
-                (out.get(key), output.get(key))
+                "Failure in zcml parsing.\nGot:%s\nExpected:%s"
+                % (out.get(key), output.get(key)),
             )
         self.assertEqual(len(out), len(output))
 
     def test_read_include_line_numbers(self):
         me = catalog.MessageEntry
-        dirpath = os.path.join(TESTDATA_DIR, 'input')
-        filepath = os.path.join(dirpath, 'test.zcml')
+        dirpath = os.path.join(TESTDATA_DIR, "input")
+        filepath = os.path.join(dirpath, "test.zcml")
         input_ = dirpath
         output = {
-            u'Plone Site':
-                me(u'Plone Site',
-                        references=[filepath + ':14']),
-            u'Profile for a default Plone.':
-                me(u'Profile for a default Plone.',
-                        references=[filepath + ':14']),
-            u'Mandatory dependencies for a Plone site':
-                me(u'Mandatory dependencies for a Plone site',
-                        references=[filepath + ':22']),
-            u'Adds title and description fields.':
-                me(u'Adds title and description fields.',
-                        references=[filepath + ':42']),
-            u'Basic metadata':
-                me(u'Basic metadata',
-                        references=[filepath + ':42']),
-            u'Content rule names should be translated.':
-                me(u'Content rule names should be translated.',
-                        references=[filepath + ':53']),
+            "Plone Site": me("Plone Site", references=[filepath + ":14"]),
+            "Profile for a default Plone.": me(
+                "Profile for a default Plone.", references=[filepath + ":14"]
+            ),
+            "Mandatory dependencies for a Plone site": me(
+                "Mandatory dependencies for a Plone site", references=[filepath + ":22"]
+            ),
+            "Adds title and description fields.": me(
+                "Adds title and description fields.", references=[filepath + ":42"]
+            ),
+            "Basic metadata": me("Basic metadata", references=[filepath + ":42"]),
+            "Content rule names should be translated.": me(
+                "Content rule names should be translated.",
+                references=[filepath + ":53"],
+            ),
         }
 
-        reader = catalog.ZCMLReader(input_, 'plone')
+        reader = catalog.ZCMLReader(input_, "plone")
         reader.read()
-        out = reader.catalogs['plone']
+        out = reader.catalogs["plone"]
         for key in out:
             self.assertTrue(
-                key in output,
-                'Failure in zcml parsing.\nUnexpected msgid: %s' % key)
+                key in output, "Failure in zcml parsing.\nUnexpected msgid: %s" % key
+            )
         for key in output:
             self.assertTrue(
                 out.get(key, False),
-                'Failure in zcml parsing.\nMissing:%s' % output.get(key))
+                "Failure in zcml parsing.\nMissing:%s" % output.get(key),
+            )
             self.assertTrue(
                 out.get(key) == output.get(key),
-                'Failure in zcml parsing.\nGot:%s\nExpected:%s' %
-                (out.get(key), output.get(key))
+                "Failure in zcml parsing.\nGot:%s\nExpected:%s"
+                % (out.get(key), output.get(key)),
             )
         self.assertEqual(len(out), len(output))
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(TestGlobal))
-    suite.addTest(unittest.makeSuite(TestMessageEntry))
-    suite.addTest(unittest.makeSuite(TestMessageCatalogInit))
-    suite.addTest(unittest.makeSuite(TestMessageCatalog))
-    suite.addTest(unittest.makeSuite(TestMessageCatalogSync))
-    suite.addTest(unittest.makeSuite(TestMessagePoWriter))
-    suite.addTest(unittest.makeSuite(TestMessagePTReader))
-    suite.addTest(unittest.makeSuite(TestMessagePYReader))
-    suite.addTest(unittest.makeSuite(TestMessageGSReader))
-    suite.addTest(unittest.makeSuite(TestMessageZCMLReader))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestGlobal))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageEntry))
+    suite.addTest(
+        unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageCatalogInit)
+    )
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageCatalog))
+    suite.addTest(
+        unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageCatalogSync)
+    )
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessagePoWriter))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessagePTReader))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessagePYReader))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageGSReader))
+    suite.addTest(
+        unittest.defaultTestLoader.loadTestsFromTestCase(TestMessageZCMLReader)
+    )
     return suite
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/tests/test_untranslated.py` & `i18ndude-6.1.0/src/i18ndude/tests/test_untranslated.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,198 +1,190 @@
 """Tests for finding untranslated prose.
 """
+from argparse import Namespace
+from i18ndude.script import find_untranslated as script
+from i18ndude.tests.utils import suppress_stdout
+from i18ndude.tests.utils import TESTDATA_DIR
+
+import i18ndude.untranslated
+import io
 import os
 import sys
 import unittest
 import xml.sax
-import io
-import i18ndude.untranslated
-from argparse import Namespace
-from i18ndude.script import find_untranslated as script
-from i18ndude.tests.utils import suppress_stdout, TESTDATA_DIR
-
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
-    unicode_StringIO = io.StringIO
-else:
-    import StringIO
-    # io.StringIO in python2 (but not in python3) raises:
-    # TypeError: unicode argument expected, got 'str'
-    unicode_StringIO = StringIO.StringIO
 
 
 def find_untranslated(input):
-    out = unicode_StringIO()
-    parser = xml.sax.make_parser(['expat'])
+    out = io.StringIO()
+    parser = xml.sax.make_parser(["expat"])
     handler = i18ndude.untranslated.VerboseHandler(parser, out)
     parser.setContentHandler(handler)
-    parser.parse(unicode_StringIO(input))
+    parser.parse(io.StringIO(input))
     return out.getvalue()
 
 
 class TestUntranslated(unittest.TestCase):
-
     def test_untranslated_content(self):
         """
         find-untranslated can find strings missing the i18n:translate marker
         and it will show an error.
         """
-        result_with_errors = find_untranslated('<div><p>foo</p></div>')
-        self.assertIn(
-            'i18n:translate missing for this:\n"""\nfoo\n"""',
-            result_with_errors)
+        result_with_errors = find_untranslated("<div><p>foo</p></div>")
         self.assertIn(
-            '(0 warnings, 1 errors)',
-            result_with_errors)
+            'i18n:translate missing for this:\n"""\nfoo\n"""', result_with_errors
+        )
+        self.assertIn("(0 warnings, 1 errors)", result_with_errors)
 
     def test_untranslated(self):
         """
         find-untranslated finds no error if the i18n:translate marker is set.
         """
         result_without_errors = find_untranslated(
-            '<div><p i18n:translate="">foo</p></div>')
-        self.assertNotIn(
-            'i18n:translate missing',
-            result_without_errors)
-        self.assertIn('(0 warnings, 0 errors)', result_without_errors)
+            '<div><p i18n:translate="">foo</p></div>'
+        )
+        self.assertNotIn("i18n:translate missing", result_without_errors)
+        self.assertIn("(0 warnings, 0 errors)", result_without_errors)
 
     def test_ignore_untranslated_with_marker(self):
         """
         Adding the i18n:ignore marker will skip untranslated strings.
         """
-        result_with_marker = find_untranslated(
-            '<div><p i18n:ignore="">foo</p></div>')
-        self.assertIn('(0 warnings, 0 errors)', result_with_marker)
+        result_with_marker = find_untranslated('<div><p i18n:ignore="">foo</p></div>')
+        self.assertIn("(0 warnings, 0 errors)", result_with_marker)
 
     def test_ignore_untranslated_attribute(self):
         """
         Attributes missing the i18n:attributes marker will cause
         find-untranslated to show an error.
 
         Attributes marked with i18n:ignore-attributes will cause
         find-untranslated to not show an error.
         """
         result_without_attributes = find_untranslated(
-            '<div><a title="bar" i18n:translate="">spam</a></div>')
+            '<div><a title="bar" i18n:translate="">spam</a></div>'
+        )
         self.assertIn(
-            'title attribute of <a> lacks i18n:attributes',
-            result_without_attributes)
-        self.assertIn('(0 warnings, 1 errors)', result_without_attributes)
+            "title attribute of <a> lacks i18n:attributes", result_without_attributes
+        )
+        self.assertIn("(0 warnings, 1 errors)", result_without_attributes)
 
         result_with_ignore_attributes = find_untranslated(
-            '''<div><a title="bar"
+            """<div><a title="bar"
                 i18n:ignore-attributes="title"
                 i18n:translate=""
-                >spam</a></div>''')
-        self.assertIn('(0 warnings, 0 errors)', result_with_ignore_attributes)
+                >spam</a></div>"""
+        )
+        self.assertIn("(0 warnings, 0 errors)", result_with_ignore_attributes)
 
     def test_ignore_untranslated_attribute_complain_about_other_attrs(self):
         """
         find-untranslated will find an error if not all attributes are marked
         to be ignored.
         """
         result_without_attributes = find_untranslated(
-            '''<div><img title="bar" alt="qux"
-            i18n:ignore-attributes="title"/></div>''')
-        self.assertIn(
-            'alt attribute of <img> lacks i18n:attributes',
-            result_without_attributes)
-        self.assertIn('(0 warnings, 1 errors)', result_without_attributes)
+            """<div><img title="bar" alt="qux"
+            i18n:ignore-attributes="title"/></div>"""
+        )
+        self.assertIn(
+            "alt attribute of <img> lacks i18n:attributes", result_without_attributes
+        )
+        self.assertIn("(0 warnings, 1 errors)", result_without_attributes)
 
     def test_ignore_untranslated_attribute_multiple_attrs(self):
         """
         find-untranslated finds no error if multiple attributes are marked
         to be ignored.
         """
         result_with_multiple_ignore_attributes = find_untranslated(
-            '''<div><img title="bar" alt="qux"
-            i18n:ignore-attributes="title;alt"/></div>''')
-        self.assertIn('(0 warnings, 0 errors)',
-                      result_with_multiple_ignore_attributes)
+            """<div><img title="bar" alt="qux"
+            i18n:ignore-attributes="title;alt"/></div>"""
+        )
+        self.assertIn("(0 warnings, 0 errors)", result_with_multiple_ignore_attributes)
 
     def test_find_untranslated_placeholder_attribute(self):
         result_with_untranslated_placeholder = find_untranslated(
-            '<div><input type="text" placeholder="search for bar"/></div>')
+            '<div><input type="text" placeholder="search for bar"/></div>'
+        )
         self.assertIn(
-            'placeholder attribute of <input> lacks i18n:attributes',
-            result_with_untranslated_placeholder)
+            "placeholder attribute of <input> lacks i18n:attributes",
+            result_with_untranslated_placeholder,
+        )
 
     def test_ignore_translated_placeholder_attribute(self):
         result_with_translated_placeholder = find_untranslated(
-            '<div><input type="text" i18n:attributes="placeholder" placeholder="search for bar"/></div>')
+            '<div><input type="text" i18n:attributes="placeholder" placeholder="search for bar"/></div>'
+        )
         self.assertNotIn(
-            'placeholder attribute of <input> lacks i18n:attributes',
-            result_with_translated_placeholder)
+            "placeholder attribute of <input> lacks i18n:attributes",
+            result_with_translated_placeholder,
+        )
 
     def test_find_untranslated_aria_label_attribute(self):
         result_with_untranslated_aria_label = find_untranslated(
-            '<div><button aria-label="cookies"/></div>')
+            '<div><button aria-label="cookies"/></div>'
+        )
         self.assertIn(
-            'aria-label attribute of <button> lacks i18n:attributes',
-            result_with_untranslated_aria_label)
+            "aria-label attribute of <button> lacks i18n:attributes",
+            result_with_untranslated_aria_label,
+        )
 
         result_with_translated_aria_label = find_untranslated(
-            '<div><button aria-label="cookies" i18n:attributes="aria-label"/></div>')
-        self.assertNotIn(
-            'lacks i18n:attributes',
-            result_with_translated_aria_label)
+            '<div><button aria-label="cookies" i18n:attributes="aria-label"/></div>'
+        )
+        self.assertNotIn("lacks i18n:attributes", result_with_translated_aria_label)
 
     def test_find_untranslated_disallows_nonword_chars_in_i18n_name(self):
-        error = 'invalid non-word characters (space, punctuation) in i18n:name'
+        error = "invalid non-word characters (space, punctuation) in i18n:name"
         result_with_space_in_name = find_untranslated(
-            '<div i18n:translate="">Something <span i18n:name="xfoo xbar">amiss</span></div>')
+            '<div i18n:translate="">Something <span i18n:name="xfoo xbar">amiss</span></div>'
+        )
         self.assertIn(error, result_with_space_in_name)
-        self.assertIn('1 errors', result_with_space_in_name)
+        self.assertIn("1 errors", result_with_space_in_name)
         result_with_slash_in_name = find_untranslated(
-            '<div i18n:translate="">Something <span i18n:name="xfoo/xbar">amiss</span></div>')
+            '<div i18n:translate="">Something <span i18n:name="xfoo/xbar">amiss</span></div>'
+        )
         self.assertIn(error, result_with_slash_in_name)
-        self.assertIn('1 errors', result_with_slash_in_name)
+        self.assertIn("1 errors", result_with_slash_in_name)
         result_with_dash_in_name = find_untranslated(
-            '<div i18n:translate="">Something <span i18n:name="x_foo-x_bar">amiss</span></div>')
+            '<div i18n:translate="">Something <span i18n:name="x_foo-x_bar">amiss</span></div>'
+        )
         self.assertNotIn(error, result_with_dash_in_name)
-        self.assertIn('0 errors', result_with_dash_in_name)
+        self.assertIn("0 errors", result_with_dash_in_name)
 
 
 class TestUntranslatedScript(unittest.TestCase):
-
     def test_script_template_1(self):
-        path = os.path.join(TESTDATA_DIR, 'input', 'test1.pt')
+        path = os.path.join(TESTDATA_DIR, "input", "test1.pt")
         with suppress_stdout():
-            result = script(Namespace(
-                silent=False, nosummary=False, files=[path]))
+            result = script(Namespace(silent=False, nosummary=False, files=[path]))
         self.assertEqual(result, 0)
 
     def test_script_template_3(self):
-        path = os.path.join(TESTDATA_DIR, 'input', 'test3.pt')
+        path = os.path.join(TESTDATA_DIR, "input", "test3.pt")
         with suppress_stdout():
-            result = script(Namespace(
-                silent=False, nosummary=False, files=[path]))
+            result = script(Namespace(silent=False, nosummary=False, files=[path]))
         self.assertEqual(result, 1)
 
     def test_script_template_4(self):
-        path = os.path.join(TESTDATA_DIR, 'input', 'test4.pt')
-        output = unicode_StringIO()
+        path = os.path.join(TESTDATA_DIR, "input", "test4.pt")
+        output = io.StringIO()
         old_stdout = sys.stdout
         sys.stdout = output
         try:
-            result = script(Namespace(
-                silent=False, nosummary=False, files=[path]))
+            result = script(Namespace(silent=False, nosummary=False, files=[path]))
         finally:
             sys.stdout = old_stdout
         self.assertEqual(result, 1)
         # A specific line should be reported as missing an i18n.
-        self.assertIn('{}:16'.format(path), output.getvalue())
+        self.assertIn(f"{path}:16", output.getvalue())
 
     def test_script_chameleon(self):
-        path = os.path.join(TESTDATA_DIR, 'input', 'chameleon.pt')
+        path = os.path.join(TESTDATA_DIR, "input", "chameleon.pt")
         with suppress_stdout():
-            result = script(Namespace(
-                silent=False, nosummary=False, files=[path]))
+            result = script(Namespace(silent=False, nosummary=False, files=[path]))
         self.assertEqual(result, 0)
 
     def test_script_directory(self):
-        path = os.path.join(TESTDATA_DIR, 'input')
+        path = os.path.join(TESTDATA_DIR, "input")
         with suppress_stdout():
-            result = script(Namespace(
-                silent=False, nosummary=False, files=[path]))
+            result = script(Namespace(silent=False, nosummary=False, files=[path]))
         self.assertEqual(result, 2)
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/tests/test_utils.py` & `i18ndude-6.1.0/src/i18ndude/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
+from i18ndude.utils import undouble_unicode_escape
 from i18ndude.utils import wrapAndQuoteString
 from i18ndude.utils import wrapString
-from i18ndude.utils import undouble_unicode_escape
+
 import i18ndude.utils
 import unittest
 
 
 class TestUtils(unittest.TestCase):
-
     def setUp(self):
         self.original_max_width = i18ndude.utils.MAX_WIDTH
         self.original_wrap = i18ndude.utils.WRAP
 
         # Enable wrapping.
         i18ndude.utils.WRAP = True
 
@@ -19,132 +18,130 @@
         i18ndude.utils.MAX_WIDTH = self.original_max_width
         i18ndude.utils.WRAP = self.original_wrap
 
     def test_wrapString_no_wrapping(self):
         # Disable wrapping.
         i18ndude.utils.WRAP = False
 
-        line = 'a' * 50 + ' ' + 'b' * 50
-        self.assertEqual(wrapString(line),
-                         ['a' * 50 + ' ' + 'b' * 50])
+        line = "a" * 50 + " " + "b" * 50
+        self.assertEqual(wrapString(line), ["a" * 50 + " " + "b" * 50])
 
     def test_wrapString_wrapping_single_line(self):
         # Enable wrapping.
         i18ndude.utils.WRAP = True
 
         # This all fits on one line.
-        self.assertEqual(wrapString(''), [''])
-        self.assertEqual(wrapString('a'), ['a'])
-        self.assertEqual(wrapString('a b'), ['a b'])
+        self.assertEqual(wrapString(""), [""])
+        self.assertEqual(wrapString("a"), ["a"])
+        self.assertEqual(wrapString("a b"), ["a b"])
 
     def test_wrapString_wrapping_first_line_edge_case(self):
         """Lines that are just a bit shorter than MAX_WIDTH are still longer
         at the end, as the line also contains the 'msgstr '.
         This test makes sure that this edge case is taken care of
         """
-        msgstr_length = len('msgstr ')
+        msgstr_length = len("msgstr ")
         # the maximum amount of characters on the first line should be:
         max_line_length = i18ndude.utils.MAX_WIDTH - msgstr_length - 2
 
-        line = 'a' * max_line_length
+        line = "a" * max_line_length
         self.assertEqual(wrapString(line), [line])
 
         # but only one character more would make it split into two lines
-        line += 'a'
-        self.assertEqual(wrapString(line), ['', line])
+        line += "a"
+        self.assertEqual(wrapString(line), ["", line])
 
     def test_wrapString_wrapping_multiline(self):
         # This does not fit on a single line.
-        line = 'a' * 20 + ' ' + 'b' * 50 + ' ' + 'c' * 20 + ' ' + 'd' * 50
-        self.assertEqual(wrapString(line),
-                         ['',
-                          'a' * 20 + ' ' + 'b' * 50 + ' ',
-                          'c' * 20 + ' ' + 'd' * 50])
+        line = "a" * 20 + " " + "b" * 50 + " " + "c" * 20 + " " + "d" * 50
+        self.assertEqual(
+            wrapString(line),
+            ["", "a" * 20 + " " + "b" * 50 + " ", "c" * 20 + " " + "d" * 50],
+        )
 
     def test_wrapString_wrapping_long_words(self):
         # What happens when some words are really too long?
-        A = 'a' * 99
-        B = 'b' * 99
-        C = 'c' * 99
-        self.assertEqual(wrapString(A), ['', A])
-        line = ' '.join((A, B))
-        self.assertEqual(wrapString(line), ['', A + ' ', B])
-        line = ' '.join((A, B, C))
-        self.assertEqual(wrapString(line), ['', A + ' ', B + ' ', C])
+        A = "a" * 99
+        B = "b" * 99
+        C = "c" * 99
+        self.assertEqual(wrapString(A), ["", A])
+        line = " ".join((A, B))
+        self.assertEqual(wrapString(line), ["", A + " ", B])
+        line = " ".join((A, B, C))
+        self.assertEqual(wrapString(line), ["", A + " ", B + " ", C])
 
         # Accept a line of 12: 3 characters plus 2 quotes (and 'msgstr ').
         i18ndude.utils.MAX_WIDTH = 12
-        self.assertEqual(wrapString('aaa'), ['aaa'])
-        self.assertEqual(wrapString('aaaa'), ['', 'aaaa'])
-        self.assertEqual(wrapString('aaa' + ' ' + 'a' * 12),
-                         ['', 'aaa ', 'a' * 12])
+        self.assertEqual(wrapString("aaa"), ["aaa"])
+        self.assertEqual(wrapString("aaaa"), ["", "aaaa"])
+        self.assertEqual(wrapString("aaa" + " " + "a" * 12), ["", "aaa ", "a" * 12])
 
         # If this is 2 or less, we do not wrap lines.
         i18ndude.utils.MAX_WIDTH = 2
-        self.assertEqual(wrapString('aaa aaaaa'), ['aaa aaaaa'])
+        self.assertEqual(wrapString("aaa aaaaa"), ["aaa aaaaa"])
 
     def test_wrapAndQuoteString(self):
-        self.assertEqual(wrapAndQuoteString(''), '""')
-        lineA = 'a' * 50
-        self.assertEqual(wrapAndQuoteString(lineA), '"{0}"'.format(lineA))
-        lineB = 'b' * 50
-        lineAB = lineA + ' ' + lineB
-        self.assertEqual(wrapAndQuoteString(lineAB),
-                         '"{0} "\n"{1}"'.format(lineA, lineB))
+        self.assertEqual(wrapAndQuoteString(""), '""')
+        lineA = "a" * 50
+        self.assertEqual(wrapAndQuoteString(lineA), f'"{lineA}"')
+        lineB = "b" * 50
+        lineAB = lineA + " " + lineB
+        self.assertEqual(wrapAndQuoteString(lineAB), f'"{lineA} "\n"{lineB}"')
 
     def test_wrapAndQuoteString_singleline_unicode(self):
         # disable wrapping
         i18ndude.utils.WRAP = False
-        val = u'ø' * 100
+        val = "ø" * 100
         try:
             wrapAndQuoteString(val)
         except UnicodeEncodeError:
-            self.fail("wrapAndQuoteString raised UnicodeEncodeError unexpectedly!")  # noqa
+            self.fail(
+                "wrapAndQuoteString raised UnicodeEncodeError unexpectedly!"
+            )  # noqa
 
 
 class TestUndoubleEscape(unittest.TestCase):
-
     def test_roundtrip_string(self):
-        self.assertEqual(undouble_unicode_escape('foo'), 'foo')
+        self.assertEqual(undouble_unicode_escape("foo"), "foo")
 
     def test_roundtrip_simple_unicode(self):
-        self.assertEqual(undouble_unicode_escape(u'foo'), u'foo')
+        self.assertEqual(undouble_unicode_escape("foo"), "foo")
 
     def test_roundtrip_complex_unicode(self):
-        goodname = u'Kılıçaslan'
+        goodname = "Kılıçaslan"
         self.assertEqual(undouble_unicode_escape(goodname), goodname)
 
     def test_encoded(self):
-        garbled = u'K\u0131l\u0131\xe7aslan'
-        goodname = u'Kılıçaslan'
+        garbled = "K\u0131l\u0131\xe7aslan"
+        goodname = "Kılıçaslan"
         self.assertEqual(undouble_unicode_escape(garbled), goodname)
 
     def test_double_encoded(self):
-        garbled = u'K\xc4\xb1l\xc4\xb1\xc3\xa7aslan'
-        goodname = u'Kılıçaslan'
+        garbled = "K\xc4\xb1l\xc4\xb1\xc3\xa7aslan"
+        goodname = "Kılıçaslan"
         self.assertEqual(undouble_unicode_escape(garbled), goodname)
 
     def test_triple_encoded(self):
-        garbled = 'K\xc3\x84\xc2\xb1l\xc3\x84\xc2\xb1\xc3\x83\xc2\xa7aslan'
-        goodname = u'Kılıçaslan'
+        garbled = "K\xc3\x84\xc2\xb1l\xc3\x84\xc2\xb1\xc3\x83\xc2\xa7aslan"
+        goodname = "Kılıçaslan"
         self.assertEqual(undouble_unicode_escape(garbled), goodname)
 
     def test_object(self):
         NO_VALUE = object()
         self.assertEqual(undouble_unicode_escape(NO_VALUE), NO_VALUE)
 
     def test_encoded_escaped_kili(self):
-        garbled = 'K\\u0131l\\u0131\xe7aslan'  # actually: bytes
-        goodname = u'Kılıçaslan'
+        garbled = "K\\u0131l\\u0131\xe7aslan"  # actually: bytes
+        goodname = "Kılıçaslan"
         self.assertEqual(undouble_unicode_escape(garbled), goodname)
 
     def test_encoded_escaped_seen_in_wild(self):
         garbled = 'msgstr "Polo\\u017eka ${title} byla odstran\\u011bna."'
-        goodname = u'msgstr "Položka ${title} byla odstraněna."'
+        goodname = 'msgstr "Položka ${title} byla odstraněna."'
         self.assertEqual(undouble_unicode_escape(garbled), goodname)
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    suite.addTest(unittest.makeSuite(TestUtils))
-    suite.addTest(unittest.makeSuite(TestUndoubleEscape))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestUtils))
+    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(TestUndoubleEscape))
     return suite
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/tests/tox-check-i18ndude-command.sh` & `i18ndude-6.1.0/src/i18ndude/tests/tox-check-i18ndude-command.sh`

 * *Files identical despite different names*

### Comparing `i18ndude-6.0.0a1/src/i18ndude/tests/utils.py` & `i18ndude-6.1.0/src/i18ndude/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from contextlib import contextmanager
+
 import os
 import sys
-from contextlib import contextmanager
 
 
 def package_home(globals_dict):
-    __name__ = globals_dict['__name__']
+    __name__ = globals_dict["__name__"]
     m = sys.modules[__name__]
-    if hasattr(m, '__path__'):
+    if hasattr(m, "__path__"):
         r = m.__path__[0]
     elif "." in __name__:
-        r = sys.modules[__name__[:__name__.rfind('.')]].__path__[0]
+        r = sys.modules[__name__[: __name__.rfind(".")]].__path__[0]
     else:
         r = __name__
     return os.path.abspath(r)
 
+
 GLOBALS = globals()
 PACKAGE_HOME = os.path.dirname(package_home(GLOBALS))
 
-TESTDATA_DIR = os.path.join(PACKAGE_HOME, 'testdata')
+TESTDATA_DIR = os.path.join(PACKAGE_HOME, "testdata")
 
 
 @contextmanager
 def suppress_stdout():
     # Taken with thanks from Dave Smith's site:
     # https://thesmithfam.org/blog/2012/10/25/
     with open(os.devnull, "w") as devnull:
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/untranslated.py` & `i18ndude-6.1.0/src/i18ndude/untranslated.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import io
-import xml.sax
 import re
+import xml.sax
+
 
-import sys
-PY3 = sys.version_info > (3,)
-if PY3:
-    unicode = str
-
-IGNORE_UNTRANSLATED = 'i18n:ignore'
-IGNORE_UNTRANSLATED_ATTRIBUTES = 'i18n:ignore-attributes'
-CHAMELEON_SUBST = re.compile(r'^\${.*}$')
-NOT_ALLOWED_IN_NAME = re.compile(r'[^\w-]')
+IGNORE_UNTRANSLATED = "i18n:ignore"
+IGNORE_UNTRANSLATED_ATTRIBUTES = "i18n:ignore-attributes"
+CHAMELEON_SUBST = re.compile(r"^\${.*}$")
+NOT_ALLOWED_IN_NAME = re.compile(r"[^\w-]")
 
 
 def _translatable(data):
     """Returns 1 for strings that contain alphanumeric characters."""
 
     for ch in data:
         if ch.isalpha():
@@ -34,58 +30,61 @@
     # <tal:block tal:condition...
     # All of those should result in tal:condition as attribute key.
     # And since the lxml html parser strips off the tal namespace from tags, we
     # should also support:
     # <block condition...
 
     # So lets simplify the keys.
-    keys = set([key[key.find(':') + 1:] for key in keys])
+    keys = {key[key.find(":") + 1 :] for key in keys}
 
-    if 'use-macro' in keys:
+    if "use-macro" in keys:
         # metal
-        return ''
+        return ""
 
     # comments
-    if 'condition' in keys:
-        cond_val = attrs.get('tal:condition', attrs.get('condition', None))
-        if cond_val == 'nothing':
-            return ''
-        return 'ERROR'
+    if "condition" in keys:
+        cond_val = attrs.get("tal:condition", attrs.get("condition", None))
+        if cond_val == "nothing":
+            return ""
+        return "ERROR"
 
-    elif 'replace' in keys or 'content' in keys:
-        return 'WARNING'
+    elif "replace" in keys or "content" in keys:
+        return "WARNING"
 
-    return 'ERROR'
+    return "ERROR"
 
 
 def _tal_replaced_content(tag, attrs):
     """Will the data get replaced by tal?
 
     So: is there a tal:content or tal:replace?  Or is it '<tal:block
     content=.".."'?  Problem with that last one is that the lxml html
     parser strips off the 'tal:' namespace, unlike the standard lxml
     parser that is tried first.
     """
-    if 'tal:content' in attrs or 'content' in attrs:
+    if "tal:content" in attrs or "content" in attrs:
         return True
-    if 'tal:replace' in attrs or 'replace' in attrs:
+    if "tal:replace" in attrs or "replace" in attrs:
         return True
     return False
 
 
 def _tal_replaced_attr(attrs, attr):
     # Is the attribute replaced by tal?
-    if 'tal:attributes' not in attrs and 'attributes' not in attrs:
+    if "tal:attributes" not in attrs and "attributes" not in attrs:
         # Not replaced by tal, but could be chameleon syntax.
-        value = attrs.get(attr, '')
+        value = attrs.get(attr, "")
         if CHAMELEON_SUBST.match(value):
             return True
         return False
-    talattrs = [talattr.strip().split()[0] for talattr in
-                attrs['tal:attributes'].split(';') if talattr]
+    talattrs = [
+        talattr.strip().split()[0]
+        for talattr in attrs["tal:attributes"].split(";")
+        if talattr
+    ]
     if attr in talattrs:
         return True
     return False
 
 
 def _valid_i18ned_attr(attr, attrs):
     """This returns 1 for attributes attr that are part of attrs and are
@@ -93,25 +92,29 @@
     not exist at all in attrs.
 
     When the attr gets replaced by tal, all is fine so we return 1 as well.
     """
 
     if attr in attrs and _translatable(attrs[attr]):
         if IGNORE_UNTRANSLATED_ATTRIBUTES in attrs:
-            if attr in attrs[IGNORE_UNTRANSLATED_ATTRIBUTES].split(';'):
+            if attr in attrs[IGNORE_UNTRANSLATED_ATTRIBUTES].split(";"):
                 return 1
-        if 'i18n:attributes' in attrs:
+        if "i18n:attributes" in attrs:
             # First check old syntax, or the simple case of one single
             # i18n:attribute.
-            if attrs['i18n:attributes'].find(';') == -1:
-                i18nattrs = [i18nattr.strip() for i18nattr in
-                             attrs['i18n:attributes'].split()]
+            if attrs["i18n:attributes"].find(";") == -1:
+                i18nattrs = [
+                    i18nattr.strip() for i18nattr in attrs["i18n:attributes"].split()
+                ]
             else:  # new syntax
-                i18nattrs = [i18nattr.strip().split()[0] for i18nattr in
-                             attrs['i18n:attributes'].split(';') if i18nattr]
+                i18nattrs = [
+                    i18nattr.strip().split()[0]
+                    for i18nattr in attrs["i18n:attributes"].split(";")
+                    if i18nattr
+                ]
             if attr in i18nattrs:
                 return 1
             if _tal_replaced_attr(attrs, attr):
                 return 1
             return 0
         else:
             if _tal_replaced_attr(attrs, attr):
@@ -126,177 +129,198 @@
     if
        1) Each tag that has a title attribute has it i18ned.
        2) Each image tag has its alt attribute i18ned.
        3) Each tag that is a <input type="submit *or* button"> has its value
           i18ned.
     """
 
-    if not _valid_i18ned_attr('title', attrs):
-        logfct('title attribute of <%s> lacks i18n:attributes' % tag,
-               'ERROR')
-
-    if not _valid_i18ned_attr('aria-label', attrs):
-        logfct('aria-label attribute of <%s> lacks i18n:attributes' % tag,
-               'ERROR')
-
-    if tag == 'img':
-        if not _valid_i18ned_attr('alt', attrs):
-            logfct('alt attribute of <img> lacks i18n:attributes',
-                   'ERROR')
-
-    if tag == 'input' and \
-              'type' in attrs.keys() and \
-              attrs['type'] in ('submit', 'button'):
-        if not _valid_i18ned_attr('value', attrs):
-            logfct('value attribute of <... submit/button> lacks '
-                   'i18n:attribute', 'ERROR')
-
-    if tag == 'input' and 'placeholder' in attrs.keys():
-        if not _valid_i18ned_attr('placeholder', attrs):
-            logfct('placeholder attribute of <%s> lacks i18n:attributes' % tag,
-                   'ERROR')
+    if not _valid_i18ned_attr("title", attrs):
+        logfct("title attribute of <%s> lacks i18n:attributes" % tag, "ERROR")
+
+    if not _valid_i18ned_attr("aria-label", attrs):
+        logfct("aria-label attribute of <%s> lacks i18n:attributes" % tag, "ERROR")
+
+    if tag == "img":
+        if not _valid_i18ned_attr("alt", attrs):
+            logfct("alt attribute of <img> lacks i18n:attributes", "ERROR")
+
+    if (
+        tag == "input"
+        and "type" in attrs.keys()
+        and attrs["type"] in ("submit", "button")
+    ):
+        if not _valid_i18ned_attr("value", attrs):
+            logfct(
+                "value attribute of <... submit/button> lacks " "i18n:attributes",
+                "ERROR",
+            )
+
+    if tag == "input" and "placeholder" in attrs.keys():
+        if not _valid_i18ned_attr("placeholder", attrs):
+            logfct("placeholder attribute of <%s> lacks i18n:attributes" % tag, "ERROR")
 
-    name = attrs.get('i18n:name')
+    name = attrs.get("i18n:name")
     if name and NOT_ALLOWED_IN_NAME.search(name):
-        logfct('invalid non-word characters (space, punctuation) '
-               'in i18n:name="{}"'.format(name), 'ERROR')
+        logfct(
+            "invalid non-word characters (space, punctuation) "
+            'in i18n:name="{}"'.format(name),
+            "ERROR",
+        )
 
 
 class Handler(xml.sax.ContentHandler):
-
     def __init__(self, parser, out=None):
         self._parser = parser
         if out is None:
             self._out = io.StringIO()
         else:
             self._out = out
-        self._filename = 'Undefined'
+        self._filename = "Undefined"
 
     def show_output(self):
         value = self._out.getvalue().strip()
         if value:
-            if not isinstance(value, unicode):
-                value = value.decode('utf-8')
+            if not isinstance(value, str):
+                value = value.decode("utf-8")
             # Note: if value contains non-ascii and we redirect stdout
             # or pipe the output through 'grep', we get a UnicodeEncodeError.
             # Solution: export PYTHONIOENCODING=utf-8
             # See https://stackoverflow.com/questions/492483
-            print(value + u'\n')
+            print(value + "\n")
 
     def clear_output(self):
         self._out = io.StringIO()
 
     def log(self, msg, severity):
         """Severity may be one out of 'WARNING', 'ERROR' or 'FATAL'."""
-        assert(severity in self._stats.keys())
+        assert severity in self._stats.keys()
         self._stats[severity] += 1
 
     def has_errors(self):
-        return self._stats['ERROR'] or self._stats['FATAL']
+        return self._stats["ERROR"] or self._stats["FATAL"]
 
     def set_filename(self, filename):
         self._filename = filename
 
     def startDocument(self):
-        self._history = []  # history contains 3-tuples in the form
+        # history contains 3-tuples in the form
         # (tag, attrs, characterdata)
-        self._i18nlevel = 0  # 0 means not inside i18n:translate area
-        self._stats = {'WARNING': 0, 'ERROR': 0, 'FATAL': 0}
+        self._history = []
+        # 0 means not inside i18n:translate area
+        self._i18nlevel = 0
+        # When you add i18n:ignore on a tag, then all untranslated messages on this
+        # or enclosed tags are ignored.
+        self._ignore_untranslated = False
+        self._stats = {"WARNING": 0, "ERROR": 0, "FATAL": 0}
 
     def endDocument(self):
         pass
 
     def startElement(self, tag, attrs):
-        self._history.append([tag, attrs, ''])
-
-        attr_validator(tag, attrs, self.log)
+        self._history.append([tag, attrs, ""])
 
-        if 'i18n:translate' in attrs.keys():
+        if "i18n:translate" in attrs.keys():
             self._i18nlevel += 1
         elif self._i18nlevel != 0:
             self._i18nlevel += 1
+        if IGNORE_UNTRANSLATED in attrs:
+            self._ignore_untranslated = True
+        if not self._ignore_untranslated:
+            attr_validator(tag, attrs, self.log)
 
     def endElement(self, tag):
         tag, attrs, data = self._history.pop()
         data = data.strip()
 
-        if _translatable(data) and not _tal_replaced_content(tag, attrs):
-            # not enclosed
-            if (self._i18nlevel == 0) and tag not in [
-                    'script', 'style', 'html']:
-                severity = _severity(tag, attrs) or ''
-                if severity:
-                    if IGNORE_UNTRANSLATED in attrs.keys():
-                        # Ignore untranslated data. This is necessary for
-                        # including literal content, that does not need to be
-                        # translated.
-                        pass
-                    elif not CHAMELEON_SUBST.match(data):
-                        self.log(
-                            'i18n:translate missing for this:\n'
-                            '"""\n%s\n"""' % (data,), severity)
+        if (
+            not self._ignore_untranslated
+            and _translatable(data)
+            and not _tal_replaced_content(tag, attrs)
+            and (self._i18nlevel == 0)
+            and tag not in ["script", "style", "html"]
+        ):
+            severity = _severity(tag, attrs) or ""
+            if severity and not CHAMELEON_SUBST.match(data):
+                self.log(
+                    "i18n:translate missing for this:\n" '"""\n%s\n"""' % (data,),
+                    severity,
+                )
 
         if self._i18nlevel != 0:
             self._i18nlevel -= 1
+        if IGNORE_UNTRANSLATED in attrs:
+            # reset
+            self._ignore_untranslated = False
 
     def characters(self, data):
         self._history[-1][2] += data
 
 
 class SilentHandler(Handler):
-
     def log(self, msg, severity):
         Handler.log(self, msg, severity)
 
-        if severity == 'FATAL':
-            self._out.write('Fatal error in document %s' % self._filename)
-            self._out.write('\n')
+        if severity == "FATAL":
+            self._out.write("Fatal error in document %s" % self._filename)
+            self._out.write("\n")
 
     def endDocument(self):
-        if not (self._stats['WARNING'] or self._stats['ERROR']):
+        if not (self._stats["WARNING"] or self._stats["ERROR"]):
             return
 
-        self._out.write('%s: %s warnings, %s errors'
-                        % (self._filename, self._stats['WARNING'],
-                           self._stats['ERROR']))
+        self._out.write(
+            "%s: %s warnings, %s errors"
+            % (self._filename, self._stats["WARNING"], self._stats["ERROR"])
+        )
 
 
 class VerboseHandler(Handler):
-
     def log(self, msg, severity):
         Handler.log(self, msg, severity)
 
-        self._out.write(unicode('%s:%s:%s:\n-%s- - %s\n' % (
-            self._filename,
-            self._parser.getLineNumber(),
-            self._parser.getColumnNumber(),
-            severity,
-            msg)))
+        self._out.write(
+            str(
+                "{}:{}:{}:\n-{}- - {}\n".format(
+                    self._filename,
+                    self._parser.getLineNumber(),
+                    self._parser.getColumnNumber(),
+                    severity,
+                    msg,
+                )
+            )
+        )
 
-        if severity == 'FATAL':
-            char = '='
+        if severity == "FATAL":
+            char = "="
         else:
-            char = '-'
-        self._out.write(unicode(char * 79) + '\n')
+            char = "-"
+        self._out.write(str(char * 79) + "\n")
 
     def endDocument(self):
-        self._out.write(unicode(
-            'Processing of %s finished. (%s warnings, %s errors)\n'
-            % (self._filename, self._stats['WARNING'], self._stats['ERROR'])))
-        self._out.write(unicode('=' * 79) + '\n')
+        self._out.write(
+            str(
+                "Processing of %s finished. (%s warnings, %s errors)\n"
+                % (self._filename, self._stats["WARNING"], self._stats["ERROR"])
+            )
+        )
+        self._out.write(str("=" * 79) + "\n")
 
 
 class NoSummaryVerboseHandler(Handler):
-
     def log(self, msg, severity):
         Handler.log(self, msg, severity)
 
-        self._out.write(unicode('%s:%s:%s:\n-%s- - %s' % (
-            self._filename,
-            self._parser.getLineNumber(),
-            self._parser.getColumnNumber(),
-            severity,
-            msg)))
-        self._out.write(u'\n')
+        self._out.write(
+            str(
+                "{}:{}:{}:\n-{}- - {}".format(
+                    self._filename,
+                    self._parser.getLineNumber(),
+                    self._parser.getColumnNumber(),
+                    severity,
+                    msg,
+                )
+            )
+        )
+        self._out.write("\n")
 
     def endDocument(self):
         pass
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/utils.py` & `i18ndude-6.1.0/src/i18ndude/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,138 @@
 import os
 import subprocess
-import sys
 
-PY3 = sys.version_info > (3,)
 
 # Two parameters determine the wrapping of lines.  If WRAP is False,
 # no wrapping is done.  If WRAP is True, the lines will be wrapped at
 # MAX_WIDTH characters.  Both values can be changed by the script,
 # based on command line arguments.
 #
 # By default no wrapping is done, as that has always been the default
 # and only behaviour.  This may change in the future.
 MAX_WIDTH = 79
 WRAP = False
 
 
 def getPoFiles(product, all=False):
-    """Returns all product*.po files in the current folder.
-    """
+    """Returns all product*.po files in the current folder."""
     # First try old style i18n directory that has all .pot and .po files in
     # one directory.
     files = os.listdir(os.curdir)
     if all:
-        files = [file for file in files if file.startswith('%s-' % product)
-                 and file.endswith('.po')]
+        files = [
+            file
+            for file in files
+            if file.startswith("%s-" % product) and file.endswith(".po")
+        ]
     else:
-        files = [file for file in files if file.startswith('%s-' % product)
-                 and file.endswith('.po') and file != '%s-en.po' % product]
+        files = [
+            file
+            for file in files
+            if file.startswith("%s-" % product)
+            and file.endswith(".po")
+            and file != "%s-en.po" % product
+        ]
     if files:
         return files
     # We may be in a locales directory.
-    po_name = '%s.po' % product
+    po_name = "%s.po" % product
     files = []
-    for dirpath, dirnames, filenames in os.walk('.'):
+    for dirpath, dirnames, filenames in os.walk("."):
         # Look for LC_MESSAGES directories
-        if dirpath.split(os.path.sep)[-1] != 'LC_MESSAGES':
+        if dirpath.split(os.path.sep)[-1] != "LC_MESSAGES":
             continue
         if po_name in filenames:
             files.append(os.path.join(dirpath, po_name))
     return files
 
 
 def getPotFiles(product=None, all=False):
     """Returns all pot files in the current folder.
     Normally it doesn't return manual.pots and generated.pots.
     """
     files = os.listdir(os.curdir)
     if all:
-        files = [f for f in files if f.endswith('.pot')]
+        files = [f for f in files if f.endswith(".pot")]
     else:
         files = [
-            f for f in files
-            if f.endswith('.pot')
-            and not f[:-4].endswith('manual')
-            and not f[:-4].endswith('generated')
+            f
+            for f in files
+            if f.endswith(".pot")
+            and not f[:-4].endswith("manual")
+            and not f[:-4].endswith("generated")
         ]
     if product is not None:
-        files = [f for f in files if f.startswith('%s.pot' % product)]
+        files = [f for f in files if f.startswith("%s.pot" % product)]
     return files
 
 
 def getPoFilesAsCmdLine(product):
     files = getPoFiles(product)
-    filestring = ''
+    filestring = ""
     for file in files:
-        filestring += file + ' '
+        filestring += file + " "
     return filestring.rstrip()
 
 
 def getPoFilesByLanguageCode(lang):
-    """Returns all po files which ends with given language code.
-    """
+    """Returns all po files which ends with given language code."""
     files = os.listdir(os.curdir)
-    files = [file for file in files if file.endswith(
-        '.po') and file[:-3].endswith(lang)]
+    files = [
+        file for file in files if file.endswith(".po") and file[:-3].endswith(lang)
+    ]
     return files
 
 
 def getLanguage(product, file):
-    """Returns the language part of a po-file.
-    """
+    """Returns the language part of a po-file."""
     lang = None
-    if file.endswith('.po'):
+    if file.endswith(".po"):
         if file.startswith(product):
-            lang = '-'.join(file.split('-')[1:])[:-3]
+            lang = "-".join(file.split("-")[1:])[:-3]
         else:
             # Get directory name in case of locales structure:
             # lang/LC_MESSAGES/product.po
             lc_found = False
             for part in reversed(file.split(os.path.sep)):
                 if lc_found:
                     lang = part
                     break
-                if part == 'LC_MESSAGES':
+                if part == "LC_MESSAGES":
                     lc_found = True
     return lang
 
 
 def getProduct(file):
     """Returns the product part of a file. We assume files to be something like
     domain-language.po.
     Example: atcontenttypes-pt-br.po
     """
-    assert file.endswith('.po') or file.endswith('.pot')
+    assert file.endswith(".po") or file.endswith(".pot")
 
-    file = file.split('.')[0]  # strip of ending
-    file = file.split('-')[0]  # only take product
+    file = file.split(".")[0]  # strip of ending
+    file = file.split("-")[0]  # only take product
 
     return file
 
 
 def wrapAndQuoteString(value):
-    """Wrap a string in multiple quoted lines.
-    """
+    """Wrap a string in multiple quoted lines."""
     if not value:
-        return u'""'
+        return '""'
     # Wrap over multiple lines if needed.
     lineparts = wrapString(value)
     if len(lineparts) == 1:
-        return u'"{0}"'.format(lineparts[0])
+        return f'"{lineparts[0]}"'
     # We expect the first line to be empty.  Remove it.
     if not lineparts[0]:
         lineparts.pop(0)
     # Quote all and separate them by newlines.
-    newline = u'"\n"'.join(lineparts)
-    return u'"{0}"'.format(newline)
+    newline = '"\n"'.join(lineparts)
+    return f'"{newline}"'
 
 
 def wrapString(value):
     """Wrap a string in multiple lines.
 
     They should have a length of at most MAX_WIDTH, minus 3 for the
     start quote, end quote and a space before the end quote, although
@@ -140,125 +144,127 @@
     if not WRAP:
         return [value]
     # Determine the maximum line length.  At first we only reserve
     # room for the two enclosing quotes.
     max_len = MAX_WIDTH - 2
     # For a single line the maximum length is shorter, it has to account
     # for the 'msgstr ' that goes before the string.
-    single_line_max_len = max_len - len('msgstr ')
+    single_line_max_len = max_len - len("msgstr ")
     # Maybe we have it easy.
     if max_len <= 0 or len(value) <= single_line_max_len:
         return [value]
     # The line maybe is just in between max_len and single_line_max_len
     if len(value) <= max_len:
-        return [u'', value]
+        return ["", value]
     # No, the value does not fit on one line.  This means we need to
     # reserve room for a space at the end of all but the last line.
     max_len -= 1
-    words = value.split(u' ')
+    words = value.split(" ")
     len_words = len(words)
     # We always start with an empty first line
-    lines = [u'']
-    line = u''
+    lines = [""]
+    line = ""
     for index, word in enumerate(words):
         if index == len_words - 1:
             # This is the last word.  The last line needs no space at
             # the end, so we are allowed to use one more character.
             max_len += 1
         if not line:
             new_line = word
         else:
-            new_line = u'{0} {1}'.format(line, word)
+            new_line = f"{line} {word}"
         if len(new_line) <= max_len or not line:
             # There is room or we had an empty line and the current
             # single word is already too large so we accept it as a
             # line anyway.  Use the new line and continue with the
             # next word.
             line = new_line
             continue
         # There is no more room so we store the line.  If it is not
         # empty it should end with a space.
         if line:
-            line += u' '
+            line += " "
         lines.append(line)
         # Start a fresh line with the current word.
         line = word
     # The last line has not been added yet.
     lines.append(line)
     return lines
 
 
 def prepare_cli_documentation(data):
     """Update the command line docs in the docs dir.
 
     This uses a hook from zest.releaser to update some documentation
     when doing a release.  See our setup.py and setup.cfg.
     """
-    if data['name'] != 'i18ndude':
+    if data["name"] != "i18ndude":
         # We're available everywhere, but we're only intended to be
         # used when we release i18ndude.
         return
-    target = os.path.join(data['workingdir'], 'docs',
-                          'command.rst')
-    marker = '.. ### AUTOGENERATED FROM HERE ###'
+    target = os.path.join(data["workingdir"], "docs", "command.rst")
+    marker = ".. ### AUTOGENERATED FROM HERE ###"
     result = []
     for line in open(target).readlines():
         line = line.rstrip()
         if line == marker:
             break
         result.append(line)
     result.append(marker)
-    result.append('')
+    result.append("")
 
     def indent(text):
         result = []
         for line in text.splitlines():
             if line:
-                result.append('  ' + line.decode())
+                result.append("  " + line.decode())
             else:
-                result.append('')
+                result.append("")
         return result
 
-    base_cmd = 'bin/i18ndude'
+    base_cmd = "bin/i18ndude"
     # Add result off calling bin/i18ndude --help
-    result.append('i18ndude')
-    result.append('--------')
+    result.append("i18ndude")
+    result.append("--------")
     result.append("\n::\n")
-    res = subprocess.check_output([base_cmd, '--help'])
+    res = subprocess.check_output([base_cmd, "--help"])
     result.extend(indent(res))
     # Same for the subcommands.
     subcommands = [
-        'find-untranslated',
-        'rebuild-pot',
-        'merge',
-        'sync',
-        'filter',
-        'admix',
-        'list',
-        'trmerge']
+        "find-untranslated",
+        "rebuild-pot",
+        "merge",
+        "sync",
+        "filter",
+        "admix",
+        "list",
+        "trmerge",
+    ]
     for sub in subcommands:
-        result.append('')
+        result.append("")
         result.append(sub)
-        result.append('-' * len(sub))
+        result.append("-" * len(sub))
         result.append("\n::\n")
-        res = subprocess.check_output([base_cmd, sub, '--help'])
+        res = subprocess.check_output([base_cmd, sub, "--help"])
         result.extend(indent(res))
 
-    result.append('')
-    open(target, 'w').write('\n'.join(result))
+    result.append("")
+    open(target, "w").write("\n".join(result))
     print("Wrote command line documentation to", target)
 
     # If there is a diff, we want to commit it.
     from zest.releaser import choose
-    from zest.releaser.utils import ask, execute_command
+    from zest.releaser.utils import ask
+    from zest.releaser.utils import execute_command
+
     vcs = choose.version_control()
     diff_cmd = vcs.cmd_diff()
     diff = execute_command(diff_cmd)
     if diff.strip():
-        print("The %r:\n\n%s\n" % (diff_cmd, diff))
+        print(f"The {diff_cmd!r}:\n\n{diff}\n")
         if ask("OK to commit this"):
             msg = "Wrote command line documentation."
             commit_cmd = vcs.cmd_commit(msg)
             print(execute_command(commit_cmd))
 
 
 def quote(s):
@@ -267,43 +273,43 @@
     if [ch for ch in s if ch.isspace()]:
         return '"%s"' % s
     else:
         return s
 
 
 def undouble_unicode_escape(value):
-    """ The mother of all hacks.
+    """The mother of all hacks.
     This tries to work around unicode/string confusion between
     python2 and python3 while opening files in text mode that contain
     bytes, or strings, that represent UTF-8 encoded unicode, or various
     levels of escaped UTF-8 representing unicode, or whatever...
 
     All of this is end-of-pipe window dressing to work around the confusion
     in the i18ndude code base about filehandles, unicode, printing to stdout
     and then redirecting stdout to filehandles again and then ... etc.
     """
 
     # debug = lambda x: ''  # print(x)
 
     # first pass -- handle triply escaped python2
     try:
-        value = value.decode('raw_unicode_escape')
+        value = value.decode("raw_unicode_escape")
     except UnicodeEncodeError:
         # debug("1-- UnicodeEncodeError on {}".format(repr(value)))
         # py2: 'ascii' codec can't encode characters
         pass
     except AttributeError:
         # debug("1-- AttributeError on {}".format(repr(value)))
         # py3: 'str' object has no attribute 'decode'
         # object or str, we don't know yet, keep processing
         pass
 
     # second pass -- handle triply escaped python3
     try:
-        value = value.encode('raw_unicode_escape').decode('utf-8')
+        value = value.encode("raw_unicode_escape").decode("utf-8")
     except UnicodeDecodeError:
         # debug("2-- UnicodeDecodeError on {}".format(repr(value)))
         pass
     except UnicodeEncodeError:
         # debug("2-- UnicodeEncodeError on {}".format(repr(value)))
         # py2: 'ascii' codec can't encode characters
         pass
@@ -311,26 +317,26 @@
         # debug("2-- AttributeError on {}".format(repr(value)))
         # debug("--2: returning {}".format(value))
         return value  # object
 
     # third pass --
     try:
         # doubly encoded?
-        value = value.encode('raw_unicode_escape').decode('utf-8')
+        value = value.encode("raw_unicode_escape").decode("utf-8")
     except UnicodeDecodeError:
         # normal unicode, either from input or first pass
         # debug("3-- UnicodeDecodeError on {}".format(repr(value)))
         pass
 
     # fourth pass - suffices in python3
-    value = value.encode('raw_unicode_escape').decode('raw_unicode_escape')
+    value = value.encode("raw_unicode_escape").decode("raw_unicode_escape")
 
     # fifth pass - needed in python2.7 only for escaped encoded
     try:
-        value = value.decode('raw_unicode_escape')
+        value = value.decode("raw_unicode_escape")
     except UnicodeEncodeError:
         # py27 UnicodeEncodeError: 'ascii' codec can't encode character
         pass
     except AttributeError:
         # py36 AttributeError: 'str' object has no attribute 'decode
         pass
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/visualisation.py` & `i18ndude-6.1.0/src/i18ndude/visualisation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,61 @@
 from operator import itemgetter
 
 
 # For the '--tiered' option, we use the IGNORE, GROUP1 and GROUP2 options.
 # This was the only way for years.
-IGNORE = frozenset(('zh', 'sr-Latn', ))
+IGNORE = frozenset(
+    (
+        "zh",
+        "sr-Latn",
+    )
+)
 
 GROUP1 = [
-    'fr', 'it', 'de', 'es', 'nl', 'zh-cn', 'zh-tw', 'ja', 'ko', 'pt-br',
-    'ru', 'pl', 'tr', 'th', 'ar',
+    "fr",
+    "it",
+    "de",
+    "es",
+    "nl",
+    "zh-cn",
+    "zh-tw",
+    "ja",
+    "ko",
+    "pt-br",
+    "ru",
+    "pl",
+    "tr",
+    "th",
+    "ar",
 ]
 
 GROUP2 = [
-    'sv', 'fi', 'da', 'pt', 'ro', 'hu', 'he', 'id', 'cs', 'el', 'no', 'vi',
-    'bg', 'hr', 'lt', 'sk', 'tl', 'sl', 'sr', 'ca', 'lv', 'uk', 'hi',
+    "sv",
+    "fi",
+    "da",
+    "pt",
+    "ro",
+    "hu",
+    "he",
+    "id",
+    "cs",
+    "el",
+    "no",
+    "vi",
+    "bg",
+    "hr",
+    "lt",
+    "sk",
+    "tl",
+    "sl",
+    "sr",
+    "ca",
+    "lv",
+    "uk",
+    "hi",
 ]
 
 _TEMPLATE = """
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
                       "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 <html>
 <head>
@@ -40,178 +79,179 @@
 """  # noqa
 
 
 def print_row(percentage, desc):
     width = percentage * 2
     if width == 0:
         width = 1
-    color = '#0d0'  # some kind of green
+    color = "#0d0"  # some kind of green
     if percentage < 90:
-        color = 'yellow'
+        color = "yellow"
     if percentage < 50:
-        color = 'red'
+        color = "red"
 
     return _ROW % dict(
         width=width,
         color=color,
         percent=percentage,
         name=desc,
     )
 
 
 def sort_languages(values):
-    return sorted(values, key=itemgetter('percentage'), reverse=True)
+    return sorted(values, key=itemgetter("percentage"), reverse=True)
 
 
 def output_table(out, languagelist, total, tiered):
-    body = ''
-    table = ''
+    body = ""
+    table = ""
 
     body += "<h1>Messages: %s</h1>\n" % total
 
     if not tiered:
         for value in sort_languages(out.values()):
-            perc = value['percentage']
+            perc = value["percentage"]
             if perc == 0:
                 continue
-            table += print_row(perc, value['desc'])
+            table += print_row(perc, value["desc"])
     else:
-        body += '<h2>Tier 1:</h2>\n'
+        body += "<h2>Tier 1:</h2>\n"
 
-        table += print_row(100, 'English (en)')
+        table += print_row(100, "English (en)")
         for code in GROUP1:
             if code in out:
-                table += print_row(out[code]['percentage'], out[code]['desc'])
+                table += print_row(out[code]["percentage"], out[code]["desc"])
                 del out[code]
             else:
                 lang = languagelist.get(code)
                 if lang is None:
                     name = code
                 else:
-                    name = lang['name']
-                desc = '%s (%s)' % (name, code)
+                    name = lang["name"]
+                desc = f"{name} ({code})"
                 table += print_row(0, desc)
 
         body += _TABLE % dict(table=table)
-        table = ''
+        table = ""
 
-        body += '\n<h2>Tier 2:</h2>\n'
+        body += "\n<h2>Tier 2:</h2>\n"
         for code in GROUP2:
             if code in out:
-                table += print_row(out[code]['percentage'], out[code]['desc'])
+                table += print_row(out[code]["percentage"], out[code]["desc"])
                 del out[code]
             else:
                 lang = languagelist.get(code)
                 if lang is None:
                     name = code
                 else:
-                    name = lang['name']
-                desc = '%s (%s)' % (name, code)
+                    name = lang["name"]
+                desc = f"{name} ({code})"
                 table += print_row(0, desc)
 
         body += _TABLE % dict(table=table)
-        table = ''
+        table = ""
 
-        body += '\n<h2>Tier 3:</h2>\n'
+        body += "\n<h2>Tier 3:</h2>\n"
         group3 = sorted(out.values())
         for value in group3:
-            perc = value['percentage']
+            perc = value["percentage"]
             if perc == 0:
                 continue
-            table += print_row(perc, value['desc'])
+            table += print_row(perc, value["desc"])
 
     body += _TABLE % dict(table=table)
     template = _TEMPLATE % dict(body=body)
 
     print(template)
 
 
 def aligned_print(percentage, desc):
     if percentage < 10:
-        percentage = '  %d' % percentage
+        percentage = "  %d" % percentage
     elif percentage < 100:
-        percentage = ' %d' % percentage
-    print("%s%% - %s" % (percentage, desc))
+        percentage = " %d" % percentage
+    print(f"{percentage}% - {desc}")
 
 
 def output_list(out, languagelist, total, tiered):
     print("Messages: %s\n" % total)
     if not tiered:
         for value in sort_languages(out.values()):
-            perc = value['percentage']
+            perc = value["percentage"]
             if perc == 0:
                 continue
-            aligned_print(perc, value['desc'])
+            aligned_print(perc, value["desc"])
         return
 
-    print('Tier 1:\n')
-    print('100% - English (en)')
+    print("Tier 1:\n")
+    print("100% - English (en)")
     for code in GROUP1:
         if code in out:
-            aligned_print(out[code]['percentage'], out[code]['desc'])
+            aligned_print(out[code]["percentage"], out[code]["desc"])
             del out[code]
         else:
             lang = languagelist.get(code)
             if lang is None:
                 name = code
             else:
-                name = lang['name']
-            desc = '%s (%s)' % (name, code)
+                name = lang["name"]
+            desc = f"{name} ({code})"
             aligned_print(0, desc)
 
-    print('\nTier 2:\n')
+    print("\nTier 2:\n")
     for code in GROUP2:
         if code in out:
-            aligned_print(out[code]['percentage'], out[code]['desc'])
+            aligned_print(out[code]["percentage"], out[code]["desc"])
             del out[code]
         else:
             continue
             lang = languagelist.get(code)
             if lang is None:
                 name = code
             else:
-                name = lang['name']
-            desc = '%s (%s)' % (name, code)
+                name = lang["name"]
+            desc = f"{name} ({code})"
             aligned_print(0, desc)
 
-    print('\nTier 3:\n')
+    print("\nTier 3:\n")
     group3 = sorted(out.values())
     for value in group3:
-        perc = value['percentage']
+        perc = value["percentage"]
         if perc == 0:
             continue
-        aligned_print(perc, value['desc'])
+        aligned_print(perc, value["desc"])
 
 
 def make_listing(pot, pos, table=False, tiered=False):
     try:
         from plone.i18n.locales.languages import LanguageAvailability
+
         languagelist = LanguageAvailability().getLanguages(combined=True)
     except ImportError:
         languagelist = {}
 
     msgids = pot.keys()
     total = len(msgids)
     values = {}
 
-    for po in [p for p in pos if p.mime_header['Language-Code'] != 'en']:
-        code = po.mime_header.get('Language-Code')
+    for po in [p for p in pos if p.mime_header["Language-Code"] != "en"]:
+        code = po.mime_header.get("Language-Code")
         if tiered and code in IGNORE:
             continue
-        name = po.mime_header.get('Language-Name')
+        name = po.mime_header.get("Language-Name")
         language = languagelist.get(code)
         if language is not None:
-            desc = "%s (%s)" % (language['name'], code)
+            desc = "{} ({})".format(language["name"], code)
         else:
-            desc = "%s (%s)" % (name, code)
+            desc = f"{name} ({code})"
 
         value = 0
         for msgid in msgids:
             if msgid in po and po[msgid].msgstr:  # translated
-                if not [1 for fuzzy in po[msgid].comments if 'fuzzy' in fuzzy]:
+                if not [1 for fuzzy in po[msgid].comments if "fuzzy" in fuzzy]:
                     value += 1
 
         percentage = int(value / (total * 1.0) * 100)
         values[code] = dict(percentage=percentage, desc=desc)
 
     total = len(msgids)
     if table:
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude/zcmlextract.py` & `i18ndude-6.1.0/src/i18ndude/zcmlextract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import sys
-
+from i18ndude.extract import find_files
 from lxml import etree
 
-from i18ndude.extract import find_files
+import sys
+
 
 # Namespaces.
 ZOPE_NS = "http://namespaces.zope.org/zope"
 GS_NS = "http://namespaces.zope.org/genericsetup"
 MONKEY_NS = "http://namespaces.plone.org/monkey"
 # Directives using those namespaces.
-GS_EXPORT_STEP = '{%s}exportStep' % GS_NS
-GS_IMPORT_STEP = '{%s}importStep' % GS_NS
-GS_UPGRADE_DEPENDS = '{%s}upgradeDepends' % GS_NS
-GS_UPGRADE_STEP = '{%s}upgradeStep' % GS_NS
-GS_UPGRADE_STEPS = '{%s}upgradeSteps' % GS_NS
-INTERFACE = '{%s}interface' % ZOPE_NS
-MONKEY_PATCH = '{%s}patch' % MONKEY_NS
-PERMISSION = '{%s}permission' % ZOPE_NS
-I18N_DOMAIN = 'i18n_domain'
-RULE_TYPE = 'plone.contentrules.rule.interfaces.IRuleEventType'
+GS_EXPORT_STEP = "{%s}exportStep" % GS_NS
+GS_IMPORT_STEP = "{%s}importStep" % GS_NS
+GS_UPGRADE_DEPENDS = "{%s}upgradeDepends" % GS_NS
+GS_UPGRADE_STEP = "{%s}upgradeStep" % GS_NS
+GS_UPGRADE_STEPS = "{%s}upgradeSteps" % GS_NS
+INTERFACE = "{%s}interface" % ZOPE_NS
+MONKEY_PATCH = "{%s}patch" % MONKEY_NS
+PERMISSION = "{%s}permission" % ZOPE_NS
+I18N_DOMAIN = "i18n_domain"
+RULE_TYPE = "plone.contentrules.rule.interfaces.IRuleEventType"
 
 # These zcml directives should not be translated, because it is not useful.
 BLACKLISTED_DIRECTIVES = [
     GS_EXPORT_STEP,
     GS_IMPORT_STEP,
     GS_UPGRADE_DEPENDS,
     GS_UPGRADE_STEP,
@@ -30,33 +30,32 @@
     MONKEY_PATCH,
     PERMISSION,
 ]
 # We cannot really read and interpret the meta zcml to figure out which
 # properties are translatable MessageIDs instead of simple TextLines.  So we
 # simply take all these properties:
 TRANSLATABLE_PROPERTIES = [
-    'description',
-    'title',
+    "description",
+    "title",
 ]
 
 
-class ZCMLParser(object):
-    """ZCML profile i18n parser.
-    """
+class ZCMLParser:
+    """ZCML profile i18n parser."""
 
     def __init__(self):
         self.catalogs = {}
         self.filename = None
 
     def parse(self, filename):
         self.filename = filename
         try:
             tree = etree.parse(filename)
         except Exception as e:
-            print(u"There was an error in parsing %s: %s" % (filename, e))
+            print(f"There was an error in parsing {filename}: {e}")
             sys.exit(0)
         elem = tree.getroot()
         domain = elem.get(I18N_DOMAIN, None)
         self.parseNode(elem, domain)
         self.parseChildren(elem, domain)
 
     def parseChildren(self, elem, domain):
@@ -69,36 +68,35 @@
         # We only extract title and description from a registerProfile tag.
         domain = elem.get(I18N_DOMAIN, domain)
         if domain is not None:
             if domain not in self.catalogs:
                 self.catalogs[domain] = []
             if elem.tag in BLACKLISTED_DIRECTIVES:
                 return
-            if elem.tag == INTERFACE and elem.get('type') == RULE_TYPE:
-                self.maybe_add(domain, elem, 'name')
+            if elem.tag == INTERFACE and elem.get("type") == RULE_TYPE:
+                self.maybe_add(domain, elem, "name")
             for key in TRANSLATABLE_PROPERTIES:
                 self.maybe_add(domain, elem, key)
 
     def maybe_add(self, domain, elem, key):
         text = elem.get(key)
         if text is not None:
             text = text.strip()
         if not text:
             return
         msgid = text
-        msgstr = u""
+        msgstr = ""
         self.catalogs[domain].append(
-            (msgid, msgstr,
-             '{}:{}'.format(self.filename, elem.sourceline)))
+            (msgid, msgstr, f"{self.filename}:{elem.sourceline}")
+        )
 
     def getCatalogs(self):
         return self.catalogs
 
 
 def zcml_strings(dir, domain="none", exclude=()):
-    """Retrieve all messages from `dir` that are in the `domain`.
-    """
+    """Retrieve all messages from `dir` that are in the `domain`."""
     parser = ZCMLParser()
-    for filename in find_files(dir, '*.zcml', exclude=tuple(exclude)):
+    for filename in find_files(dir, "*.zcml", exclude=tuple(exclude)):
         parser.parse(filename)
 
     return parser.getCatalogs()
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude.egg-info/PKG-INFO` & `i18ndude-6.1.0/src/i18ndude.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i18ndude
-Version: 6.0.0a1
+Version: 6.1.0
 Summary: i18ndude performs various tasks related to ZPT's, Python Scripts and i18n.
 Home-page: https://github.com/collective/i18ndude
 Author: Daniel Nouri
 Author-email: plone-i18n@lists.sourceforge.net
 Maintainer: Maurits van Rees
 Maintainer-email: maurits@vanrees.org
 License: GPL
@@ -78,14 +78,15 @@
     -   repo: https://github.com/collective/i18ndude
         rev: "master"
         hooks:
         -   id: i18ndude
 
 For now it only finds the strings not marked for translation.
 
+
 Command line interface
 ======================
 
 These are the various command line options.
 
 .. ### AUTOGENERATED FROM HERE ###
 
@@ -376,24 +377,51 @@
     --width NUMBER      Set output page width. Default is 79.
     -i, --ignore-extra  Ignore extra messages: do not add msgids that are not in
                         the original po-file. Only update translations for
                         existing msgids.
     --no-override       Do not override translations, only add missing
                         translations.
 
+
 Changelog
 =========
 
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+6.1.0 (2023-07-18)
+------------------
+
+New features:
+
+
+- Let i18n:ignore ignore all translatable strings in its scope. (#109)
+
+
+Bug fixes:
+
+
+- Remove Python 2 support code.  Use pyupgrade, isort, black, flake8.
+  [maurits] (#23)
+
+
+6.0.0 (2023-05-30)
+------------------
+
+Bug fixes:
+
+
+- Fix pre-commit integration.
+  [gforcada] (#1)
+
+
 6.0.0a1 (2023-05-08)
 --------------------
 
 Breaking changes:
 
 
 - Drop support for Python 2.
```

### Comparing `i18ndude-6.0.0a1/src/i18ndude.egg-info/SOURCES.txt` & `i18ndude-6.1.0/src/i18ndude.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/i18ndude/__init__.py
 src/i18ndude/catalog.py
 src/i18ndude/common.py
 src/i18ndude/extract.py
 src/i18ndude/generator.py
 src/i18ndude/gsextract.py
 src/i18ndude/interfaces.py
+src/i18ndude/messages.pot
 src/i18ndude/pygettext.py
 src/i18ndude/script.py
 src/i18ndude/untranslated.py
 src/i18ndude/utils.py
 src/i18ndude/visualisation.py
 src/i18ndude/zcmlextract.py
 src/i18ndude.egg-info/PKG-INFO
```

