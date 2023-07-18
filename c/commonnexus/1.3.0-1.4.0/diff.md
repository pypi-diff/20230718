# Comparing `tmp/commonnexus-1.3.0.tar.gz` & `tmp/commonnexus-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonnexus-1.3.0.tar", last modified: Wed May 17 06:36:13 2023, max compression
+gzip compressed data, was "commonnexus-1.4.0.tar", last modified: Tue Jul 18 11:26:33 2023, max compression
```

## Comparing `commonnexus-1.3.0.tar` & `commonnexus-1.4.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2023-02-08 09:11:27.000000 commonnexus-1.3.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)     4659 2023-05-17 06:36:13.753529 commonnexus-1.3.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     3106 2023-03-14 06:35:07.000000 commonnexus-1.3.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)     2441 2023-05-17 06:36:13.753529 commonnexus-1.3.0/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2023-02-08 09:14:01.000000 commonnexus-1.3.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/
--rw-rw-r--   0 robert    (1000) robert    (1000)      121 2023-05-17 06:35:26.000000 commonnexus-1.3.0/src/commonnexus/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4361 2023-03-04 14:48:53.000000 commonnexus-1.3.0/src/commonnexus/__main__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      189 2023-03-15 10:02:49.000000 commonnexus-1.3.0/src/commonnexus/_compat.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/blocks/
--rw-rw-r--   0 robert    (1000) robert    (1000)      602 2023-03-05 14:33:36.000000 commonnexus-1.3.0/src/commonnexus/blocks/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11215 2023-02-14 14:50:23.000000 commonnexus-1.3.0/src/commonnexus/blocks/assumptions.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7979 2023-03-08 10:40:36.000000 commonnexus-1.3.0/src/commonnexus/blocks/base.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    57499 2023-03-13 15:54:49.000000 commonnexus-1.3.0/src/commonnexus/blocks/characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7365 2023-02-16 11:10:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/codons.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    15853 2023-03-08 09:06:05.000000 commonnexus-1.3.0/src/commonnexus/blocks/distances.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8333 2023-03-13 07:11:10.000000 commonnexus-1.3.0/src/commonnexus/blocks/notes.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     7699 2023-02-14 12:01:40.000000 commonnexus-1.3.0/src/commonnexus/blocks/sets.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3040 2023-03-07 08:22:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/taxa.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    17067 2023-05-15 14:44:35.000000 commonnexus-1.3.0/src/commonnexus/blocks/trees.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2240 2023-02-16 11:10:00.000000 commonnexus-1.3.0/src/commonnexus/blocks/unaligned.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3710 2023-03-13 14:04:48.000000 commonnexus-1.3.0/src/commonnexus/cli_util.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4318 2023-03-08 10:24:09.000000 commonnexus-1.3.0/src/commonnexus/command.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/commands/
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2023-03-02 07:16:22.000000 commonnexus-1.3.0/src/commonnexus/commands/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5977 2023-03-10 08:48:03.000000 commonnexus-1.3.0/src/commonnexus/commands/characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      530 2023-03-02 09:45:35.000000 commonnexus-1.3.0/src/commonnexus/commands/combine.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      316 2023-03-04 14:51:27.000000 commonnexus-1.3.0/src/commonnexus/commands/help.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      349 2023-03-06 11:27:02.000000 commonnexus-1.3.0/src/commonnexus/commands/normalise.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1201 2023-03-10 11:18:14.000000 commonnexus-1.3.0/src/commonnexus/commands/split.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8705 2023-03-13 14:05:09.000000 commonnexus-1.3.0/src/commonnexus/commands/taxa.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3174 2023-03-13 14:15:33.000000 commonnexus-1.3.0/src/commonnexus/commands/trees.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    17585 2023-03-10 14:17:53.000000 commonnexus-1.3.0/src/commonnexus/nexus.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11459 2023-03-08 14:41:35.000000 commonnexus-1.3.0/src/commonnexus/tokenizer.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus/tools/
--rw-rw-r--   0 robert    (1000) robert    (1000)      213 2023-03-02 07:36:37.000000 commonnexus-1.3.0/src/commonnexus/tools/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3061 2023-03-07 09:13:58.000000 commonnexus-1.3.0/src/commonnexus/tools/combine.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11492 2023-03-10 08:40:51.000000 commonnexus-1.3.0/src/commonnexus/tools/matrix.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     4137 2023-03-09 12:21:29.000000 commonnexus-1.3.0/src/commonnexus/tools/normalise.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      168 2023-02-16 08:50:17.000000 commonnexus-1.3.0/src/commonnexus/util.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-05-17 06:36:13.753529 commonnexus-1.3.0/src/commonnexus.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)     4659 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1316 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       58 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/entry_points.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-02-08 09:38:01.000000 commonnexus-1.3.0/src/commonnexus.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      220 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       12 2023-05-17 06:36:13.000000 commonnexus-1.3.0/src/commonnexus.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2023-02-08 09:11:27.000000 commonnexus-1.4.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4609 2023-07-18 11:26:33.223477 commonnexus-1.4.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3106 2023-03-14 06:35:07.000000 commonnexus-1.4.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2398 2023-07-18 11:26:33.223477 commonnexus-1.4.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2023-02-08 09:14:01.000000 commonnexus-1.4.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/commonnexus/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      121 2023-07-18 11:24:54.000000 commonnexus-1.4.0/src/commonnexus/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4361 2023-03-04 14:48:53.000000 commonnexus-1.4.0/src/commonnexus/__main__.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/commonnexus/blocks/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      602 2023-03-05 14:33:36.000000 commonnexus-1.4.0/src/commonnexus/blocks/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11215 2023-02-14 14:50:23.000000 commonnexus-1.4.0/src/commonnexus/blocks/assumptions.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7988 2023-06-29 08:02:04.000000 commonnexus-1.4.0/src/commonnexus/blocks/base.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    59647 2023-07-18 07:05:10.000000 commonnexus-1.4.0/src/commonnexus/blocks/characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7365 2023-02-16 11:10:00.000000 commonnexus-1.4.0/src/commonnexus/blocks/codons.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    15853 2023-03-08 09:06:05.000000 commonnexus-1.4.0/src/commonnexus/blocks/distances.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8333 2023-03-13 07:11:10.000000 commonnexus-1.4.0/src/commonnexus/blocks/notes.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7699 2023-02-14 12:01:40.000000 commonnexus-1.4.0/src/commonnexus/blocks/sets.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3040 2023-03-07 08:22:00.000000 commonnexus-1.4.0/src/commonnexus/blocks/taxa.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17066 2023-06-29 08:02:38.000000 commonnexus-1.4.0/src/commonnexus/blocks/trees.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2240 2023-02-16 11:10:00.000000 commonnexus-1.4.0/src/commonnexus/blocks/unaligned.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3710 2023-03-13 14:04:48.000000 commonnexus-1.4.0/src/commonnexus/cli_util.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4308 2023-06-29 08:01:14.000000 commonnexus-1.4.0/src/commonnexus/command.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/commonnexus/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2023-03-02 07:16:22.000000 commonnexus-1.4.0/src/commonnexus/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5977 2023-03-10 08:48:03.000000 commonnexus-1.4.0/src/commonnexus/commands/characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      530 2023-03-02 09:45:35.000000 commonnexus-1.4.0/src/commonnexus/commands/combine.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      316 2023-03-04 14:51:27.000000 commonnexus-1.4.0/src/commonnexus/commands/help.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      349 2023-03-06 11:27:02.000000 commonnexus-1.4.0/src/commonnexus/commands/normalise.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1201 2023-03-10 11:18:14.000000 commonnexus-1.4.0/src/commonnexus/commands/split.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     8705 2023-03-13 14:05:09.000000 commonnexus-1.4.0/src/commonnexus/commands/taxa.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3174 2023-03-13 14:15:33.000000 commonnexus-1.4.0/src/commonnexus/commands/trees.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17585 2023-03-10 14:17:53.000000 commonnexus-1.4.0/src/commonnexus/nexus.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11459 2023-03-08 14:41:35.000000 commonnexus-1.4.0/src/commonnexus/tokenizer.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/commonnexus/tools/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      213 2023-03-02 07:36:37.000000 commonnexus-1.4.0/src/commonnexus/tools/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3061 2023-03-07 09:13:58.000000 commonnexus-1.4.0/src/commonnexus/tools/combine.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11492 2023-03-10 08:40:51.000000 commonnexus-1.4.0/src/commonnexus/tools/matrix.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4137 2023-07-17 08:48:11.000000 commonnexus-1.4.0/src/commonnexus/tools/normalise.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      168 2023-02-16 08:50:17.000000 commonnexus-1.4.0/src/commonnexus/util.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-18 11:26:33.223477 commonnexus-1.4.0/src/commonnexus.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4609 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1289 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       58 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-02-08 09:38:01.000000 commonnexus-1.4.0/src/commonnexus.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      222 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       12 2023-07-18 11:26:33.000000 commonnexus-1.4.0/src/commonnexus.egg-info/top_level.txt
```

### Comparing `commonnexus-1.3.0/LICENSE` & `commonnexus-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/PKG-INFO` & `commonnexus-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonnexus
-Version: 1.3.0
+Version: 1.4.0
 Summary: A nexus (phylogenetics) file reader and writer (.nex, .trees)
 Home-page: https://github.com/dlce-eva/commonnexus
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/commonnexus/issues
 Keywords: phylogenetics nexus newick paup splitstree
