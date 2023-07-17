# Comparing `tmp/genomap-1.2.3.tar.gz` & `tmp/genomap-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.2.3.tar", last modified: Mon Jul 17 22:18:46 2023, max compression
+gzip compressed data, was "genomap-1.2.4.tar", last modified: Mon Jul 17 23:14:06 2023, max compression
```

## Comparing `genomap-1.2.3.tar` & `genomap-1.2.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.497747 genomap-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 22:14:51.000000 genomap-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 22:14:51.000000 genomap-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 22:18:46.497747 genomap-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-17 22:14:52.000000 genomap-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 22:14:52.000000 genomap-1.2.3/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.485747 genomap-1.2.3/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.489747 genomap-1.2.3/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.493747 genomap-1.2.3/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.497747 genomap-1.2.3/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 22:14:52.000000 genomap-1.2.3/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:18:46.481747 genomap-1.2.3/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 22:18:46.000000 genomap-1.2.3/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 22:14:52.000000 genomap-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:18:46.497747 genomap-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 22:14:52.000000 genomap-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.761431 genomap-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 23:10:10.000000 genomap-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 23:10:10.000000 genomap-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-17 23:14:06.761431 genomap-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-17 23:10:10.000000 genomap-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.741431 genomap-1.2.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 23:10:10.000000 genomap-1.2.4/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.741431 genomap-1.2.4/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.749431 genomap-1.2.4/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.749431 genomap-1.2.4/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.761431 genomap-1.2.4/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 23:10:10.000000 genomap-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:14:06.761431 genomap-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 23:10:10.000000 genomap-1.2.4/setup.py
```

### Comparing `genomap-1.2.3/LICENSE.txt` & `genomap-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/PKG-INFO` & `genomap-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.3
+Version: 1.2.4
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -35,24 +35,24 @@
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
-from genomap import construct_genomap
+import genomap as gp
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 colNum=33 # Column number of genomap
 rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
+genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
 findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
 plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
 plt.show()
@@ -60,30 +60,30 @@
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoVis import genoVis
+import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
-resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
@@ -99,25 +99,25 @@
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genomap.genoDR import genoDR
+import genomap.genoDR as gp
 import matplotlib.pyplot as plt
 import umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -135,24 +135,24 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
-from genomap.genoTraj import genoTraj
+import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=genoTraj(data)
+outGenoTraj=gp.genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
@@ -178,15 +178,15 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-from genomap.genoMOI import genoMOI
+import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import umap
 
 
 # Load five different pancreatic datasets
@@ -204,15 +204,15 @@
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -226,15 +226,15 @@
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from genomap.genoSig import genoSig
+import genomap.genoSig as gp
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
@@ -245,26 +245,26 @@
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
-result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
+result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoClassification import genoClassification
+import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
@@ -282,27 +282,27 @@
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
-est=genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
+est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoRegression import genoRegression
+import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
 from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('GT_Org.mat')
@@ -313,15 +313,15 @@
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
-est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
+est=gp.genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
 print(f'MSE: {mse}')
 ```
 
 # Citation
```

### Comparing `genomap-1.2.3/README.md` & `genomap-1.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,24 @@
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
-from genomap import construct_genomap
+import genomap as gp
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 colNum=33 # Column number of genomap
 rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
+genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
 findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
 plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
 plt.show()
@@ -47,30 +47,30 @@
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoVis import genoVis
+import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
-resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
@@ -86,25 +86,25 @@
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genomap.genoDR import genoDR
+import genomap.genoDR as gp
 import matplotlib.pyplot as plt
 import umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -122,24 +122,24 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
-from genomap.genoTraj import genoTraj
+import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=genoTraj(data)
+outGenoTraj=gp.genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
@@ -165,15 +165,15 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-from genomap.genoMOI import genoMOI
+import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import umap
 
 
 # Load five different pancreatic datasets
@@ -191,15 +191,15 @@
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -213,15 +213,15 @@
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from genomap.genoSig import genoSig
+import genomap.genoSig as gp
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
@@ -232,26 +232,26 @@
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
-result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
+result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoClassification import genoClassification
+import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
@@ -269,27 +269,27 @@
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
-est=genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
+est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoRegression import genoRegression
+import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
 from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('GT_Org.mat')
@@ -300,15 +300,15 @@
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
-est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
+est=gp.genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
 print(f'MSE: {mse}')
 ```
 
 # Citation
```

### Comparing `genomap-1.2.3/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.2.4/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoClassification/genoClassification.py` & `genomap-1.2.4/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoDR/genoDimReduction.py` & `genomap-1.2.4/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoMOI/genoMOI.py` & `genomap-1.2.4/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoNet/genoNet.py` & `genomap-1.2.4/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.2.4/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoNetus/genoNetus.py` & `genomap-1.2.4/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoRegression/genoRegression.py` & `genomap-1.2.4/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoSig/genoSig.py` & `genomap-1.2.4/genomap/genoSig/genoSig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoTraj/genoTraj.py` & `genomap-1.2.4/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genoVis/genoVis.py` & `genomap-1.2.4/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genomap.py` & `genomap-1.2.4/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genomapOPT/genomapOPT.py` & `genomap-1.2.4/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/genomapT/genomapT.py` & `genomap-1.2.4/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/ConvDEC.py` & `genomap-1.2.4/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/ConvIDEC.py` & `genomap-1.2.4/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/FcDEC.py` & `genomap-1.2.4/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/FcIDEC.py` & `genomap-1.2.4/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/class_discriminative_opt.py` & `genomap-1.2.4/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/gTraj_utils.py` & `genomap-1.2.4/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/group_centroid_opt.py` & `genomap-1.2.4/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/metrics.py` & `genomap-1.2.4/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/util_Sig.py` & `genomap-1.2.4/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap/utils/utils_MOI.py` & `genomap-1.2.4/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.3/genomap.egg-info/PKG-INFO` & `genomap-1.2.4/genomap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.3
+Version: 1.2.4
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -35,24 +35,24 @@
 ### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy
