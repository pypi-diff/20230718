# Comparing `tmp/green_tsetlin-0.1.0.tar.gz` & `tmp/green_tsetlin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green_tsetlin-0.1.0.tar", last modified: Mon Jul 17 23:22:38 2023, max compression
+gzip compressed data, was "green_tsetlin-0.1.1.tar", last modified: Mon Jul 17 23:36:17 2023, max compression
```

## Comparing `green_tsetlin-0.1.0.tar` & `green_tsetlin-0.1.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.684156 green_tsetlin-0.1.0/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1066 2023-07-17 21:10:12.000000 green_tsetlin-0.1.0/LICENSE
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      169 2023-07-17 21:28:58.000000 green_tsetlin-0.1.0/MANIFEST.in
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-07-17 23:22:38.684156 green_tsetlin-0.1.0/PKG-INFO
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      742 2023-07-17 23:21:05.000000 green_tsetlin-0.1.0/README.md
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.664156 green_tsetlin-0.1.0/docs/
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.664156 green_tsetlin-0.1.0/docs/_build/
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.668156 green_tsetlin-0.1.0/docs/_build/doctrees/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    11277 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4963 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/doctrees/index.doctree
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.668156 green_tsetlin-0.1.0/docs/_build/html/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      230 2023-07-15 15:16:13.000000 green_tsetlin-0.1.0/docs/_build/html/.buildinfo
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.668156 green_tsetlin-0.1.0/docs/_build/html/_sources/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.0/docs/_build/html/_sources/index.rst.txt
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.668156 green_tsetlin-0.1.0/docs/_build/html/_static/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4418 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    11185 2023-07-15 15:16:13.000000 green_tsetlin-0.1.0/docs/_build/html/_static/alabaster.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15228 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/_static/basic.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       42 2021-01-29 11:59:09.000000 green_tsetlin-0.1.0/docs/_build/html/_static/custom.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     8171 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      421 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      286 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)   288580 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/jquery-3.6.0.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    89501 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4758 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5249 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    17088 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    68420 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/underscore-1.13.1.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19530 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2482 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/genindex.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3431 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/index.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      268 2023-07-15 15:16:13.000000 green_tsetlin-0.1.0/docs/_build/html/objects.inv
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2759 2023-07-15 15:16:12.000000 green_tsetlin-0.1.0/docs/_build/html/search.html
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      633 2023-07-15 15:16:13.000000 green_tsetlin-0.1.0/docs/_build/html/searchindex.js
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.676156 green_tsetlin-0.1.0/docs/_build/latex/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4366 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/LICRcyr2utf8.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10188 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/LICRlatin2utf8.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    18693 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/LatinRules.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2465 2023-07-15 15:17:48.000000 green_tsetlin-0.1.0/docs/_build/latex/green_tsetlin.tex
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      473 2023-07-15 15:17:48.000000 green_tsetlin-0.1.0/docs/_build/latex/make.bat
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      392 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/python.ist
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    12780 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinx.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9474 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinx.xdy
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6679 2023-07-15 15:17:48.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxhighlight.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3256 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxhowto.cls
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6238 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexadmonitions.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      901 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexcontainers.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4840 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexgraphics.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexindbibtoc.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5139 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexlists.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    35719 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexliterals.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4532 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexnumfig.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexobjects.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3885 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexshadowbox.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3253 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstyleheadings.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3064 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstylepage.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6177 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstyletext.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    21848 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxlatextables.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4241 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxmanual.cls
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      745 2023-07-15 15:17:48.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxmessages.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2061 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxoptionsgeometry.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1094 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxoptionshyperref.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2590 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxpackagecyrillic.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15217 2022-07-14 07:38:19.000000 green_tsetlin-0.1.0/docs/_build/latex/sphinxpackagefootnote.sty
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1950 2023-07-08 11:11:41.000000 green_tsetlin-0.1.0/docs/conf.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.0/docs/index.rst
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      800 2023-07-08 11:11:41.000000 green_tsetlin-0.1.0/docs/make.bat
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.676156 green_tsetlin-0.1.0/green_tsetlin/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      399 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/green_tsetlin/__init__.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     6439 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/green_tsetlin/dataset_generator.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      484 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/green_tsetlin/pandas_connector.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      403 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/green_tsetlin/predictor.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     7155 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/green_tsetlin/rules.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10819 2023-07-17 20:36:36.000000 green_tsetlin-0.1.0/green_tsetlin/trainer.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     8251 2023-07-17 01:00:53.000000 green_tsetlin-0.1.0/green_tsetlin/tsetlin_machine.py
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.676156 green_tsetlin-0.1.0/green_tsetlin.egg-info/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-07-17 23:22:38.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/PKG-INFO
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3276 2023-07-17 23:22:38.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/SOURCES.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-07-17 23:22:38.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/dependency_links.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-07-16 16:16:33.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/not-zip-safe
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       27 2023-07-17 23:22:38.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/requires.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       33 2023-07-17 23:22:38.000000 green_tsetlin-0.1.0/green_tsetlin.egg-info/top_level.txt
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      429 2023-07-17 22:54:56.000000 green_tsetlin-0.1.0/pyproject.toml
--rw-rw-r--   0 ooki      (1000) ooki      (1000)       38 2023-07-17 23:22:38.684156 green_tsetlin-0.1.0/setup.cfg
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3248 2023-07-17 23:22:21.000000 green_tsetlin-0.1.0/setup.py
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.680156 green_tsetlin-0.1.0/src/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    33063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/BS_thread_pool.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2164 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/circular_buffer.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    20989 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/clause_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9094 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/executor.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    10261 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/feedback_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    38013 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/func_avx2.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    41681 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/func_neon.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/func_nv.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     4662 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/func_sparse.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5568 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/functors_interface.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      214 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/gt_common.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1049 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/gt_utils.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     7701 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/inference.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    13436 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/input_block.hpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19079 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/main copy.cpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19079 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/src/main.cpp
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     9885 2023-07-15 10:37:24.000000 green_tsetlin-0.1.0/src/random_generator.hpp
-drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:22:38.684156 green_tsetlin-0.1.0/tests/
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    19029 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_clause_block_avx2_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    15805 2023-07-15 10:37:24.000000 green_tsetlin-0.1.0/tests/test_clause_block_neon_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)    14813 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_clause_block_nv_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1223 2023-07-15 10:37:24.000000 green_tsetlin-0.1.0/tests/test_dataset_reader.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     1460 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_dense_multi_label.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2783 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_inference_impl.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     2248 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_input_block.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5483 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_rules.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)      548 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/test_sparse_block.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3716 2023-07-17 20:10:37.000000 green_tsetlin-0.1.0/tests/test_trainer.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     5050 2023-07-17 01:01:03.000000 green_tsetlin-0.1.0/tests/test_tsetlin_machine.py
--rw-rw-r--   0 ooki      (1000) ooki      (1000)     3523 2023-07-08 09:51:47.000000 green_tsetlin-0.1.0/tests/tests_dataset_generator.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.044474 green_tsetlin-0.1.1/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1066 2023-07-17 21:10:12.000000 green_tsetlin-0.1.1/LICENSE
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      169 2023-07-17 21:28:58.000000 green_tsetlin-0.1.1/MANIFEST.in
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-07-17 23:36:17.044474 green_tsetlin-0.1.1/PKG-INFO
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      742 2023-07-17 23:21:05.000000 green_tsetlin-0.1.1/README.md
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.024474 green_tsetlin-0.1.1/docs/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.024474 green_tsetlin-0.1.1/docs/_build/
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.024474 green_tsetlin-0.1.1/docs/_build/doctrees/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    11277 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4963 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/doctrees/index.doctree
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.024474 green_tsetlin-0.1.1/docs/_build/html/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      230 2023-07-15 15:16:13.000000 green_tsetlin-0.1.1/docs/_build/html/.buildinfo
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.028474 green_tsetlin-0.1.1/docs/_build/html/_sources/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.1/docs/_build/html/_sources/index.rst.txt
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.028474 green_tsetlin-0.1.1/docs/_build/html/_static/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4418 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    11185 2023-07-15 15:16:13.000000 green_tsetlin-0.1.1/docs/_build/html/_static/alabaster.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15228 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       42 2021-01-29 11:59:09.000000 green_tsetlin-0.1.1/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     8171 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      421 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      286 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)   288580 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/jquery-3.6.0.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    89501 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/jquery.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4758 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       90 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5249 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    17088 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    68420 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/underscore-1.13.1.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19530 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/html/_static/underscore.js
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2482 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/genindex.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3431 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/index.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      268 2023-07-15 15:16:13.000000 green_tsetlin-0.1.1/docs/_build/html/objects.inv
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2759 2023-07-15 15:16:12.000000 green_tsetlin-0.1.1/docs/_build/html/search.html
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      633 2023-07-15 15:16:13.000000 green_tsetlin-0.1.1/docs/_build/html/searchindex.js
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.036474 green_tsetlin-0.1.1/docs/_build/latex/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4366 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/LICRcyr2utf8.xdy
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    10188 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/LICRlatin2utf8.xdy
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    18693 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/LatinRules.xdy
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2465 2023-07-15 15:17:48.000000 green_tsetlin-0.1.1/docs/_build/latex/green_tsetlin.tex
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      473 2023-07-15 15:17:48.000000 green_tsetlin-0.1.1/docs/_build/latex/make.bat
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      392 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/python.ist
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    12780 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinx.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9474 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinx.xdy
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6679 2023-07-15 15:17:48.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxhighlight.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3256 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxhowto.cls
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6238 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexadmonitions.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      901 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexcontainers.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4840 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexgraphics.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexindbibtoc.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5139 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexlists.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    35719 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexliterals.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4532 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexnumfig.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9066 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexobjects.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3885 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexshadowbox.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3253 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstyleheadings.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3064 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstylepage.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6177 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstyletext.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    21848 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxlatextables.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4241 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxmanual.cls
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      745 2023-07-15 15:17:48.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxmessages.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2061 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxoptionsgeometry.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1094 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxoptionshyperref.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2590 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxpackagecyrillic.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15217 2022-07-14 07:38:19.000000 green_tsetlin-0.1.1/docs/_build/latex/sphinxpackagefootnote.sty
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1950 2023-07-08 11:11:41.000000 green_tsetlin-0.1.1/docs/conf.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      455 2023-07-08 11:11:41.000000 green_tsetlin-0.1.1/docs/index.rst
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      800 2023-07-08 11:11:41.000000 green_tsetlin-0.1.1/docs/make.bat
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.036474 green_tsetlin-0.1.1/green_tsetlin/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      399 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/green_tsetlin/__init__.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     6439 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/green_tsetlin/dataset_generator.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      484 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/green_tsetlin/pandas_connector.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      403 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/green_tsetlin/predictor.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7155 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/green_tsetlin/rules.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    10819 2023-07-17 20:36:36.000000 green_tsetlin-0.1.1/green_tsetlin/trainer.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     8251 2023-07-17 01:00:53.000000 green_tsetlin-0.1.1/green_tsetlin/tsetlin_machine.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.040474 green_tsetlin-0.1.1/green_tsetlin.egg-info/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1967 2023-07-17 23:36:17.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/PKG-INFO
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3276 2023-07-17 23:36:17.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/SOURCES.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-07-17 23:36:17.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/dependency_links.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)        1 2023-07-16 16:16:33.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/not-zip-safe
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       68 2023-07-17 23:36:17.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/requires.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       33 2023-07-17 23:36:17.000000 green_tsetlin-0.1.1/green_tsetlin.egg-info/top_level.txt
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      429 2023-07-17 22:54:56.000000 green_tsetlin-0.1.1/pyproject.toml
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)       38 2023-07-17 23:36:17.044474 green_tsetlin-0.1.1/setup.cfg
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3344 2023-07-17 23:36:08.000000 green_tsetlin-0.1.1/setup.py
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.040474 green_tsetlin-0.1.1/src/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    33063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/BS_thread_pool.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2164 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/circular_buffer.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    20989 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/clause_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9094 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/executor.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    10261 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/feedback_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    38013 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/func_avx2.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    41681 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/func_neon.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19063 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/func_nv.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     4662 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/func_sparse.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5568 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/functors_interface.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      214 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/gt_common.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1049 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/gt_utils.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     7701 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/inference.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    13436 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/input_block.hpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19079 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/main copy.cpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19079 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/src/main.cpp
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     9885 2023-07-15 10:37:24.000000 green_tsetlin-0.1.1/src/random_generator.hpp
+drwxrwxr-x   0 ooki      (1000) ooki      (1000)        0 2023-07-17 23:36:17.044474 green_tsetlin-0.1.1/tests/
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    19029 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_clause_block_avx2_impl.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    15805 2023-07-15 10:37:24.000000 green_tsetlin-0.1.1/tests/test_clause_block_neon_impl.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)    14813 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_clause_block_nv_impl.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1223 2023-07-15 10:37:24.000000 green_tsetlin-0.1.1/tests/test_dataset_reader.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     1460 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_dense_multi_label.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2783 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_inference_impl.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     2248 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_input_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5483 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_rules.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)      548 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/test_sparse_block.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3716 2023-07-17 20:10:37.000000 green_tsetlin-0.1.1/tests/test_trainer.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     5050 2023-07-17 01:01:03.000000 green_tsetlin-0.1.1/tests/test_tsetlin_machine.py
+-rw-rw-r--   0 ooki      (1000) ooki      (1000)     3523 2023-07-08 09:51:47.000000 green_tsetlin-0.1.1/tests/tests_dataset_generator.py
```

### Comparing `green_tsetlin-0.1.0/LICENSE` & `green_tsetlin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/PKG-INFO` & `green_tsetlin-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green_tsetlin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A fast Tsetlin Machine impl, based on c++
 Home-page: https://github.com/ooki/green_tsetlin
 Author: Sondre 'Ooki' Glimsdal
 Author-email: sondre.glimsdal@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ooki/green_tsetlin/issues
 Project-URL: Documentation, https://github.com/ooki/green_tsetlin