@@ -16,23 +16,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # commonnexus
```

### Comparing `commonnexus-1.3.0/README.md` & `commonnexus-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/setup.cfg` & `commonnexus-1.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commonnexus
-version = 1.3.0
+version = 1.4.0
 author = Robert Forkel
 author_email = robert_forkel@eva.mpg.de
 description = A nexus (phylogenetics) file reader and writer (.nex, .trees)
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = phylogenetics nexus newick paup splitstree
 license = Apache 2.0
@@ -21,29 +21,28 @@
 	Operating System :: OS Independent
 	Environment :: Console
 	License :: OSI Approved :: Apache Software License
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Software Development :: Libraries :: Python Modules
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	License :: OSI Approved :: BSD License
 
 [options]
 zip_safe = False
 packages = find:
 package_dir = 
 	= src
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	newick>=1.8.1
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
@@ -59,15 +58,15 @@
 	build
 test = 
 	pytest>=5
 	pytest-mock
 	pytest-cov
 	coverage>=4.2
 docs = 
-	sphinx
+	sphinx<7
 	sphinx-autodoc-typehints
 	sphinx-rtd-theme
 	sphinx-prompt
 	sphinxcontrib-programoutput
 	termgraph
 
 [bdist_wheel]
@@ -94,15 +93,15 @@
 	tests
 
 [coverage:report]
 show_missing = true
 skip_covered = true
 
 [tox:tox]
