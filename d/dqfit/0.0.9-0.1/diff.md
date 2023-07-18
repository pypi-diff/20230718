# Comparing `tmp/dqfit-0.0.9.tar.gz` & `tmp/dqfit-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqfit-0.0.9.tar", last modified: Tue Nov 29 15:42:03 2022, max compression
+gzip compressed data, was "dqfit-0.1.tar", last modified: Tue Jul 18 14:47:51 2023, max compression
```

## Comparing `dqfit-0.0.9.tar` & `dqfit-0.1.tar`

### file list

```diff
@@ -1,18 +1,42 @@
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.614936 dqfit-0.0.9/
--rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:42:03.614328 dqfit-0.0.9/PKG-INFO
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.598997 dqfit-0.0.9/dqfit/
--rw-r--r--   0 ah24562    (502) staff       (20)        0 2022-11-29 12:48:24.000000 dqfit-0.0.9/dqfit/__init__.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.610298 dqfit-0.0.9/dqfit/model/
--rw-r--r--   0 ah24562    (502) staff       (20)     6421 2022-11-29 15:40:20.000000 dqfit-0.0.9/dqfit/model/dqi_model.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.611787 dqfit-0.0.9/dqfit/preprocessing/
--rw-r--r--   0 ah24562    (502) staff       (20)     2816 2022-11-29 13:16:08.000000 dqfit-0.0.9/dqfit/preprocessing/ResourceFeatures.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.613315 dqfit-0.0.9/dqfit/preprocessing/resource_helpers/
--rw-r--r--   0 ah24562    (502) staff       (20)     3868 2022-11-29 13:13:37.000000 dqfit-0.0.9/dqfit/preprocessing/resource_helpers/r401.py
--rw-r--r--   0 ah24562    (502) staff       (20)     2397 2022-11-29 15:27:00.000000 dqfit-0.0.9/dqfit/query.py
-drwxr-xr-x   0 ah24562    (502) staff       (20)        0 2022-11-29 15:42:03.608847 dqfit-0.0.9/dqfit.egg-info/
--rw-r--r--   0 ah24562    (502) staff       (20)      223 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/PKG-INFO
--rw-r--r--   0 ah24562    (502) staff       (20)      273 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/SOURCES.txt
--rw-r--r--   0 ah24562    (502) staff       (20)        1 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/dependency_links.txt
--rw-r--r--   0 ah24562    (502) staff       (20)        6 2022-11-29 15:42:03.000000 dqfit-0.0.9/dqfit.egg-info/top_level.txt
--rw-r--r--   0 ah24562    (502) staff       (20)      301 2022-11-29 15:41:18.000000 dqfit-0.0.9/pyproject.toml
--rw-r--r--   0 ah24562    (502) staff       (20)       38 2022-11-29 15:42:03.615065 dqfit-0.0.9/setup.cfg
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.908818 dqfit-0.1/
+-rw-r--r--   0 parker     (501) staff       (20)       11 2023-07-18 14:46:45.000000 dqfit-0.1/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)     3893 2023-07-18 14:47:51.908674 dqfit-0.1/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     3643 2023-07-18 14:46:48.000000 dqfit-0.1/README.md
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.902475 dqfit-0.1/dqfit/
+-rw-r--r--   0 parker     (501) staff       (20)      817 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.900852 dqfit-0.1/dqfit/data/
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.904089 dqfit-0.1/dqfit/data/context/
+-rw-r--r--   0 parker     (501) staff       (20)     7309 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/context/COLE.json
+-rw-r--r--   0 parker     (501) staff       (20)   104281 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/context/hello-world.json
+-rw-r--r--   0 parker     (501) staff       (20)      628 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/context/patient-demographic.json
+-rw-r--r--   0 parker     (501) staff       (20)      170 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/context/systolic.json
+-rw-r--r--   0 parker     (501) staff       (20)   125219 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/context/uscdi.json
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.900955 dqfit-0.1/dqfit/data/synthetic/
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.904316 dqfit-0.1/dqfit/data/synthetic/synthea_1/
+-rw-r--r--   0 parker     (501) staff       (20)    10600 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/data/synthetic/synthea_1/hello-world-bundle.json
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.908239 dqfit-0.1/dqfit/data/synthetic/synthea_10/
+-rw-r--r--   0 parker     (501) staff       (20)   448345 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Aaron697_Veum823_f11ade6b-fae3-c20d-0a46-e344db669410.json
+-rw-r--r--   0 parker     (501) staff       (20)  1853828 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Abdul218_Gislason620_81469779-7e7f-4864-6fdc-41e52a68ba80.json
+-rw-r--r--   0 parker     (501) staff       (20)   250797 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Addie421_Weber641_6d7ea981-c548-3d1e-0b59-ba2acbb149d2.json
+-rw-r--r--   0 parker     (501) staff       (20)   313530 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Adele475_Barton704_4d604ebf-23a9-7a3f-affe-ec4c69f1644d.json
+-rw-r--r--   0 parker     (501) staff       (20)   514069 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Adena533_Rice937_3470129b-6f4d-27d6-b25b-65a2903514b6.json
+-rw-r--r--   0 parker     (501) staff       (20)   406074 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Adina377_Barton704_5bde62b3-df9f-623d-e6f8-bd335bc02dc0.json
+-rw-r--r--   0 parker     (501) staff       (20)   608466 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Adrian111_Collins926_c9e3828c-7466-5f82-a675-213e088c6e7c.json
+-rw-r--r--   0 parker     (501) staff       (20)   252925 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Agustin437_Russel238_fc56a4f3-04d6-364a-5131-803138497da1.json
+-rw-r--r--   0 parker     (501) staff       (20)   689780 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Aida517_Spencer878_87bc62d9-7a08-3ecf-0723-d3d918698e0c.json
+-rw-r--r--   0 parker     (501) staff       (20)   449052 2023-07-18 14:46:45.000000 dqfit-0.1/dqfit/data/synthetic/synthea_10/Aileen250_Bahringer146_5cc757f3-f20b-e88f-c23e-5faee619e6ac.json
+-rw-r--r--   0 parker     (501) staff       (20)     9164 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/dimensions.py
+-rw-r--r--   0 parker     (501) staff       (20)      928 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     2994 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/io.py
+-rw-r--r--   0 parker     (501) staff       (20)     6045 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/model.py
+-rw-r--r--   0 parker     (501) staff       (20)     3341 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/population.py
+-rw-r--r--   0 parker     (501) staff       (20)     3065 2023-07-18 14:46:48.000000 dqfit-0.1/dqfit/transform.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-18 14:47:51.903123 dqfit-0.1/dqfit.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)     3893 2023-07-18 14:47:51.000000 dqfit-0.1/dqfit.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1472 2023-07-18 14:47:51.000000 dqfit-0.1/dqfit.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-18 14:47:51.000000 dqfit-0.1/dqfit.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)       40 2023-07-18 14:47:51.000000 dqfit-0.1/dqfit.egg-info/requires.txt
+-rw-r--r--   0 parker     (501) staff       (20)        6 2023-07-18 14:47:51.000000 dqfit-0.1/dqfit.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      427 2023-07-18 14:46:48.000000 dqfit-0.1/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-18 14:47:51.908854 dqfit-0.1/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      141 2023-07-18 14:46:45.000000 dqfit-0.1/setup.py
```

