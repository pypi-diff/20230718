# Comparing `tmp/tuned-lens-0.1.1.tar.gz` & `tmp/tuned-lens-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuned-lens-0.1.1.tar", last modified: Tue Jun 13 16:09:59 2023, max compression
+gzip compressed data, was "tuned-lens-0.2.0.tar", last modified: Tue Jul 18 17:04:29 2023, max compression
```

## Comparing `tuned-lens-0.1.1.tar` & `tuned-lens-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.962218 tuned-lens-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.962218 tuned-lens-0.1.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/scripts/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_load_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_model_surgery.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_unembed.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/ablation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/model_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/unembed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/prediction_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/token_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/trajectory_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/eval_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/ingredients.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/train_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/tuned_lens/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/logit_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.605602 tuned-lens-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-18 17:04:29.605602 tuned-lens-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:04:29.605602 tuned-lens-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.597602 tuned-lens-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.597602 tuned-lens-0.2.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/scripts/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_load_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_model_surgery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_unembed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.597602 tuned-lens-0.2.0/tuned_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.601602 tuned-lens-0.2.0/tuned_lens/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/causal/ablation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/causal/subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/causal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/model_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.601602 tuned-lens-0.2.0/tuned_lens/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/nn/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/nn/unembed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.601602 tuned-lens-0.2.0/tuned_lens/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28184 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/plotting/prediction_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/plotting/token_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9454 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/plotting/trajectory_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.601602 tuned-lens-0.2.0/tuned_lens/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/scripts/eval_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/scripts/ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/scripts/train_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.605602 tuned-lens-0.2.0/tuned_lens/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/stats/logit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-18 17:04:20.000000 tuned-lens-0.2.0/tuned_lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:04:29.601602 tuned-lens-0.2.0/tuned_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 17:04:29.000000 tuned-lens-0.2.0/tuned_lens.egg-info/top_level.txt
```

### Comparing `tuned-lens-0.1.1/LICENSE` & `tuned-lens-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/PKG-INFO` & `tuned-lens-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: transformer_lens
 Provides-Extra: slow_tokenizers
 Provides-Extra: notebooks
 Provides-Extra: 8bit
 License-File: LICENSE
 
 # Tuned Lens 🔎
 <a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
```

### Comparing `tuned-lens-0.1.1/README.md` & `tuned-lens-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/pyproject.toml` & `tuned-lens-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "torch>=1.13.0",
     "transformers>=4.28.1",
     "huggingface_hub>=0.12.1",
     "simple-parsing>=0.1.1",
     "flatten-dict>=0.4.1",
     "wandb>=0.15.0",
 ]
-version = "0.1.1"
+version = "0.2.0"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "bump2version",
     "pytest-skip-slow",
     "pytest",
@@ -36,20 +36,24 @@
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-rtd-theme",
     "nbsphinx",
 ]
 test = [
     "sentencepiece>=0.1.99",
+    "transformer-lens>=1.2.2",
     "pytest-skip-slow",
     "pytest-cov",
     "nbmake",
     "pytest",
     "mock",
 ]