-envlist = py37, py38, py39, py310, py311
+envlist = py38, py39, py310, py311
 isolated_build = true
 skip_missing_interpreter = true
 
 [testenv]
 deps = .[test]
 commands = pytest {posargs}
```

### Comparing `commonnexus-1.3.0/src/commonnexus/__main__.py` & `commonnexus-1.4.0/src/commonnexus/__main__.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/__init__.py` & `commonnexus-1.4.0/src/commonnexus/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/assumptions.py` & `commonnexus-1.4.0/src/commonnexus/blocks/assumptions.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/base.py` & `commonnexus-1.4.0/src/commonnexus/blocks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Basic building blocks of NEXUS files.
 """
 import re
 import typing
+import functools
 import collections
 
-from commonnexus._compat import cached_property
 from commonnexus.tokenizer import (
     get_name, iter_tokens, iter_words_and_punctuation, word_after_equals, TokenType, Word,
 )
 from commonnexus.command import Command
 
 
 class Payload:
@@ -18,15 +18,15 @@
     """
     __multivalued__ = False
 
     def __init__(self, tokens, nexus=None):
         self.nexus = nexus
         self._tokens = list(iter_tokens(iter(tokens))) if isinstance(tokens, str) else tokens
 
-    @cached_property
+    @functools.cached_property
     def comments(self):
         return [t.text for t in self._tokens if t.type == TokenType.COMMENT]
 
     def format(self, *args, **kw):
         """
         Derived classes may provide functionality to format command data as correct Nexus payload.
         """
@@ -99,15 +99,15 @@
 
     def __init__(self, nexus, cmds):
         self.nexus = nexus
 
     def __str__(self):
         return ''.join(str(cmd) for cmd in self)
 
