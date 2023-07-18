# Comparing `tmp/whylogs-1.2.4.tar.gz` & `tmp/whylogs-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.2.4.tar", max compression
+gzip compressed data, was "whylogs-1.2.5.tar", max compression
```

## Comparing `whylogs-1.2.4.tar` & `whylogs-1.2.5.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0     3166 2023-07-14 14:40:50.259786 whylogs-1.2.4/DESCRIPTION.md
--rw-r--r--   0        0        0     5846 2023-07-14 14:41:16.932217 whylogs-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0     8157 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
--rw-r--r--   0        0        0      468 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
--rw-r--r--   0        0        0     2119 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
--rw-r--r--   0        0        0    15693 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
--rw-r--r--   0        0        0     3964 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
--rw-r--r--   0        0        0     4770 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    19765 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9550 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6333 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-07-14 14:40:50.303787 whylogs-1.2.4/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0     7497 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      329 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3813 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0    10646 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0      666 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      947 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    40899 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1217 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0     1090 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3391 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30671 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11486 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4120 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     1740 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0     8976 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14489 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2023-07-14 14:41:20.464272 whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2023-07-14 14:41:20.612274 whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-07-14 14:41:19.172253 whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2023-07-14 14:41:19.076251 whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-07-14 14:41:19.076251 whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/relations.py
--rw-r--r--   0        0        0    11101 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10029 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2087 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     1602 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      210 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4760 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0      508 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17663 2023-07-14 14:40:50.307787 whylogs-1.2.4/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     8747 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    13776 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0     8861 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    10031 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15367 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6959 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-07-14 14:40:50.311787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-07-14 14:40:50.315787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-07-14 14:40:50.319787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-07-14 14:40:50.323787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-07-14 14:40:50.327787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-07-14 14:40:50.327787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    21376 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-07-14 14:40:50.331787 whylogs-1.2.4/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-07-18 21:18:16.685593 whylogs-1.2.5/DESCRIPTION.md
+-rw-r--r--   0        0        0     5846 2023-07-18 21:18:44.473772 whylogs-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0     8157 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/future_util.py
+-rw-r--r--   0        0        0     2119 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py
+-rw-r--r--   0        0        0    15693 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py
+-rw-r--r--   0        0        0     3964 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py
+-rw-r--r--   0        0        0     4770 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    19765 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6333 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6168 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-07-18 21:18:16.733594 whylogs-1.2.5/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0     7497 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      329 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3813 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0    10646 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0      666 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      947 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    41758 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1217 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0     1090 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3391 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30671 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11486 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     1740 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0     8976 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14489 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-07-18 21:18:47.921796 whylogs-1.2.5/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-07-18 21:18:46.909789 whylogs-1.2.5/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-07-18 21:18:46.909789 whylogs-1.2.5/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-07-18 21:18:46.909789 whylogs-1.2.5/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-07-18 21:18:48.061797 whylogs-1.2.5/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-07-18 21:18:46.909789 whylogs-1.2.5/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-07-18 21:18:46.809788 whylogs-1.2.5/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-07-18 21:18:46.809788 whylogs-1.2.5/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10029 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2087 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     1602 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      210 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4760 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0      508 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    17663 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     8747 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-07-18 21:18:16.737594 whylogs-1.2.5/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    14261 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0     8861 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    10031 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15367 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6959 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-07-18 21:18:16.741593 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-07-18 21:18:16.745594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-07-18 21:18:16.749594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-07-18 21:18:16.753594 whylogs-1.2.5/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-07-18 21:18:16.757594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    21376 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-07-18 21:18:16.761594 whylogs-1.2.5/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     6558 1970-01-01 00:00:00.000000 whylogs-1.2.5/PKG-INFO
```

### Comparing `whylogs-1.2.4/DESCRIPTION.md` & `whylogs-1.2.5/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/pyproject.toml` & `whylogs-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.2.4"
+version = "1.2.5"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.2.4/whylogs/__init__.py` & `whylogs-1.2.5/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/annotations.py` & `whylogs-1.2.5/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/fugue/profiler.py` & `whylogs-1.2.5/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/fugue/registry.py` & `whylogs-1.2.5/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/__init__.py` & `whylogs-1.2.5/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py` & `whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/message_processor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py` & `whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/multi_dataset_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py` & `whylogs-1.2.5/whylogs/api/logger/experimental/multi_dataset_logger/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/logger.py` & `whylogs-1.2.5/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/result_set.py` & `whylogs-1.2.5/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/rolling.py` & `whylogs-1.2.5/whylogs/api/logger/rolling.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             file_extension = ".bin"
 
         self.file_extension = file_extension
         self.base_name = base_name
         self.aligned = aligned
         self.fork = fork
         self.skip_empty = skip_empty
