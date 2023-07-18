# Comparing `tmp/vfbLib-0.4.6.tar.gz` & `tmp/vfbLib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfbLib-0.4.6.tar", last modified: Tue Apr 25 15:53:31 2023, max compression
+gzip compressed data, was "vfbLib-0.5.0.tar", last modified: Tue Jul 18 14:58:12 2023, max compression
```

## Comparing `vfbLib-0.4.6.tar` & `vfbLib-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.910002 vfbLib-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-25 15:53:14.000000 vfbLib-0.4.6/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 15:53:14.000000 vfbLib-0.4.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.898002 vfbLib-0.4.6/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.902002 vfbLib-0.4.6/Lib/vfbLib/
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.906002 vfbLib-0.4.6/Lib/vfbLib/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/mm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/parsers/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/truetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.910002 vfbLib-0.4.6/Lib/vfbLib/ufo/
--rw-r--r--   0 runner    (1001) docker     (123)    28171 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/designspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/guides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/kerning.py
--rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/pshints.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/tth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/ufo/vfb2ufo.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-25 15:53:14.000000 vfbLib-0.4.6/Lib/vfbLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:53:31.902002 vfbLib-0.4.6/Lib/vfbLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 15:53:31.000000 vfbLib-0.4.6/Lib/vfbLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-25 15:53:31.910002 vfbLib-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-25 15:53:14.000000 vfbLib-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 15:53:15.000000 vfbLib-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 15:53:31.910002 vfbLib-0.4.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-04-25 15:53:15.000000 vfbLib-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-18 14:58:02.000000 vfbLib-0.5.0/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 14:58:02.000000 vfbLib-0.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.854471 vfbLib-0.5.0/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/cmdline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/compilers/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/cu2qu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/mm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/parsers/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/templates/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/truetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/Lib/vfbLib/ufo/
+-rw-r--r--   0 runner    (1001) docker     (123)    29773 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/designspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/guides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/kerning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/pshints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/tth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/ufo/vfb2ufo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.862471 vfbLib-0.5.0/Lib/vfbLib/vfb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-18 14:58:02.000000 vfbLib-0.5.0/Lib/vfbLib/vfb/vfb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:58:12.858471 vfbLib-0.5.0/Lib/vfbLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 14:58:12.000000 vfbLib-0.5.0/Lib/vfbLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-18 14:58:12.862471 vfbLib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-18 14:58:02.000000 vfbLib-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 14:58:02.000000 vfbLib-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-18 14:58:12.862471 vfbLib-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-18 14:58:02.000000 vfbLib-0.5.0/setup.py
```

### Comparing `vfbLib-0.4.6/DESCRIPTION.md` & `vfbLib-0.5.0/DESCRIPTION.md`

 * *Files 15% similar despite different names*

```diff
@@ -39,38 +39,35 @@
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
 usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2022 by LucasFonts Build 2022-12-12
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  output folder
   -fo, --force-overwrite
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
-
-Additional options:
-
-  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
+  -z, --zip             write UFOZ (compressed UFO)
+  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
 
-Unimplemented options:
+Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
-  -z, --zip             write UFOZ (compressed UFO)
 ```
 
 
 ### vfb2json
 
 Generate a representation that closely adheres to the VFB structure.
 
@@ -80,36 +77,67 @@
 
 will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
-usage: vfb2json [-h] [-m] [-p PATH] inputpath
+usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
 
-VFB2JSON Converter Copyright (c) 2022 by LucasFonts Build 2022-11-08
+VFB2JSON Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
 
 options:
   -h, --help            show this help message and exit
+  -d, --no-decompile    don't decompile data, output binary in JSON
+  --header              only read the VFB header, not the actual data
   -m, --minimal         parse only minimal amount of data
   -p PATH, --path PATH  output folder
 ```
 
 