-    @cached_property
+    @functools.cached_property
     def payload_map(self):
         res = {cls.__name__.upper(): cls for cls in self.__commands__}
         res.update(LINK=Link, TITLE=Title, ID=Id)
         return res
 
     @property
     def id(self):
@@ -136,19 +136,19 @@
         if name.isupper():
             try:
                 return self.commands[name][0]
             except IndexError:
                 return None
         return super().__getattribute__(name)
 
-    @cached_property
+    @functools.cached_property
     def name(self):
         return get_name(self[0].iter_payload_tokens())
 
-    @cached_property
+    @functools.cached_property
     def commands(self):
         res = collections.defaultdict(list)
         for cmd in self:
             if not (cmd.is_beginblock or cmd.is_endblock):
                 cls = self.payload_map.get(cmd.name, Payload)
                 res[cmd.name].append(cls(tuple(cmd.iter_payload_tokens()), nexus=self.nexus))
         return res
```

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/characters.py` & `commonnexus-1.4.0/src/commonnexus/blocks/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 StateMatrix = typing.OrderedDict[str, typing.OrderedDict[str, State]]
 
 GAP = '\uFFFD'  # REPLACEMENT CHARACTER used to replace an [...] unrepresentable character
 #: Some - but not all - punctuation is invalid as (special) state symbol.
 INVALID_SYMBOLS = "()[]{}/\\,;:=*'\"*`<>^"
 
 
