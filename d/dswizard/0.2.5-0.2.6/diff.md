# Comparing `tmp/dswizard-0.2.5.tar.gz` & `tmp/dswizard-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dswizard-0.2.5.tar", last modified: Thu Jul  7 11:25:25 2022, max compression
+gzip compressed data, was "dswizard-0.2.6.tar", last modified: Tue Jul 18 11:40:59 2023, max compression
```

## Comparing `dswizard-0.2.5.tar` & `dswizard-0.2.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.986013 dswizard-0.2.5/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1511 2020-10-20 12:41:00.000000 dswizard-0.2.5/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1000)      132 2022-02-18 14:55:46.000000 dswizard-0.2.5/MANIFEST.in
--rw-rw-r--   0 marc      (1000) marc      (1000)     7721 2022-07-07 11:25:25.986013 dswizard-0.2.5/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     7013 2022-06-30 07:48:43.000000 dswizard-0.2.5/README.md
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.978013 dswizard-0.2.5/automl/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.978013 dswizard-0.2.5/automl/util/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2021-04-17 11:08:28.000000 dswizard-0.2.5/automl/util/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      200 2021-04-17 11:08:28.000000 dswizard-0.2.5/automl/util/util.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.978013 dswizard-0.2.5/dswizard/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/core/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2020-10-20 12:41:00.000000 dswizard-0.2.5/dswizard/core/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2693 2022-03-01 08:06:05.000000 dswizard-0.2.5/dswizard/core/base_bandit_learner.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1836 2022-01-09 17:02:15.000000 dswizard-0.2.5/dswizard/core/base_config_generator.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7513 2022-01-05 22:40:11.000000 dswizard-0.2.5/dswizard/core/base_iteration.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2153 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/core/base_structure_generator.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4612 2022-03-01 08:15:46.000000 dswizard-0.2.5/dswizard/core/config_cache.py
--rw-rw-r--   0 marc      (1000) marc      (1000)       26 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/core/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5545 2022-03-01 09:41:47.000000 dswizard-0.2.5/dswizard/core/dispatcher.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6575 2022-01-09 14:32:51.000000 dswizard-0.2.5/dswizard/core/ensemble.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7775 2022-01-27 21:37:03.000000 dswizard-0.2.5/dswizard/core/logger.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    18962 2022-03-09 09:45:55.000000 dswizard-0.2.5/dswizard/core/master.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    14047 2022-06-30 07:44:36.000000 dswizard-0.2.5/dswizard/core/model.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5335 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/core/renderer.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6954 2022-03-01 08:56:00.000000 dswizard-0.2.5/dswizard/core/runhistory.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1602 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/core/similaritystore.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     7337 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/core/worker.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/optimizers/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2020-10-20 12:41:00.000000 dswizard-0.2.5/dswizard/optimizers/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/optimizers/bandit_learners/
--rw-rw-r--   0 marc      (1000) marc      (1000)      143 2020-11-09 08:42:39.000000 dswizard-0.2.5/dswizard/optimizers/bandit_learners/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2637 2022-03-01 09:06:40.000000 dswizard-0.2.5/dswizard/optimizers/bandit_learners/hyperband.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      590 2022-03-01 08:10:16.000000 dswizard-0.2.5/dswizard/optimizers/bandit_learners/pseudo.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/optimizers/config_generators/
--rw-rw-r--   0 marc      (1000) marc      (1000)      315 2021-11-11 15:08:37.000000 dswizard-0.2.5/dswizard/optimizers/config_generators/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    14167 2022-03-01 08:21:40.000000 dswizard-0.2.5/dswizard/optimizers/config_generators/hyperopt.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2167 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/optimizers/config_generators/random_sampling.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5102 2022-01-04 17:18:41.000000 dswizard-0.2.5/dswizard/optimizers/config_generators/smac_generator.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/optimizers/iterations/
--rw-rw-r--   0 marc      (1000) marc      (1000)      230 2020-11-09 08:42:58.000000 dswizard-0.2.5/dswizard/optimizers/iterations/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      550 2022-01-05 22:42:28.000000 dswizard-0.2.5/dswizard/optimizers/iterations/pseudo.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      395 2020-10-20 12:41:00.000000 dswizard-0.2.5/dswizard/optimizers/iterations/successivehalving.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1413 2021-06-03 09:29:35.000000 dswizard-0.2.5/dswizard/optimizers/iterations/successiveresampling.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/optimizers/structure_generators/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2020-10-20 12:41:00.000000 dswizard-0.2.5/dswizard/optimizers/structure_generators/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1313 2022-01-01 20:52:00.000000 dswizard-0.2.5/dswizard/optimizers/structure_generators/fixed.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    31077 2022-07-07 11:24:20.000000 dswizard-0.2.5/dswizard/optimizers/structure_generators/mcts.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3222 2022-03-01 08:46:42.000000 dswizard-0.2.5/dswizard/optimizers/structure_generators/random_search.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/pipeline/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2021-04-17 11:08:28.000000 dswizard-0.2.5/dswizard/pipeline/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     5616 2022-03-01 08:25:03.000000 dswizard-0.2.5/dswizard/pipeline/pipeline.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2444 2022-03-01 08:51:46.000000 dswizard-0.2.5/dswizard/pipeline/voting_ensemble.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard/util/
--rw-rw-r--   0 marc      (1000) marc      (1000)        0 2021-12-11 17:18:43.000000 dswizard-0.2.5/dswizard/util/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1889 2022-03-01 10:17:29.000000 dswizard-0.2.5/dswizard/util/autoproxy.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4627 2022-03-01 09:02:16.000000 dswizard-0.2.5/dswizard/util/util.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.986013 dswizard-0.2.5/dswizard/workers/
--rw-rw-r--   0 marc      (1000) marc      (1000)       58 2020-10-20 12:41:00.000000 dswizard-0.2.5/dswizard/workers/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6156 2022-03-01 09:02:38.000000 dswizard-0.2.5/dswizard/workers/sklearn_worker.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-07-07 11:25:25.982013 dswizard-0.2.5/dswizard.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1000)     7721 2022-07-07 11:25:25.000000 dswizard-0.2.5/dswizard.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     1752 2022-07-07 11:25:25.000000 dswizard-0.2.5/dswizard.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-07-07 11:25:25.000000 dswizard-0.2.5/dswizard.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      313 2022-07-07 11:25:25.000000 dswizard-0.2.5/dswizard.egg-info/requires.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)       16 2022-07-07 11:25:25.000000 dswizard-0.2.5/dswizard.egg-info/top_level.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      261 2022-07-07 11:20:48.000000 dswizard-0.2.5/requirements.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-07-07 11:25:25.986013 dswizard-0.2.5/setup.cfg
--rw-rw-r--   0 marc      (1000) marc      (1000)     1577 2022-07-07 11:22:25.000000 dswizard-0.2.5/setup.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1511 2022-09-01 07:49:45.000000 dswizard-0.2.6/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1000)      132 2022-09-01 07:49:45.000000 dswizard-0.2.6/MANIFEST.in
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7701 2023-07-18 11:40:59.845644 dswizard-0.2.6/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7013 2022-09-01 07:49:45.000000 dswizard-0.2.6/README.md
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.841644 dswizard-0.2.6/automl/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/automl/util/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/automl/util/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      200 2022-09-01 07:49:45.000000 dswizard-0.2.6/automl/util/util.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/core/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2693 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/base_bandit_learner.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1836 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/base_config_generator.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7513 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/base_iteration.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2153 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/base_structure_generator.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4612 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/config_cache.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)       26 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5545 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/dispatcher.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6575 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/ensemble.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7775 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/logger.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18962 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/master.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14047 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/model.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5335 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/renderer.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6954 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/runhistory.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1601 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/similaritystore.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7337 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/core/worker.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/optimizers/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/optimizers/bandit_learners/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      143 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/bandit_learners/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2637 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/bandit_learners/hyperband.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      590 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/bandit_learners/pseudo.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/optimizers/config_generators/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      315 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/config_generators/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14167 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/config_generators/hyperopt.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2167 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/config_generators/random_sampling.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5102 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/config_generators/smac_generator.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/optimizers/iterations/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      230 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/iterations/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      550 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/iterations/pseudo.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      395 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/iterations/successivehalving.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1413 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/iterations/successiveresampling.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/optimizers/structure_generators/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/structure_generators/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1313 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/structure_generators/fixed.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    31099 2023-03-03 09:53:15.000000 dswizard-0.2.6/dswizard/optimizers/structure_generators/mcts.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3222 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/optimizers/structure_generators/random_search.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/pipeline/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/pipeline/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5616 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/pipeline/pipeline.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2444 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/pipeline/voting_ensemble.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/util/
+-rw-rw-r--   0 marc      (1000) marc      (1000)        0 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/util/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1889 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/util/autoproxy.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4627 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/util/util.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard/workers/
+-rw-rw-r--   0 marc      (1000) marc      (1000)       58 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/workers/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6156 2022-09-01 07:49:45.000000 dswizard-0.2.6/dswizard/workers/sklearn_worker.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2023-07-18 11:40:59.845644 dswizard-0.2.6/dswizard.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7701 2023-07-18 11:40:59.000000 dswizard-0.2.6/dswizard.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1752 2023-07-18 11:40:59.000000 dswizard-0.2.6/dswizard.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2023-07-18 11:40:59.000000 dswizard-0.2.6/dswizard.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      313 2023-07-18 11:40:59.000000 dswizard-0.2.6/dswizard.egg-info/requires.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)       16 2023-07-18 11:40:59.000000 dswizard-0.2.6/dswizard.egg-info/top_level.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      261 2023-07-18 11:40:49.000000 dswizard-0.2.6/requirements.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2023-07-18 11:40:59.845644 dswizard-0.2.6/setup.cfg
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1577 2023-07-18 11:40:38.000000 dswizard-0.2.6/setup.py
```

### Comparing `dswizard-0.2.5/LICENSE` & `dswizard-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/PKG-INFO` & `dswizard-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dswizard
-Version: 0.2.5
+Version: 0.2.6
 Summary: DataScience Wizard for automatic assembly of machine learning pipelines
 Home-page: https://github.com/Ennosigaeon/dswizard
 Author: Marc Zoeller
 Author-email: m.zoeller@usu.de
 License: MIT
 Keywords: automl,machine learning,pipeline synthesis
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -155,9 +154,7 @@
 supported.
 
 
 ## Release New Version
 
 Increase the version number in `setup.py` and build a new release with `python setup.py sdist`. Finally, upload the
 new version using `twine upload dist/dswizard-<VERSION>.tar.gz`.
