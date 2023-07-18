# Comparing `tmp/edu_rdm_integration-0.0.1.tar.gz` & `tmp/edu_rdm_integration-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_rdm_integration-0.0.1.tar", last modified: Tue Jul 18 06:39:55 2023, max compression
+gzip compressed data, was "edu_rdm_integration-0.1.0.tar", last modified: Tue Jul 18 09:33:09 2023, max compression
```

## Comparing `edu_rdm_integration-0.0.1.tar` & `edu_rdm_integration-0.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0     3458 2023-07-18 06:39:46.917456 edu_rdm_integration-0.0.1/LICENSE
--rw-r--r--   0        0        0    11460 2023-07-18 06:39:46.917456 edu_rdm_integration-0.0.1/README.md
--rw-r--r--   0        0        0      692 2023-07-18 06:39:46.918456 edu_rdm_integration-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       72 2023-07-18 06:39:46.919456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/__init__.py
--rw-r--r--   0        0        0       83 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/__init__.py
--rw-r--r--   0        0        0      363 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/apps.py
--rw-r--r--   0        0        0     1505 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/caches.py
--rw-r--r--   0        0        0       66 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/enums.py
--rw-r--r--   0        0        0      255 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/errors.py
--rw-r--r--   0        0        0     2075 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/functions.py
--rw-r--r--   0        0        0     1105 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/helpers.py
--rw-r--r--   0        0        0      589 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/managers.py
--rw-r--r--   0        0        0      327 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/presenters.py
--rw-r--r--   0        0        0      598 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/receivers.py
--rw-r--r--   0        0        0      515 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/results.py
--rw-r--r--   0        0        0     2164 2023-07-18 06:39:46.920456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/runners.py
--rw-r--r--   0        0        0     5504 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/strategies.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/tests.py
--rw-r--r--   0        0        0      496 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/validators.py
--rw-r--r--   0        0        0     1822 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/app_settings.py
--rw-r--r--   0        0        0     2339 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/apps.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/__init__.py
--rw-r--r--   0        0        0     1310 2023-07-18 06:39:46.921456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/caches.py
--rw-r--r--   0        0        0     2369 2023-07-18 06:39:46.922456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/functions.py
--rw-r--r--   0        0        0     5235 2023-07-18 06:39:46.922456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/managers.py
--rw-r--r--   0        0        0     1440 2023-07-18 06:39:46.922456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/runners.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.922456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
--rw-r--r--   0        0        0     7212 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/caches.py
--rw-r--r--   0        0        0       84 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/enums.py
--rw-r--r--   0        0        0      326 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/errors.py
--rw-r--r--   0        0        0     1670 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/functions.py
--rw-r--r--   0        0        0     1490 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
--rw-r--r--   0        0        0      838 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/managers.py
--rw-r--r--   0        0        0      438 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
--rw-r--r--   0        0        0      708 2023-07-18 06:39:46.923456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/results.py
--rw-r--r--   0        0        0     1648 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/tests.py
--rw-r--r--   0        0        0     1057 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/validators.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
--rw-r--r--   0        0        0     5674 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
--rw-r--r--   0        0        0       66 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
--rw-r--r--   0        0        0      297 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
--rw-r--r--   0        0        0     1563 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
--rw-r--r--   0        0        0     1376 2023-07-18 06:39:46.924456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
--rw-r--r--   0        0        0      783 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
--rw-r--r--   0        0        0      409 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
--rw-r--r--   0        0        0      674 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
--rw-r--r--   0        0        0     1541 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
--rw-r--r--   0        0        0      973 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
--rw-r--r--   0        0        0      635 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/consts.py
--rw-r--r--   0        0        0     9117 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/entities.py
--rw-r--r--   0        0        0     4876 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/enums.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.925456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/caches.py
--rw-r--r--   0        0        0      369 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/enums.py
--rw-r--r--   0        0        0      291 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/errors.py
--rw-r--r--   0        0        0    11681 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/functions.py
--rw-r--r--   0        0        0     3076 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/helpers.py
--rw-r--r--   0        0        0     5680 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/managers.py
--rw-r--r--   0        0        0      403 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/presenters.py
--rw-r--r--   0        0        0     2548 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/requests.py
--rw-r--r--   0        0        0      662 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/results.py
--rw-r--r--   0        0        0     2732 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.926456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/tests.py
--rw-r--r--   0        0        0      961 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/validators.py
--rw-r--r--   0        0        0       16 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/consts.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/commands/__init__.py
--rw-r--r--   0        0        0      487 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/commands/collect_models_data.py
--rw-r--r--   0        0        0      388 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/commands/export_entities_data.py
--rw-r--r--   0        0        0    19793 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/general.py
--rw-r--r--   0        0        0     2302 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/generators.py
--rw-r--r--   0        0        0      473 2023-07-18 06:39:46.927456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/mapping.py
--rw-r--r--   0        0        0    18718 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/migrations/0001_initial.py
--rw-r--r--   0        0        0      944 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/migrations/__init__.py
--rw-r--r--   0        0        0    19850 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/models.py
--rw-r--r--   0        0        0     6806 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/storages.py
--rw-r--r--   0        0        0     1936 2023-07-18 06:39:46.928456 edu_rdm_integration-0.0.1/src/edu_rdm_integration/utils.py
--rw-r--r--   0        0        0    12926 2023-07-18 06:39:55.905407 edu_rdm_integration-0.0.1/setup.py
--rw-r--r--   0        0        0    11862 2023-07-18 06:39:55.906717 edu_rdm_integration-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3458 2023-07-18 06:39:46.917456 edu_rdm_integration-0.1.0/LICENSE
+-rw-r--r--   0        0        0    11460 2023-07-18 06:39:46.917456 edu_rdm_integration-0.1.0/README.md
+-rw-r--r--   0        0        0      692 2023-07-18 09:33:02.018481 edu_rdm_integration-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-07-18 06:39:46.919456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/apps.py
+-rw-r--r--   0        0        0     1505 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/caches.py
+-rw-r--r--   0        0        0       66 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/consts.py
+-rw-r--r--   0        0        0       93 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/enums.py
+-rw-r--r--   0        0        0      255 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/errors.py
+-rw-r--r--   0        0        0     2075 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/functions.py
+-rw-r--r--   0        0        0     1105 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/helpers.py
+-rw-r--r--   0        0        0      589 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/managers.py
+-rw-r--r--   0        0        0      327 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/presenters.py
+-rw-r--r--   0        0        0      598 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/receivers.py
+-rw-r--r--   0        0        0      515 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/results.py
+-rw-r--r--   0        0        0     2164 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/runners.py
+-rw-r--r--   0        0        0     5504 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/strategies.py
+-rw-r--r--   0        0        0      181 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/strings.py
+-rw-r--r--   0        0        0       59 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/tests.py
+-rw-r--r--   0        0        0      496 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/validators.py
+-rw-r--r--   0        0        0     1822 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/app_settings.py
+-rw-r--r--   0        0        0     2339 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/apps.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/__init__.py
+-rw-r--r--   0        0        0     1310 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/caches.py
+-rw-r--r--   0        0        0     2369 2023-07-18 06:39:46.922456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/functions.py
+-rw-r--r--   0        0        0     5235 2023-07-18 06:39:46.922456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/managers.py
+-rw-r--r--   0        0        0     1440 2023-07-18 06:39:46.922456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/runners.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.922456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
+-rw-r--r--   0        0        0     7212 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py
+-rw-r--r--   0        0        0       84 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/consts.py
+-rw-r--r--   0        0        0       93 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/enums.py
+-rw-r--r--   0        0        0      326 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/errors.py
+-rw-r--r--   0        0        0     1670 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py
+-rw-r--r--   0        0        0     1490 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
+-rw-r--r--   0        0        0      838 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py
+-rw-r--r--   0        0        0      438 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
+-rw-r--r--   0        0        0      708 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/results.py
+-rw-r--r--   0        0        0     1648 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py
+-rw-r--r--   0        0        0      181 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/strings.py
+-rw-r--r--   0        0        0       59 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/tests.py
+-rw-r--r--   0        0        0     1057 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
+-rw-r--r--   0        0        0     5674 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
+-rw-r--r--   0        0        0       66 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
+-rw-r--r--   0        0        0       93 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
+-rw-r--r--   0        0        0      297 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
+-rw-r--r--   0        0        0     1563 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
+-rw-r--r--   0        0        0     1376 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
+-rw-r--r--   0        0        0      783 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
+-rw-r--r--   0        0        0      409 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
+-rw-r--r--   0        0        0      674 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
+-rw-r--r--   0        0        0     1541 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
+-rw-r--r--   0        0        0      181 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
+-rw-r--r--   0        0        0       59 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
+-rw-r--r--   0        0        0      973 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
+-rw-r--r--   0        0        0      635 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/consts.py
+-rw-r--r--   0        0        0     9117 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/entities.py
+-rw-r--r--   0        0        0     4876 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/enums.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/__init__.py
+-rw-r--r--   0        0        0     1380 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/caches.py
+-rw-r--r--   0        0        0      369 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/consts.py
+-rw-r--r--   0        0        0       93 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/enums.py
+-rw-r--r--   0        0        0      291 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/errors.py
+-rw-r--r--   0        0        0    11681 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/functions.py
+-rw-r--r--   0        0        0     3076 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/helpers.py
+-rw-r--r--   0        0        0     5680 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/managers.py
+-rw-r--r--   0        0        0      403 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/presenters.py
+-rw-r--r--   0        0        0     2548 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/requests.py
+-rw-r--r--   0        0        0      662 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/results.py
+-rw-r--r--   0        0        0     2732 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/runners.py
+-rw-r--r--   0        0        0      181 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/strings.py
+-rw-r--r--   0        0        0       59 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/tests.py
+-rw-r--r--   0        0        0      961 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/validators.py
+-rw-r--r--   0        0        0       16 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/consts.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/commands/__init__.py
+-rw-r--r--   0        0        0      487 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/commands/collect_models_data.py
+-rw-r--r--   0        0        0      388 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/commands/export_entities_data.py
+-rw-r--r--   0        0        0    19793 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/general.py
+-rw-r--r--   0        0        0     2302 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/generators.py
+-rw-r--r--   0        0        0      473 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/mapping.py
+-rw-r--r--   0        0        0    18718 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/migrations/0001_initial.py
+-rw-r--r--   0        0        0      944 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/migrations/__init__.py
+-rw-r--r--   0        0        0    19850 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/models.py
+-rw-r--r--   0        0        0     6806 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/storages.py
+-rw-r--r--   0        0        0     1936 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.0/src/edu_rdm_integration/utils.py
+-rw-r--r--   0        0        0    12926 2023-07-18 09:33:09.304164 edu_rdm_integration-0.1.0/setup.py
+-rw-r--r--   0        0        0    11862 2023-07-18 09:33:09.305432 edu_rdm_integration-0.1.0/PKG-INFO
```

### Comparing `edu_rdm_integration-0.0.1/LICENSE` & `edu_rdm_integration-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/README.md` & `edu_rdm_integration-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/pyproject.toml` & `edu_rdm_integration-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edu_rdm_integration"
-version = "0.0.1"
+version = "0.1.0"
 description = "Интеграция с Региональной витриной данных"
 authors = ["BARS Group"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/caches.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/functions.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/helpers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/managers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/receivers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/receivers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/results.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/runners.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/adapters/strategies.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/adapters/strategies.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/app_settings.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/app_settings.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/apps.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/apps.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/caches.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/functions.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/managers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/base/runners.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/caches.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/functions.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/helpers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/managers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/results.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/runners.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/calculated/base/validators.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/results.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/consts.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/consts.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/entities.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/entities.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/enums.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/enums.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/caches.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/functions.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/helpers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/managers.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/requests.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/requests.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/results.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/runners.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/export_data/base/validators.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/export_data/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/general.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/general.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/management/generators.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/management/generators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/migrations/0001_initial.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/models.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/models.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/storages.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/storages.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/src/edu_rdm_integration/utils.py` & `edu_rdm_integration-0.1.0/src/edu_rdm_integration/utils.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.0.1/setup.py` & `edu_rdm_integration-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'edu_rdm_integration.migrations']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'edu-rdm-integration',