-        self._metadatay = metadata
+        self._metadata = metadata
 
         # base on TimedRotatingFileHandler
         self.when = when.upper()
         if self.when == "S":
             self.interval = 1  # one second
             self.suffix = "%Y-%m-%d_%H-%M-%S"
         elif self.when == "M":
```

### Comparing `whylogs-1.2.4/whylogs/api/logger/segment_cache.py` & `whylogs-1.2.5/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/segment_processing.py` & `whylogs-1.2.5/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/logger/transient.py` & `whylogs-1.2.5/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.2.5/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.2.5/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/reader/local.py` & `whylogs-1.2.5/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/reader/reader.py` & `whylogs-1.2.5/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/reader/s3.py` & `whylogs-1.2.5/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/store/local_store.py` & `whylogs-1.2.5/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/store/profile_store.py` & `whylogs-1.2.5/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/store/query.py` & `whylogs-1.2.5/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/store/sqlite_store.py` & `whylogs-1.2.5/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/usage_stats/__init__.py` & `whylogs-1.2.5/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/whylabs/session/config.py` & `whylogs-1.2.5/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.2.5/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.2.5/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.2.5/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/__init__.py` & `whylogs-1.2.5/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/gcs.py` & `whylogs-1.2.5/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/local.py` & `whylogs-1.2.5/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/mlflow.py` & `whylogs-1.2.5/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/s3.py` & `whylogs-1.2.5/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/api/writer/whylabs.py` & `whylogs-1.2.5/whylogs/api/writer/whylabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,24 @@
 _API_CLIENT_CACHE: Dict[str, ApiClient] = dict()
 _UPLOAD_POOLER_CACHE: Dict[str, Union[PoolManager, ProxyManager]] = dict()
 
 _US_WEST2_DOMAIN = "songbird-20201223060057342600000001.s3.us-west-2.amazonaws.com"
 _S3_PUBLIC_DOMAIN = os.environ.get("_WHYLABS_PRIVATE_S3_DOMAIN") or _US_WEST2_DOMAIN
 _WHYLABS_SKIP_CONFIG_READ = os.environ.get("_WHYLABS_SKIP_CONFIG_READ") or False
 
+KNOWN_CUSTOM_PERFORMANCE_METRICS = {
+    "mean_average_precision_k_": "mean",
+    "accuracy_k_": "mean",
+    "mean_reciprocal_rank": "mean",
+    "precision_k_": "mean",
+    "recall_k_": "mean",
+    "top_rank": "mean",
+    "average_precision_k_": "mean",
+}
+
 
 def _check_whylabs_condition_count_uncompound() -> bool:
     global _WHYLABS_SKIP_CONFIG_READ
     if _WHYLABS_SKIP_CONFIG_READ:
         return True
     whylabs_config_url = (
         "https://whylabs-public.s3.us-west-2.amazonaws.com/whylogs_config/whylabs_condition_count_disabled"
@@ -585,25 +595,35 @@
                 )
                 upload_statuses.append(upload_res)
         if all([status[0] for status in upload_statuses]):
             return upload_statuses[0]
         else:
             return False, "Failed to upload all segments"
 
+    def _tag_custom_perf_metrics(self, view: Union[DatasetProfileView, SegmentedDatasetProfileView]):
+        if isinstance(view, DatasetProfileView):
+            column_names = view.get_columns().keys()
+            for column_name in column_names:
+                for perf_col in KNOWN_CUSTOM_PERFORMANCE_METRICS:
+                    if column_name.startswith(perf_col):
+                        metric = KNOWN_CUSTOM_PERFORMANCE_METRICS[perf_col]
+                        self.tag_custom_performance_column(column_name, default_metric=metric)
+        return
+
     @deprecated_alias(profile="file")
     def write(self, file: Writable, **kwargs: Any) -> Tuple[bool, str]:
         if isinstance(file, FeatureWeights):
             return self.write_feature_weights(file, **kwargs)
         elif isinstance(file, EstimationResult):
             return self.write_estimation_result(file, **kwargs)
         elif isinstance(file, SegmentedResultSet) and self._reference_profile_name is not None:
             return self._write_segmented_reference_result_set(file, **kwargs)
         view = file.view() if isinstance(file, DatasetProfile) else file
         has_segments = isinstance(view, SegmentedDatasetProfileView)