+### vfbcu2qu
+
+Convert a VFB file to quadratic using the `cu2qu` library. Single master only.
+
+```bash
+$ vfbcu2qu MyFile.vfb
+```
+
+will convert the file and save it with the suffix `.qu.vfb` in the same directory.
+
+```
+usage: vfbcu2qu [-h] [-p PATH] [-fo] [-m MAX_ERR_EM] inputpath [outputpath]
+
+VFB Cubic to Quadratic Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+
+positional arguments:
+  inputpath             input file path (.vfb)
+  outputpath            output file path (.vfb)
+
+options:
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  output folder
+  -fo, --force-overwrite
+                        force overwrite
+  -m MAX_ERR_EM, --max-err-em MAX_ERR_EM
+                        Maximum allowed error, relative to the font's units per em.
+```
+
+
 ### diffvfb
 
 Generate a diff of two VFB files, either in unified diff or HTML format.
 
 ```
 usage: diffvfb [-h] [--html HTML] file1 file2
 
-diffvfb Copyright (c) 2023 by LucasFonts Build 2023-03-14
+diffvfb Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   file1        First input file path (.vfb)
   file2        Second input file path (.vfb)
 
 options:
   -h, --help   show this help message and exit
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/__init__.py` & `vfbLib-0.5.0/Lib/vfbLib/vfb/vfb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,182 @@
 from __future__ import annotations
 
 import logging
 
-from fontTools.misc.textTools import hexStr
-from io import BufferedReader
 from pathlib import Path
 from time import time
-from typing import Any, List, Tuple, Type
-from vfbLib.constants import ignore_minimal, parser_classes
-from vfbLib.parsers import BaseParser
-from vfbLib.parsers.header import VfbHeaderParser
+from typing import TYPE_CHECKING, Any, Dict, Iterable, List, Set, Tuple
+from vfbLib.vfb.glyph import VfbGlyph
+from vfbLib.vfb.entry import VfbEntry
+from vfbLib.vfb.header import VfbHeader
+from vfbLib.vfb.info import VfbInfo
+
+if TYPE_CHECKING:
+    from io import BufferedReader
 
 
 logger = logging.getLogger(__name__)
 
-FALLBACK_PARSER = BaseParser
+
+# Convenience objects for vfb access
 
 
-class VFBReader:
+class Vfb:
     """
-    Base class to read data from a vfb file
+    Object to represent the vfb data, with the ability to read and write. You can use
+    the Vfb object to access glyphs through dict methods, where the glyph name is the
+    key and the glyph object is the value.
     """
 
     def __init__(
         self,
         vfb_path: Path,
         timing=True,
         minimal=False,
-        only_keys: List[str] | None = None,
+        drop_keys: Set[str] | None = None,
+        only_header=False,
     ) -> None:
         self.vfb_path = vfb_path
-        self.data: List[List[Any]] = []
         self.timing = timing
         self.minimal = minimal
-        if only_keys is None:
-            self.only_keys = []
+        if drop_keys is None:
+            self.drop_keys = set()
         else:
-            self.only_keys = only_keys
-        self.master_count = None
+            self.drop_keys = set(drop_keys)
+        self.only_header = only_header
+
+        # We need some minimal API to make pen access work ...
+        self._glyphs: Dict[str, VfbGlyph] = {}
+        self.glyph_order: List[str] = []
+
+        # cu2qu accesses the info and lib ...
+        self.info = VfbInfo(vfb=self)
+        self.lib = {}
+
+        self.num_masters: int = 0
+        self.read()
+
+    def as_dict(self) -> Dict[str, Dict[str, Any]]:
+        """
+        Return the Vfb structure as Dict, e.g. for saving as JSON. The dict has the keys
+        "header" and "entries".
+        """
+        d = {}
+        if self.header is not None:
+            d["header"] = self.header.as_dict()
+        if self.entries:
+            d["entries"] = [e.as_dict() for e in self.entries]
+        return d
 
-    def __repr__(self) -> str:
-        return str(self.data)
+    def clear(self):
+        """
+        Clear any data that may have been read before.
+        """
+        self.header: VfbHeader | None = None
+        self.entries: List[VfbEntry] = []
 
-    def parse(self, stream: BufferedReader):
+    def _decompile_glyphs(self):
+        for entry in self.entries:
+            if entry.key == "Glyph":
+                glyph = VfbGlyph(entry, self)
+                name = glyph.decompile()
+                if name in self._glyphs:
+                    logger.error(f"VFB contains duplicate glyph name: {name}")
+                    # FIXME: Disambiguate duplicate names
+                self._glyphs[name] = glyph
+                self.glyph_order.append(name)
+
+    def __contains__(self, key: str) -> bool:
+        if not self._glyphs:
+            self._decompile_glyphs()
+        return key in self._glyphs
+
+    def __getitem__(self, key: str) -> VfbGlyph:
+        if not self._glyphs:
+            self._decompile_glyphs()
+        return self._glyphs[key]
+
+    def decompile(self) -> None:
+        """
+        Decompile all entries, except for the ones listed in `drop_keys`.
+        """
         start = time()
-        self.stream = stream
-        header = VfbHeaderParser.parse(stream)
-        self.data.append(["header", header])
+        for entry in self.entries:
+            entry.decompile()
+
+        end = time()
+        if self.timing:
+            print(f"Interpreting binary data took {round((end - start) * 1000)} ms.")
+
+    def items(self) -> Iterable[Tuple[str, VfbGlyph]]:
+        if not self._glyphs:
+            self._decompile_glyphs()
+        return self._glyphs.items()
+
+    def keys(self) -> Iterable[str]:
+        if not self._glyphs:
+            self._decompile_glyphs()
+        return self._glyphs.keys()
+
+    def read_stream(self, stream: BufferedReader):
+        """
+        Lazily read and parse the vfb stream, i.e. parse the header, but only read the
+        binary data of other entries.
+        """
+        start = time()
+        self.header = VfbHeader()
+        self.header.read(stream)
+        if self.only_header:
+            return
+
+        entry: VfbEntry | None = None
         while True:
             try:
-                entry = self._parse_entry()
+                entry = VfbEntry(self)
+                entry.read(stream)
             except EOFError:
                 break
 
-            if entry:
-                self.data.append(entry)
+            if entry is not None:
+                if entry.key == "Master Count":
+                    entry.decompile()
+                    self.num_masters = entry.decompiled
+                    entry.decompiled = None
 
-                # Save information that is needed by parsers
-
-                if entry[0] == "Master Count":
-                    if self.master_count is None:
-                        self.master_count = entry[1]
-                    else:
-                        print("WARNING: Redefined master count")
+                if entry.key not in self.drop_keys:
+                    self.entries.append(entry)
 
         end = time()
         if self.timing:
             print(
-                "Source file was successfully imported in",
-                round((end - start) * 1000),
-                "ms.",
+                "Source file was successfully read in "
+                f"{round((end - start) * 1000)} ms."
             )
 
     def read(self):
-        self.data = []
-        with open(self.vfb_path, "rb") as vfb:
-            self.parse(vfb)
-
-    def _parse_entry(self) -> List[Any]:
         """
-        Read, parse and return an entry from the stream
+        Read data from the file at vfb_path, without decompiling
         """
-        entry_id, parser_class, size = self._read_entry()
-
-        if (
-            self.minimal
-            and entry_id in ignore_minimal
-            or self.only_keys
-            and entry_id not in self.only_keys
-        ):
-            self.stream.seek(size, 1)
-            return []
-
-        try:
-            parsed = parser_class.parse(self.stream, size, self.master_count)
-        except:  # noqa: E722
-            logger.error(
-                f"Parse error for data: {entry_id}; {hexStr(self.stream.read(size))}"
-            )
-            logger.error(f"Parser class: {parser_class}")
-            parsed = f"ParseError ({parser_class})"
-            raise
-
-        if parsed:
-            return [entry_id, parsed]
-        else:
-            return []
+        self.clear()
+        with open(self.vfb_path, "rb") as vfb:
+            self.read_stream(vfb)
 
-    def _read_entry(self) -> Tuple[str, Type[BaseParser], int]:
+    def write(self, out_path: Path) -> None:
         """
-        Read an entry from the stream and return its key, specialized parser
-        class, and data.
+        Compile any entries with changes, and write the VFB to out_path.
         """
-        entry_id = BaseParser.read_uint16(self.stream)
-        entry_info = parser_classes.get(
-            entry_id & ~0x8000, (str(entry_id), FALLBACK_PARSER)
-        )
-        key, parser_class = entry_info
-
-        if entry_id == 5:
-            # File end marker?
-            BaseParser.read_uint16(self.stream)
-            two = BaseParser.read_uint16(self.stream)
-            if two == 2:
-                BaseParser.read_uint16(self.stream)
-                raise EOFError
-
-        if entry_id & 0x8000:
-            # Uses uint32 for data length
-            num_bytes = BaseParser.read_uint32(self.stream)
-        else:
-            # Uses uint16 for data length
-            num_bytes = BaseParser.read_uint16(self.stream)
+        if self.header is None:
+            raise ValueError
 
-        return key, parser_class, num_bytes
+        with open(out_path, "wb") as vfb:
+            if self.header.modified:
+                self.header.compile()
+            assert self.header.data
+            vfb.write(self.header.data)
+
+            for entry in self.entries:
+                if entry.modified:
+                    entry.compile()
+                vfb.write(entry.header)
+                vfb.write(entry.data)
+            # File end marker
+            vfb.write(b"\05\00\00\00\02\00\00\00")
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/cmdline.py` & `vfbLib-0.5.0/Lib/vfbLib/cmdline.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import codecs
 import json
 import logging
 
 from argparse import ArgumentParser
 from pathlib import Path
-from vfbLib import VFBReader
-from vfbLib.ufo import VfbToUfoWriter
+from vfbLib.reader import VFBReader
+from vfbLib.ufo import VfbToUfoBuilder
 from vfbLib.version import build_date
+from vfbLib.vfb.vfb import Vfb
 
 
 logger = logging.getLogger(__name__)
 
 
 def read_vfb(vfb_path: Path, minimal=False) -> VFBReader:
     reader = VFBReader(vfb_path, minimal=minimal)
@@ -24,18 +25,31 @@
     with codecs.open(str(json_path), "wb", "utf-8") as f:
         json.dump(reader.data, f, ensure_ascii=False, indent=4)
 
 
 def vfb2json():
     parser = ArgumentParser(
         description=(
-            f"VFB2JSON Converter\nCopyright (c) 2022 by LucasFonts\nBuild {build_date}"
+            f"VFB2JSON Converter\nCopyright (c) 2023 by LucasFonts\nBuild {build_date}"
         )
     )
     parser.add_argument(
+        "-d",
+        "--no-decompile",
+        action="store_true",
+        default=False,
+        help="don't decompile data, output binary in JSON",
+    )
+    parser.add_argument(
+        "--header",
+        action="store_true",
+        default=False,
+        help="only read the VFB header, not the actual data",
+    )
+    parser.add_argument(
         "-m",
         "--minimal",
         action="store_true",
         default=False,
         help="parse only minimal amount of data",
     )
     parser.add_argument(
@@ -50,28 +64,34 @@
         type=str,
         nargs=1,
         help="input file path (.vfb)",
     )
     args = parser.parse_args()
     if args:
         vfb_path = Path(args.inputpath[0])
-        reader = read_vfb(vfb_path, minimal=args.minimal)
+        print(parser.description)
+        print(f"Reading file {vfb_path} ...")
+        vfb = Vfb(vfb_path, only_header=args.header, minimal=args.minimal)
+        if not args.no_decompile:
+            vfb.decompile()
+        suffix = ".vfb.json"
         if args.path:
-            out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(".json")
+            out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(suffix)
         else:
-            out_path = vfb_path.with_suffix(".json")
-        write_json(reader, out_path)
+            out_path = vfb_path.with_suffix(suffix)
+        with codecs.open(str(out_path), "wb", "utf-8") as f:
+            json.dump(vfb.as_dict(), f, ensure_ascii=False, indent=4)
     else:
         parser.print_help()
 
 
 def vfb2ufo():
     parser = ArgumentParser(
         description=(
-            f"VFB3UFO Converter\nCopyright (c) 2022 by LucasFonts\nBuild {build_date}"
+            f"VFB3UFO Converter\nCopyright (c) 2023 by LucasFonts\nBuild {build_date}"
         )
     )
     parser.add_argument(
         "-p",
         "--path",
         type=str,
         nargs=1,
@@ -140,29 +160,32 @@
     )
     args = parser.parse_args()
     if args:
         vfb_path = Path(args.inputpath[0])
         if not args.silent:
             print(parser.description)
             print(f"Reading file {vfb_path} ...")
-        reader = read_vfb(vfb_path, minimal=args.minimal)
+        vfb = Vfb(
+            vfb_path, minimal=args.minimal, drop_keys={"Encoding", "Encoding Mac"}
+        )
         suffix = ".ufo"
-        # if args.zip:
-        #     suffix += "z"
+        if args.zip:
+            suffix += "z"
         if args.path:
             out_path = (Path(args.path[0]) / vfb_path.name).with_suffix(suffix)
         else:
             out_path = vfb_path.with_suffix(suffix)
-        writer = VfbToUfoWriter(
-            reader.data,
+        vfb.decompile()
+        builder = VfbToUfoBuilder(
+            vfb,
             minimal=args.minimal,
             base64=args.base64,
             pshints=not args.no_postscript_hints,
         )
-        writer.write(
+        builder.write(
             out_path,
             overwrite=args.force_overwrite,
             silent=args.silent,
-            ufoz=False,  # FIXME
+            ufoz=args.zip,
         )
     else:
         parser.print_help()
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/diff.py` & `vfbLib-0.5.0/Lib/vfbLib/diff.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 import json
 import logging
 
 from argparse import ArgumentParser
 from difflib import unified_diff, HtmlDiff
 from pathlib import Path
-from vfbLib import VFBReader
+from vfbLib.vfb.vfb import Vfb
 from vfbLib.version import build_date
 
 
 logger = logging.getLogger(__name__)
 
 
 def diffvfb():
@@ -39,20 +39,22 @@
     if not args:
         parser.print_help()
         return
 
     vfb1_path = Path(args.file1[0])
     vfb2_path = Path(args.file2[0])
 
-    vfb1 = VFBReader(vfb_path=vfb1_path, timing=False)
-    vfb2 = VFBReader(vfb_path=vfb2_path, timing=False)
+    vfb1 = Vfb(vfb_path=vfb1_path, timing=False)
+    vfb2 = Vfb(vfb_path=vfb2_path, timing=False)
     vfb1.read()
     vfb2.read()
-    vfb1_str = json.dumps(vfb1.data, ensure_ascii=False, indent=4).splitlines()
-    vfb2_str = json.dumps(vfb2.data, ensure_ascii=False, indent=4).splitlines()
+    vfb1.decompile()
+    vfb2.decompile()
+    vfb1_str = json.dumps(vfb1.as_dict(), ensure_ascii=False, indent=4).splitlines()
+    vfb2_str = json.dumps(vfb2.as_dict(), ensure_ascii=False, indent=4).splitlines()
     if args.html:
         html_diff = HtmlDiff()
         html = html_diff.make_file(
             vfb1_str, vfb2_str, str(vfb1_path), str(vfb2_path), context=True, numlines=5
         )
         with codecs.open(args.html[0], "wb", "utf-8") as f:
             f.write(html)
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/__init__.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 uint8 = 1
 uint16 = 2
 uint32 = 4
 
 
 class BaseParser:
     """
-    Base class to read data from a vfb file
+    Base class to parse data from a vfb file
     """
 
     master_count: int | None = None
     stream: BytesIO = BytesIO()
 
     @classmethod
     def parse(
@@ -43,27 +43,27 @@
         return hexStr(cls.stream.read())
 
     @classmethod
     def read_double(cls, stream=None):
         if stream is None:
             stream = cls.stream
         return read_doubles(1, stream)[0]
-    
+
     @classmethod
     def read_doubles(cls, num, stream=None):
         if stream is None:
             stream = cls.stream
         return read_doubles(num, stream)
 
     @classmethod
     def read_float(cls, stream=None):
         if stream is None:
             stream = cls.stream
         return read_floats(1, stream)[0]
-    
+
     @classmethod
     def read_floats(cls, num, stream=None):
         if stream is None:
             stream = cls.stream
         return read_floats(num, stream)
 
     @classmethod
@@ -182,15 +182,14 @@
             for a, b in zip(it, it)
         ]
 
 
 class GlyphEncodingParser(BaseParser):
     @classmethod
     def _parse(cls):
-        return 0  # FIXME: Encoding is ignored for now
         gid = int.from_bytes(cls.stream.read(2), byteorder="little")
         nam = cls.stream.read().decode("ascii")
         return gid, nam
 
 
 class OpenTypeClassFlagsParser(BaseParser):
     @classmethod
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/bitmap.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/bitmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/cmap.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/cmap.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/glyph.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/glyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,20 +154,22 @@
         y = int.from_bytes(stream.read(2), signed=True, byteorder="little")
         return {"x": x, "y": y}
 
 
 class GlyphParser(BaseParser):
     @classmethod
     def parse_guides(cls, stream: BytesIO, glyphdata: GlyphData, num_masters=1) -> None:
+        # Guidelines
         guides = parse_guides(stream, num_masters)
         if guides:
             glyphdata["guides"] = guides
 
     @classmethod
     def parse_binary(cls, stream: BytesIO, glyphdata: GlyphData) -> None:
+        # Imported binary TrueType data
         imported: Dict[str, Any] = {}
         while True:
             key = cls.read_uint8()
 
             if key == 0x28:
                 break
 
@@ -283,15 +285,17 @@
                 hints["hintmasks"] = hintmasks
 
         if hints["v"] or hints["h"] or "hintmasks" in hints:
             glyphdata["hints"] = hints
 
     @classmethod
     def parse_instructions(cls, stream: BytesIO, glyphdata: GlyphData) -> None:
-        _ = read_encoded_value(stream)  # XXX: What's this?
+        # Number of bytes for instructions that follow;
+        # we don't use it
+        _ = read_encoded_value(stream)
         num_commands = read_encoded_value(stream)
         commands: List[Instruction] = []
         for i in range(num_commands):
             cmd = cls.read_uint8(stream)
             params = [
                 read_encoded_value(stream)
                 for _ in range(len(TT_COMMANDS[cmd]["params"]))
@@ -322,22 +326,26 @@
             metrics.append(master_metrics)
         glyphdata["metrics"] = metrics
 
     @classmethod
     def parse_outlines(cls, stream: BytesIO, glyphdata: GlyphData) -> int:
         # Nodes
         num_masters = read_encoded_value(stream)
-        _ = read_encoded_value(stream)  # XXX: What's this?
-        num_nodes = read_encoded_value(stream)
         glyphdata["num_masters"] = num_masters
+
+        # 2 x the number of values to be read after num_nodes, the reason is unclear.
+        _ = read_encoded_value(stream)
+        # glyphdata["num_node_values"] = num_node_values
+
+        num_nodes = read_encoded_value(stream)
         segments: List[MMNode] = []
         x = [0 for _ in range(num_masters)]
         y = [0 for _ in range(num_masters)]
 
-        for i in range(num_nodes):
+        for _ in range(num_nodes):
             byte = cls.read_uint8(stream)
             flags = byte >> 4
             cmd = byte & 0x0F
 
             segment_type = cmd_name[cmd]
             # logger.debug(f"    {i}: {segment_type}, flags: {flags}")
 
@@ -397,15 +405,19 @@
             04 8c 92 89 8a
             8b 8b 8b
         0f
         """
         s = cls.stream
         glyphdata = GlyphData()
         start = unpack("<4B", s.read(4))
-        glyphdata["constants"] = start
+        if start != (1, 9, 7, 1):
+            logger.warning(
+                f"Unexpected glyph constant: {start}, please notify developer"
+            )
+        # glyphdata["constants"] = start
         num_masters = 1
         while True:
             # Read a value to decide what kind of information follows
             v = cls.read_uint8(s)
 
             if v == 0x01:
                 # Glyph name
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/guides.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/header.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/header.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from __future__ import annotations
 
 import logging
 
 from io import BufferedReader
-from typing import Any, Dict
+from typing import Any, Dict, Tuple
 from vfbLib.parsers import read_encoded_value, uint8, uint16
 
 
 logger = logging.getLogger(__name__)
 
 
 class VfbHeaderParser:
     stream: BufferedReader | None = None
 
     @classmethod
-    def parse(cls, stream: BufferedReader):
+    def parse(cls, stream: BufferedReader) -> Tuple[Dict[str, Any], int]:
         cls.stream = stream
         header: Dict[str, Any] = {}
         header["header0"] = cls.read_uint8()
         header["filetype"] = cls.stream.read(5).decode("cp1252")
         header["header1"] = cls.read_uint16()
         header["header2"] = cls.read_uint16()
         header["reserved"] = str(cls.stream.read(34))
         header["header3"] = cls.read_uint16()
         header["header4"] = cls.read_uint16()
         header["header5"] = cls.read_uint16()
         header["header6"] = cls.read_uint16()
         header["header7"] = cls.read_uint16()
-        header["header8"] = cls.read_uint16()
-        for i in range(9, 12):
-            key = cls.read_uint8()
-            val = read_encoded_value(stream)
-            header[f"header{i}"] = {key: val}
-
-        header["header12"] = cls.read_uint16()
-        header["header13"] = cls.read_uint16()
-        header["header14"] = cls.read_uint8()
+        if header["header7"] == 10:
+            # FL5 additions over FL3
+            header["header8"] = cls.read_uint16()
+            for i in range(9, 12):
+                key = cls.read_uint8()
+                val = read_encoded_value(stream)
+                header[f"header{i}"] = {key: val}
+            header["header12"] = cls.read_uint8()
+            header["header13"] = cls.read_uint16()
+        else:
+            header["header13"] = header["header7"]
+            del header["header7"]
+        header["header14"] = cls.read_uint16()
 
-        return header
+        # Get the size of the original binary data
+        datasize = cls.stream.tell()
+
+        return header, datasize
 
     @classmethod
     def read_uint8(cls) -> int:
         assert cls.stream is not None
         return int.from_bytes(cls.stream.read(uint8), byteorder="little", signed=False)
 
     @classmethod
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/mm.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/mm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import logging
 
-from struct import unpack
 from typing import Any, Dict, List, Tuple
 from vfbLib.parsers import BaseParser, read_encoded_value
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -40,15 +39,16 @@
         return [cls.read_uint32() for _ in range(4)]
 
 
 class AxisMappingsParser(BaseParser):
     @classmethod
     def _parse(cls) -> List[Tuple[float, float]]:
         # 10 pairs of (user, design) coordinates per axis.
-        # Look at "Axis Mappings Count" to find out which mappings are used in each axis.
+        # Look at "Axis Mappings Count" to find out which mappings are used in each
+        # axis.
         # The trailing unused fields may contain junk and must be ignored.
         assert cls.stream is not None
         mappings = []
         for _ in range(cls.stream.getbuffer().nbytes // 16):
             src_tgt = cls.read_doubles(2)
             mappings.append(src_tgt)
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/numeric.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/numeric.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/options.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/options.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/ps.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/ps.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/text.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/text.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/truetype.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/truetype.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/parsers/value.py` & `vfbLib-0.5.0/Lib/vfbLib/parsers/value.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,51 +5,36 @@
 
 
 def read_encoded_value(stream: BufferedReader | BytesIO, signed=True) -> int:
     val = int.from_bytes(stream.read(1), byteorder="little")
     if val == 0:
         raise EOFError
 
-    # logger.debug(f"Read: {hex(val)}")
-
     if val < 0x20:
-        # logger.debug(f"  Illegal value {hex(val)}. Rest of stream:")
-        # logger.debug(hexStr(stream.read()))
         raise ValueError
 
     elif val < 0xF7:
-        decoded = val - 0x8B
-        # logger.debug(f"  {hex(val)} - 0x8b = {val - 0x8b}")
-        return decoded
+        # -107 to 107, represented by 1 byte
+        return val - 0x8B
 
     elif val <= 0xFA:
+        # 108 to 1131, represented by 2 bytes
         val2 = int.from_bytes(stream.read(1), byteorder="little")
-        # logger.debug(f"  Read next: {hex(val2)}")
-        decoded = val - 0x8B + (val - 0xF7) * 0xFF + val2
-        # logger.debug(
-        #     f"    {hex(val)} - 0x8b + {val - 0xf7} * 0xff + {hex(val2)} = {decoded}"
-        # )
-        return decoded
+        # val - 0x8B + (val - 0xF7) * 0xFF + val2
+        return 0x100 * val - 0xF694 + val2
 
     elif val <= 0xFE:
-        # Negative
-        # FIXME
-
+        # -108 to -1131, represented by 2 bytes
         val2 = int.from_bytes(stream.read(1), byteorder="little")
-        # fb 1f -> 0x8f - 0xfb - 0x1f
-        decoded = 0x8F - val - (val - 0xFB) * 0xFF - val2
-        # logger.debug(
-        #     f"    0x8f - {hex(val)} - {val - 0xf7} * 0xff - {hex(val2)} = {decoded}"
-        # )
-        return decoded
+        # 0x8F - val - (val - 0xFB) * 0xFF - val2
+        return -0x100 * val + 0xFA94 - val2
 
     elif val == 0xFF:
         # 4-byte integer follows
         decoded = int.from_bytes(stream.read(4), byteorder="big", signed=signed)
-        # logger.debug(f"  Read next 4 bytes: {decoded}")
         return decoded
 
     raise ValueError
 
 
 def read_doubles(num, stream):
     # Read a number of doubles from the stream and return them
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/truetype.py` & `vfbLib-0.5.0/Lib/vfbLib/truetype.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,7 +46,10 @@
         "params": ["pt", "shift", "ppm1", "ppm2"],
     },
     0x17: {
         "name": "FDeltaV",
         "params": ["pt", "shift", "ppm1", "ppm2"],
     },
 }
+
+# TT command names to constants
+TT_COMMAND_CONSTANTS = {v["name"]: k for k, v in TT_COMMANDS.items()}
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/typing.py` & `vfbLib-0.5.0/Lib/vfbLib/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,24 @@
     carets: NotRequired[List[Tuple[int, int]]]
     glyph_class: NotRequired[str]
     unknown: NotRequired[List[int]]
 
 
 class GlyphData(TypedDict):
     components: NotRequired[List[Component]]
-    constants: NotRequired[Tuple[Any, ...]]
+    # constants: NotRequired[Tuple[Any, ...]]
     guides: NotRequired[GuideDict]
     hints: NotRequired[HintDict]
     imported: NotRequired[Any]  # FIXME
     kerning: NotRequired[Dict[int, List[int]]]
     metrics: NotRequired[List[Point]]
     name: NotRequired[str]
     nodes: NotRequired[List[MMNode]]
     num_masters: NotRequired[int]
+    # num_node_values: NotRequired[int]
     tth: NotRequired[List[Instruction]]
 
 
 class Guide(TypedDict):
     angle: float | int
     pos: int
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/__init__.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import logging
 
+from copy import deepcopy
 from fontTools.designspaceLib import (
     AxisDescriptor,
     AxisLabelDescriptor,
     DesignSpaceDocument,
 )
-from fontTools.ufoLib import UFOFileStructure, UFOWriter
-from fontTools.ufoLib.glifLib import GlyphSet
+from fontTools.ufoLib import UFOFileStructure
 from pathlib import Path
-from shutil import rmtree
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
+from ufoLib2.objects.font import Font
+from ufoLib2.objects.features import Features
 from ufonormalizer import normalizeUFO
-from vfbLib.ufo.designspace import get_ds_design_location, get_ds_location
+from vfbLib.ufo.designspace import get_ds_location
 from vfbLib.ufo.glyph import VfbToUfoGlyph
 from vfbLib.ufo.groups import transform_groups
 from vfbLib.ufo.guides import apply_guide_properties, get_master_guides
 from vfbLib.ufo.info import VfbToUfoInfo
 from vfbLib.ufo.kerning import UfoKerning
 from vfbLib.ufo.paths import UfoMasterGlyph
 from vfbLib.ufo.tth import TTGlyphHints, transform_stem_rounds
@@ -29,39 +30,40 @@
 )
 from vfbLib.ufo.vfb2ufo import TT_GLYPH_LIB_KEY, TT_LIB_KEY
 
 if TYPE_CHECKING:
     from fontTools.designspaceLib import DiscreteAxisDescriptor
     from vfbLib.typing import Anchor, ClassFlagDict, GuidePropertyList
     from vfbLib.ufo.typing import UfoGroups, UfoMMKerning
+    from vfbLib.vfb.vfb import Vfb
 
 
 logger = logging.getLogger(__name__)
 
 
-class VfbToUfoWriter:
+class VfbToUfoBuilder:
     def __init__(
         self,
-        json: List[List[Any]],
+        vfb: Vfb,
         minimal=False,
         base64=False,
         pshints=True,
     ) -> None:
         """
         Serialize the JSON structure to UFO(s)
         """
         self.axes: List[AxisDescriptor | DiscreteAxisDescriptor] = []
         self.axis_count = 0
-        self.json = json
+        self.vfb = vfb
         self.minimal = minimal
         self.encode_data_base64 = base64
         self.include_ps_hints = pshints
 
         self.features_classes = ""
-        self.features = ""
+        self.features_code = ""
         self.groups: UfoGroups = {}
         self.guide_properties: GuidePropertyList = []
         self.info = VfbToUfoInfo()
         self.kerning_class_flags: ClassFlagDict = {}
         self.num_blue_values = 0
         self.num_other_blues = 0
         self.num_family_blues = 0
@@ -86,15 +88,16 @@
         self.tt_zone_names: List[str] = []
         self.zone_names: Dict[str, List[str]] = {}
         self.build()
 
     def add_axis_mappings(self, data: List[Tuple[float, float]]) -> None:
         if not self.axis_mappings_count:
             raise ValueError(
-                "If axis mappings are present, axis mappings count must be set before parsing them."
+                "If axis mappings are present, axis mappings count must be set before "
+                "parsing them."
             )
         for i in range(self.axis_count):
             # Get the number of mappings for the current axis
             n = self.axis_mappings_count[i]
             if n > 0:
                 # Use only n mappings out of 10 for the current axis
                 mappings = data[:n]
@@ -292,16 +295,21 @@
     def build_tt_zones_lib(self) -> None:
         self.assure_tt_lib()
         if self.tt_zones:
             self.lib[TT_LIB_KEY]["zones"] = self.tt_zones
 
     def build(self) -> None:  # noqa: C901
         # Non-MM data
-        for e in self.json:
-            name, data = e
+        for e in self.vfb.entries:
+            name = e.key
+            if name is None:
+                raise TypeError
+            data = e.decompiled
+            if data is None:
+                continue
 
             # Font Info
             attr = self.info.mapping.get(name, None)
             if attr is not None:
                 self.info.set_attr(attr, data)
                 continue
 
@@ -349,15 +357,15 @@
             elif name == "TrueType Zone Deltas":  # 1273
                 self.set_tt_zone_deltas(data)
             elif name == "Zone Stop PPEM":  # 1274
                 self.set_tt_zone_stop(data)
             elif name == "Code Stop PPEM":  # 1275
                 self.set_tt_code_stop(data)
             elif name == "openTypeFeatures":  # 1276
-                self.features = "\n".join(data)
+                self.features_code = "\n".join(data)
             elif name == "OpenType Class":  # 1277
                 self.add_ot_class(data)
             elif name == "Global Guides":  # 1294
                 self.mm_guides = data
             elif name == "Global Guide Properties":  # 1296
                 self.guide_properties = data
             elif name == "Encoding":  # 1500
@@ -499,14 +507,15 @@
         self.build_tt_stems_lib()
         self.build_tt_zones_lib()
         if not self.lib[TT_LIB_KEY]:
             del self.lib[TT_LIB_KEY]
         self.info.fix_underline_position()
 
     def get_master_info(self, master_index: int = 0) -> VfbToUfoInfo:
+        master_info = deepcopy(self.info)
         # Update the info with master-specific values
         properties = [
             ("ascender", "ascender"),
             ("descender", "descender"),
             ("x_height", "xHeight"),
             ("cap_height", "capHeight"),
         ]
@@ -519,21 +528,21 @@
                     ("blue_fuzz", "postscriptBlueFuzz"),
                 ]
             )
 
         for key, attr in properties:
             value = self.masters_ps_info[master_index].get(key, None)
             if value is not None:
-                setattr(self.info, attr, value)
+                setattr(master_info, attr, value)
 
         if self.include_ps_hints:
             # Set "force bold"
             value = self.masters_ps_info[master_index].get("force_bold", None)
             if value is not None:
-                self.info.postscriptForceBold = bool(value)
+                master_info.postscriptForceBold = bool(value)
 
             # Set attributes that must be clipped at a certain index
             for key, attr in (
                 ("blue_values", "postscriptBlueValues"),
                 ("other_blues", "postscriptOtherBlues"),
                 ("family_blues", "postscriptFamilyBlues"),
                 ("family_other_blues", "postscriptFamilyOtherBlues"),
@@ -543,47 +552,130 @@
                 # Get the number of values from the corresponding attribute
                 num_values = getattr(self, f"num_{key}")
                 if num_values == 0:
                     continue
 
                 value = self.masters_ps_info[master_index].get(key, None)
                 if value is not None:
-                    setattr(self.info, attr, value[:num_values])
+                    setattr(master_info, attr, value[:num_values])
 
         # Guides
         if not self.minimal and self.mm_guides is not None:
             guides = get_master_guides(self.mm_guides, master_index)
             apply_guide_properties(guides, self.guide_properties)
 
             if guides:
-                self.info.guidelines = guides
+                master_info.guidelines = guides
 
-        return self.info
+        return master_info
 
-    def write(self, out_path: Path, overwrite=False, silent=False, ufoz=False) -> None:
+    def get_ufo_master(self, index: int, silent=False) -> Font:
+        if not silent:
+            print(f"Processing font: {self.info.ui_name.strip()}, master {index}")
+
+        # Build the master-specific data that can be passed when instantiating the UFO
+        master_kerning = self.ufo_kerning.get_master_kerning(master_index=index)
+        master_info = self.get_master_info(master_index=index)
+
+        # Pass as much data right to the UFO
+        ufo = Font(
+            features=self.ufo_features.text,
+            groups=deepcopy(self.ufo_groups),
+            info=master_info,
+            kerning=master_kerning,
+            lib=self.lib,
+        )
+
+        # Add the glyphs
+        for name, mm_glyph in self.glyph_masters.items():
+            logger.debug(f"    {name}, {type(name)}, {mm_glyph}")
+            # TODO: Any way to use the ufoLib2 Glyph directly?
+            master_glyph = UfoMasterGlyph(mm_glyph, self.glyphOrder, index)
+            master_glyph.build(
+                self.minimal, self.include_ps_hints, self.encode_data_base64
+            )
+            ufo_glyph = ufo.newGlyph(name)
+            pen = ufo_glyph.getPointPen()
+            master_glyph.drawPoints(pen)
+            # FIXME: Anchors work, but typing wrong
+            ufo_glyph.anchors = master_glyph.anchors
+            ufo_glyph.guidelines = master_glyph.guidelines
+            ufo_glyph.height = master_glyph.height
+            ufo_glyph.lib = master_glyph.lib
+            ufo_glyph.width = master_glyph.width
+            ufo_glyph.unicodes = master_glyph.unicodes
+
+        return ufo
+
+    def get_ufo_masters(self, silent=False) -> List[Font]:
+        # Prepare data shared by the master UFOs
         self.ufo_groups = transform_groups(
             self.groups,
             self.kerning_class_flags,
             self.glyphOrder,
             self.minimal,
         )
         self.ufo_kerning = UfoKerning(self.glyphOrder, self.ufo_groups, self.mm_kerning)
         self.ufo_groups = self.ufo_kerning.groups
+        self.ufo_features = Features(self.features_code)
+        if self.features_classes:
+            self.ufo_features.text = self.features_classes + "\n\n" + self.features_code
+
+        ufo_masters = []
         for i in range(len(self.masters)):
-            self.write_master(i, out_path, overwrite, silent, ufoz)
+            ufo_masters.append(self.get_ufo_master(i, silent))
+        return ufo_masters
+
+    def get_ufos_designspace(
+        self, out_path: Path, silent=False
+    ) -> Tuple[List[Font], DesignSpaceDocument | None]:
+        """
+        Build UFOs and a DesignSpaceDocument from the VFB contents in memory and return
+        them. The DesignSpaceDocument is only returned for VFBs containing more than one
+        master. In other cases, the second element of the returned tuple is None.
+        """
+        ufo_masters = self.get_ufo_masters(silent)
+        ds: DesignSpaceDocument | None = None
         if self.axes:
-            self.write_designspace(
-                out_path.with_suffix(".designspace"), overwrite, silent
-            )
+            ds = self.get_designspace(out_path)
+        return ufo_masters, ds
+
+    def write(self, out_path: Path, overwrite=False, silent=False, ufoz=False) -> None:
+        """
+        Write a the VFB contents to master UFOs and a designspace file. The designspace
+        file is only written if the VFB contains more than one master.
+        """
+        # Build UFOs and DesignSpace
+        ufos, ds = self.get_ufos_designspace(out_path, silent)
+
+        # Write the master UFOs
+        strct = UFOFileStructure.ZIP if ufoz else None
+        for index, ufo in enumerate(ufos):
+            master_path = self.get_master_path(out_path, index)
+            ufo.save(master_path, structure=strct, overwrite=overwrite)
+            if not ufoz:
+                normalizeUFO(
+                    ufoPath=master_path, onlyModified=False, writeModTimes=False
+                )
 
-    def write_designspace(self, out_path: Path, overwrite=False, silent=False) -> None:
-        if out_path.exists():
-            if not overwrite:
-                raise FileExistsError(str(out_path))
+        # Write the Designspace
+        if ds:
+            ds_path = out_path.with_suffix(".designspace")
+            if ds_path.exists():
+                if not overwrite:
+                    raise FileExistsError(str(ds_path))
+            if not silent:
+                print(f"Writing designspace: {ds_path}")
+            ds.write(str(ds_path))
 
+    def get_designspace(self, out_path: Path) -> DesignSpaceDocument:
+        """
+        Build and return a DesignSpaceDocument. The out_path argument will be used to
+        construct the UFO paths assigned to the source descriptors.
+        """
         ds = DesignSpaceDocument()
         ds.axes = self.axes
 
         # Add labels
         if self.axis_count == 1:
             # Only support the simple case here
             for p in self.primary_instances:
@@ -620,76 +712,20 @@
                 # designLocation=get_ds_design_location(self.axes, loc),
                 familyName=self.info.ds_family_name,
                 filename=f"instance_ufo/{self.info.ds_family_name}-{style_name}.ufo",
                 # lib=,
                 # locationLabel="",
                 name=f"instance_{i}",
                 # postScriptFontName="",
-                styleMapFamilyName=f"{self.info.ds_family_name} {style_name}".strip(),  # FIXME
+                # FIXME:
+                styleMapFamilyName=f"{self.info.ds_family_name} {style_name}".strip(),
                 styleMapStyleName=self.info.styleMapStyleName,
                 styleName=style_name,
                 userLocation=get_ds_location(self.axes, loc, 1),
             )
 
-        if not silent:
-            print(f"Writing designspace: {out_path}")
-
-        ds.write(str(out_path))
+        return ds
 
     def get_master_path(self, out_path: Path, master_index: int) -> Path:
         if master_index > 0:
             return out_path.with_stem(f"{out_path.stem}-{master_index}")
         return out_path
-
-    def write_master(
-        self, index: int, out_path: Path, overwrite=False, silent=False, ufoz=False
-    ) -> None:
-        master_path = self.get_master_path(out_path, index)
-
-        if master_path.exists():
-            if overwrite:
-                rmtree(master_path)
-            else:
-                raise FileExistsError(str(master_path))
-
-        if not silent:
-            print(f"Processing font: {self.info.ui_name.strip()}, master {index}")
-
-        strct = UFOFileStructure.ZIP if ufoz else None
-        writer = UFOWriter(
-            master_path, fileCreator="com.lucasfonts.vfb3ufo", structure=strct
-        )
-        # FIXME: In ufoz, we can't make a directory
-        glyphs_path = master_path / "glyphs"
-        glyphs_path.mkdir()
-        self.glyph_set = GlyphSet(glyphs_path)
-        for name, mm_glyph in self.glyph_masters.items():
-            logger.debug(f"    {name}, {type(name)}, {mm_glyph}")
-            master_glyph = UfoMasterGlyph(mm_glyph, self.glyphOrder, index)
-            master_glyph.build(
-                self.minimal, self.include_ps_hints, self.encode_data_base64
-            )
-            self.glyph_set.writeGlyph(
-                name, glyphObject=master_glyph, drawPointsFunc=master_glyph.draw_glyph
-            )
-
-        self.glyph_set.writeContents()
-        self.glyph_set.writeLayerInfo(writer.getGlyphSet())
-
-        writer.writeLayerContents()
-        writer.writeGroups(self.ufo_groups)
-
-        master_info = self.get_master_info(master_index=index)
-        writer.writeInfo(master_info)
-
-        self.ufo_kerning.extract_master_kerning(master_index=index)
-        writer.writeKerning(self.ufo_kerning.master_kerning)
-
-        if self.features:
-            if self.features_classes:
-                features = self.features_classes + "\n\n" + self.features
-            else:
-                features = self.features
-            writer.writeFeatures(features)
-        writer.writeLib(self.lib)
-        writer.close()
-        normalizeUFO(ufoPath=str(master_path), onlyModified=False, writeModTimes=False)
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/designspace.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/designspace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-import logging
-
 from typing import TYPE_CHECKING, Dict, List
 
 if TYPE_CHECKING:
     from fontTools.designspaceLib import (
         AxisDescriptor,
         DiscreteAxisDescriptor,
     )
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/glyph.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/glyph.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/groups.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/groups.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/guides.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/guides.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/helpers.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/helpers.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/info.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
 import logging
 
 from functools import cached_property
 from typing import TYPE_CHECKING, List, Tuple
+from ufoLib2.objects.info import Info, WidthClass
 from vfbLib.helpers import binaryToIntList
 from vfbLib.ufo.time import convert_timestamp
 from vfbLib.ufo.typing import TUfoGaspRecDict
 
 
 if TYPE_CHECKING:
     from vfbLib.typing import GaspList
     from vfbLib.ufo.typing import UfoGuide
 
 
 logger = logging.getLogger(__name__)
 
 
-class VfbToUfoInfo:
+class VfbToUfoInfo(Info):
     def __init__(self) -> None:
+        super(VfbToUfoInfo, self).__init__()
         # Chance to set some defaults that should always be written
         self.familyName = "Untitled"
         self.guidelines: List[UfoGuide] = []
         self.italicAngle: float | int = 0
         self.openTypeGaspRangeRecords: List[TUfoGaspRecDict] = []
         self.openTypeHeadCreated: str | None = None
         self.openTypeHeadFlags: List[int] = []
@@ -44,15 +46,15 @@
         self.openTypeOS2SuperscriptXOffset = 0
         self.openTypeOS2SuperscriptYOffset = 0
         self.openTypeOS2StrikeoutPosition = 0
         self.openTypeOS2StrikeoutSize = 0
         self.openTypeOS2Type: List[int] = []
         self.openTypeOS2UnicodeRanges: List[int] = []
         self.openTypeOS2WeightClass = 400
-        self.openTypeOS2WidthClass = 5
+        self.openTypeOS2WidthClass = WidthClass(5)
         self.postscriptBlueValues: List[int] = []
         self.postscriptFamilyBlues: List[int] = []
         self.postscriptFamilyOtherBlues: List[int] = []
         self.postscriptFontName = "Untitled-Regular"
         self.postscriptForceBold = False
         self.postscriptFullName = "Untitled Regular"
         self.postscriptIsFixedPitch = False
@@ -73,25 +75,31 @@
         self.openTypeOS2TypoDescender = 0
         self.openTypeOS2TypoLineGap = 0
         self.openTypeOS2WinAscent = 0
         self.openTypeOS2WinDescent = 0
         self.openTypeOS2CodePageRanges: List[int] = []
 
         self.build_mapping()
-    
+
     @cached_property
-    def ds_family_name(self) -> str:
+    def ds_family_name(self) -> str | None:
+        """
+        Return the family name for use in the DesignSpaceDocument.
+        """
         if self.openTypeNamePreferredFamilyName:
             return self.openTypeNamePreferredFamilyName
         if self.familyName:
             return self.familyName
         return self.styleMapFamilyName
-    
+
     @cached_property
-    def ds_style_name(self) -> str:
+    def ds_style_name(self) -> str | None:
+        """
+        Return the style name for use in the DesignSpaceDocument.
+        """
         if self.openTypeNamePreferredSubfamilyName:
             return self.openTypeNamePreferredSubfamilyName
         if self.styleName:
             return self.styleName
         return self.styleMapStyleName
 
     @cached_property
@@ -170,14 +178,23 @@
             "OpenTypeOS2WinAscent": "openTypeOS2WinAscent",
             "OpenTypeOS2WinDescent": "openTypeOS2WinDescent",
         }
 
     def fix_underline_position(self):
         # VFB stores middle of line and thickness, but spec says it must be
         # stored as top of line and thickness.
+        if (
+            self.postscriptUnderlinePosition is None
+            or self.postscriptUnderlineThickness is None
+        ):
+            logger.error(
+                "Can't fix underline position because position or thickness is None"
+            )
+            return
+
         self.postscriptUnderlinePosition += int(
             round(0.5 * self.postscriptUnderlineThickness)
         )
 
     def set_attr(self, attr: str, data):
         setattr(self, attr, data)
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/kerning.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/kerning.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         groups: UfoGroups,
         mm_kerning: UfoMMKerning,
     ):
         self.glyph_order = glyph_order
         group_info = build_glyph_to_group_maps(groups)
         self.groups, self.glyph_group_1, self.glyph_group_2 = group_info
         self.mm_kerning = mm_kerning
-        self.master_kerning: UfoMasterKerning = {}
         self._make_name_based_kerning()
 
     def _is_exception(self, L: str, R: str):
         L_is_key = f"public.kern1.{L}" in self.groups or L not in self.glyph_group_1
 
         R_is_key = f"public.kern2.{R}" in self.groups or R not in self.glyph_group_2
 
@@ -55,16 +54,18 @@
 
             # Is the right glyph a keyglyph?
             right_group = f"public.kern2.{R}"
             right = right_group if right_group in self.groups else R
 
             self.mm_kerning_names[left, right] = values
 
-    def extract_master_kerning(self, master_index) -> None:
+    def get_master_kerning(self, master_index: int) -> UfoMasterKerning:
         """
-        Extract the kerning value for master_index.
+        Extract the kerning values for master_index and return the kerning as
+        Dict[Tuple[str, str], int].
         """
-        self.master_kerning = {}
+        master_kerning: UfoMasterKerning = {}
         for pair, values in self.mm_kerning_names.items():
             value = values[master_index]
             if value != 0 or self._is_exception(*pair):
-                self.master_kerning[pair] = value
+                master_kerning[pair] = value
+        return master_kerning
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/paths.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, List, TYPE_CHECKING
 from vfbLib.ufo.guides import apply_guide_properties, get_master_guides
 from vfbLib.ufo.pshints import build_ps_glyph_hints, get_master_hints
 from vfbLib.ufo.tth import set_tth_lib
 from vfbLib.ufo.vfb2ufo import TT_GLYPH_LIB_KEY
 
 if TYPE_CHECKING:
-    from fontTools.ufoLib.glifLib import GLIFPointPen
+    from fontTools.pens.pointPen import AbstractPointPen
     from vfbLib.typing import Anchor
     from vfbLib.ufo.glyph import VfbToUfoGlyph
     from vfbLib.ufo.typing import UfoComponent, UfoContour
 
 
 logger = logging.getLogger(__name__)
 
@@ -62,29 +62,29 @@
         self._extract_master_tt_hints()
         self._extract_master_contours()
         self._finalize_point_labels(include_ps_hints)
         self._extract_master_anchors()
         if not minimal:
             self._extract_master_guides()
         self._finalize_lib(encode_data_base64)
-        self.unicodes = self.mm_glyph.unicodes
+        self.unicodes = self.mm_glyph.unicodes.copy()
         self.width, self.height = self.mm_glyph.mm_metrics[self.master_index]
 
-    def draw_glyph(self, pen: GLIFPointPen) -> None:
+    def drawPoints(self, pen: AbstractPointPen) -> None:
         """
-        Draw the glyph to the supplied point pen.
+        Draw the glyph onto the supplied point pen.
         """
         for contour in self.contours:
             pen.beginPath()
             for segment_type, smooth, name, pt in contour:
                 pen.addPoint(pt, segment_type, name=name, smooth=smooth)
             pen.endPath()
 
         for gn, tr in self.components:
-            pen.addComponent(glyphName=gn, transformation=tr)
+            pen.addComponent(gn, tr)
 
     def _extract_master_anchors(self) -> None:
         if self.mm_glyph.anchors is None:
             return
 
         # Copy anchors from the mm glyph
         self.anchors = deepcopy(self.mm_glyph.anchors)
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/pshints.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/pshints.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/tth.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/tth.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,24 @@
                     stem = params["stem"]
                     if stem <= -2:
                         d["round"] = True
                     elif stem == -1:
                         pass
                     else:
                         stem_dir = "ttStemsH" if code.endswith("H") else "ttStemsV"
+                        if stem >= len(self.stems[stem_dir]):
+                            logger.warning(
+                                f"Stem index in {stem_dir} out of range in "
+                                f"{self.glyph.name}: {stem} (of "
+                                f"{len(self.stems[stem_dir])} existing stems). "
+                                "Choosing first stem."
+                            )
+                            logger.warning(f"{code}: {params}")
+                            logger.warning(self.stems[stem_dir])
+                            stem = 0
                         d["stem"] = self.stems[stem_dir][stem]["name"]
                 if "align" in params:
                     align = params["align"]
                     if align > -1:
                         d["align"] = vfb2ufo_alignment_rev[align]
             elif code in (
                 "InterpolateH",
```

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/typing.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/typing.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib/ufo/vfb2ufo.py` & `vfbLib-0.5.0/Lib/vfbLib/ufo/vfb2ufo.py`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/Lib/vfbLib.egg-info/PKG-INFO` & `vfbLib-0.5.0/Lib/vfbLib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.4.6
+Version: 0.5.0
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -56,38 +56,35 @@
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
 usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2022 by LucasFonts Build 2022-12-12
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  output folder
   -fo, --force-overwrite
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
-
-Additional options:
-
-  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
+  -z, --zip             write UFOZ (compressed UFO)
+  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
 
-Unimplemented options:
+Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
-  -z, --zip             write UFOZ (compressed UFO)
 ```
 
 
 ### vfb2json
 
 Generate a representation that closely adheres to the VFB structure.
 