-    'version': '0.0.1',
+    'version': '0.1.0',
     'description': 'Интеграция с Региональной витриной данных',
     'long_description': '# Проект "Интеграция с Региональной витриной данных"\n\n## Описание концепции\n\n## Принцип работы\n\n## Требования к окружению\n\n## Разворачивание\n\n## Параметры конфигурационного файла\n\n\nВ разных проектах существуют различные способы добавления настроек, где-то через плагины, где-то напрямую в settings.py.\nБудет рассмотрен подход указания настроек в settings.py и указания параметров в конфигурационном файле.\n\nДля возможности конфигурирования необходимо проделать ряд действий. В settings.py нужно добавить:\n\n- Определение значений по умолчанию настроек:\n    ```\n    PROJECT_DEFAULT_CONFIG.update({\n        # Настройки РВД\n        (\'rdm_general\', \'EXPORT_ENTITY_ID_PREFIX\'): \'\', # Дефолтное значение нужно изменить на специфическое системе\n        (\'rdm_general\', \'COLLECT_CHUNK_SIZE\'): 500,\n        (\'rdm_general\', \'EXPORT_CHUNK_SIZE\'): 500,\n        (\'rdm_transfer_task\', \'MINUTE\'): \'0\',\n        (\'rdm_transfer_task\', \'HOUR\'): \'*/4\',\n        (\'rdm_transfer_task\', \'TRANSFER_TASK_DAY_OF_WEEK\'): \'*\',\n        (\'rdm_transfer_task\', \'TIMEDELTA\'): 3600,\n        (\'rdm_upload_status_task\', \'MINUTE\'): \'*/30\',\n        (\'rdm_upload_status_task\', \'HOUR\'): \'*\',\n        (\'rdm_upload_status_task\', \'DAY_OF_WEEK\'): \'*\',\n        (\'uploader_client\', \'URL\'): \'http://localhost:8090\',\n        (\'uploader_client\', \'DATAMART_NAME\'): \'\',\n        (\'uploader_client\', \'REQUEST_RETRIES\'): 10,\n        (\'uploader_client\', \'REQUEST_TIMEOUT\'): 10,\n        (\'uploader_client\', \'ENABLE_REQUEST_EMULATION\'): False,\n    })\n    ```\n- Получение значений настроек из конфигурационного файла:\n\n    ```\n    # Ссылка на каталог с файлами для загрузки\n    UPLOADS = \'uploads\'\n  \n    # =============================================================================\n    # Интеграция с Региональной витриной данных (РВД)\n    # =============================================================================\n    \n    # Префикс идентификаторов записей сущностей специфический для продукта\n    RDM_EXPORT_ENTITY_ID_PREFIX = conf.get(\'rdm_general\', \'EXPORT_ENTITY_ID_PREFIX\') \n  \n    # Количество записей моделей ЭШ обрабатываемых за одну итерацию сбора данных\n    RDM_COLLECT_CHUNK_SIZE = conf.get_int(\'rdm_general\', \'COLLECT_CHUNK_SIZE\')\n    \n    # Количество записей моделей обрабатываемых за одну итерацию экспорта данных\n    RDM_EXPORT_CHUNK_SIZE = conf.get_int(\'rdm_general\', \'EXPORT_CHUNK_SIZE\')\n    \n    # Настройка запуска периодической задачи выгрузки данных:\n    RDM_TRANSFER_TASK_MINUTE = conf.get(\'rdm_transfer_task\', \'MINUTE\')\n    RDM_TRANSFER_TASK_HOUR = conf.get(\'rdm_transfer_task\', \'HOUR\')\n    RDM_TRANSFER_TASK_DAY_OF_WEEK = conf.get(\'rdm_transfer_task\', \'DAY_OF_WEEK\')\n    RDM_TRANSFER_TASK_TIMEDELTA = conf.get_int(\'rdm_transfer_task\', \'TIMEDELTA\')\n    \n    # Настройка запуска периодической задачи статуса загрузки данных в витрину:\n    RDM_UPLOAD_STATUS_TASK_MINUTE = conf.get(\'rdm_upload_status_task\', \'MINUTE\')\n    RDM_UPLOAD_STATUS_TASK_HOUR = conf.get(\'rdm_upload_status_task\', \'HOUR\')\n    RDM_UPLOAD_STATUS_TASK_DAY_OF_WEEK = conf.get(\'rdm_upload_status_task\', \'DAY_OF_WEEK\')\n    \n    # Загрузка данных в Региональную витрину данных (РВД)\n    # Адрес витрины (schema://host:port)\n    RDM_UPLOADER_CLIENT_URL = conf.get(\'uploader_client\', \'URL\')\n    \n    # Мнемоника Витрины\n    RDM_UPLOADER_CLIENT_DATAMART_NAME = conf.get(\'uploader_client\', \'DATAMART_NAME\')\n    \n    # Количество повторных попыток запроса\n    RDM_UPLOADER_CLIENT_REQUEST_RETRIES = conf.get_int(\'uploader_client\', \'REQUEST_RETRIES\')\n    \n    # Таймаут запроса, сек\n    RDM_UPLOADER_CLIENT_REQUEST_TIMEOUT = conf.get_int(\'uploader_client\', \'REQUEST_TIMEOUT\')\n    \n    # Включить эмуляцию отправки запросов\n    RDM_UPLOADER_CLIENT_ENABLE_REQUEST_EMULATION = conf.get_bool(\'uploader_client\', \'ENABLE_REQUEST_EMULATION\')\n    \n    ```\n\nВ дефолтный конфиг проекта необходимо добавить:\n\n```\n# Общие настройки интеграции с РВД\n[rmd_general]\n# Префикс идентификаторов записей сущностей специфический для продукта. Указывается в settings.py и не должен \n# изменяться. Возможность изменения через конфигурационный файл оставлена для экстренных случаев.\n# EXPORT_ENTITY_ID_PREFIX = \n# Количество записей моделей обрабатываемых за одну итерацию экспорта данных\nEXPORT_CHUNK_SIZE = 500\n# Количество записей моделей ЭШ обрабатываемых за одну итерацию сбора данных\nCOLLECT_CHUNK_SIZE = 500\n\n# Настройка запуска периодической задачи выгрузки данных\n[rdm_transfer_task]\nMINUTE=*/2\nHOUR=*\nDAY_OF_WEEK=*\n# Дельта между прошлым и текущим запуском, сек\nTIMEDELTA=120\n\n# Настройка запуска периодической задачи статуса загрузки данных в витрину\n[rdm_upload_status_task]\nMINUTE=*/2\nHOUR=*\nDAY_OF_WEEK=*\n\n[uploader_client]\n# Адрес витрины\nURL = http://localhost:8090\n# Мнемоника Витрины\nDATAMART_NAME = test\n# Количество повторных попыток запроса\nREQUEST_RETRIES = 10\n# Таймаут запроса, сек\nREQUEST_TIMEOUT = 10\n# Включить эмуляцию отправки запросов\nENABLE_REQUEST_EMULATION = True\n```\n\nНа основе дефолтного конфига произвести конфигурирование приложений.\n\nПеречень настроек в settings.py указан в таблице ниже.\n\n| Название настройки в settings                | Описание                                                                                                                           | Значение по умолчанию   |\n|----------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|-------------------------|\n| UPLOADS                                      | Основная директория в MEDIA, в которой будет создана директория edu_rdm_integration  для сохранения файлов для дальнейшей выгрузки | 500                     |\n| RDM_COLLECT_CHUNK_SIZE                       | Количество записей моделей обрабатываемых за одну итерацию сбора данных                                                            | 500                     |\n| RDM_EXPORT_CHUNK_SIZE                        | Количество записей моделей обрабатываемых за одну итерацию экспорта                                                                | 500                     |\n| RDM_UPLOADER_CLIENT_URL                      | Адрес витрины (schema://host:port)                                                                                                 | \'http://localhost:8090\' |\n| RDM_UPLOADER_CLIENT_DATAMART_NAME            | Мнемоника Витрины                                                                                                                  | \'test\'                  |\n| RDM_UPLOADER_CLIENT_REQUEST_RETRIES          | Количество повторных попыток запроса                                                                                               | 10                      |\n| RDM_UPLOADER_CLIENT_REQUEST_TIMEOUT          | Таймаут запроса, сек                                                                                                               | 10                      |\n| RDM_UPLOADER_CLIENT_ENABLE_REQUEST_EMULATION | Включить эмуляцию отправки запросов                                                                                                | True                    |\n| RDM_TRANSFER_TASK_MINUTE                     | Настройка запуска периодической задачи выгрузки данных. Минута                                                                     | \'0\'                     |\n| RDM_TRANSFER_TASK_HOUR                       | Настройка запуска периодической задачи выгрузки данных. Час                                                                        | \'*/4\'                   |\n| RDM_TRANSFER_TASK_DAY_OF_WEEK                | Настройка запуска периодической задачи выгрузки данных. День недели                                                                | \'*\'                     |\n| RDM_TRANSFER_TASK_TIMEDELTA                  | Дельта между предыдущим и следующим запуском периодической задачи в секундах                                                       | 3600                    |\n| RDM_UPLOAD_STATUS_TASK_MINUTE                | Настройка запуска периодической задачи статуса загрузки данных в витрину. Минута                                                   | \'*/30\'                  |\n| RDM_UPLOAD_STATUS_TASK_HOUR                  | Настройка запуска периодической задачи статуса загрузки данных в витрину. Час                                                      | \'*\'                     |\n| RDM_UPLOAD_STATUS_TASK_DAY_OF_WEEK           | Настройка запуска периодической задачи статуса загрузки данных в витрину. День недели                                              | \'*\'                     |\n\n\n## Сборка и распространение\n\n## Инструкция для разработчика\n\n## Настройка PyCharm для работы\n\n## Запуск в системе\n\n## Запуск в контейнере\n\n## Правила внесения изменений\n',
     'author': 'BARS Group',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `edu_rdm_integration-0.0.1/PKG-INFO` & `edu_rdm_integration-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 0.0.1
+Version: 0.1.0
 Summary: Интеграция с Региональной витриной данных
 License: MIT
 Author: BARS Group
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