+def duplicate_charlabel(label, cmd, nexus):
+    if nexus and nexus.cfg.strict:  # pragma: no cover
+        raise ValueError('character names must be unique!')
+    else:
+        warnings.warn(
+            'Duplicate character name "{}" in {} command'.format(label, cmd))
+
+
 class Eliminate(Payload):
     """
     This command allows specification of a list of characters that are to be excluded from
     consideration. Programs are expected to ignore ELIMINATEd characters completely during reading.
     In avoiding allocation of memory to store character information, the programs can save a
     considerable amount of computer memory. (This subcommand is similar to ZAP in version 3.1.1
     of PAUP.) For example,
@@ -107,15 +115,23 @@
        in the FORMAT command. Standard data consist of any general sort of discrete character data,
        and this class is typically used for morphological data, restriction site data, and so on.
        DNA, RNA, NUCLEOTIDE, and PROTEIN designate molecular sequence data. Meristic morphometric
        data and other information with continuous values can be housed in matrices of
        DATATYPE=CONTINUOUS. These DATATYPES are described in detail, with examples, at the end of
        the description of the CHARACTERS block.
 
-       .. warning:: ``DATATYPE=CONTINUOUS`` is currently not supported in `commonnexus`.
+       .. warning::
+
+        ``DATATYPE=CONTINUOUS`` is currently not supported in `commonnexus`.
+        Some programs accept (or expect) datatypes beyond the ones defined in the NEXUS spec;
+        e.g. MrBayes has ``DATATYPE=RESTRICTION`` and Beauti may create "NEXUS" files with
+        ``DATATYPE=BINARY``. `commonnexus` does not accept these non-standard datatypes and raises
+        an exception when trying to read the MATRIX. Thus, to make "NEXUS" files with
+        non-standard datatypes readable for `commonnexus`, substituting ``DATATYPE=STANDARD`` is
+        typically the right thing to do.
 
     2. RESPECTCASE. By default, information in a MATRIX may be entered in uppercase, lowercase, or
        a mixture of uppercase and lowercase. If RESPECTCASE is requested, case is considered
        significant in SYMBOLS, MISSING, GAP, and MATCHCHAR subcommands and in subsequent references
        to states. For example, if RESPECTCASE is invoked, then SYMBOLS="A a B b" designates four
        states whose symbols are A, a, B, and b, which can then each be used in the MATRIX command
        and elsewhere. If RESPECTCASE is not invoked, then A and a are considered homonymous state
@@ -137,14 +153,21 @@
        SYMBOLS="012" is equivalent to SYMBOLS="0 1 2". For STANDARD DATATYPES, a SYMBOLS subcommand
        will replace the default symbols list of "0 1". For DNA, RNA, NUCLEOTIDE, and PROTEIN
        DATATYPES, a SYMBOLS subcommand will not replace the default symbols list but will add
        character-state symbols to the SYMBOLS list. The NEXUS standard does not define the position
        of these additional symbols within the SYMBOLS list. (These additional symbols will be
        inserted at the beginning of the SYMBOLS list in PAUP and at the end in MacClade. MacClade
        will accept additional symbols for PROTEIN but not DNA, RNA, and NUCLEOTIDE matrices.)
+
+       .. warning::
+
+            While the specification requires the content of the SYMBOLS subcommand to be enclosed in
+            doublequotes, `commonnexus` also allows unquoted content; i.e. `SYMBOLS=01` is treated
+            as equivalent to `SYMBOLS="01"`.
+
     6. EQUATE. This subcommand allows one to define symbols to represent one matrix entry. For
        example, EQUATE="E=(012)" means that each occurrence of E in the MATRIX command will be
        interpreted as meaning states 0, 1, and 2. The equate symbols cannot be any of the
        :data:`INVALID_SYMBOLS` or any or the currently defined MISSING, GAP, MATCHCHAR, or state
        SYMBOLS. Case is significant in equate symbols. That is, MISSING=? EQUATE="E=(012)e=?" means
        that E will be interpreted as 0, 1, and 2 and e will be interpreted as missing data.
     7. MATCHCHAR. This subcommand defines a matching character symbol. If this subcommand is
@@ -318,46 +341,53 @@
         if tokens is None:
             return
 
         words = iter_words_and_punctuation(self._tokens, nexus=nexus)
         after_equals = functools.partial(word_after_equals, words)
 
         subcommand = None
+        subcommands_set = set()
         while 1:
             try:
                 word = next(words)
                 if isinstance(word, str):
                     subcommand = word.upper()
                 elif isinstance(word, Token) and word.text == '=':
                     if subcommand in ['RESPECTCASE', 'TRANSPOSE', 'INTERLEAVE', 'LABELS', 'TOKENS']:
                         # Some NEXUS variants set boolean subcommands always with "=no|yes"
                         word = next(words).lower()
                         if subcommand == 'LABELS' and word == 'left':
                             word = 'yes'
                         setattr(self, subcommand.lower(), BOOLEAN[word])
+                        subcommands_set.add(subcommand)
                     elif subcommand:  # pragma: no cover
                         raise ValueError(subcommand)
 
                 if subcommand in ['DATATYPE', 'MISSING', 'MATCHCHAR', 'GAP', 'STATESFORMAT']:
                     setattr(self, subcommand.lower(), after_equals())
                     if subcommand == 'DATATYPE' and self.datatype.upper() != 'STANDARD':
                         self.symbols = []
                 elif subcommand in ['RESPECTCASE', 'TRANSPOSE', 'INTERLEAVE']:
-                    setattr(self, subcommand.lower(), True)
+                    if subcommand not in subcommands_set:
+                        setattr(self, subcommand.lower(), True)
                 elif subcommand in ['NOLABELS', 'LABELS', 'NOTOKENS', 'TOKENS']:
                     setattr(self, subcommand.replace('NO', '').lower(), 'NO' not in subcommand)
                 elif subcommand == 'SYMBOLS':
                     self.explicit_symbols = True
                     self.symbols = []
-                    for w in iter_delimited(after_equals(), words):
-                        if isinstance(w, str):
-                            self.symbols.extend(list(w))
-                        else:
-                            assert w.text in '+-'
-                            self.symbols.append(w.text)
+                    next_token_text = after_equals()
+                    if not next_token_text.startswith('"'):
+                        self.symbols = list(next_token_text)
+                    else:
+                        for w in iter_delimited(next_token_text, words):
+                            if isinstance(w, str):
+                                self.symbols.extend(list(w))
+                            else:
+                                assert w.text in '+-'
+                                self.symbols.append(w.text)
                 elif subcommand == 'EQUATE':
                     key, e, bracket = None, False, None
                     for t in iter_delimited(after_equals(), words):
                         if isinstance(t, Token):
                             if t.text == '=':
                                 assert key
                                 e = True
@@ -476,30 +506,40 @@
     .. code-block:: python
 
         >>> cmd = Charstatelabels('1 eye_color/red blue green, 3 head_shape/round square')
         >>> cmd.characters[0].name
         'eye_color'
         >>> cmd.characters[0].states
         ['red', 'blue', 'green']
+
+    .. warning::
+
+        In strict mode (see :class:`commonnexus.nexus.Config`) duplicate character names will raise
+        a ``ValueError``, otherwise a ``UserWarning`` will be emitted. While a matrix with duplicate
+        character names can still be read, it will typically **not** be as expected, because only
+        the values for the last character for a given name will be present.
     """
     def __init__(self, tokens, nexus=None):
         super().__init__(tokens, nexus=nexus)
         self.characters = []