+transformer_lens = [
+    "transformer-lens>=1.2.2"
+]
 slow_tokenizers = [
     "sentencepiece>=0.1.99"
 ]
 notebooks = [
     "ipywidgets",
 ]
 8bit = [
```

### Comparing `tuned-lens-0.1.1/tests/conftest.py` & `tuned-lens-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/scripts/test_integration.py` & `tuned-lens-0.2.0/tests/scripts/test_integration.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_data.py` & `tuned-lens-0.2.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_distance.py` & `tuned-lens-0.2.0/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_lenses.py` & `tuned-lens-0.2.0/tests/test_lenses.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_model_surgery.py` & `tuned-lens-0.2.0/tests/test_model_surgery.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_stats.py` & `tuned-lens-0.2.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_subspaces.py` & `tuned-lens-0.2.0/tests/test_subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tests/test_unembed.py` & `tuned-lens-0.2.0/tests/test_unembed.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/__main__.py` & `tuned-lens-0.2.0/tuned_lens/__main__.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/causal/ablation.py` & `tuned-lens-0.2.0/tuned_lens/causal/ablation.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/causal/subspaces.py` & `tuned-lens-0.2.0/tuned_lens/causal/subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/causal/utils.py` & `tuned-lens-0.2.0/tuned_lens/causal/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/data.py` & `tuned-lens-0.2.0/tuned_lens/data.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/load_artifacts.py` & `tuned-lens-0.2.0/tuned_lens/load_artifacts.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/model_surgery.py` & `tuned-lens-0.2.0/tuned_lens/model_surgery.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Tools for finding and modifying components in a transformer model."""
 
 from contextlib import contextmanager
 from typing import Any, Generator, TypeVar, Union
 
+try:
+    import transformer_lens as tl
+
+    _transformer_lens_available = True
+except ImportError:
+    _transformer_lens_available = False
+
 import torch as th
 import transformers as tr
+from torch import nn
 from transformers import models
 
 
 def get_value_for_key(obj: Any, key: str) -> Any:
     """Get a value using `__getitem__` if `key` is numeric and `getattr` otherwise."""
     return obj[int(key)] if key.isdigit() else getattr(obj, key)
 
@@ -50,23 +58,46 @@
     set_key_path_(model, key_path, value)
     try:
         yield model
     finally:
         set_key_path_(model, key_path, old_value)
 
 
-Norm = Union[th.nn.LayerNorm, models.llama.modeling_llama.LlamaRMSNorm]
+Model = Union[tr.PreTrainedModel, "tl.HookedTransformer"]
+Norm = Union[th.nn.LayerNorm, models.llama.modeling_llama.LlamaRMSNorm, nn.Module]
+
+
+def get_unembedding_matrix(model: Model) -> nn.Linear:
+    """The final linear tranformation from the model hidden state to the output."""
+    if isinstance(model, tr.PreTrainedModel):
+        unembed = model.get_output_embeddings()
+        if not isinstance(unembed, nn.Linear):
+            raise ValueError("We currently only support linear unemebdings")
+        return unembed
+    elif _transformer_lens_available and isinstance(model, tl.HookedTransformer):
+        linear = nn.Linear(
+            in_features=model.cfg.d_model,
+            out_features=model.cfg.d_vocab_out,
+        )
+        linear.bias.data = model.unembed.b_U
+        linear.weight.data = model.unembed.W_U.transpose(0, 1)
+        return linear
+    else:
+        raise ValueError(f"Model class {type(model)} not recognized!")
 
 
-def get_final_norm(model: tr.PreTrainedModel) -> Norm:
+def get_final_norm(model: Model) -> Norm:
     """Get the final norm from a model.
 
     This isn't standardized across models, so this will need to be updated as
     we add new models.
     """
+    if _transformer_lens_available and isinstance(model, tl.HookedTransformer):
+        return model.ln_final
+
     if not hasattr(model, "base_model"):
         raise ValueError("Model does not have a `base_model` attribute.")
 
     base_model = model.base_model
     if isinstance(base_model, models.opt.modeling_opt.OPTModel):
         final_layer_norm = base_model.decoder.final_layer_norm
     elif isinstance(base_model, models.gpt_neox.modeling_gpt_neox.GPTNeoXModel):
@@ -90,26 +121,27 @@
         raise ValueError("Model does not have a final layer norm.")
 
     assert isinstance(final_layer_norm, Norm.__args__)  # type: ignore
 
     return final_layer_norm
 
 
-def get_transformer_layers(model: tr.PreTrainedModel) -> tuple[str, th.nn.ModuleList]:
+def get_transformer_layers(model: Model) -> tuple[str, th.nn.ModuleList]:
     """Get the decoder layers from a model.
 
     Args:
         model: The model to search.
 
     Returns:
         A tuple containing the key path to the layer list and the list itself.
 
     Raises:
         ValueError: If no such list exists.
     """
+    # TODO implement this so that we can do hooked transformer training.
     if not hasattr(model, "base_model"):
         raise ValueError("Model does not have a `base_model` attribute.")
 
     path_to_layers = ["base_model"]
     base_model = model.base_model
     if isinstance(base_model, models.opt.modeling_opt.OPTModel):
         path_to_layers += ["decoder", "layers"]
```

### Comparing `tuned-lens-0.1.1/tuned_lens/nn/lenses.py` & `tuned-lens-0.2.0/tuned_lens/nn/lenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         """
         super().__init__()
 
         self.unembed = unembed
 
     @abc.abstractmethod
     def transform_hidden(self, h: th.Tensor, idx: int) -> th.Tensor:
-        """Convert a hidden state to the final hidden just before the unembeding.
+        """Convert a hidden state to the final hidden just before the unembedding.
 
         Args:
             h: The hidden state to convert.
             idx: The layer of the transformer these hidden states come from.
         """
         ...
 
@@ -216,15 +216,15 @@
             lens_resource_id: The resource id of the lens to load. Defaults to the
                 model's name_or_path.
             **kwargs: Additional arguments to pass to
                 :func:`tuned_lens.load_artifacts.load_lens_artifacts` and
                 `th.load <https://pytorch.org/docs/stable/generated/torch.load.html>`_.
 
         Returns:
-            A TunedLens instance whose unembeding is derived from the given model
+            A TunedLens instance whose unembedding is derived from the given model
             and whose layer translators are loaded from the given resource id.
         """
         if lens_resource_id is None:
             lens_resource_id = model.config.name_or_path
 
         return cls.from_unembed_and_pretrained(
             Unembed(model), lens_resource_id, **kwargs
@@ -259,15 +259,15 @@
 
         with open(config_path, "r") as f:
             config = TunedLensConfig.from_dict(json.load(f))
 
         # validate the unembed is the same as the one used to train the lens
         if config.unembed_hash and unembed.unembedding_hash() != config.unembed_hash:
             warning(
-                "The unembeding matrix hash does not match the lens' hash."
+                "The unembedding matrix hash does not match the lens' hash."
                 "This lens may have been trained with a different unembedding."
             )
 
         # Create the lens
         lens = cls(unembed, config)
 
         th_load_kwargs = {
```

### Comparing `tuned-lens-0.1.1/tuned_lens/nn/unembed.py` & `tuned-lens-0.2.0/tuned_lens/nn/unembed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """Provides a class for mapping transformer hidden states to logits (and vice versa)."""
 import copy
 from dataclasses import dataclass
 from typing import Literal, Optional, cast
 
+try:
+    # Needed for the docs to build without complaining
+    import transformer_lens as tl  # noqa: F401
+
+    _transformer_lens_available = True
+except ImportError:
+    _transformer_lens_available = False
+
 import torch as th
 from torch.distributions import Distribution
-from transformers import PreTrainedModel
 
 from tuned_lens import model_surgery
 from tuned_lens.utils import tensor_hash
 
 
 @dataclass
 class InversionOutput:
@@ -26,32 +33,27 @@
     """Module that maps transformer hidden states to logits (and vice versa)."""
 
     final_norm: model_surgery.Norm
     unembedding: th.nn.Linear
 
     def __init__(
         self,
-        model: PreTrainedModel,
+        model: model_surgery.Model,
     ):
         """Initialize unmebed.
 
         Args:
             model: A HuggingFace model from which to extract the unembedding matrix.
         """
         super().__init__()
         final_norm = model_surgery.get_final_norm(model)
-
-        unembeding_matrix = model.get_output_embeddings()
-        if not isinstance(unembeding_matrix, th.nn.Linear):
-            # With nn.Linear we know that the unembedding matrix is .weight;
-            # we don't want to guess incorrectly for other module classes.
-            raise ValueError("Currently we only support nn.Linear unembeddings.")
+        unembedding_matrix = model_surgery.get_unembedding_matrix(model)
 
         self.final_norm = copy.deepcopy(final_norm)
-        self.unembedding = copy.deepcopy(unembeding_matrix)
+        self.unembedding = copy.deepcopy(unembedding_matrix)
 
         # In general we don't want to finetune the unembed operation.
         self.requires_grad_(False)
 
     def unembedding_hash(self) -> str:
         """Hash the unmbedding matrix to identify the model."""
         parameter = self.unembedding.weight.data.detach().cpu().float().numpy()
```

### Comparing `tuned-lens-0.1.1/tuned_lens/plotting/prediction_trajectory.py` & `tuned-lens-0.2.0/tuned_lens/scripts/train_loop.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,441 +1,451 @@
-"""Plot a lens table for some given text and model."""
-
-import logging
+"""Training loop for training a TunedLens model against a transformer on a dataset."""
+import dataclasses
+import enum
+import re
+from collections import defaultdict
 from dataclasses import dataclass
-from typing import Optional, Sequence, Union
+from pathlib import Path
+from typing import Optional, Union
 
-import numpy as np
 import torch as th
-from numpy.typing import NDArray
-from transformers import (
-    PreTrainedModel,
-    PreTrainedTokenizer,
-    PreTrainedTokenizerFast,
-)
-
-from ..nn.lenses import Lens
-from .token_formatter import TokenFormatter
-from .trajectory_plotting import TrajectoryLabels, TrajectoryStatistic
-
-Tokenizer = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]
-
-
-@dataclass
-class PredictionTrajectory:
-    """Contains the trajectory predictions for a sequence of tokens.
-
-    A prediction trajectory is the set of next token predictions produced by the
-    conjunction of a lens and a model when evaluated on a specific sequence of tokens.
-    This class include multiple methods for visualizing different
-    aspects of the trajectory.
-    """
-
-    # The log probabilities of the predictions for each hidden layer + the models logits
-    # Shape: (num_layers, seq_len, vocab_size)
-    log_probs: NDArray[np.float32]
-    input_ids: NDArray[np.int64]
-    targets: Optional[NDArray[np.int64]] = None
-    tokenizer: Optional[Tokenizer] = None
-
-    def __post_init__(self) -> None:
-        """Validate class invariants."""
-        assert len(self.log_probs.shape) == 3, "log_probs.shape: {}".format(
-            self.log_probs.shape
-        )
-        assert (
-            self.log_probs.shape[1] == self.input_ids.shape[0]
-        ), "log_probs.shape: {}, input_ids.shape: {}".format(
-            self.log_probs.shape, self.input_ids.shape
-        )
-        assert (
-            self.targets is None or self.targets.shape[0] == self.input_ids.shape[0]
-        ), "targets.shape: {}, input_ids.shape: {}".format(
-            self.targets.shape, self.input_ids.shape
-        )
+from simple_parsing import field
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+from torch.distributed.optim import ZeroRedundancyOptimizer
+from torch.optim import Optimizer
+from torch.optim.lr_scheduler import LambdaLR
+from torchdata.dataloader2 import DataLoader2
+from tqdm.auto import trange
+from transformers import PreTrainedModel
+
+import tuned_lens.scripts.ingredients as ing
+from tuned_lens import TunedLens
+from tuned_lens.utils import maybe_all_reduce, shift_labels, shift_preds
 
-    @property
-    def num_layers(self) -> int:
-        """Returns the number of layers in the stream."""
-        return self.log_probs.shape[0] - 1
-
-    @property
-    def num_tokens(self) -> int:
-        """Returns the number of tokens in this slice of the sequence."""
-        return self.log_probs.shape[1]
-
-    @property
-    def vocab_size(self) -> int:
-        """Returns the size of the vocabulary."""
-        return self.log_probs.shape[2]
-
-    @property
-    def model_log_probs(self) -> NDArray[np.float32]:
-        """Returns the log probs of the model."""
-        return self.log_probs[-1, ...]
-
-    @property
-    def probs(self) -> NDArray[np.float32]:
-        """Returns the probabilities of the predictions."""
-        return np.exp(self.log_probs)
-
-    @classmethod
-    def from_lens_and_model(
-        cls,
-        lens: Lens,
-        model: PreTrainedModel,
-        input_ids: Sequence[int],
-        tokenizer: Optional[Tokenizer] = None,
-        targets: Optional[Sequence[int]] = None,
-        start_pos: int = 0,
-        end_pos: Optional[int] = None,
-        mask_input: bool = False,
-    ) -> "PredictionTrajectory":
-        """Constructs a slice of the model's prediction trajectory.
-
-        Args:
-            lens : The lens to use for constructing the latent predictions.
-            model : The model to get the predictions from.
-            tokenizer : The tokenizer to use for decoding the predictions.
-            input_ids : The input ids to pass to the model.
-            targets : The targets for the input sequence.
-            start_pos : The start position of the slice across the sequence dimension.
-            end_pos : The end position of the slice accross the sequence dimension.
-            mask_input : whether to forbid the lens from predicting the input tokens.
-
-        Returns:
-            A PredictionTrajectory object containing the requested slice.
-        """
-        with th.no_grad():
-            input_ids_th = th.tensor(input_ids, dtype=th.int64, device=model.device)
-            outputs = model(input_ids_th.unsqueeze(0), output_hidden_states=True)
-
-        # Slice arrays the specified range
-        model_log_probs = (
-            outputs.logits[..., start_pos:end_pos, :]
-            .log_softmax(-1)
-            .squeeze()
-            .detach()
-            .cpu()
-            .numpy()
-        )
-        stream = [h[..., start_pos:end_pos, :] for h in outputs.hidden_states]
 
-        input_ids_np = np.array(input_ids[start_pos:end_pos])
-        targets_np = (
-            np.array(targets[start_pos:end_pos]) if targets is not None else None
-        )
+class LossChoice(enum.Enum):
+    """Options of what loss to select when training the model."""
 
-        # Create the stream of log probabilities from the lens
-        traj_log_probs = []
-        for i, h in enumerate(stream[:-1]):
-            logits = lens.forward(h, i)
+    CE = "ce"
+    KL = "kl"
 
-            if mask_input:
-                logits[..., input_ids_np] = -th.finfo(h.dtype).max
 
-            traj_log_probs.append(
-                logits.log_softmax(dim=-1).squeeze().detach().cpu().numpy()
-            )
+@dataclass
+class State:
+    """All of the stateful information in the training loop."""
 
-        # Add model predictions
-        if traj_log_probs[-1].shape[-1] != model_log_probs.shape[-1]:
-            logging.warning(
-                "Lens vocab size does not match model vocab size."
-                "Truncating model outputs to match lens vocab size."
-            )
-        # Handle the case where the model has more/less tokens than the lens
-        min_logit = -np.finfo(model_log_probs.dtype).max
-        trunc_model_log_probs = np.full_like(traj_log_probs[-1], min_logit)
-        trunc_model_log_probs[..., : model_log_probs.shape[-1]] = model_log_probs
-
-        traj_log_probs.append(trunc_model_log_probs)
-
-        return cls(
-            tokenizer=tokenizer,
-            log_probs=np.array(traj_log_probs),
-            targets=targets_np,
-            input_ids=input_ids_np,
+    dataloader: DataLoader2
+    lens: TunedLens
+    opt: Optimizer
+    scheduler: LambdaLR
+    wandb_id: Optional[str]
+    nats_to_bpb: float
+    step: int = 0
+
+    def load(self, snapshot_file: Path, device: th.device) -> None:
+        """Load a snapshot file."""
+        print(f"Loading snapshot from {snapshot_file}...")
+        snapshot = th.load(snapshot_file, map_location=device)
+        self.step = snapshot["step"]
+        self.wandb_id = snapshot["wandb_id"]
+        self.lens.load_state_dict(snapshot["lens"])
+        self.opt.load_state_dict(snapshot["optim"])
+        self.scheduler.load_state_dict(snapshot["scheduler"])
+        self.dataloader.load_state_dict(snapshot["dataloader"])
+
+    def save(self, snapshot_file: Path) -> None:
+        """Save a snapshot file."""
+        print(f"Saving snapshot to {snapshot_file}...")
+        if isinstance(self.opt, ZeroRedundancyOptimizer):
+            self.opt.consolidate_state_dict()
+
+        th.save(
+            {
+                "lens": self.lens.state_dict(),
+                "optim": self.opt.state_dict(),
+                "scheduler": self.scheduler.state_dict(),
+                "dataloader": self.dataloader.state_dict(),
+                "step": self.step,
+                "wandb_id": self.wandb_id,
+            },
+            snapshot_file,
         )
 
-    def _get_topk_tokens_and_values(
-        self,
-        k: int,
-        sort_by: NDArray[np.float32],
-        values: NDArray[np.float32],
-    ) -> NDArray[np.str_]:
-
-        # Get the top-k tokens & probabilities for each
-        topk_inds = np.argpartition(sort_by, -k, axis=-1)[..., -k:]
-        topk_sort_by = np.take_along_axis(sort_by, topk_inds, axis=-1)
-        topk_values = np.take_along_axis(values, topk_inds, axis=-1)
-
-        # Ensure that the top-k tokens are sorted by probability
-        sorted_top_k_inds = np.argsort(-topk_sort_by, axis=-1)
-        topk_inds = np.take_along_axis(topk_inds, sorted_top_k_inds, axis=-1)
-        topk_values = np.take_along_axis(topk_values, sorted_top_k_inds, axis=-1)
-
-        # reshape topk_ind from (layers, seq, k) to (layers*seq*k),
-        # convert_ids_to_tokens, then reshape back to (layers, seq, k)
-        topk_tokens = self.tokenizer.convert_ids_to_tokens(topk_inds.flatten().tolist())
-        topk_tokens = np.array(topk_tokens).reshape(topk_inds.shape)
 
-        return topk_tokens, topk_values
-
-    def largest_prob_labels(
-        self,
-        formatter: Optional[TokenFormatter] = None,
-        min_prob: np.float_ = np.finfo(np.float32).eps,
-        topk: int = 10,
-    ) -> TrajectoryLabels:
-        """Labels for the prediction trajectory based on the most probable tokens.
-
-        Args:
-            formatter : The formatter to use for formatting the tokens.
-            min_prob : The minimum probability for a token to used as a label.
-            topk : The number of top tokens to include in the hover over menu.
-
-        Raises:
-            ValueError: If the tokenizer is not set.
-
-        Returns:
-            a set of stream labels that can be applied to a trajectory statistic.
-        """
-        if self.tokenizer is None:
-            raise ValueError("Tokenizer must be set to get labels.")
-
-        if formatter is None:
-            formatter = TokenFormatter()
-
-        input_tokens = self.tokenizer.convert_ids_to_tokens(self.input_ids.tolist())
+@dataclass
+class Train:
+    """Training loop for the tuned lens."""
 
-        entry_format_fn = np.vectorize(
-            lambda token, percent: f"{formatter.format(token)} {percent:.2f}%"
-        )
+    model: ing.Model
+    """Model configuration."""
 
-        topk_tokens, topk_probs = self._get_topk_tokens_and_values(
-            k=topk, sort_by=self.log_probs, values=self.probs
-        )
+    data: ing.Data
+    """Data configuration."""
 
-        top_tokens = topk_tokens[..., 0]
-        top_probs = topk_probs[..., 0]
+    opt: ing.Optimizer
+    """Optimizer configuration."""
 
-        label_strings = np.where(
-            top_probs > min_prob, formatter.vectorized_format(top_tokens), ""
-        )
+    dist: ing.Distributed
+    """Configuration for how to distribute the training."""
 
-        return TrajectoryLabels(
-            label_strings=label_strings,
-            sequence_labels=formatter.vectorized_format(input_tokens),
-            hover_over_entries=entry_format_fn(topk_tokens, topk_probs * 100),
-        )
+    output: Path = field(alias=["-o"])
+    """Directory to save the lenses to."""
 
-    def largest_delta_in_prob_labels(
-        self,
-        other: "PredictionTrajectory",
-        formatter: Optional[TokenFormatter] = None,
-        min_prob_delta: np.float_ = np.finfo(np.float32).eps,
-        topk: int = 10,
-    ) -> TrajectoryLabels:
-        """Labels for a trajectory statistic based on the largest change in probability.
-
-        Args:
-            other : The other prediction trajectory to compare to.
-            formatter : A TokenFormatter to use for formatting the labels.
-            min_prob_delta : The minimum change in probability to include a label.
-            topk : The number of top tokens to include in the hover over menu.
-
-        Raises:
-            ValueError: If the tokenizer is not set.
-
-        Returns:
-            A set of stream labels that can be added to a trajectory statistic.
-        """
-        if self.tokenizer is None:
-            raise ValueError("Tokenizer must be set to get labels.")
+    seed: int = 42
+    """Random seed for data shuffling."""
 
-        if formatter is None:
-            formatter = TokenFormatter()
+    lens_name_or_path: Optional[str] = field(alias=["-l"], default=None)
+    """Name of a pretrained lens to load for fine-tuning."""
 
-        input_tokens = self.tokenizer.convert_ids_to_tokens(self.input_ids.tolist())
+    bias_only: Optional[bool] = field(action="store_true")
+    """Train only the bias term."""
 
-        entry_format_fn = np.vectorize(
-            lambda token, percent: f"{formatter.format(token)} Δ{percent:.2f}%"
-        )
+    num_steps: int = 250
+    """Number of training steps."""
 
-        deltas = other.probs - self.probs
+    tokens_per_step: int = 2**18
+    """Number of tokens per step."""
 
-        topk_tokens, topk_deltas = self._get_topk_tokens_and_values(
-            k=topk, sort_by=np.abs(deltas), values=deltas
-        )
+    wandb: Optional[str] = None
+    """Name of run in Weights & Biases."""
 
-        top_tokens = topk_tokens[..., 0]
-        top_deltas = topk_deltas[..., 0]
+    token_shift: Optional[int] = None
+    """How to shift the labels wrt the input tokens (1 = next token, 0 = current token,
+    -1 = previous token, etc.)"""
 
-        label_strings = np.where(
-            np.abs(top_deltas) > min_prob_delta,
-            formatter.vectorized_format(top_tokens),
-            "",
-        )
+    checkpoint_freq: Optional[int] = None
+    """Steps between saving a checkpoint. If None, no checkpoints are saved."""
 
-        return TrajectoryLabels(
-            label_strings=label_strings,
-            sequence_labels=formatter.vectorized_format(input_tokens),
-            hover_over_entries=entry_format_fn(topk_tokens, 100 * topk_deltas),
-        )
+    checkpoint_dir: Optional[Path] = None
+    """Directory to save checkpoints to. If None, will use <output>/checkpoints."""
 
-    def cross_entropy(self, **kwargs) -> TrajectoryStatistic:
-        """The cross entropy of the predictions to the targets.
+    loss: LossChoice = LossChoice.KL
+    """Loss function to use."""
 
-        Args:
-            **kwargs: are passed to largest_prob_labels.
+    def __post_init__(self):
+        """Set defaults for some fields."""
+        if self.checkpoint_dir is None:
+            self.checkpoint_dir = self.output / "checkpoints"
 
-        Returns:
-            A TrajectoryStatistic with the cross entropy of the predictions to the
-            targets.
-        """
-        if self.targets is None:
-            raise ValueError("Cannot compute cross entropy without targets.")
-
-        assert self.targets.shape == self.log_probs[-1].shape[:-1], (
-            "Batch and sequence lengths of targets and log probs must match."
-            f"Got {self.targets.shape} and {self.log_probs[-1].shape[:-1]}."
-        )
+    def get_lens(self, model: PreTrainedModel) -> TunedLens:
+        """Load or create a TunedLens model."""
+        if self.lens_name_or_path is None:
+            lens = TunedLens.from_model(model)
+        else:
+            lens = TunedLens.from_model_and_pretrained(model, self.lens_name_or_path)
 
-        return TrajectoryStatistic(
-            name="Cross Entropy",
-            units="nats",
-            labels=self.largest_prob_labels(**kwargs) if self.tokenizer else None,
-            stats=-self.log_probs[:, np.arange(self.num_tokens), self.targets],
-        )
+        dtypes = {p.dtype for p in lens.parameters()}
+        assert (
+            len(dtypes) == 1
+        ), f"Expected all parameters to have the same dtype, got {dtypes}"
 
-    def entropy(self, **kwargs) -> TrajectoryStatistic:
-        """The entropy of the predictions.
+        lens_dtype = next(iter(dtypes))
+        lens_size = sum(p.numel() * p.element_size() for p in lens.parameters())
 
-        Args:
-            **kwargs: are passed to largest_prob_labels.
+        # Include the optimizer state in the memory usage
+        num_bytes = lens_size * (self.opt.per_parameter_optim_state_size() + 1)
+        print(f"Tuned lens memory usage: {num_bytes / 2 ** 20:.2f} MB in {lens_dtype}")
 
-        Returns:
-            A TrajectoryStatistic with the entropy of the predictions.
-        """
-        return TrajectoryStatistic(
-            name="Entropy",
-            units="nats",
-            labels=self.largest_prob_labels(**kwargs) if self.tokenizer else None,
-            stats=-np.sum(np.exp(self.log_probs) * self.log_probs, axis=-1),
-        )
+        if self.bias_only:
+            for probe in lens:
+                probe.weight.requires_grad_(False)
 
-    def forward_kl(self, **kwargs) -> TrajectoryStatistic:
-        """KL divergence of the lens predictions to the model predictions.
+        return lens
 
-        Args:
-            **kwargs: are passed to largest_prob_labels.
+    def _get_wandb_id(self) -> Optional[str]:
+        if not self.dist.primary or not self.wandb:
+            return None
 
-        Returns:
-            A TrajectoryStatistic with the KL divergence of the lens predictions to the
-            final output of the model.
-        """
-        model_log_probs = self.model_log_probs.reshape(
-            1, self.num_tokens, self.vocab_size
-        )
-        return TrajectoryStatistic(
-            name="Forward KL",
-            units="nats",
-            labels=self.largest_prob_labels(**kwargs) if self.tokenizer else None,
-            stats=np.sum(
-                np.exp(model_log_probs) * (model_log_probs - self.log_probs), axis=-1
-            ),
-        )
+        from wandb.sdk.lib import runid
 
-    def max_probability(self, **kwargs) -> TrajectoryStatistic:
-        """Max probability of the among the predictions.
+        return runid.generate_id()
 
-        Args:
-            **kwargs: are passed to largest_prob_labels.
+    def _init_logging(self, model_name: str, lens: TunedLens, wandb_id: Optional[str]):
+        """Initialize logging to weights and biases."""
+        if not self.dist.primary or not self.wandb:
+            return
 
-        Returns:
-            A TrajectoryStatistic with the max probability of the among the predictions.
-        """
-        return TrajectoryStatistic(
-            name="Max Probability",
-            units="probs",
-            labels=self.largest_prob_labels(**kwargs) if self.tokenizer else None,
-            stats=np.exp(self.log_probs.max(-1)),
-        )
+        import wandb
 
-    def kl_divergence(
-        self, other: "PredictionTrajectory", **kwargs
-    ) -> TrajectoryStatistic:
-        """Compute the KL divergence between self and other prediction trajectory.
-
-        Args:
-            other : The other prediction trajectory to compare to.
-            **kwargs: are passed to largest_delta_in_prob_labels.
-
-        Returns:
-            A TrajectoryStatistic with the KL divergence between self and other.
-        """
-        kl_div = np.sum(self.probs * (self.log_probs - other.log_probs), axis=-1)
-
-        return TrajectoryStatistic(
-            name="KL(Self | Other)",
-            units="nats",
-            stats=kl_div,
-            labels=self.largest_delta_in_prob_labels(other, **kwargs)
-            if self.tokenizer
-            else None,
-            min=0,
-            max=None,
+        wandb.init(
+            config=dataclasses.asdict(self),
+            group=model_name,
+            name=self.wandb,
+            id=wandb_id,
+            resume="allow",
         )
+        wandb.watch(lens)
 
-    def js_divergence(
-        self, other: "PredictionTrajectory", **kwargs
-    ) -> TrajectoryStatistic:
-        """Compute the JS divergence between self and other prediction trajectory.
-
-        Args:
-            other : The other prediction trajectory to compare to.
-            **kwargs: are passed to largest_delta_in_prob_labels.
-
-        Returns:
-            A TrajectoryStatistic with the JS divergence between self and other.
-        """
-        js_div = 0.5 * np.sum(
-            self.probs * (self.log_probs - other.log_probs), axis=-1
-        ) + 0.5 * np.sum(other.probs * (other.log_probs - self.log_probs), axis=-1)
-
-        return TrajectoryStatistic(
-            name="JS(Self | Other)",
-            units="nats",
-            stats=js_div,
-            labels=self.largest_delta_in_prob_labels(other, **kwargs)
-            if self.tokenizer
-            else None,
-            min=0,
-            max=None,
-        )
+    def _log(
+        self,
+        opt: th.optim.Optimizer,
+        step: int,
+        losses: dict[str, list[float]],
+        tuned_lens: TunedLens,
+        nats_to_bpb: float,
+    ):
+        """Log statistics about the training process to weights and biases."""
+        if not self.dist.primary or not self.wandb:
+            return
+
+        import wandb
+
+        log_dict = {}
+        log_dict.update(
+            {f"loss/{k}": th.tensor(v).mean() * nats_to_bpb for k, v in losses.items()}
+        )
+
+        # Log statistics about optimizer & probes
+        for i, probe in enumerate(tuned_lens):
+            name = "input" if i == 0 else f"{i - 1}.ffn"
+            states = [opt.state[p] for p in probe.parameters()]
+
+            # Approximate the true grad norm using the optimizer's moving
+            # avg
+            corr = 1 - self.opt.momentum**step
+            if self.opt.optimizer == "sgd" and not self.opt.zero:
+                log_dict["grad_norm/" + name] = th.cat(
+                    [
+                        # Undo PyTorch's scaling of the gradient by
+                        # 1 / (1 - β)
+                        (1 - self.opt.momentum) * s["momentum_buffer"].flatten() / corr
+                        for s in states
+                    ]
+                ).norm()
+            elif self.opt.optimizer == "adam" and not self.opt.zero:
+                log_dict["grad_norm/" + name] = th.cat(
+                    [s["exp_avg"].flatten() / corr for s in states]
+                ).norm()
+
+            if isinstance(probe, th.nn.Linear):
+                log_dict["bias_norm/" + name] = probe.bias.data.norm()
+                log_dict["weight_norm/" + name] = probe.weight.data.norm()
+
+        wandb.log(log_dict)
+
+    def snapshot(self, state: State):
+        """Save a snapshot of the training process to disk."""
+        if self.dist.primary:
+            assert self.checkpoint_dir is not None
+            self.checkpoint_dir.mkdir(parents=True, exist_ok=True)
+            state.save(self.checkpoint_dir / f"snapshot_{state.step}.pth")
+
+    def load_recent_snapshot(self, state: State) -> None:
+        """Load the most recent snapshot of the training process from disk."""
+        assert self.checkpoint_dir is not None
+
+        if not self.checkpoint_dir.exists():
+            return None
+
+        # Find the folder containing the most recent snapshot
+        def sort_key_from_path(p: Path):
+            if match := re.match(r".*snapshot_(\d+)\.pth", str(p)):
+                return int(match.group(1))
+            else:
+                return -1
+
+        snapshot_location = max(
+            self.checkpoint_dir.glob("snapshot_*.pth"),
+            key=sort_key_from_path,
+            default=None,
+        )
+
+        if snapshot_location is None:
+            return None
+
+        state.load(snapshot_location, self.dist.device)
+
+    def calculate_gradient_accumulation_steps(self, tokens_per_sample: int) -> int:
+        """Calculate the number of batches of data to process before taking a step."""
+        # chunk_and_tokenize ensures the samples are all the same length
+        samples_per_step, rem = divmod(self.tokens_per_step, tokens_per_sample)
+        if rem:
+            raise ValueError(
+                f"Number of tokens per step ({self.tokens_per_step:_}) must be "
+                f"divisible by the number of tokens per sample ({tokens_per_sample})."
+            )
 
-    def total_variation(
-        self, other: "PredictionTrajectory", **kwargs
-    ) -> TrajectoryStatistic:
-        """Total variation distance between self and other prediction trajectory.
-
-        Args:
-            other : The other prediction trajectory to compare to.
-            **kwargs: are passed to largest_delta_in_prob_labels.
-
-        Returns:
-            A TrajectoryStatistic with the total variational distance between
-            self and other.
-        """
-        t_var = np.abs(self.probs - other.probs).max(axis=-1)
-
-        return TrajectoryStatistic(
-            name="TV(Self | Other)",
-            units="probs",
-            stats=t_var,
-            labels=self.largest_delta_in_prob_labels(other, **kwargs)
-            if self.tokenizer
-            else None,
-            min=0,
-            max=1,
-        )
+        global_batch_size = self.dist.per_gpu_batch_size * self.dist.world_size
+        grad_acc_steps, rem = divmod(samples_per_step, global_batch_size)
+        if rem:
+            # If the number of samples per step isn't divisible by the global batch
+            # size, use ceil division and let the user know about it.
+            grad_acc_steps += 1
+            adjusted_count = grad_acc_steps * global_batch_size * tokens_per_sample
+            print(
+                f"Note: Increasing grad acc steps from {grad_acc_steps - 1} to "
+                f"{grad_acc_steps} to maintain load balance across "
+                f"{self.dist.world_size} GPUs."
+            )
+            print(
+                f"Using {adjusted_count:_} tokens per training step "
+                f"({self.tokens_per_step:_} requested)."
+            )
+        else:
+            print(f"Gradient accumulation steps: {grad_acc_steps}")
+            print(f"Using {self.tokens_per_step:_} tokens per training step.")
+        return grad_acc_steps
+
+    def setup(self) -> tuple[State, Union[PreTrainedModel, FSDP], int]:
+        """Initialize the training process."""
+        self.dist.init()
+        model = tokenizer = data = lens = nats_to_bpb = None
+
+        # Annoyingly, FSDP is incompatible with the `device_map` parameter on
+        # `from_pretrained`, because it adds forward hooks to the submodules that move
+        # things around to different devices. But `bitsandbytes` requires `device_map`
+        # to work at all. So we use `device_map` iff we're using FSDP.
+        load_device = self.dist.device if not self.dist.fsdp else None
+
+        if self.dist.primary:
+            # Let the primary processes populate the cache
+            model, tokenizer = self.model.load(load_device)
+            data, nats_to_bpb = self.data.load(tokenizer)
+            lens = self.get_lens(model)
+
+        self.dist.barrier()  # Wait for primary to finish filling the cache
+
+        if not self.dist.primary:
+            # Let the non-primary processes load from the cache
+            model, tokenizer = self.model.load(load_device, must_use_cache=True)
+            data, nats_to_bpb = self.data.load(tokenizer)
+            lens = self.get_lens(model)
+
+        assert model and tokenizer and data and lens and nats_to_bpb
+
+        dl = self.dist.data_loader(data)
+        dl.seed(self.seed)
+        params = [p for p in lens.parameters() if p.requires_grad]
+        opt = self.opt.create_optim(params)
+        scheduler = self.opt.create_scheduler(opt, self.num_steps)
+
+        # Distribute the lens across the GPUS using distributed data parallel
+        ddp_lens = self.dist.distribute_lens(lens)
+
+        state = State(
+            step=0,
+            wandb_id=self._get_wandb_id(),
+            lens=ddp_lens,  # type: ignore
+            opt=opt,
+            scheduler=scheduler,
+            dataloader=dl,
+            nats_to_bpb=nats_to_bpb,
+        )
+
+        self.load_recent_snapshot(state)
+
+        # Shard the model using fully shared data parallel
+        model = self.dist.shard_model(model)
+
+        self._init_logging(
+            model_name=self.model.name, lens=state.lens, wandb_id=state.wandb_id
+        )
+
+        tokens_per_sample = len(data[0]["input_ids"])
+        grad_acc_steps = self.calculate_gradient_accumulation_steps(tokens_per_sample)
+        self.dist.barrier()  # Wait for all processes to finish setup
+        print("All processes have completed setup.")
+        return state, model, grad_acc_steps
+
+    def execute(self):
+        """Trains a TunedLens model against a transformer on a dataset."""
+        # Load model, tokenizer, data, and lens
+        state, model, grad_acc_steps = self.setup()
+
+        losses = defaultdict(list)
+        init_batches = state.step * grad_acc_steps
+        total_batches = self.num_steps * grad_acc_steps
+
+        # Wait for all processes to finish setup
+        self.dist.barrier()
+        print("All processes have completed setup. Starting training.")
+
+        # Main training loop
+        t = trange(
+            init_batches,
+            total_batches,
+            desc="Training",
+            initial=init_batches,
+            total=total_batches,
+        )
+        # TODO this currently silently fails if the dataloader is exhausted
+        for batch_idx, batch in zip(t, state.dataloader):
+            assert isinstance(batch, dict), f"Expected dict, got {type(batch)}"
+
+            with th.no_grad():
+                batch = self.dist.send_to_device(batch)
+                output = model(**batch, output_hidden_states=True)
+
+            final_logits = output.logits
+            hidden_states = output.hidden_states[:-1]
+
+            shift = self.token_shift
+            if self.loss == LossChoice.CE:
+                labels = batch["input_ids"]
+
+                # Predict the *next* token by default w/ cross entropy
+                if shift is None:
+                    shift = 1
+            elif self.loss == LossChoice.KL:
+                labels = final_logits.float().log_softmax(dim=-1)
+
+                # Match the *current* token distribution by default
+                if shift is None:
+                    shift = 0
+            else:
+                raise NotImplementedError(f"Unknown loss {self.loss}")
+
+            labels = shift_labels(labels, shift)
+
+            # We do this sequentially to save VRAM
+            for i, h in enumerate(hidden_states):
+                # We use bfloat16 because it has a larger dynamic range than float16
+                # and it seems to remove the need for doing grad scaling, which is very
+                # annoying to set up in the context of multiple backward passes.
+                with th.autocast(self.dist.device.type, dtype=th.bfloat16):
+                    logits = shift_preds(state.lens(h, idx=i), shift)
+
+                    if self.loss == LossChoice.CE:
+                        loss = th.nn.functional.cross_entropy(
+                            logits.flatten(0, -2), labels.flatten()
+                        )
+                    elif self.loss == LossChoice.KL:
+                        loss = th.sum(
+                            labels.exp() * (labels - logits.log_softmax(-1)), dim=-1
+                        ).mean()
+                    else:
+                        raise NotImplementedError
+
+                    # Log the loss *before* LASSO regularization
+                    logging_loss = loss.detach()
+                    logging_loss = maybe_all_reduce(logging_loss).item()
+                    if self.dist.primary:
+                        losses[f"translator_{i}"].append(logging_loss)
+
+                    scaled_loss = loss / grad_acc_steps
+
+                scaled_loss.backward()
+
+            step, rem = divmod(batch_idx, grad_acc_steps)
+            if rem == grad_acc_steps - 1:
+                th.nn.utils.clip_grad_norm_(state.lens.parameters(), 1.0)
+                state.opt.step()
+                state.opt.zero_grad(set_to_none=False)
+                state.scheduler.step()
+
+                # Unwrap the lens from DDP if needed
+                lens = getattr(state.lens, "module", state.lens)
+                self._log(state.opt, step, losses, lens, state.nats_to_bpb)
+                losses.clear()
+                state.step = step + 1
+                if (
+                    self.checkpoint_freq
+                    and step % self.checkpoint_freq == self.checkpoint_freq - 1
+                ):
+                    self.snapshot(state)
+
+        if self.dist.primary:
+            print(f"Saving lens to {self.output}")
+
+            # Unwrap the lens from DDP if needed
+            lens = getattr(state.lens, "module", state.lens)
+            lens.save(self.output)
```

### Comparing `tuned-lens-0.1.1/tuned_lens/plotting/token_formatter.py` & `tuned-lens-0.2.0/tuned_lens/plotting/token_formatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,7 +26,15 @@
             return "<unk>"
 
         if self.max_string_len is not None and len(token) > self.max_string_len:
             token = token[: self.max_string_len - len(self.ellipsis)] + self.ellipsis
         token = token.replace(self.newline_token, self.newline_replacement)
         token = token.replace(self.whitespace_token, self.whitespace_replacement)
         return token
+
+    def pad_token_repr_to_max_len(self, token_repr: str) -> str:
+        """Pad a token representation to the max string length."""
+        if self.max_string_len is None:
+            return token_repr
+        return token_repr[: self.max_string_len] + " " * (
+            self.max_string_len - len(token_repr)
+        )
```

### Comparing `tuned-lens-0.1.1/tuned_lens/scripts/eval_loop.py` & `tuned-lens-0.2.0/tuned_lens/scripts/eval_loop.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/scripts/ingredients.py` & `tuned-lens-0.2.0/tuned_lens/scripts/ingredients.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/stats/distance.py` & `tuned-lens-0.2.0/tuned_lens/stats/distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/stats/logit_stats.py` & `tuned-lens-0.2.0/tuned_lens/stats/logit_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens/utils.py` & `tuned-lens-0.2.0/tuned_lens/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.1/tuned_lens.egg-info/PKG-INFO` & `tuned-lens-0.2.0/tuned_lens.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: transformer_lens
 Provides-Extra: slow_tokenizers
 Provides-Extra: notebooks
 Provides-Extra: 8bit
 License-File: LICENSE
 
 # Tuned Lens 🔎
 <a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
```

### Comparing `tuned-lens-0.1.1/tuned_lens.egg-info/SOURCES.txt` & `tuned-lens-0.2.0/tuned_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

