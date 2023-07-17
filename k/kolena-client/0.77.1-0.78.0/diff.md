# Comparing `tmp/kolena_client-0.77.1.tar.gz` & `tmp/kolena_client-0.78.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.77.1.tar", max compression
+gzip compressed data, was "kolena_client-0.78.0.tar", max compression
```

## Comparing `kolena_client-0.77.1.tar` & `kolena_client-0.78.0.tar`

### file list

```diff
@@ -1,115 +1,116 @@
--rw-r--r--   0        0        0    11346 2023-07-17 18:15:30.569075 kolena_client-0.77.1/LICENSE
--rw-r--r--   0        0        0      556 2023-07-17 18:15:30.569075 kolena_client-0.77.1/LICENSE_HEADER
--rw-r--r--   0        0        0     1948 2023-07-17 18:15:30.569075 kolena_client-0.77.1/README.md
--rw-r--r--   0        0        0     1356 2023-07-17 18:20:57.688686 kolena_client-0.77.1/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5654 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    15446 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    10294 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    13260 2023-07-17 18:15:30.617075 kolena_client-0.77.1/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     5029 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      783 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/cli.py
--rw-r--r--   0        0        0      921 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/initialize.py
--rw-r--r--   0        0        0     2439 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-07-17 18:15:30.621075 kolena_client-0.77.1/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1103 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2977 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22734 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    10564 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      792 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     9419 2023-07-17 18:15:30.625075 kolena_client-0.77.1/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3037 2023-07-17 18:20:57.688686 kolena_client-0.77.1/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kolena_client-0.77.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-17 22:07:07.936741 kolena_client-0.78.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-07-17 22:07:07.936741 kolena_client-0.78.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     1948 2023-07-17 22:07:07.936741 kolena_client-0.78.0/README.md
+-rw-r--r--   0        0        0     1356 2023-07-17 22:14:34.547923 kolena_client-0.78.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5597 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5654 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    15465 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    10294 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    13260 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     5173 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      783 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      921 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-07-17 22:07:08.012742 kolena_client-0.78.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-07-17 22:07:08.016742 kolena_client-0.78.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2439 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1150 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3931 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22734 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    10564 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      841 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     1910 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/visualization/_utils.py
+-rw-r--r--   0        0        0     9419 2023-07-17 22:07:08.020742 kolena_client-0.78.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3037 2023-07-17 22:14:34.547923 kolena_client-0.78.0/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kolena_client-0.78.0/PKG-INFO
```

### Comparing `kolena_client-0.77.1/LICENSE` & `kolena_client-0.78.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/LICENSE_HEADER` & `kolena_client-0.78.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/README.md` & `kolena_client-0.78.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/__init__.py` & `kolena_client-0.78.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/__init__.py` & `kolena_client-0.78.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/__init__.py` & `kolena_client-0.78.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/batched_load.py` & `kolena_client-0.78.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/client_log.py` & `kolena_client-0.78.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/core.py` & `kolena_client-0.78.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/detection.py` & `kolena_client-0.78.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/fr.py` & `kolena_client-0.78.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/generic.py` & `kolena_client-0.78.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/repository.py` & `kolena_client-0.78.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/token.py` & `kolena_client-0.78.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_api/v1/workflow.py` & `kolena_client-0.78.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/__init__.py` & `kolena_client-0.78.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Set
 from typing import Tuple
 
 import numpy as np
 
 from kolena._experimental.object_detection.utils import compute_average_precision
 from kolena._experimental.object_detection.utils import compute_confusion_matrix_plot
 from kolena._experimental.object_detection.utils import compute_f1_plot_multiclass