-
-
```

### Comparing `dswizard-0.2.5/README.md` & `dswizard-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/base_bandit_learner.py` & `dswizard-0.2.6/dswizard/core/base_bandit_learner.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/base_config_generator.py` & `dswizard-0.2.6/dswizard/core/base_config_generator.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/base_iteration.py` & `dswizard-0.2.6/dswizard/core/base_iteration.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/base_structure_generator.py` & `dswizard-0.2.6/dswizard/core/base_structure_generator.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/config_cache.py` & `dswizard-0.2.6/dswizard/core/config_cache.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/dispatcher.py` & `dswizard-0.2.6/dswizard/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/ensemble.py` & `dswizard-0.2.6/dswizard/core/ensemble.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/logger.py` & `dswizard-0.2.6/dswizard/core/logger.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/master.py` & `dswizard-0.2.6/dswizard/core/master.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/model.py` & `dswizard-0.2.6/dswizard/core/model.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/renderer.py` & `dswizard-0.2.6/dswizard/core/renderer.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/runhistory.py` & `dswizard-0.2.6/dswizard/core/runhistory.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/core/similaritystore.py` & `dswizard-0.2.6/dswizard/core/similaritystore.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             self.model: Pipeline = model
             # Remove OHE encoded algorithm
             self.weight = self.model.steps[-1][1].feature_importances_[0:SimilarityStore.N_MF]
             self.weight = (self.weight / self.weight.sum()) * SimilarityStore.N_MF
         else:
             self.model = None
             self.weight = np.ones(SimilarityStore.N_MF)
