# Comparing `tmp/genomap-1.2.4.tar.gz` & `tmp/genomap-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.2.4.tar", last modified: Mon Jul 17 23:14:06 2023, max compression
+gzip compressed data, was "genomap-1.2.9.tar", last modified: Tue Jul 18 16:58:25 2023, max compression
```

## Comparing `genomap-1.2.4.tar` & `genomap-1.2.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.761431 genomap-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-17 23:10:10.000000 genomap-1.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 23:10:10.000000 genomap-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-17 23:14:06.761431 genomap-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-17 23:10:10.000000 genomap-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.741431 genomap-1.2.4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-17 23:10:10.000000 genomap-1.2.4/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.741431 genomap-1.2.4/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap/genoClassification/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoClassification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoClassification/genoClassification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.749431 genomap-1.2.4/genomap/genoDR/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoDR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoDR/genoDimReduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.749431 genomap-1.2.4/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNet/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNet/genoNet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNetRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetRegression/genoNet_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.753431 genomap-1.2.4/genomap/genoNetus/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoNetus/genoNetus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoRegression/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoRegression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoRegression/genoRegression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoSig/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoSig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoSig/genoSig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.757431 genomap-1.2.4/genomap/genomapT/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/genomapT/genomapT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.761431 genomap-1.2.4/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/util_Sig.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/util_genoClassReg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-17 23:10:10.000000 genomap-1.2.4/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 23:14:06.745431 genomap-1.2.4/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 23:14:06.000000 genomap-1.2.4/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-17 23:10:10.000000 genomap-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 23:14:06.761431 genomap-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-17 23:10:10.000000 genomap-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.949687 genomap-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-18 16:54:01.000000 genomap-1.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 16:54:01.000000 genomap-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-18 16:58:25.945687 genomap-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-18 16:54:01.000000 genomap-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 16:54:01.000000 genomap-1.2.9/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoClassification/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoClassification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoClassification/genoClassification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoDR/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoDR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoDR/genoDimReduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.933687 genomap-1.2.9/genomap/genoNet/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNet/genoNet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoNetRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetRegression/genoNet_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoNetus/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoNetus/genoNetus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoRegression/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoRegression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoRegression/genoRegression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoSig/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoSig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoSig/genoSig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.937687 genomap-1.2.9/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.941687 genomap-1.2.9/genomap/genomapT/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/genomapT/genomapT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.945687 genomap-1.2.9/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/util_Sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/util_genoClassReg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-18 16:54:01.000000 genomap-1.2.9/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:58:25.929687 genomap-1.2.9/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 16:58:25.000000 genomap-1.2.9/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 16:54:01.000000 genomap-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:58:25.949687 genomap-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-18 16:54:01.000000 genomap-1.2.9/setup.py
```

### Comparing `genomap-1.2.4/LICENSE.txt` & `genomap-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/PKG-INFO` & `genomap-1.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.4
+Version: 1.2.9
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -76,27 +76,28 @@
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
+# Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
 import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
@@ -109,24 +110,25 @@
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-#resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
+reduced_dim=32 # Number of reduced dimension
+resDR=gp.genoDR(data, n_dim=reduced_dim, n_clusters=n_clusters, colNum=33,rowNum=33) 
+#resDR=gp.genoDR(data, n_dim=reduced_dim, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
@@ -203,25 +205,25 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
@@ -234,14 +236,15 @@
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
+# Here we create artificial gene names as Gene_1, Gene_2. You can upload your gene sets
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
@@ -284,15 +287,15 @@
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
-print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
+print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
```

### Comparing `genomap-1.2.4/README.md` & `genomap-1.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,27 +63,28 @@
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
+# Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
 import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