-
+        names = set()
         words = iter_words_and_punctuation(self._tokens, nexus=nexus)
         num, name, states, in_states, comma = None, None, [], False, False
 
         while 1:
             try:
                 w = next(words)
                 if num is None:
                     num = int(w)
                     continue
                 if isinstance(w, Token) and w.text == ',':
                     comma = True  # We want to be able to detect trailing commas!
+                    if name and name in names:
+                        duplicate_charlabel(name, 'CHARSTATELABELS', nexus)
+                    names.add(name)
                     self.characters.append(
                         types.SimpleNamespace(number=num, name=name, states=states))
                     num, name, states, in_states = None, None, [], False
                     continue
                 if in_states:
                     states.append(w)
                     continue
@@ -540,16 +580,20 @@
     CHARLABELS because many existing NEXUS files use CHARLABELS.
 
     :ivar typing.List[types.SimpleNamespace] characters:
     """
     def __init__(self, tokens, nexus=None):
         super().__init__(tokens, nexus=nexus)
         self.characters = []
+        names = set()
         for i, w in enumerate(iter_words_and_punctuation(self._tokens, nexus=nexus)):
             assert isinstance(w, str)
+            if w and w in names:
+                duplicate_charlabel(w, 'CHARLABELS', nexus)
+            names.add(w)
             self.characters.append(types.SimpleNamespace(number=i + 1, name=w, states=[]))
 
 
 class Statelabels(Payload):
     """
     This command allows specification of the names of states:
 
@@ -1124,15 +1168,15 @@
         if any(k != v for k, v in charlabels.items()):
             cmds.append((
                 'CHARSTATELABELS',
                 ', '.join('\n    {} {}{}'.format(
                     n,
                     Word(l).as_nexus_string(),
                     '/' + ' '.join(Word(ll).as_nexus_string() for ll in statelabels[l].values())
-                    if l in statelabels else '',
+                    if statelabels.get(l) else '',
                 ) for n, l in charlabels.items())))
         if taxlabels:
             cmds.append(('TAXLABELS', ' '.join(tlabels.values())))
         cmds.append(('MATRIX', ''.join(rows)))
         return cls.from_commands(cmds, nexus=nexus, TITLE=TITLE, ID=ID, LINK=LINK)
```

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/codons.py` & `commonnexus-1.4.0/src/commonnexus/blocks/codons.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/distances.py` & `commonnexus-1.4.0/src/commonnexus/blocks/distances.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/notes.py` & `commonnexus-1.4.0/src/commonnexus/blocks/notes.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/sets.py` & `commonnexus-1.4.0/src/commonnexus/blocks/sets.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/taxa.py` & `commonnexus-1.4.0/src/commonnexus/blocks/taxa.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/trees.py` & `commonnexus-1.4.0/src/commonnexus/blocks/trees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 import warnings
+import functools
 import collections
 
 import newick
 
 from .base import Payload, Block
-from commonnexus._compat import cached_property
 from commonnexus.util import log_or_raise
 from commonnexus.tokenizer import TokenType, iter_words_and_punctuation, Word, Token
 
 TreeSpec = typing.Tuple[str, typing.Union[str, newick.Node], typing.Union[None, bool]]
 
 
 class Translate(Payload):
@@ -195,15 +195,15 @@
     def rooted(self) -> typing.Union[None, bool]:
         """
         Whether the tree is rooted (`True`) or not (`False`) or no information is given (`None`).
         """
         if self._rooted:
             return self._rooted == '&R'
 
-    @cached_property
+    @functools.cached_property
     def newick_string(self) -> str:
         """
         The Newick-formatted string representation of the tree.
 
         .. note::
 
             This property is intended for cases where only the string representation is of interest
@@ -222,15 +222,15 @@
                 >>> nex.TREES.TREE.newick_string
                 '(a,b)\\nc;'
                 >>> nex.TREES.TREE.newick.newick
                 '(a,b)c'
         """
         return ''.join(str(t) for t in self.newick_tokens) + ';'
 
-    @cached_property
+    @functools.cached_property
     def newick(self) -> newick.Node:
         """
         A `newick.Node` instance parsed from the Newick representation of the tree.
 
         .. code-block:: python
 
             >>> from commonnexus import Nexus
@@ -321,15 +321,15 @@
                         'TRANSLATE command **after** TREE command', log=log, level='warning')
                 else:
                     with_translate = True
             else:
                 tree_seen = True
         return valid
 
-    @cached_property
+    @functools.cached_property
     def translate_mapping(self):
         mapping = {}
         if 'TRANSLATE' in self.commands:
             mapping.update(self.TRANSLATE.mapping)
         if 'TAXA' in self.linked_blocks:
             mapping.update({
                 str(k): v for k, v in self.linked_blocks['TAXA'].TAXLABELS.labels.items()})
```