@@ -78,25 +77,20 @@
 
     def compute_image_metrics(
         self,
         ground_truth: GroundTruth,
         inference: Inference,
         configuration: ThresholdConfiguration,
         test_case_name: str,
-        labels: Set[str],  # the labels being tested in this test case
     ) -> TestSampleMetrics:
         assert configuration is not None, "must specify configuration"
         thresholds = self.get_confidence_thresholds(configuration)
         bbox_matches: MulticlassInferenceMatches = match_inferences_multiclass(
             ground_truth.bboxes,
-            [
-                inf
-                for inf in inference.bboxes
-                if inf.label in labels and inf.score >= configuration.min_confidence_score
-            ],
+            [inf for inf in inference.bboxes if inf.score >= configuration.min_confidence_score],
             ignored_ground_truths=ground_truth.ignored_bboxes,
             mode="pascal",
             iou_threshold=configuration.iou_threshold,
         )
         self.matchings_by_test_case[test_case_name].append(bbox_matches)
         tp = [inf for _, inf in bbox_matches.matched if inf.score >= thresholds[inf.label]]
         fp = [inf for inf in bbox_matches.unmatched_inf if inf.score >= thresholds[inf.label]]
@@ -111,29 +105,34 @@
         image_labels = {gt.label for gt in ground_truth.bboxes}
         fields = [
             ScoredClassificationLabel(label=label, score=thresholds[label])
             for label in thresholds.keys()
             if label in image_labels
         ]
         return TestSampleMetrics(
+            TP_labels=sorted({inf.label for inf in tp}),
             TP=tp,
+            FP_labels=sorted({inf.label for inf in fp}),
             FP=fp,
+            FN_labels=sorted({inf.label for inf in fn}),
             FN=fn,
+            Confused_labels=sorted({inf.label for inf in confused}),
             Confused=confused,
             count_TP=len(tp),
             count_FP=len(fp),
             count_FN=len(fn),
             count_Confused=len(confused),
             has_TP=len(tp) > 0,
             has_FP=len(fp) > 0,
             has_FN=len(fn) > 0,
             has_Confused=len(confused) > 0,
             max_confidence_above_t=max(scores) if len(scores) > 0 else None,
             min_confidence_above_t=min(scores) if len(scores) > 0 else None,
             thresholds=fields,
+            inference_labels=sorted({inf.label for inf in inference.bboxes}),
         )
 
     def compute_and_cache_f1_optimal_thresholds(
         self,
         configuration: ThresholdConfiguration,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
     ) -> None:
@@ -164,19 +163,15 @@
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> List[Tuple[TestSample, TestSampleMetrics]]:
         assert configuration is not None, "must specify configuration"
         # compute thresholds to cache values for subsequent steps
         self.compute_and_cache_f1_optimal_thresholds(configuration, inferences)
-        labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
-        return [
-            (ts, self.compute_image_metrics(gt, inf, configuration, test_case.name, labels))
-            for ts, gt, inf in inferences
-        ]
+        return [(ts, self.compute_image_metrics(gt, inf, configuration, test_case.name)) for ts, gt, inf in inferences]
 
     def compute_aggregate_label_metrics(
         self,
         matchings: List[MulticlassInferenceMatches],
         label: str,
         thresholds: Dict[str, float],
     ) -> ClassMetricsPerTestCase:
```

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_experimental/object_detection/workflow.py` & `kolena_client-0.78.0/kolena/_experimental/object_detection/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,21 @@
     Recall: float
     F1: float
     AP: float
 
 
 @dataclass(frozen=True)
 class TestSampleMetrics(MetricsTestSample):
+    TP_labels: List[str]
     TP: List[ScoredLabeledBoundingBox]
+    FP_labels: List[str]
     FP: List[ScoredLabeledBoundingBox]
+    FN_labels: List[str]
     FN: List[LabeledBoundingBox]
+    Confused_labels: List[str]
     Confused: List[ScoredLabeledBoundingBox]
 
     count_TP: int
     count_FP: int
     count_FN: int
     count_Confused: int
 
@@ -110,14 +114,15 @@
     has_FP: bool
     has_FN: bool
     has_Confused: bool
 
     max_confidence_above_t: Optional[float]
     min_confidence_above_t: Optional[float]
     thresholds: List[ScoredClassificationLabel]
+    inference_labels: List[str]
 
 
 @dataclass(frozen=True)
 class ClassMetricsPerTestCase(MetricsTestCase):
     Class: str
     nImages: int
     Threshold: float
@@ -170,16 +175,16 @@
         raise RuntimeError(f"unrecognized threshold strategy: {self}")
 
 
 @dataclass(frozen=True)
 class ThresholdConfiguration(EvaluatorConfiguration):
     threshold_strategy: ThresholdStrategy
     iou_threshold: float
-    min_confidence_score: float
     with_class_level_metrics: bool
+    min_confidence_score: float = 0.0
 
     def display_name(self) -> str:
         return (
             f"Threshold: {self.threshold_strategy.display_name()}"
             f"{' by class' if self.with_class_level_metrics else ''}, "
             f"IoU: {self.iou_threshold}, confidence ≥ {self.min_confidence_score}"
         )
```