```

### Comparing `green_tsetlin-0.1.0/README.md` & `green_tsetlin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/doctrees/environment.pickle` & `green_tsetlin-0.1.1/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/doctrees/index.doctree` & `green_tsetlin-0.1.1/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/alabaster.css` & `green_tsetlin-0.1.1/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/basic.css` & `green_tsetlin-0.1.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/doctools.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/jquery-3.6.0.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/jquery.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/language_data.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/pygments.css` & `green_tsetlin-0.1.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/searchtools.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/underscore-1.13.1.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/_static/underscore.js` & `green_tsetlin-0.1.1/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/genindex.html` & `green_tsetlin-0.1.1/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/index.html` & `green_tsetlin-0.1.1/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/search.html` & `green_tsetlin-0.1.1/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/html/searchindex.js` & `green_tsetlin-0.1.1/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/LICRcyr2utf8.xdy` & `green_tsetlin-0.1.1/docs/_build/latex/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/LICRlatin2utf8.xdy` & `green_tsetlin-0.1.1/docs/_build/latex/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/LatinRules.xdy` & `green_tsetlin-0.1.1/docs/_build/latex/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/green_tsetlin.tex` & `green_tsetlin-0.1.1/docs/_build/latex/green_tsetlin.tex`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinx.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinx.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinx.xdy` & `green_tsetlin-0.1.1/docs/_build/latex/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxhighlight.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxhighlight.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxhowto.cls` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexadmonitions.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexcontainers.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexgraphics.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexindbibtoc.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexlists.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexliterals.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexnumfig.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexobjects.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexshadowbox.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstyleheadings.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstylepage.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatexstyletext.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxlatextables.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxmanual.cls` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxmessages.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxmessages.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxoptionsgeometry.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxoptionshyperref.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxpackagecyrillic.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/_build/latex/sphinxpackagefootnote.sty` & `green_tsetlin-0.1.1/docs/_build/latex/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/conf.py` & `green_tsetlin-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/docs/make.bat` & `green_tsetlin-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/green_tsetlin/dataset_generator.py` & `green_tsetlin-0.1.1/green_tsetlin/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/green_tsetlin/rules.py` & `green_tsetlin-0.1.1/green_tsetlin/rules.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/green_tsetlin/trainer.py` & `green_tsetlin-0.1.1/green_tsetlin/trainer.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/green_tsetlin/tsetlin_machine.py` & `green_tsetlin-0.1.1/green_tsetlin/tsetlin_machine.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/green_tsetlin.egg-info/PKG-INFO` & `green_tsetlin-0.1.1/green_tsetlin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-tsetlin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A fast Tsetlin Machine impl, based on c++
 Home-page: https://github.com/ooki/green_tsetlin
 Author: Sondre 'Ooki' Glimsdal
 Author-email: sondre.glimsdal@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ooki/green_tsetlin/issues
 Project-URL: Documentation, https://github.com/ooki/green_tsetlin
```