-
+        self._tag_custom_perf_metrics(view)
         if not has_segments and not isinstance(view, DatasetProfileView):
             raise ValueError(
                 "You must pass either a DatasetProfile or a DatasetProfileView in order to use this writer!"
             )
 
         flags = FeatureFlags(_check_whylabs_condition_count_uncompound())
```

### Comparing `whylogs-1.2.4/whylogs/api/writer/writer.py` & `whylogs-1.2.5/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/__init__.py` & `whylogs-1.2.5/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/column_profile.py` & `whylogs-1.2.5/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/configs.py` & `whylogs-1.2.5/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.2.5/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.2.5/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/dataset_profile.py` & `whylogs-1.2.5/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/datatypes.py` & `whylogs-1.2.5/whylogs/core/datatypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,14 +120,17 @@
 
 
 class TypeMapper(ABC):
     @abstractmethod
     def __call__(self, dtype_or_type: Any) -> DataType:
         raise NotImplementedError
 
+    def __eq__(self, other):  # just here for unit testing purposes
+        return type(self) == type(other)
+
 
 class StandardTypeMapper(TypeMapper):
     """Map a dtype (Pandas) or a Python type to a data type."""
 
     def __init__(self, custom_types: Optional[List[Type[DataType]]] = None):
         """
```

### Comparing `whylogs-1.2.4/whylogs/core/errors.py` & `whylogs-1.2.5/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/feature_weights.py` & `whylogs-1.2.5/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/input_resolver.py` & `whylogs-1.2.5/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metric_getters.py` & `whylogs-1.2.5/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/__init__.py` & `whylogs-1.2.5/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/aggregators.py` & `whylogs-1.2.5/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/column_metrics.py` & `whylogs-1.2.5/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/compound_metric.py` & `whylogs-1.2.5/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.2.5/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/decorators.py` & `whylogs-1.2.5/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/deserializers.py` & `whylogs-1.2.5/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/maths.py` & `whylogs-1.2.5/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/metric_components.py` & `whylogs-1.2.5/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/metrics.py` & `whylogs-1.2.5/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/multimetric.py` & `whylogs-1.2.5/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/serializers.py` & `whylogs-1.2.5/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/metrics/unicode_range.py` & `whylogs-1.2.5/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.2.5/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.2.5/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.2.5/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/predicate_parser.py` & `whylogs-1.2.5/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/preprocessing.py` & `whylogs-1.2.5/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.2.5/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.2.5/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.2.5/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/relations.py` & `whylogs-1.2.5/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/resolvers.py` & `whylogs-1.2.5/whylogs/core/resolvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import logging
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
 from typing_extensions import TypeAlias
 
-from whylogs.core.datatypes import AnyType, DataType, Fractional, Integral, String
+from whylogs.core.datatypes import (
+    AnyType,
+    DataType,
+    Fractional,
+    Integral,
+    StandardTypeMapper,
+    String,
+    TypeMapper,
+)
 from whylogs.core.metrics import StandardMetric
 from whylogs.core.metrics.metrics import Metric, MetricConfig
 
 logger = logging.getLogger(__name__)
 
 
 M = TypeVar("M", bound=Metric)
@@ -106,25 +114,29 @@
     takes precedence over column_type. column_type should be a subclass
     of DataType, i.e., AnyType, Frational, Integral, or String. Pass the
     class, not an instance. If the exclude field is True, the listed metrics
     will be excluded from any matched columns.
     """
 
     column_name: Optional[str] = None  # TODO: maybe make this a regex
-    column_type: Optional[DataType] = None
+    column_type: Optional[Type] = None
     metrics: List[MetricSpec] = field(default_factory=list)
     exclude: bool = False
+    type_mapper: TypeMapper = field(default_factory=StandardTypeMapper)
 
     def __post_init__(self):
         if self.column_name and self.column_type:
             logger.warning(f"ResolverSpec: column {self.column_name} also specified type, name takes precedence")
         if not (self.column_name or self.column_type):
             raise ValueError("ResolverSpec: resolver specification must supply name or type")
 