@@ -96,24 +97,25 @@
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-#resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
+reduced_dim=32 # Number of reduced dimension
+resDR=gp.genoDR(data, n_dim=reduced_dim, n_clusters=n_clusters, colNum=33,rowNum=33) 
+#resDR=gp.genoDR(data, n_dim=reduced_dim, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
@@ -190,25 +192,25 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
@@ -221,14 +223,15 @@
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
+# Here we create artificial gene names as Gene_1, Gene_2. You can upload your gene sets
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
@@ -271,15 +274,15 @@
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
-print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
+print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
```

### Comparing `genomap-1.2.4/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.2.9/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoClassification/genoClassification.py` & `genomap-1.2.9/genomap/genoClassification/genoClassification.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoDR/genoDimReduction.py` & `genomap-1.2.9/genomap/genoDR/genoDimReduction.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoMOI/genoMOI.py` & `genomap-1.2.9/genomap/genoMOI/genoMOI.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
 from genomap.utils.gTraj_utils import nearest_divisible_by_four
 from genomap.utils.utils_MOI import * 
 from genomap.utils.util_Sig import select_n_features
 
-def genoMOI(*arrays,n_clusters=None, colNum, rowNum):  
+def genoMOI(*arrays, n_clusters=None, n_dim=32, colNum=32, rowNum=32):
 
-# arrays: number of arrays such as array1,array2
+# arrays: a number of arrays such as array1, array2 from different sources
 # n_clusters: number of data classes
-# colNum and rowNum: column are rwo number of genomaps
+# n_dim: number of the dimension in returned integrated data
+# colNum and rowNum: column and row number of genomaps
 #
 # Pre-align data with bbknn
     batch_corrected_data=apply_bbknn_and_return_batch_corrected(*arrays)
     dataDX=scipy.stats.zscore(batch_corrected_data, axis=0, ddof=1) 
     
     if n_clusters==None:
         array1=arrays[0]
@@ -30,20 +31,20 @@
         # Perform Louvain clustering
         sc.pp.neighbors(adata)
         sc.tl.louvain(adata, resolution=1.0)
         # Access the cluster assignments
         cluster_labels = adata.obs['louvain']
         n_clusters = len(np.unique(cluster_labels))        
     
-    resVis=extract_genoVis_features(dataDX,n_clusters=n_clusters, colNum=colNum,rowNum=rowNum)
+    resVis=extract_genoVis_features(dataDX, n_clusters=n_clusters, n_dim=n_dim, colNum=colNum,rowNum=rowNum)
     return resVis
 
 
-def extract_genoVis_features(data,n_clusters=20, colNum=32,rowNum=32,batch_size=64,verbose=1,
-                    pretrain_epochs=100,maxiter=300):
+def extract_genoVis_features(data,n_clusters=20, n_dim=32, colNum=32, rowNum=32, batch_size=64, verbose=1,
+                    pretrain_epochs=100, maxiter=300):
 # rowNum and colNum are the row and column numbers of constructed genomaps
 # n_clusters: number of data classes in the data
 # batch_size: number of samples in each mini batch while training the deep neural network
 # verbose: whether training progress will be shown or not
 # pretrain_epochs: number of epoch for pre-training the CNN
 # maxiter: number of epoch of fine-tuning training
 # Construction of genomap    
@@ -52,15 +53,15 @@
     nump=rowNum*colNum 
     if nump<data.shape[1]:
         data,index=select_n_features(data,nump) 
     genoMaps=construct_genomap(data,rowNum,colNum,epsilon=0.0,num_iter=200)
 
 # Deep learning-based dimensionality reduction and clustering
     optimizer = Adam()    