@@ -97,36 +94,67 @@
 
 will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
-usage: vfb2json [-h] [-m] [-p PATH] inputpath
+usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
 
-VFB2JSON Converter Copyright (c) 2022 by LucasFonts Build 2022-11-08
+VFB2JSON Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
 
 options:
   -h, --help            show this help message and exit
+  -d, --no-decompile    don't decompile data, output binary in JSON
+  --header              only read the VFB header, not the actual data
   -m, --minimal         parse only minimal amount of data
   -p PATH, --path PATH  output folder
 ```
 
 
+### vfbcu2qu
+
+Convert a VFB file to quadratic using the `cu2qu` library. Single master only.
+
+```bash
+$ vfbcu2qu MyFile.vfb
+```
+
+will convert the file and save it with the suffix `.qu.vfb` in the same directory.
+
+```
+usage: vfbcu2qu [-h] [-p PATH] [-fo] [-m MAX_ERR_EM] inputpath [outputpath]
+
+VFB Cubic to Quadratic Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+
+positional arguments:
+  inputpath             input file path (.vfb)
+  outputpath            output file path (.vfb)
+
+options:
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  output folder
+  -fo, --force-overwrite
+                        force overwrite
+  -m MAX_ERR_EM, --max-err-em MAX_ERR_EM
+                        Maximum allowed error, relative to the font's units per em.
+```
+
+
 ### diffvfb
 
 Generate a diff of two VFB files, either in unified diff or HTML format.
 
 ```
 usage: diffvfb [-h] [--html HTML] file1 file2
 
