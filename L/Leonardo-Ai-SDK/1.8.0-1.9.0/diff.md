# Comparing `tmp/Leonardo-Ai-SDK-1.8.0.tar.gz` & `tmp/Leonardo-Ai-SDK-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-1.8.0.tar", last modified: Fri Jul 14 00:24:18 2023, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-1.9.0.tar", last modified: Tue Jul 18 00:34:09 2023, max compression
```

## Comparing `Leonardo-Ai-SDK-1.8.0.tar` & `Leonardo-Ai-SDK-1.9.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 00:24:18.000000 Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8343 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6385 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/generation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/initimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.065943 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createdataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7310 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/creategeneration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createmodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createvariationupscale.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getmodelbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getuserself.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getvariationbyid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploadinitimage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/controlnet_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/custom_model_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/job_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_generation_style.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/sd_versions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/strength.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/variation_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdkconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:24:18.069944 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3363 2023-07-14 00:24:05.000000 Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1168 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.627634 Leonardo-Ai-SDK-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.627634 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-18 00:34:09.000000 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-18 00:34:09.000000 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:34:09.000000 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 00:34:09.000000 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 00:34:09.000000 Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.627634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9116 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7005 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/generation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5268 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/initimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5183 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.627634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.627634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/errors/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/errors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2034 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createdataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7310 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/creategeneration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3867 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createmodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1746 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1764 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7835 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8100 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2072 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4207 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getuserself.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2720 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2397 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2440 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploadinitimage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/controlnet_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/custom_model_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      277 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/job_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      260 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      345 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/sd_versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      331 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/strength.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/variation_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2063 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:34:09.631634 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3762 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3677 2023-07-18 00:33:58.000000 Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-1.8.0/LICENSE.md` & `Leonardo-Ai-SDK-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/PKG-INFO` & `Leonardo-Ai-SDK-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.8.0
+Version: 1.9.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `Leonardo-Ai-SDK-1.8.0/README.md` & `Leonardo-Ai-SDK-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/setup.py` & `Leonardo-Ai-SDK-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="Leonardo-Ai-SDK",
-    version="1.8.0",
+    version="1.9.0",
     author="Leonardo-Ai",
     description="Leonardo Ai Python Client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 1.8.0
+Version: 1.9.0
 Summary: Leonardo Ai Python Client SDK
 Home-page: UNKNOWN
 Author: Leonardo-Ai
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-1.9.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 src/leonardoaisdk/initimage.py
 src/leonardoaisdk/model.py
 src/leonardoaisdk/sdk.py
 src/leonardoaisdk/sdkconfiguration.py
 src/leonardoaisdk/user.py
 src/leonardoaisdk/variation.py
 src/leonardoaisdk/models/__init__.py
+src/leonardoaisdk/models/errors/__init__.py
+src/leonardoaisdk/models/errors/sdkerror.py
 src/leonardoaisdk/models/operations/__init__.py
 src/leonardoaisdk/models/operations/createdataset.py
 src/leonardoaisdk/models/operations/creategeneration.py
 src/leonardoaisdk/models/operations/createmodel.py
 src/leonardoaisdk/models/operations/createvariationupscale.py
 src/leonardoaisdk/models/operations/deletedatasetbyid.py
 src/leonardoaisdk/models/operations/deletegenerationbyid.py
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Dataset:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -35,14 +35,16 @@
 
         res = operations.CreateDatasetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDataset200ApplicationJSON])
                 res.create_dataset_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def delete_dataset_by_id(self, request: operations.DeleteDatasetByIDRequest) -> operations.DeleteDatasetByIDResponse:
         r"""Delete a Single Dataset by ID
         This endpoint deletes the specific dataset
@@ -61,14 +63,16 @@
 
         res = operations.DeleteDatasetByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteDatasetByID200ApplicationJSON])
                 res.delete_dataset_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_dataset_by_id(self, request: operations.GetDatasetByIDRequest) -> operations.GetDatasetByIDResponse:
         r"""Get a Single Dataset by ID
         This endpoint gets the specific dataset
@@ -87,14 +91,16 @@
 
         res = operations.GetDatasetByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDatasetByID200ApplicationJSON])
                 res.get_dataset_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def upload_dataset_image(self, request: operations.UploadDatasetImageRequest) -> operations.UploadDatasetImageResponse:
         r"""Upload dataset image
         This endpoint returns presigned details to upload a dataset image to S3
@@ -118,14 +124,16 @@
 
         res = operations.UploadDatasetImageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadDatasetImage200ApplicationJSON])
                 res.upload_dataset_image_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def upload_dataset_image_from_gen(self, request: operations.UploadDatasetImageFromGenRequest) -> operations.UploadDatasetImageFromGenResponse:
         r"""Upload a Single Generated Image to a Dataset
         This endpoint will upload a previously generated image to the dataset
@@ -149,11 +157,13 @@
 
         res = operations.UploadDatasetImageFromGenResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadDatasetImageFromGen200ApplicationJSON])
                 res.upload_dataset_image_from_gen_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Generation:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -35,14 +35,16 @@
 
         res = operations.CreateGenerationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateGeneration200ApplicationJSON])
                 res.create_generation_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def delete_generation_by_id(self, request: operations.DeleteGenerationByIDRequest) -> operations.DeleteGenerationByIDResponse:
         r"""Delete a Single Generation
         This endpoint deletes a specific generation
@@ -61,14 +63,16 @@
 
         res = operations.DeleteGenerationByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteGenerationByID200ApplicationJSON])
                 res.delete_generation_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_generation_by_id(self, request: operations.GetGenerationByIDRequest) -> operations.GetGenerationByIDResponse:
         r"""Get a Single Generation
         This endpoint will provide information about a specific generation
@@ -87,14 +91,16 @@
 
         res = operations.GetGenerationByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGenerationByID200ApplicationJSON])
                 res.get_generation_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_generations_by_user_id(self, request: operations.GetGenerationsByUserIDRequest) -> operations.GetGenerationsByUserIDResponse:
         r"""Get generations by user ID
         This endpoint returns all generations by a specific user
@@ -114,11 +120,13 @@
 
         res = operations.GetGenerationsByUserIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGenerationsByUserID200ApplicationJSON])
                 res.get_generations_by_user_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/initimage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class InitImage:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -30,14 +30,16 @@
 
         res = operations.DeleteInitImageByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteInitImageByID200ApplicationJSON])
                 res.delete_init_image_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_init_image_by_id(self, request: operations.GetInitImageByIDRequest) -> operations.GetInitImageByIDResponse:
         r"""Get single init image
         This endpoint will return a single init image
@@ -56,14 +58,16 @@
 
         res = operations.GetInitImageByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetInitImageByID200ApplicationJSON])
                 res.get_init_image_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def upload_init_image(self, request: operations.UploadInitImageRequestBody) -> operations.UploadInitImageResponse:
         r"""Upload init image
         This endpoint returns presigned details to upload an init image to S3
@@ -87,11 +91,13 @@
 
         res = operations.UploadInitImageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadInitImage200ApplicationJSON])
                 res.upload_init_image_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Model:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -35,14 +35,16 @@
 
         res = operations.CreateModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateModel200ApplicationJSON])
                 res.create_model_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def delete_model_by_id(self, request: operations.DeleteModelByIDRequest) -> operations.DeleteModelByIDResponse:
         r"""Delete a Single Custom Model by ID
         This endpoint will delete a specific custom model
@@ -61,14 +63,16 @@
 
         res = operations.DeleteModelByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteModelByID200ApplicationJSON])
                 res.delete_model_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_model_by_id(self, request: operations.GetModelByIDRequest) -> operations.GetModelByIDResponse:
         r"""Get a Single Custom Model by ID
         This endpoint gets the specific custom model
@@ -87,11 +91,13 @@
 
         res = operations.GetModelByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetModelByID200ApplicationJSON])
                 res.get_model_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '1.8.0'
-    gen_version: str = '2.65.0'
+    sdk_version: str = '1.9.0'
+    gen_version: str = '2.70.0'
 
     def get_server_details(self) -> tuple[str, dict[str, str]]:
         if self.server_url:
             return self.server_url.removesuffix('/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/user.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class User:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -30,11 +30,13 @@
 
         res = operations.GetUserSelfResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetUserSelf200ApplicationJSON])
                 res.get_user_self_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-1.8.0/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-1.9.0/src/leonardoaisdk/variation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk.models import operations
+from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Variation:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
@@ -33,14 +33,16 @@
 
         res = operations.CreateVariationUpscaleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateVariationUpscale200ApplicationJSON])
                 res.create_variation_upscale_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     def get_variation_by_id(self, request: operations.GetVariationByIDRequest) -> operations.GetVariationByIDResponse:
         r"""Get variation by ID
         This endpoint will get the variation by ID
@@ -59,11 +61,13 @@
 
         res = operations.GetVariationByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetVariationByID200ApplicationJSON])
                 res.get_variation_by_id_200_application_json_object = out
+            else:
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