### Comparing `commonnexus-1.3.0/src/commonnexus/blocks/unaligned.py` & `commonnexus-1.4.0/src/commonnexus/blocks/unaligned.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/cli_util.py` & `commonnexus-1.4.0/src/commonnexus/cli_util.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/command.py` & `commonnexus-1.4.0/src/commonnexus/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+import functools
 import itertools
 
-from ._compat import cached_property
 from .tokenizer import TokenType, iter_tokens, Token, get_name
 
 
 class Command(tuple):
     """
     From the specification:
 
         A command is a collection of tokens terminated by a semicolon. Commands cannot contain
         semicolons, except as terminators, unless the semicolons are contained within a comment
         or within a quoted token consisting of more than one text character.
     """
-    @cached_property
+    @functools.cached_property
     def name(self):
         return get_name(self)
 
     def __str__(self):
         return ''.join(str(t) for t in self)
 
     def __eq__(self, other):  # To make command removal in Nexus.replace_block work.
```

### Comparing `commonnexus-1.3.0/src/commonnexus/commands/characters.py` & `commonnexus-1.4.0/src/commonnexus/commands/characters.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/commands/combine.py` & `commonnexus-1.4.0/src/commonnexus/commands/combine.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/commands/split.py` & `commonnexus-1.4.0/src/commonnexus/commands/split.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/commands/taxa.py` & `commonnexus-1.4.0/src/commonnexus/commands/taxa.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/commands/trees.py` & `commonnexus-1.4.0/src/commonnexus/commands/trees.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/nexus.py` & `commonnexus-1.4.0/src/commonnexus/nexus.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/tokenizer.py` & `commonnexus-1.4.0/src/commonnexus/tokenizer.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/tools/combine.py` & `commonnexus-1.4.0/src/commonnexus/tools/combine.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/tools/matrix.py` & `commonnexus-1.4.0/src/commonnexus/tools/matrix.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus/tools/normalise.py` & `commonnexus-1.4.0/src/commonnexus/tools/normalise.py`

 * *Files identical despite different names*

### Comparing `commonnexus-1.3.0/src/commonnexus.egg-info/PKG-INFO` & `commonnexus-1.4.0/src/commonnexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonnexus
-Version: 1.3.0
+Version: 1.4.0
 Summary: A nexus (phylogenetics) file reader and writer (.nex, .trees)
 Home-page: https://github.com/dlce-eva/commonnexus
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/commonnexus/issues
 Keywords: phylogenetics nexus newick paup splitstree
@@ -16,23 +16,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
 
 # commonnexus
```

### Comparing `commonnexus-1.3.0/src/commonnexus.egg-info/SOURCES.txt` & `commonnexus-1.4.0/src/commonnexus.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/commonnexus/__init__.py
 src/commonnexus/__main__.py
-src/commonnexus/_compat.py
 src/commonnexus/cli_util.py
 src/commonnexus/command.py
 src/commonnexus/nexus.py
 src/commonnexus/tokenizer.py
 src/commonnexus/util.py
 src/commonnexus.egg-info/PKG-INFO
 src/commonnexus.egg-info/SOURCES.txt
```