### Comparing `green_tsetlin-0.1.0/green_tsetlin.egg-info/SOURCES.txt` & `green_tsetlin-0.1.1/green_tsetlin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/setup.py` & `green_tsetlin-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from cpuinfo import get_cpu_info
 from setuptools import setup
 
 import distutils
 distutils.log.set_verbosity(1)
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 cpu_info = get_cpu_info()
 has_avx2 = "avx2" in cpu_info.get("flags", "")
 
@@ -90,10 +90,14 @@
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     zip_safe=False,
     python_requires=">=3.8",
     packages=['green_tsetlin'],
     install_requires=[
           'numpy >= 1.24',
+          'scipy >= 1.11',
+          'scikit-learn >= 1.2',
+          'tqdm >= 4.65'
+          
       ],
     
 )
```

### Comparing `green_tsetlin-0.1.0/src/BS_thread_pool.hpp` & `green_tsetlin-0.1.1/src/BS_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/circular_buffer.hpp` & `green_tsetlin-0.1.1/src/circular_buffer.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/clause_block.hpp` & `green_tsetlin-0.1.1/src/clause_block.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/executor.hpp` & `green_tsetlin-0.1.1/src/executor.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/feedback_block.hpp` & `green_tsetlin-0.1.1/src/feedback_block.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/func_avx2.hpp` & `green_tsetlin-0.1.1/src/func_avx2.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/func_neon.hpp` & `green_tsetlin-0.1.1/src/func_neon.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/func_nv.hpp` & `green_tsetlin-0.1.1/src/func_nv.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/func_sparse.hpp` & `green_tsetlin-0.1.1/src/func_sparse.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/functors_interface.hpp` & `green_tsetlin-0.1.1/src/functors_interface.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/gt_utils.hpp` & `green_tsetlin-0.1.1/src/gt_utils.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/inference.hpp` & `green_tsetlin-0.1.1/src/inference.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/input_block.hpp` & `green_tsetlin-0.1.1/src/input_block.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/main copy.cpp` & `green_tsetlin-0.1.1/src/main copy.cpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/main.cpp` & `green_tsetlin-0.1.1/src/main.cpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/src/random_generator.hpp` & `green_tsetlin-0.1.1/src/random_generator.hpp`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_clause_block_avx2_impl.py` & `green_tsetlin-0.1.1/tests/test_clause_block_avx2_impl.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_clause_block_neon_impl.py` & `green_tsetlin-0.1.1/tests/test_clause_block_neon_impl.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_clause_block_nv_impl.py` & `green_tsetlin-0.1.1/tests/test_clause_block_nv_impl.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_dataset_reader.py` & `green_tsetlin-0.1.1/tests/test_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_dense_multi_label.py` & `green_tsetlin-0.1.1/tests/test_dense_multi_label.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_inference_impl.py` & `green_tsetlin-0.1.1/tests/test_inference_impl.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_input_block.py` & `green_tsetlin-0.1.1/tests/test_input_block.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_rules.py` & `green_tsetlin-0.1.1/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_sparse_block.py` & `green_tsetlin-0.1.1/tests/test_sparse_block.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_trainer.py` & `green_tsetlin-0.1.1/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/test_tsetlin_machine.py` & `green_tsetlin-0.1.1/tests/test_tsetlin_machine.py`

 * *Files identical despite different names*

### Comparing `green_tsetlin-0.1.0/tests/tests_dataset_generator.py` & `green_tsetlin-0.1.1/tests/tests_dataset_generator.py`

 * *Files identical despite different names*