-        self.neighbours = NearestNeighbors(metric='wminkowski', p=2, metric_params={'w': self.weight})
+        self.neighbours = NearestNeighbors(metric='minkowski', p=2, metric_params={'w': self.weight})
         self.data = []
 
     def add(self, mf: MetaFeatures, data=None):
         mf_normal = self._normalize(mf)
         if self.mfs is None:
             self.mfs = mf_normal.reshape(1, -1)
         else:
```

### Comparing `dswizard-0.2.5/dswizard/core/worker.py` & `dswizard-0.2.6/dswizard/core/worker.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/bandit_learners/hyperband.py` & `dswizard-0.2.6/dswizard/optimizers/bandit_learners/hyperband.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/bandit_learners/pseudo.py` & `dswizard-0.2.6/dswizard/optimizers/bandit_learners/pseudo.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/config_generators/hyperopt.py` & `dswizard-0.2.6/dswizard/optimizers/config_generators/hyperopt.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/config_generators/random_sampling.py` & `dswizard-0.2.6/dswizard/optimizers/config_generators/random_sampling.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/config_generators/smac_generator.py` & `dswizard-0.2.6/dswizard/optimizers/config_generators/smac_generator.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/iterations/pseudo.py` & `dswizard-0.2.6/dswizard/optimizers/iterations/pseudo.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/iterations/successiveresampling.py` & `dswizard-0.2.6/dswizard/optimizers/iterations/successiveresampling.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/structure_generators/fixed.py` & `dswizard-0.2.6/dswizard/optimizers/structure_generators/fixed.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/optimizers/structure_generators/mcts.py` & `dswizard-0.2.6/dswizard/optimizers/structure_generators/mcts.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,14 +284,15 @@
             exploitation = worst_score
             exploration = worst_score
         else:
             exploitation = n.reward / n.visits
             exploration = -math.sqrt(log_N_vertex / n.visits)
         score = exploitation + self._exploration_weight * exploration
 