-    model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, 32], n_clusters=n_clusters)
+    model = ConvIDEC(input_shape=genoMaps.shape[1:], filters=[32, 64, 128, n_dim], n_clusters=n_clusters)
     model.compile(optimizer=optimizer, loss=['kld', 'mse'], loss_weights=[0.1, 1.0])
     pretrain_optimizer ='adam'
     update_interval=50
     model.pretrain(genoMaps, y=None, optimizer=pretrain_optimizer, epochs=pretrain_epochs, batch_size=batch_size,
                         verbose=verbose)
 
     y_pred = model.fit(genoMaps, y=None, maxiter=maxiter, batch_size=batch_size, update_interval=update_interval,
```

### Comparing `genomap-1.2.4/genomap/genoNet/genoNet.py` & `genomap-1.2.9/genomap/genoNet/genoNet.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoNetRegression/genoNet_regression.py` & `genomap-1.2.9/genomap/genoNetRegression/genoNet_regression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoNetus/genoNetus.py` & `genomap-1.2.9/genomap/genoNetus/genoNetus.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoRegression/genoRegression.py` & `genomap-1.2.9/genomap/genoRegression/genoRegression.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoSig/genoSig.py` & `genomap-1.2.9/genomap/genoSig/genoSig.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 def rgb2gray(image):
     return np.dot(image[...,:3], [0.2989, 0.5870, 0.1140])
 
 import numpy as np
 import pandas as pd
 
 def arrays_to_dataframe(arrays, strings):
+    # converts a numpy array to a panda dataframe
     # Check if the number of arrays is even
     if len(arrays) % 2 != 0:
         raise ValueError("The number of arrays should be even.")
 
     # Check if the number of strings is half the number of arrays
     if len(strings) != len(arrays) // 2:
         raise ValueError("The number of strings should be half the number of arrays.")
@@ -101,34 +102,49 @@
 
     return df
 
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 
 def genoSig(genoMaps,T,label,userPD,gene_names, epochs=100):
+
+    """
+    Returns the gene names and their importance score in the range of 0 to 255 in a specific data class
+
+    Parameters
+    ----------
+    genoMaps : ndarray, shape (cellNum, rowNum, colNum, 1)
+    T: numpy array, shape (geneNum, geneNum)
+        transfer function that converts the transformation of 1D to 2D.
+    label : numpy array,
+         cell labels of the data
+    userPD : numpy array,
+         the classes for which gene signature should be computed
+
+    Returns
+    -------
+    result : panda dataframe containing the gene names and their importance scores in different classes
+    """
+
     genoMaps_3d = np.repeat(genoMaps, 3, axis=-1)
 
     # first, convert the strings to integer labels
     label_encoder = LabelEncoder()
     label_encoded = label_encoder.fit_transform(label)
 
     lc = np.array([])
     for i in range(0, userPD.shape[0]):
         first_occurrence = (label == userPD[i]).idxmax()
         lc = np.append(lc, label_encoded[first_occurrence[0]])
 
     lc = np.array(lc)
-
     n_clusters = len(np.unique(label))
     y_train = to_categorical(label_encoded)
-    # meanI=compute_genoSig(X_train,y_train, [y_train[0],y_train[1]])
     meanI = compute_genoSig(genoMaps_3d, label_encoded, lc, epochs=epochs)
 
-
-
     result = pd.DataFrame()
 
     for ii in range(0, len(meanI)):
         meanIX = meanI[ii]
         Ivec = np.reshape(meanIX, (1, meanIX.shape[0] * meanIX.shape[1]), order='F').copy()
         gene_namesN = np.array(gene_names)
         row_indices = np.argmax(T, axis=0)
```

### Comparing `genomap-1.2.4/genomap/genoTraj/genoTraj.py` & `genomap-1.2.9/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genoVis/genoVis.py` & `genomap-1.2.9/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genomap.py` & `genomap-1.2.9/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genomapOPT/genomapOPT.py` & `genomap-1.2.9/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/genomapT/genomapT.py` & `genomap-1.2.9/genomap/genomapT/genomapT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/ConvDEC.py` & `genomap-1.2.9/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/ConvIDEC.py` & `genomap-1.2.9/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/FcDEC.py` & `genomap-1.2.9/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/FcIDEC.py` & `genomap-1.2.9/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/class_discriminative_opt.py` & `genomap-1.2.9/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/gTraj_utils.py` & `genomap-1.2.9/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/group_centroid_opt.py` & `genomap-1.2.9/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/metrics.py` & `genomap-1.2.9/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/util_Sig.py` & `genomap-1.2.9/genomap/utils/util_Sig.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap/utils/utils_MOI.py` & `genomap-1.2.9/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/genomap.egg-info/PKG-INFO` & `genomap-1.2.9/genomap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.2.4
+Version: 1.2.9
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -76,27 +76,28 @@
 data=data.values
 gt_data = sio.loadmat('GT_TM.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
 
 resVis=gp.genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-# Use resVis=compute_genoVis(data, colNum=32,rowNum=32), if you dont know the number
+# Use resVis=gp.genoVis(data, colNum=32,rowNum=32), if you dont know the number
 # of classes in the data
 
 resVisEmb=resVis[0] # Dimensionality reduction and visualization result
 clusIndex=resVis[1] # Clustering result
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(resVisEmb[:, 0], resVisEmb[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
 plt.xlabel('genoVis1')
 plt.ylabel('genoVis2')
 plt.tight_layout()
 plt.colorbar(h1)
+plt.show()
 
 import genomap.utils.metrics as metrics
 print('acc=%.4f, nmi=%.4f, ari=%.4f' % (metrics.acc(y, clusIndex), metrics.nmi(y, clusIndex), metrics.ari(y, clusIndex)))
 ```
 
 ### Example 3 - Try genoDR for dimensionality reduction
 
@@ -109,24 +110,25 @@
 
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 gt_data = sio.loadmat('GT_divseq.mat')
 y = np.squeeze(gt_data['GT'])
 n_clusters = len(np.unique(y))
 
-resDR=gp.genoDR(data,n_clusters=n_clusters, colNum=33,rowNum=33)
-#resDR=compute_genoDimReduction(data, colNum=33,rowNum=33) # if you dont know the number
+reduced_dim=32 # Number of reduced dimension
+resDR=gp.genoDR(data, n_dim=reduced_dim, n_clusters=n_clusters, colNum=33,rowNum=33) 
+#resDR=gp.genoDR(data, n_dim=reduced_dim, colNum=33,rowNum=33) # if you dont know the number
 # of classes in the data
 embedding2D = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resDR)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding2D[:, 0], embedding2D[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 4 - Try genoTraj for cell trajectory analysis
 
@@ -203,25 +205,25 @@
 
 # Load class and batch labels
 dx = sio.loadmat('classLabel.mat')
 y = np.squeeze(dx['classLabel'])
 dx = sio.loadmat('batchLabel.mat')
 ybatch = np.squeeze(dx['batchLabel'])
 
-# Apply genoMOI
-resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+# Apply genoMOI with genomap size of 44x44 and dimension of 32 for the returned integrated data
+resVis=gp.genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44, n_dim=32)
 
 # Visualize the integrated data using UMAP
 embedding = umap.UMAP(n_neighbors=30,min_dist=0.3,n_epochs=200).fit_transform(resVis)
 
 plt.figure(figsize=(15, 10))
 plt.rcParams.update({'font.size': 28})    
 h1=plt.scatter(embedding[:, 0], embedding[:, 1], c=y,cmap='jet', marker='o', s=18)      #  ax = plt.subplot(3, n, i + 1*10+1)
-plt.xlabel('genoVis1')
-plt.ylabel('genoVis2')
+plt.xlabel('UMAP1')
+plt.ylabel('UMAP2')
 plt.tight_layout()
 plt.colorbar(h1)
 plt.show()
 ```
 
 ### Example 6 - Try genoSig for finding gene signatures for cell/data classes
 
@@ -234,14 +236,15 @@
 
 # Load data
 dx = sio.loadmat('reducedData_divseq.mat')
 data=dx['X']
 # Load data labels
 label = pd.read_csv('groundTruth_divseq.csv',header=None)
 # Load gene names corresponding to the columns of the data
+# Here we create artificial gene names as Gene_1, Gene_2. You can upload your gene sets
 gene_names = ['Gene_' + str(i) for i in range(1, data.shape[1]+1)]
 gene_names=np.array(gene_names)
 
 # The cell classes for which gene signatures will be computed
 userPD = np.array(['DG'])
 
 colNum=32 # genomap column number
@@ -284,15 +287,15 @@
 
 training_data=data.values[indxTrain-1]
 training_labels=GT[indxTrain-1]
 test_data=data.values[indxTest-1]
 
 est=gp.genoClassification(training_data, training_labels, test_data, rowNum=rowNum, colNum=colNum, epoch=150)
 
-print('Classification accuracy of genomap+genoNet:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
+print('Classification accuracy of genomap approach:'+str(np.sum(est==groundTruthTest) / est.shape[0]))  
 ```
 
 
 ### Example 8 - Try genoRegression for tabular data regression
 
 ```python
 import pandas as pd
```

### Comparing `genomap-1.2.4/genomap.egg-info/SOURCES.txt` & `genomap-1.2.9/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.2.4/setup.py` & `genomap-1.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.2.4",
+    version="1.2.9",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