-diffvfb Copyright (c) 2023 by LucasFonts Build 2023-03-14
+diffvfb Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   file1        First input file path (.vfb)
   file2        Second input file path (.vfb)
 
 options:
   -h, --help   show this help message and exit
```

### Comparing `vfbLib-0.4.6/PKG-INFO` & `vfbLib-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfbLib
-Version: 0.4.6
+Version: 0.5.0
 Summary: Tools for converting FontLab Studio 5 (VFB) files.
 Home-page: https://pypi.org/project/vfblib/
 Author: Jens Kutilek
 License: MIT
 Project-URL: Source, https://github.com/LucasFonts/vfbLib
 Project-URL: Tracker, https://github.com/LucasFonts/vfbLib/issues
 Classifier: Programming Language :: Python :: 3
@@ -56,38 +56,35 @@
 will convert the file to `MyFile.ufo` in the same directory. Existing files will
 not be overwritten unless you specify the `-fo` option.
 
 ```
 vfb3ufo -h
 usage: vfb3ufo [-h] [-p PATH] [-fo] [-ttx] [-64] [-s] [-nops] [-z] [-m] inputpath [outputpath]
 
-VFB3UFO Converter Copyright (c) 2022 by LucasFonts Build 2022-12-12
+VFB3UFO Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
   outputpath            output file path (.ufo[z])
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  output folder
   -fo, --force-overwrite
                         force overwrite
   -64, --base64         write GLIF lib 'data' section using base64 (recommended)
   -s, --silent          no display (silent mode)
-
-Additional options:
-
-  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
   -nops, --no-postscript-hints
                         Don't output PostScript hinting
+  -z, --zip             write UFOZ (compressed UFO)
+  -m, --minimal         parse only minimal amount of data, drop missing glyphs from groups, etc.
 
-Unimplemented options:
+Not yet implemented options:
 
   -ttx, --ttx           convert binary OpenType Layout data using TTX-like format
-  -z, --zip             write UFOZ (compressed UFO)
 ```
 
 
 ### vfb2json
 
 Generate a representation that closely adheres to the VFB structure.
 