+        # TODO: wrong
         overfitting = 1 - (2 ** len(n.steps)) / (2 ** 4)
         adjusted_score = score * overfitting
 
         if decompose:
             return adjusted_score, {
                 'exploit': exploitation,
                 'explore': exploration,
```

### Comparing `dswizard-0.2.5/dswizard/optimizers/structure_generators/random_search.py` & `dswizard-0.2.6/dswizard/optimizers/structure_generators/random_search.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/pipeline/pipeline.py` & `dswizard-0.2.6/dswizard/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/pipeline/voting_ensemble.py` & `dswizard-0.2.6/dswizard/pipeline/voting_ensemble.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/util/autoproxy.py` & `dswizard-0.2.6/dswizard/util/autoproxy.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/util/util.py` & `dswizard-0.2.6/dswizard/util/util.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard/workers/sklearn_worker.py` & `dswizard-0.2.6/dswizard/workers/sklearn_worker.py`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/dswizard.egg-info/PKG-INFO` & `dswizard-0.2.6/dswizard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: dswizard
-Version: 0.2.5
+Version: 0.2.6
 Summary: DataScience Wizard for automatic assembly of machine learning pipelines
 Home-page: https://github.com/Ennosigaeon/dswizard
 Author: Marc Zoeller
 Author-email: m.zoeller@usu.de
 License: MIT
 Keywords: automl,machine learning,pipeline synthesis
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -155,9 +154,7 @@
 supported.
 
 
 ## Release New Version
 
 Increase the version number in `setup.py` and build a new release with `python setup.py sdist`. Finally, upload the
 new version using `twine upload dist/dswizard-<VERSION>.tar.gz`.
-
-
```

### Comparing `dswizard-0.2.5/dswizard.egg-info/SOURCES.txt` & `dswizard-0.2.6/dswizard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dswizard-0.2.5/setup.py` & `dswizard-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # The text of the README file
 README = (pathlib.Path(__file__).parent / 'README.md').read_text()
 
 if __name__ == '__main__':
     setup(
         name='dswizard',
-        version='0.2.5',
+        version='0.2.6',
         description='DataScience Wizard for automatic assembly of machine learning pipelines',
         long_description=README,
         long_description_content_type='text/markdown',
         author='Marc Zoeller',
         author_email='m.zoeller@usu.de',
         url='https://github.com/Ennosigaeon/dswizard',
         license='MIT',
```