-        if self.column_type and not issubclass(self.column_type, DataType):
+        try:
+            if self.column_type and not issubclass(self.column_type, DataType):
+                self.column_type = type(self.type_mapper(self.column_type))
+        except:  # noqa
             raise ValueError("ResolverSpec: resolver specification column type must be a DataType")
 
 
 # whylabs expects COLUMN_METRICS to be present for every column.
 COLUMN_METRICS = [MetricSpec(StandardMetric.counts.value), MetricSpec(StandardMetric.types.value)]
```

### Comparing `whylogs-1.2.4/whylogs/core/schema.py` & `whylogs-1.2.5/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/segmentation_partition.py` & `whylogs-1.2.5/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/specialized_resolvers.py` & `whylogs-1.2.5/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/stubs.py` & `whylogs-1.2.5/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.2.5/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/utils/stats_calculations.py` & `whylogs-1.2.5/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/utils/utils.py` & `whylogs-1.2.5/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/validators/condition_validator.py` & `whylogs-1.2.5/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/view/column_profile_view.py` & `whylogs-1.2.5/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.2.5/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.2.5/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/base.py` & `whylogs-1.2.5/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/configs.py` & `whylogs-1.2.5/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.2.5/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/descr/employee.rst` & `whylogs-1.2.5/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/descr/weather.rst` & `whylogs-1.2.5/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/ecommerce.py` & `whylogs-1.2.5/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/employee.py` & `whylogs-1.2.5/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/utils.py` & `whylogs-1.2.5/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/datasets/weather.py` & `whylogs-1.2.5/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.2.5/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.2.5/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.2.5/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/core/udf_schema.py` & `whylogs-1.2.5/whylogs/experimental/core/udf_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     Callable,
     Collection,
     Dict,
     List,
     Mapping,
     Optional,
     Tuple,
+    Type,
     Union,
 )
 
-from whylogs.core.datatypes import DataType, TypeMapper
+from whylogs.core.datatypes import DataType, StandardTypeMapper, TypeMapper
 from whylogs.core.metrics.metrics import Metric, MetricConfig
 from whylogs.core.resolvers import NO_FI_RESOLVER, MetricSpec, ResolverSpec
 from whylogs.core.schema import DeclarativeSchema
 from whylogs.core.segmentation_partition import SegmentationPartition
 from whylogs.core.stubs import pd
 from whylogs.core.validators.validator import Validator
 from whylogs.experimental.core.metrics.udf_metric import (
@@ -58,47 +59,49 @@
                 raise ValueError("UdfSpec cannot specify both column_names and column_type")
         elif self.column_names is None:
             raise ValueError("UdfSpec must specify column_names or column_type")
         elif len(self.column_names) == 0 or not all([isinstance(x, str) for x in self.column_names]):
             raise ValueError("UdfSpec column_names must be a non-empty list of strings")
 
 
-def _apply_udfs_on_row(value: Any, udfs: Dict, new_columns: Dict[str, Any], input_cols: Collection[str]) -> None:
+def _apply_udfs_on_row(
+    values: Union[List, Dict[str, List]], udfs: Dict, new_columns: Dict[str, Any], input_cols: Collection[str]
+) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
-            new_columns[new_col] = udf(value)
+            new_columns[new_col] = udf(values)[0]
         except Exception:  # noqa
             new_columns[new_col] = None
             logger.exception(f"Evaluating UDF {new_col} failed")
 
 
 def _apply_udfs_on_dataframe(
     pandas: pd.DataFrame, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]
 ) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