@@ -97,36 +94,67 @@
 
 will convert the file to `MyFile.json` in the same directory. Existing files will be overwritten.
 
 We expect this to be mostly used for debugging purposes.
 
 ```
 vfb2json -h
-usage: vfb2json [-h] [-m] [-p PATH] inputpath
+usage: vfb2json [-h] [-d] [--header] [-m] [-p PATH] inputpath
 
-VFB2JSON Converter Copyright (c) 2022 by LucasFonts Build 2022-11-08
+VFB2JSON Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   inputpath             input file path (.vfb)
 
 options:
   -h, --help            show this help message and exit
+  -d, --no-decompile    don't decompile data, output binary in JSON
+  --header              only read the VFB header, not the actual data
   -m, --minimal         parse only minimal amount of data
   -p PATH, --path PATH  output folder
 ```
 
 
+### vfbcu2qu
+
+Convert a VFB file to quadratic using the `cu2qu` library. Single master only.
+
+```bash
+$ vfbcu2qu MyFile.vfb
+```
+
+will convert the file and save it with the suffix `.qu.vfb` in the same directory.
+
+```
+usage: vfbcu2qu [-h] [-p PATH] [-fo] [-m MAX_ERR_EM] inputpath [outputpath]
+
+VFB Cubic to Quadratic Converter Copyright (c) 2023 by LucasFonts Build 2023-07-18
+
+positional arguments:
+  inputpath             input file path (.vfb)
+  outputpath            output file path (.vfb)
+
+options:
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  output folder
+  -fo, --force-overwrite
+                        force overwrite
+  -m MAX_ERR_EM, --max-err-em MAX_ERR_EM
+                        Maximum allowed error, relative to the font's units per em.
+```
+
+
 ### diffvfb
 
 Generate a diff of two VFB files, either in unified diff or HTML format.
 
 ```
 usage: diffvfb [-h] [--html HTML] file1 file2
 
-diffvfb Copyright (c) 2023 by LucasFonts Build 2023-03-14
+diffvfb Copyright (c) 2023 by LucasFonts Build 2023-07-18
 
 positional arguments:
   file1        First input file path (.vfb)
   file2        Second input file path (.vfb)
 
 options:
   -h, --help   show this help message and exit
```