-from genomap import construct_genomap
+import genomap as gp
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 colNum=33 # Column number of genomap
 rowNum=33 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
-genoMaps=construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
+genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum,epsilon=0.0,num_iter=200) # Construction of genomaps
 
 findI=genoMaps[10,:,:,:]
 
 plt.figure(1) # Plot the first genomap
 plt.imshow(findI, origin = 'lower',  extent = [0, 10, 0, 10], aspect = 1)
 plt.title('Genomap of a cell from TM dataset')
 plt.show()
@@ -60,30 +60,30 @@
 
 ### Example 2 - Try genoVis for data visualization and clustering
 
 ```python
 import scipy.io as sio
 import numpy as np
 import pandas as pd
-from genomap.genoVis import genoVis
+import genomap.genoVis as gp
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
-resVis=genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 # Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
@@ -99,25 +99,25 @@
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
 ```python
 import scipy.io as sio
 import numpy as np
-from genomap.genoDR import genoDR
+import genomap.genoDR as gp
 import matplotlib.pyplot as plt
 import umap
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
 #resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -135,24 +135,24 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from sklearn.decomposition import PCA
 import phate
 import umap
-from genomap.genoTraj import genoTraj
+import genomap.genoTraj as gp
 
 # Load data
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 # Apply genoTraj for embedding showing cell trajectories
-outGenoTraj=genoTraj(data)
+outGenoTraj=gp.genoTraj(data)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(outGenoTraj[:, 0], outGenoTraj[:, 1], c=Y_time,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoTraj1')
 plt.ylabel('genoTraj2')
 plt.tight_layout()
@@ -178,15 +178,15 @@
 ```
 
 ### Example 5 - Try genoMOI for multi-omic data integration
 
 ```python
 import scanpy as sc
 import matplotlib.pyplot as plt
-from genomap.genoMOI import genoMOI
+import genomap.genoMOI as gp
 import scipy.io as sio
 import numpy as np
 import pandas as pd
 import umap
 
 
 # Load five different pancreatic datasets
@@ -204,15 +204,15 @@
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
 # Apply genoMOI
-resVis=genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
@@ -226,15 +226,15 @@
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
 ```python
 import numpy as np
 import scipy.io as sio
 from genomap.utils.util_Sig import createGenomap_for_sig
 import pandas as pd
-from genomap.genoSig import genoSig
+import genomap.genoSig as gp
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
@@ -245,26 +245,26 @@
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
 rowNum=32 # genomap row number
 # Create genomaps
 genoMaps,gene_namesRe,T=createGenomap_for_sig(data,gene_names,rowNum,colNum)
 # compute the gene signatures
-result=genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
+result=gp.genoSig(genoMaps,T,label,userPD,gene_namesRe, epochs=50)
 
 print(result.head())
 ```
 
 ### Example 7 - Try genoClassification for tabular data classification
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoClassification import genoClassification
+import genomap.genoClassification as gp
 from genomap.utils.util_genoClassReg import select_random_values
 
 # First, we load the TM data. Data should be in cells X genes format, 
 data = pd.read_csv('TM_data.csv', header=None,
                    delim_whitespace=False)
 
 # Creation of genomaps
@@ -282,27 +282,27 @@
 indxTrain, indxTest= select_random_values(start=0, end=GT.shape[0], perc=0.8)
 groundTruthTest = GT[indxTest-1]
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
-est=genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
+est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
 print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
 import numpy as np
 import scipy.io as sio
-from genomap.genoRegression import genoRegression
+import genomap.genoRegression as gp
 from sklearn.metrics import mean_squared_error
 from genomap.utils.util_genoClassReg import select_random_values
 
 # Load data and labels
 dx = sio.loadmat('organoidData.mat')
 data=dx['X3']
 gt_data = sio.loadmat('GT_Org.mat')
@@ -313,15 +313,15 @@
 indxTrain, indxTest= select_random_values(start=0, end=Y_time.shape[0], perc=0.8)
 groundTruthTest = Y_time[indxTest-1]
 training_data=data[indxTrain-1]
 training_labels=Y_time[indxTrain-1]
 test_data=data[indxTest-1]
 
 # Run genoRegression
-est=genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
+est=gp.genoRegression(training_data, training_labels, test_data, rowNum=40, colNum=40, epoch=200)
 
 # Calculate MSE
 mse = mean_squared_error(groundTruthTest, est)
 print(f'MSE: {mse}')
 ```
 
 # Citation
```

### Comparing `genomap-1.2.3/genomap.egg-info/SOURCES.txt` & `genomap-1.2.4/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

