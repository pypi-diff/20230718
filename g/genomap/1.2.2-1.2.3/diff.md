# Comparing `tmp/genomap-1.2.2.tar.gz` & `tmp/genomap-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.2.2.tar", last modified: Mon Jul 17 21:16:35 2023, max compression
+gzip compressed data, was "genomap-1.2.3.tar", last modified: Mon Jul 17 22:18:46 2023, max compression
```

## Comparing `genomap-1.2.2.tar` & `genomap-1.2.3.tar`

### file list

```diff
@@ -1,65 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.397071 genomap-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 21:12:42.000000 genomap-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 21:12:42.000000 genomap-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 21:16:35.397071 genomap-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-17 21:12:43.000000 genomap-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 21:12:43.000000 genomap-1.2.2/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.389071 genomap-1.2.2/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.393071 genomap-1.2.2/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.393071 genomap-1.2.2/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.397071 genomap-1.2.2/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 21:12:43.000000 genomap-1.2.2/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:35.385071 genomap-1.2.2/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 21:16:35.000000 genomap-1.2.2/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 21:12:43.000000 genomap-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:16:35.397071 genomap-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 21:12:43.000000 genomap-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.497747 genomap-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 22:14:51.000000 genomap-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 22:14:51.000000 genomap-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 22:18:46.497747 genomap-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-17 22:14:52.000000 genomap-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 22:14:52.000000 genomap-1.2.3/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.497747 genomap-1.2.3/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 22:14:52.000000 genomap-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:18:46.497747 genomap-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 22:14:52.000000 genomap-1.2.3/setup.py
```

### Comparing `genomap-1.2.2/LICENSE.txt` & `genomap-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/PKG-INFO` & `genomap-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.2
+Version: 1.2.3
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.2.2/README.md` & `genomap-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.2.3/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoClassification/genoClassification.py` & `genomap-1.2.3/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoDR/genoDimReduction.py` & `genomap-1.2.3/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoMOI/genoMOI.py` & `genomap-1.2.3/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.2.3/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoRegression/genoRegression.py` & `genomap-1.2.3/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoSig/genoSig.py` & `genomap-1.2.3/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoTraj/genoTraj.py` & `genomap-1.2.3/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genoVis/genoVis.py` & `genomap-1.2.3/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genomap.py` & `genomap-1.2.3/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genomapOPT/genomapOPT.py` & `genomap-1.2.3/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/genomapT/genomapT.py` & `genomap-1.2.3/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/ConvDEC.py` & `genomap-1.2.3/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/ConvIDEC.py` & `genomap-1.2.3/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/FcDEC.py` & `genomap-1.2.3/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/FcIDEC.py` & `genomap-1.2.3/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/class_discriminative_opt.py` & `genomap-1.2.3/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/gTraj_utils.py` & `genomap-1.2.3/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/group_centroid_opt.py` & `genomap-1.2.3/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/metrics.py` & `genomap-1.2.3/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/util_Sig.py` & `genomap-1.2.3/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap/utils/utils_MOI.py` & `genomap-1.2.3/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.2/genomap.egg-info/PKG-INFO` & `genomap-1.2.3/genomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.2
+Version: 1.2.3
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.2.2/setup.py` & `genomap-1.2.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.2.2",
+    version="1.2.3",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    packages=find_packages(exclude=("genomap.genoNet", "genomap.genoNetus")),
+    packages=find_packages(exclude=("genomap.genoNetus")),
     python_requires=">=3.8",
     install_requires=open("requirements.txt").readlines(),
     include_package_data=True,
 )
```