### Comparing `kolena_client-0.77.1/kolena/_extras/__init__.py` & `kolena_client-0.78.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_extras/metrics/__init__.py` & `kolena_client-0.78.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.78.0/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/__init__.py` & `kolena_client-0.78.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.78.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/batched_load.py` & `kolena_client-0.78.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/cli.py` & `kolena_client-0.78.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/consts.py` & `kolena_client-0.78.0/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.78.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/dataframes/validators.py` & `kolena_client-0.78.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/datatypes.py` & `kolena_client-0.78.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/endpoints.py` & `kolena_client-0.78.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/frozen.py` & `kolena_client-0.78.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/geometry.py` & `kolena_client-0.78.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/inference_validators.py` & `kolena_client-0.78.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/instrumentation.py` & `kolena_client-0.78.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/krequests.py` & `kolena_client-0.78.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/log.py` & `kolena_client-0.78.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/repository.py` & `kolena_client-0.78.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/serde.py` & `kolena_client-0.78.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/serializable.py` & `kolena_client-0.78.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/state.py` & `kolena_client-0.78.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/uninstantiable.py` & `kolena_client-0.78.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/_utils/validators.py` & `kolena_client-0.78.0/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/__init__.py` & `kolena_client-0.78.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/metadata.py` & `kolena_client-0.78.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/model.py` & `kolena_client-0.78.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/multiclass/__init__.py` & `kolena_client-0.78.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/multiclass/_utils.py` & `kolena_client-0.78.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.78.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/multiclass/test_run.py` & `kolena_client-0.78.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/multiclass/workflow.py` & `kolena_client-0.78.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/test_case.py` & `kolena_client-0.78.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/test_config.py` & `kolena_client-0.78.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/test_image.py` & `kolena_client-0.78.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/test_run.py` & `kolena_client-0.78.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/classification/test_suite.py` & `kolena_client-0.78.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/__init__.py` & `kolena_client-0.78.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_datatypes.py` & `kolena_client-0.78.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/__init__.py` & `kolena_client-0.78.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/datatypes.py` & `kolena_client-0.78.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/ground_truth.py` & `kolena_client-0.78.0/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/inference.py` & `kolena_client-0.78.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/metadata.py` & `kolena_client-0.78.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/model.py` & `kolena_client-0.78.0/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/test_case.py` & `kolena_client-0.78.0/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/test_config.py` & `kolena_client-0.78.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/test_image.py` & `kolena_client-0.78.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/test_run.py` & `kolena_client-0.78.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/_internal/test_suite.py` & `kolena_client-0.78.0/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/ground_truth.py` & `kolena_client-0.78.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/inference.py` & `kolena_client-0.78.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/metadata.py` & `kolena_client-0.78.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/model.py` & `kolena_client-0.78.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/test_case.py` & `kolena_client-0.78.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/test_config.py` & `kolena_client-0.78.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/test_image.py` & `kolena_client-0.78.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/test_run.py` & `kolena_client-0.78.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/detection/test_suite.py` & `kolena_client-0.78.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/errors.py` & `kolena_client-0.78.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/__init__.py` & `kolena_client-0.78.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/_utils.py` & `kolena_client-0.78.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/datatypes.py` & `kolena_client-0.78.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/model.py` & `kolena_client-0.78.0/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/test_case.py` & `kolena_client-0.78.0/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/test_images.py` & `kolena_client-0.78.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/test_run.py` & `kolena_client-0.78.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/fr/test_suite.py` & `kolena_client-0.78.0/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/initialize.py` & `kolena_client-0.78.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/__init__.py` & `kolena_client-0.78.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/_datatypes.py` & `kolena_client-0.78.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/_validators.py` & `kolena_client-0.78.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/annotation.py` & `kolena_client-0.78.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/asset.py` & `kolena_client-0.78.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/define_workflow.py` & `kolena_client-0.78.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/evaluator.py` & `kolena_client-0.78.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/evaluator_function.py` & `kolena_client-0.78.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/ground_truth.py` & `kolena_client-0.78.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/inference.py` & `kolena_client-0.78.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/metrics/__init__.py` & `kolena_client-0.78.0/kolena/workflow/metrics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from ._formula import accuracy
 from ._formula import f1_score
 from ._formula import precision
 from ._formula import recall
 from ._geometry import InferenceMatches
 from ._geometry import iou
 from ._geometry import match_inferences
 from ._geometry import match_inferences_multiclass
 from ._geometry import MulticlassInferenceMatches
 
 __all__ = [
+    "accuracy",
     "precision",
     "recall",
     "f1_score",
     "iou",
     "InferenceMatches",
     "match_inferences",
     "MulticlassInferenceMatches",
```

### Comparing `kolena_client-0.77.1/kolena/workflow/metrics/_formula.py` & `kolena_client-0.78.0/kolena/workflow/metrics/_formula.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,37 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+def accuracy(true_positives: int, false_positives: int, false_negatives: int, true_negatives: int) -> float:
+    """
+    Accuracy represents the proportion of inferences that are correct (including both positives and negatives).
+
+    $$
+    \\text{Accuracy} = \\frac{\\text{# TP} + \\text{# TN}}
+    {\\text{# TP} + \\text{# FP} + \\text{# FN} + \\text{# TN}}
+    $$
+
+    <div class="grid cards" markdown>
+    - :kolena-metrics-glossary-16: Metrics Glossary: [Accuracy ↗](../../metrics/accuracy.md)
+    </div>
+
+    :param true_positives: Number of true positive inferences.
+    :param false_positives: Number of false positive inferences.
+    :param false_negatives: Number of false negatives.
+    :param true_negatives: Number of true negatives.
+    """
+    numerator = true_positives + true_negatives
+    denominator = true_positives + false_positives + false_negatives + true_negatives
+    return numerator / denominator if denominator > 0 else 0
+
+
 def precision(true_positives: int, false_positives: int) -> float:
     """
     Precision represents the proportion of inferences that are correct.
 
     $$
     \\text{Precision} = \\frac{\\text{# True Positives}}{\\text{# True Positives} + \\text{# False Positives}}
     $$
```

### Comparing `kolena_client-0.77.1/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.78.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/model.py` & `kolena_client-0.78.0/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/plot.py` & `kolena_client-0.78.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/test_case.py` & `kolena_client-0.78.0/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/test_run.py` & `kolena_client-0.78.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/test_sample.py` & `kolena_client-0.78.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/test_suite.py` & `kolena_client-0.78.0/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/visualization/__init__.py` & `kolena_client-0.78.0/kolena/workflow/visualization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from ._activation_map import colorize_activation_map
 from ._activation_map import Colormap
 from ._activation_map import ColormapJet
+from ._utils import encode_png
 
 __all__ = [
     "Colormap",
     "ColormapJet",
     "colorize_activation_map",
+    "encode_png",
 ]
```

### Comparing `kolena_client-0.77.1/kolena/workflow/visualization/_activation_map.py` & `kolena_client-0.78.0/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/kolena/workflow/workflow.py` & `kolena_client-0.78.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.77.1/pyproject.toml` & `kolena_client-0.78.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.77.1"  # version is automatically set to latest git tag during release process
+version = "0.78.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
```

### Comparing `kolena_client-0.77.1/PKG-INFO` & `kolena_client-0.78.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.77.1
+Version: 0.78.0
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.77.1 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.78.0 Summary: Client for
 Kolena's machine learning testing platform. Home-page: https://kolena.io
 License: Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering
 Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