### Comparing `vfbLib-0.4.6/README.md` & `vfbLib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vfbLib-0.4.6/setup.cfg` & `vfbLib-0.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vfbLib
-version = 0.4.6
+version = 0.5.0
 description = Tools for converting FontLab Studio 5 (VFB) files.
 long_description = file: DESCRIPTION.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://pypi.org/project/vfblib/
 author = Jens Kutilek
 license = MIT
 license_file = LICENSE
@@ -20,32 +20,35 @@
 [options]
 zip_safe = False
 package_dir = 
 	=Lib
 packages = find:
 platforms = any
 install_requires = 
-	defcon
-	fonttools[ufo]
+	defcon >= 0.10.2
+	fonttools[ufo] >= 4.40.0
 	typing_extensions
-	ufonormalizer
+	ufonormalizer >= 0.6.1
+	ufoLib2 >= 0.14.0
 python_requires = >=3.8
 
 [options.packages.find]
 where = Lib
 
 [bdist_wheel]
 universal = 1
 
 [options.entry_points]
 console_scripts = 
 	diffvfb = vfbLib.diff:diffvfb
 	vfb2json = vfbLib.cmdline:vfb2json
 	vfb3ufo = vfbLib.cmdline:vfb2ufo
+	vfbcu2qu = vfbLib.cu2qu:vfbcu2qu
 	normalize_vfb2ufo = vfbLib.ufo.helpers:normalize
+	yuri = vfbLib.value:yuri
 
 [flake8]
 select = B, C, E, F, W, T4, B9
 ignore = W503
 max-line-length = 88
 max-complexity = 19
 exclude = .git, __pycache__, build, dist, .eggs, .tox
```

