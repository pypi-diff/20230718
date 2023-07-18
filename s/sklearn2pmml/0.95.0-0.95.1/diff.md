# Comparing `tmp/sklearn2pmml-0.95.0.tar.gz` & `tmp/sklearn2pmml-0.95.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.95.0.tar", last modified: Fri Jul 14 16:52:51 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.95.1.tar", last modified: Tue Jul 18 12:28:00 2023, max compression
```

## Comparing `sklearn2pmml-0.95.0.tar` & `sklearn2pmml-0.95.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1386 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    12289 2023-07-14 16:34:45.000000 sklearn2pmml-0.95.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   472037 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    48655 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-h2o-1.2.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6244 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    83824 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/guava-21.0.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   203268 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-python-1.1.16.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    14761 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   442644 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     5709 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.95.0/sklearn2pmml/resources/gson-2.10.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-14 16:34:49.000000 sklearn2pmml-0.95.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-14 16:52:51.000000 sklearn2pmml-0.95.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.1/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.1/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1403 2023-07-16 18:17:01.000000 sklearn2pmml-0.95.1/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    12289 2023-07-14 16:34:45.000000 sklearn2pmml-0.95.1/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    33104 2023-06-11 15:37:09.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   472037 2023-07-14 15:18:05.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    48655 2023-07-09 17:14:49.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-h2o-1.2.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68173 2023-04-08 17:17:57.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7311 2023-07-14 15:18:07.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6244 2023-07-14 15:18:07.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    83824 2023-07-14 15:18:06.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   191286 2022-08-21 07:39:07.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  2521113 2017-01-28 20:01:27.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/guava-21.0.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   203268 2023-07-13 17:26:32.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-python-1.1.16.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    14761 2023-07-14 15:18:07.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   442644 2023-07-08 05:55:57.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      810 2023-07-18 12:25:37.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     5711 2023-07-18 12:25:38.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-01-07 07:34:52.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7976 2023-07-14 15:18:07.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   286235 2022-12-26 20:16:36.000000 sklearn2pmml-0.95.1/sklearn2pmml/resources/gson-2.10.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-07-18 12:25:20.000000 sklearn2pmml-0.95.1/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-07-18 12:28:00.000000 sklearn2pmml-0.95.1/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.95.1/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.95.0/LICENSE.txt` & `sklearn2pmml-0.95.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/setup.py` & `sklearn2pmml-0.95.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,13 @@
 		"sklearn2pmml.tree",
 		"sklearn2pmml.util"
 	],
 	package_data = {
 		"sklearn2pmml.resources" : ["classpath.txt", "*.jar"]
 	},
 	install_requires = [
+		"dill>=0.3.4",
 		"joblib>=0.13.0",
 		"scikit-learn>=0.18.0",
 		"sklearn-pandas>=0.0.10"
 	]
 )
```

### Comparing `sklearn2pmml-0.95.0/PKG-INFO` & `sklearn2pmml-0.95.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.95.0
+Version: 0.95.1
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.95.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.95.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.95.1/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.95.1/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.95.1/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.95.1/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.95.1/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-statsmodels-1.0.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-h2o-1.2.8.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-h2o-1.2.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-lightgbm-1.4.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-converter-1.5.4.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-converter-1.5.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/guava-21.0.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/guava-21.0.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-python-1.1.16.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-python-1.1.16.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-logger-3.42.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/classpath.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5709 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/
--rw-r--r--  2.0 unx      158 b- defN 23-Jul-14 19:11 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 com/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 com/sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
--rw-rw-r--  2.0 unx     3741 b- defN 23-Jul-14 19:11 com/sklearn2pmml/Main.class
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-14 19:11 com/sklearn2pmml/Main$1.class
--rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
--rw-rw-r--  2.0 unx       70 b- defN 23-Jul-14 19:11 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
-11 files, 13013 bytes uncompressed, 4233 bytes compressed:  67.5%
+Zip file size: 5711 bytes, number of entries: 11
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 META-INF/
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-18 15:25 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 com/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 com/sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 META-INF/maven/com.sklearn2pmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-18 15:25 META-INF/maven/com.sklearn2pmml/sklearn2pmml/
+-rw-rw-r--  2.0 unx     3741 b- defN 23-Jul-18 15:25 com/sklearn2pmml/Main.class
+-rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-18 15:25 com/sklearn2pmml/Main$1.class
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-14 19:34 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.xml
+-rw-rw-r--  2.0 unx       70 b- defN 23-Jul-18 15:25 META-INF/maven/com.sklearn2pmml/sklearn2pmml/pom.properties
+11 files, 13013 bytes uncompressed, 4235 bytes compressed:  67.5%
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: SkLearn2PMML package
-Implementation-Version: 0.95.0
+Implementation-Version: 0.95.1
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-xgboost-1.7.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.32.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/resources/gson-2.10.jar` & `sklearn2pmml-0.95.1/sklearn2pmml/resources/gson-2.10.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.95.1/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.95.1/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.95.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.95.1/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