-            new_df[new_col] = udf(pandas)
+            new_df[new_col] = pd.Series(udf(pandas))
         except Exception as e:  # noqa
             new_df[new_col] = pd.Series([None])
             logger.exception(f"Evaluating UDF {new_col} failed on columns {pandas.keys()} with error {e}")
 
 
 def _apply_type_udfs(pandas: pd.Series, udfs: Dict, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
     for new_col, udf in udfs.items():
         if new_col in input_cols:
             continue
 
         try:
-            new_df[new_col] = udf(pandas)
+            new_df[new_col] = pd.Series(udf(pandas))
         except Exception as e:  # noqa
             new_df[new_col] = pd.Series([None])
             logger.exception(f"Evaluating UDF {new_col} failed on column {new_col} with error {e}")
 
 
 class UdfSchema(DeclarativeSchema):
     """
@@ -142,21 +145,22 @@
         return copy
 
     def _run_udfs_on_row(
         self, row: Mapping[str, Any], new_columns: Dict[str, Any], input_cols: Collection[str]
     ) -> None:
         for spec in self.multicolumn_udfs:
             if spec.column_names and set(spec.column_names).issubset(set(row.keys())):
-                _apply_udfs_on_row(row, spec.udfs, new_columns, input_cols)
+                inputs = {col: [row[col]] for col in spec.column_names}
+                _apply_udfs_on_row(inputs, spec.udfs, new_columns, input_cols)
 
         for column, value in row.items():
             why_type = type(self.type_mapper(type(value)))
             for spec in self.type_udfs[why_type]:
                 udfs = {f"{column}.{key}": spec.udfs[key] for key in spec.udfs.keys()}
-                _apply_udfs_on_row(value, udfs, new_columns, input_cols)
+                _apply_udfs_on_row([value], udfs, new_columns, input_cols)
 
     def _run_udfs_on_dataframe(self, pandas: pd.DataFrame, new_df: pd.DataFrame, input_cols: Collection[str]) -> None:
         for spec in self.multicolumn_udfs:
             if spec.column_names and set(spec.column_names).issubset(set(pandas.keys())):
                 _apply_udfs_on_dataframe(pandas[spec.column_names], spec.udfs, new_df, input_cols)
 
         for column, dtype in pandas.dtypes.items():
@@ -238,18 +242,19 @@
 
         return func
 
     return decorator_register
 
 
 def register_type_udf(
-    col_type: DataType,
+    col_type: Type,
     udf_name: Optional[str] = None,
     namespace: Optional[str] = None,
     schema_name: str = "",
+    type_mapper: Optional[TypeMapper] = None,
 ) -> Callable[[Any], Any]:
     """
     Decorator to easily configure UDFs for your data set. Decorate your UDF
     functions, then call generate_udf_dataset_schema() to create a UdfSchema
     that includes the UDFs configured by your decorator parameters. The decorated
     function will automatically be a UDF in the UdfSchema.
 
@@ -259,14 +264,20 @@
     UDF name prefixed with the input column name. Note that all lambdas are
     named "lambda", so omitting udf_name on more than one lambda will result
     in name collisions. If you pass a namespace, it will be prepended to the UDF name.
     Specifying schema_name will register the UDF in a particular schema. If omitted,
     it will be registered to the defualt schema.
 
     """
+    try:
+        if not issubclass(col_type, DataType):
+            type_mapper = type_mapper or StandardTypeMapper()
+            col_type = type(type_mapper(col_type))
+    except:  # noqa
+        raise ValueError("Column type must be a DataType or Python type mapable to one")
 
     def decorator_register(func):
         global _multicolumn_udfs, _resolver_specs
         name = udf_name or func.__name__
         name = f"{namespace}.{name}" if namespace else name
         _multicolumn_udfs[schema_name].append(UdfSpec(None, {name: func}, col_type))
```

### Comparing `whylogs-1.2.4/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.2.5/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.2.5/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.2.5/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.2.5/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.2.5/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.2.5/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/extras/image_metric.py` & `whylogs-1.2.5/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/migration/converters.py` & `whylogs-1.2.5/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/migration/uncompound.py` & `whylogs-1.2.5/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.2.5/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/drift/configs.py` & `whylogs-1.2.5/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/enums/enums.py` & `whylogs-1.2.5/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.2.5/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.2.5/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.2.5/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.2.5/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.2.5/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.2.5/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.2.5/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.2.5/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/js/d3.min.js` & `whylogs-1.2.5/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/js/handlebars.js` & `whylogs-1.2.5/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.2.5/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.2.5/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/html/templates/index.html` & `whylogs-1.2.5/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.2.5/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.2.5/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.2.5/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.2.5/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.2.5/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.2.5/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.2.5/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.2.5/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.2.4/PKG-INFO` & `whylogs-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylogs
-Version: 1.2.4
+Version: 1.2.5
 Summary: Profile and monitor your ML data pipeline end-to-end
 Home-page: https://docs.whylabs.ai
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.7.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whylogs Version: 1.2.4 Summary: Profile and monitor
+Metadata-Version: 2.1 Name: whylogs Version: 1.2.5 Summary: Profile and monitor
 your ML data pipeline end-to-end Home-page: https://docs.whylabs.ai License:
 Apache-2.0 Author: WhyLabs.ai Author-email: support@whylabs.ai Requires-Python:
 >=3.7.1,<4 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: datasets
```

