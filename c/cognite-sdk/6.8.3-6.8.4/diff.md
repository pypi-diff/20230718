# Comparing `tmp/cognite_sdk-6.8.3.tar.gz` & `tmp/cognite_sdk-6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.8.3.tar", max compression
+gzip compressed data, was "cognite_sdk-6.8.4.tar", max compression
```

## Comparing `cognite_sdk-6.8.3.tar` & `cognite_sdk-6.8.4.tar`

### file list

```diff
@@ -1,118 +1,119 @@
--rw-r--r--   0        0        0    11349 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/LICENSE
--rw-r--r--   0        0        0     3945 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/README.md
--rw-r--r--   0        0        0      574 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     8676 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49274 2023-07-12 12:31:56.960740 cognite_sdk-6.8.3/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1317 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     8056 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     9702 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     3088 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/graphql.py
--rw-r--r--   0        0        0    43356 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6620 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     8845 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-07-12 12:31:56.964740 cognite_sdk-6.8.3/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38337 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_api_client.py
--rw-r--r--   0        0        0     9688 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/beta.py
--rw-r--r--   0        0        0     5675 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/config.py
--rw-r--r--   0        0        0    22326 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0    10425 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34417 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    34142 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4207 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0      693 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/graphql.py
--rw-r--r--   0        0        0     6968 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    31469 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0    13178 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/query.py
--rw-r--r--   0        0        0     2944 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14889 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-07-12 12:31:56.968740 cognite_sdk-6.8.3/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9968 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/py.typed
--rw-r--r--   0        0        0     9163 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2222 2023-07-12 12:31:56.972740 cognite_sdk-6.8.3/pyproject.toml
--rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.8.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/LICENSE
+-rw-r--r--   0        0        0     3945 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/README.md
+-rw-r--r--   0        0        0      574 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     8676 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49274 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1317 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/_data_modeling_executor.py
+-rw-r--r--   0        0        0     8425 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0    10061 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3088 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/graphql.py
+-rw-r--r--   0        0        0    43627 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6974 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     9126 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41590 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38862 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     9688 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/beta.py
+-rw-r--r--   0        0        0     5675 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/config.py
+-rw-r--r--   0        0        0    22326 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0    10425 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34417 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    34142 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4207 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7670 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0      693 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/graphql.py
+-rw-r--r--   0        0        0     6968 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    31469 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    13178 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     2944 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14889 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6349 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9968 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/py.typed
+-rw-r--r--   0        0        0     9163 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7559 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2222 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/pyproject.toml
+-rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.8.4/PKG-INFO
```

### Comparing `cognite_sdk-6.8.3/LICENSE` & `cognite_sdk-6.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/README.md` & `cognite_sdk-6.8.4/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/__init__.py` & `cognite_sdk-6.8.4/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/annotations.py` & `cognite_sdk-6.8.4/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/assets.py` & `cognite_sdk-6.8.4/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 )
 from cognite.client.data_classes.data_modeling.ids import (
     ContainerId,
     ContainerIdentifier,
     _load_identifier,
 )
 
+from ._data_modeling_executor import get_data_modeling_executor
+
 
 class ContainersAPI(APIClient):
     _RESOURCE_PATH = "/models/containers"
 
     @overload
     def __call__(
         self,
@@ -107,15 +109,20 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes.data_modeling import ContainerId
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.containers.retrieve(ContainerId(space='mySpace', external_id='myContainer'))
         """
         identifier = _load_identifier(ids, "container")
-        return self._retrieve_multiple(list_cls=ContainerList, resource_cls=Container, identifiers=identifier)
+        return self._retrieve_multiple(
+            list_cls=ContainerList,
+            resource_cls=Container,
+            identifiers=identifier,
+            executor=get_data_modeling_executor(),
+        )
 
     def delete(self, id: ContainerIdentifier | Sequence[ContainerIdentifier]) -> list[ContainerId]:
         """`Delete one or more containers <https://developer.cognite.com/api#tag/Containers/operation/deleteContainers>`_
 
         Args:
             id (ContainerId | Sequence[ContainerId): The container identifier(s).
         Returns:
@@ -126,15 +133,20 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.containers.delete(("mySpace", "myContainer"))
         """
         deleted_containers = cast(
             list,
-            self._delete_multiple(identifiers=_load_identifier(id, "container"), wrap_ids=True, returns_items=True),
+            self._delete_multiple(
+                identifiers=_load_identifier(id, "container"),
+                wrap_ids=True,
+                returns_items=True,
+                executor=get_data_modeling_executor(),
+            ),
         )
         return [ContainerId(space=item["space"], external_id=item["externalId"]) for item in deleted_containers]
 
     def list(
         self, space: str | None = None, limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT, include_global: bool = False
     ) -> ContainerList:
         """`List containers <https://developer.cognite.com/api#tag/Containers/operation/listContainers>`_
@@ -205,9 +217,13 @@
                 >>> from cognite.client.data_classes.data_modeling import ContainerApply, ContainerProperty, Text
                 >>> c = CogniteClient()
                 >>> container = [ContainerApply(space="mySpace", external_id="myContainer",
                 ...     properties={"name": ContainerProperty(type=Text(), name="name")})]
                 >>> res = c.data_modeling.containers.apply(container)
         """
         return self._create_multiple(
-            list_cls=ContainerList, resource_cls=Container, items=container, input_resource_cls=ContainerApply
+            list_cls=ContainerList,
+            resource_cls=Container,
+            items=container,
+            input_resource_cls=ContainerApply,
+            executor=get_data_modeling_executor(),
         )
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/data_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     DataModelApply,
     DataModelFilter,
     DataModelList,
 )
 from cognite.client.data_classes.data_modeling.ids import DataModelId, DataModelIdentifier, ViewId, _load_identifier
 from cognite.client.data_classes.data_modeling.views import View
 
+from ._data_modeling_executor import get_data_modeling_executor
+
 
 class DataModelsAPI(APIClient):
     _RESOURCE_PATH = "/models/datamodels"
 
     @overload
     def __call__(
         self,
@@ -116,15 +118,19 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.data_models.retrieve(("mySpace", "myDataModel", "v1"))
 
         """
         identifier = _load_identifier(ids, "data_model")
         return self._retrieve_multiple(
-            list_cls=DataModelList, resource_cls=DataModel, identifiers=identifier, params={"inlineViews": inline_views}
+            list_cls=DataModelList,
+            resource_cls=DataModel,
+            identifiers=identifier,
+            params={"inlineViews": inline_views},
+            executor=get_data_modeling_executor(),
         )
 
     def delete(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> list[DataModelId]:
         """`Delete one or more data model <https://developer.cognite.com/api#tag/Data-models/operation/deleteDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
@@ -136,15 +142,20 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.data_models.delete(("mySpace", "myDataModel", "v1"))
         """
         deleted_data_models = cast(
             list,
-            self._delete_multiple(identifiers=_load_identifier(ids, "data_model"), wrap_ids=True, returns_items=True),
+            self._delete_multiple(
+                identifiers=_load_identifier(ids, "data_model"),
+                wrap_ids=True,
+                returns_items=True,
+                executor=get_data_modeling_executor(),
+            ),
         )
         return [DataModelId(item["space"], item["externalId"], item["version"]) for item in deleted_data_models]
 
     @overload
     def list(
         self,
         inline_views: Literal[True],
@@ -245,9 +256,13 @@
                 >>> from cognite.client.data_classes.data_modeling import DataModelApply
                 >>> c = CogniteClient()
                 >>> data_models = [DataModelApply(space="mySpace",external_id="myDataModel",version="v1"),
                 ... DataModelApply(space="mySpace",external_id="myOtherDataModel",version="v1")]
                 >>> res = c.data_modeling.data_models.apply(data_models)
         """
         return self._create_multiple(
-            list_cls=DataModelList, resource_cls=DataModel, items=data_model, input_resource_cls=DataModelApply
+            list_cls=DataModelList,
+            resource_cls=DataModel,
+            items=data_model,
+            input_resource_cls=DataModelApply,
+            executor=get_data_modeling_executor(),
         )
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/graphql.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 from cognite.client.data_classes.data_modeling.query import (
     Query,
     QueryResult,
 )
 from cognite.client.data_classes.data_modeling.views import View
 from cognite.client.utils._identifier import DataModelingIdentifierSequence
 
+from ._data_modeling_executor import get_data_modeling_executor
+
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
 
 class _NodeOrEdgeList(CogniteResourceList):
     _RESOURCE = (Node, Edge)  # type: ignore[assignment]
 
@@ -280,14 +282,15 @@
         )
 
         res = self._retrieve_multiple(
             list_cls=_NodeOrEdgeList,
             resource_cls=_NodeOrEdgeResourceAdapter,  # type: ignore[type-var]
             identifiers=identifiers,
             other_params=other_params,
+            executor=get_data_modeling_executor(),
         )
 
         return InstancesResult(
             nodes=NodeList([node for node in res if isinstance(node, Node)]),
             edges=EdgeList([edge for edge in res if isinstance(edge, Edge)]),
         )
 
@@ -353,15 +356,20 @@
                 >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId
                 >>> c = CogniteClient()
                 >>> my_view = c.data_modeling.views.retrieve('mySpace', 'myView')
                 >>> my_nodes = c.data_modeling.instances.list(instance_type='node', sources=my_view, limit=None)
                 >>> c.data_modeling.instances.delete(nodes=my_nodes.as_ids())
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
-        deleted_instances = cast(List, self._delete_multiple(identifiers, wrap_ids=True, returns_items=True))
+        deleted_instances = cast(
+            List,
+            self._delete_multiple(
+                identifiers, wrap_ids=True, returns_items=True, executor=get_data_modeling_executor()
+            ),
+        )
         node_ids = [NodeId.load(item) for item in deleted_instances if item["instanceType"] == "node"]
         edge_ids = [EdgeId.load(item) for item in deleted_instances if item["instanceType"] == "edge"]
         return InstancesDeleteResult(node_ids, edge_ids)
 
     @classmethod
     def _create_other_params(
         cls,
@@ -497,14 +505,15 @@
 
         res = self._create_multiple(
             items=(*nodes, *edges),
             list_cls=_NodeOrEdgeApplyResultList,
             resource_cls=_NodeOrEdgeApplyResultAdapter,  # type: ignore[type-var]
             extra_body_fields=other_parameters,
             input_resource_cls=_NodeOrEdgeApplyAdapter,  # type: ignore[arg-type]
+            executor=get_data_modeling_executor(),
         )
         return InstancesApplyResult(
             nodes=NodeApplyResultList([item for item in res if isinstance(item, NodeApplyResult)]),
             edges=EdgeApplyResultList([item for item in res if isinstance(item, EdgeApplyResult)]),
         )
 
     @overload
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/spaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Iterator, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.ids import _load_space_identifier
 from cognite.client.data_classes.data_modeling.spaces import Space, SpaceApply, SpaceList
 
+from ._data_modeling_executor import get_data_modeling_executor
+
 
 class SpacesAPI(APIClient):
     _RESOURCE_PATH = "/models/spaces"
 
     @overload
     def __call__(
         self,
@@ -88,15 +90,17 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.spaces.retrieve(spaces=["MySpace", "MyAwesomeSpace", "MyOtherSpace"])
 
         """
         identifier = _load_space_identifier(space)
-        return self._retrieve_multiple(list_cls=SpaceList, resource_cls=Space, identifiers=identifier)
+        return self._retrieve_multiple(
+            list_cls=SpaceList, resource_cls=Space, identifiers=identifier, executor=get_data_modeling_executor()
+        )
 
     def delete(self, space: str | Sequence[str]) -> list[str]:
         """`Delete one or more spaces <https://developer.cognite.com/api#tag/Spaces/operation/deleteSpacesV3>`_
 
         Args:
             space (str | Sequence[str]): ID or ID list ids of spaces.
         Returns:
@@ -107,15 +111,20 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.spaces.delete(space=["mySpace", "myOtherSpace"])
         """
         deleted_spaces = cast(
             list,
-            self._delete_multiple(identifiers=_load_space_identifier(space), wrap_ids=True, returns_items=True),
+            self._delete_multiple(
+                identifiers=_load_space_identifier(space),
+                wrap_ids=True,
+                returns_items=True,
+                executor=get_data_modeling_executor(),
+            ),
         )
         return [item["space"] for item in deleted_spaces]
 
     def list(
         self,
         limit: int = LIST_LIMIT_DEFAULT,
         include_global: bool = False,
@@ -184,8 +193,14 @@
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes.data_modeling import SpaceApply
                 >>> c = CogniteClient()
                 >>> spaces = [SpaceApply(space="mySpace", description="My first space", name="My Space"),
                 ... SpaceApply(space="myOtherSpace", description="My second space", name="My Other Space")]
                 >>> res = c.data_modeling.spaces.apply(spaces)
         """
-        return self._create_multiple(list_cls=SpaceList, resource_cls=Space, items=space, input_resource_cls=SpaceApply)
+        return self._create_multiple(
+            list_cls=SpaceList,
+            resource_cls=Space,
+            items=space,
+            input_resource_cls=SpaceApply,
+            executor=get_data_modeling_executor(),
+        )
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from cognite.client.data_classes.data_modeling.ids import (
     ViewId,
     ViewIdentifier,
     _load_identifier,
 )
 from cognite.client.data_classes.data_modeling.views import View, ViewApply, ViewFilter, ViewList
 
+from ._data_modeling_executor import get_data_modeling_executor
+
 
 class ViewsAPI(APIClient):
     _RESOURCE_PATH = "/models/views"
 
     @overload
     def __call__(
         self,
@@ -116,14 +118,15 @@
         """
         identifier = _load_identifier(ids, "view")
         views = self._retrieve_multiple(
             list_cls=ViewList,
             resource_cls=View,
             identifiers=identifier,
             params={"includeInheritedProperties": include_inherited_properties},
+            executor=get_data_modeling_executor(),
         )
         if all_versions is True:
             return views
         else:
             return self._get_latest_views(views)
 
     def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[ViewId]:
@@ -143,14 +146,15 @@
         """
         deleted_views = cast(
             list,
             self._delete_multiple(
                 identifiers=_load_identifier(ids, "view"),
                 wrap_ids=True,
                 returns_items=True,
+                executor=get_data_modeling_executor(),
             ),
         )
         return [ViewId(item["space"], item["externalId"], item["version"]) for item in deleted_views]
 
     def list(
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
@@ -225,8 +229,14 @@
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_classes.data_modeling import ViewApply
                 >>> c = CogniteClient()
                 >>> views = [ViewApply(space="mySpace",external_id="myView",version="v1"),
                 ... ViewApply(space="mySpace",external_id="myOtherView",version="v1")]
                 >>> res = c.data_modeling.views.apply(views)
         """
-        return self._create_multiple(list_cls=ViewList, resource_cls=View, items=view, input_resource_cls=ViewApply)
+        return self._create_multiple(
+            list_cls=ViewList,
+            resource_cls=View,
+            items=view,
+            input_resource_cls=ViewApply,
+            executor=get_data_modeling_executor(),
+        )
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/data_sets.py` & `cognite_sdk-6.8.4/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.8.4/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/datapoints.py` & `cognite_sdk-6.8.4/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/diagrams.py` & `cognite_sdk-6.8.4/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.8.4/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/events.py` & `cognite_sdk-6.8.4/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.8.4/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/files.py` & `cognite_sdk-6.8.4/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/functions.py` & `cognite_sdk-6.8.4/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/geospatial.py` & `cognite_sdk-6.8.4/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/iam.py` & `cognite_sdk-6.8.4/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/labels.py` & `cognite_sdk-6.8.4/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/raw.py` & `cognite_sdk-6.8.4/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/relationships.py` & `cognite_sdk-6.8.4/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/sequences.py` & `cognite_sdk-6.8.4/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.8.4/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/templates.py` & `cognite_sdk-6.8.4/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/three_d.py` & `cognite_sdk-6.8.4/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/time_series.py` & `cognite_sdk-6.8.4/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.8.4/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.8.4/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.8.4/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.8.4/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.8.4/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api/vision.py` & `cognite_sdk-6.8.4/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_api_client.py` & `cognite_sdk-6.8.4/cognite/client/_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     CogniteResource,
     CogniteUpdate,
     T_CogniteResource,
     T_CogniteResourceList,
 )
 from cognite.client.exceptions import CogniteAPIError, CogniteNotFoundError
 from cognite.client.utils._auxiliary import is_unlimited, split_into_chunks
+from cognite.client.utils._concurrency import TaskExecutor
 from cognite.client.utils._identifier import IdentifierCore, IdentifierSequenceCore, SingletonIdentifierSequence
 from cognite.client.utils._text import convert_all_keys_to_camel_case, shorten, to_snake_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
     from cognite.client.config import ClientConfig
 
@@ -276,41 +277,44 @@
         resource_cls: Type[T_CogniteResource],
         identifiers: SingletonIdentifierSequence,
         resource_path: Optional[str] = None,
         ignore_unknown_ids: Optional[bool] = None,
         headers: Optional[Dict[str, Any]] = None,
         other_params: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> Optional[T_CogniteResource]:
         ...
 
     @overload
     def _retrieve_multiple(
         self,
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         identifiers: IdentifierSequenceCore,
         resource_path: Optional[str] = None,
         ignore_unknown_ids: Optional[bool] = None,
         headers: Optional[Dict[str, Any]] = None,
         other_params: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> T_CogniteResourceList:
         ...
 
     def _retrieve_multiple(
         self,
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         identifiers: Union[SingletonIdentifierSequence, IdentifierSequenceCore],
         resource_path: Optional[str] = None,
         ignore_unknown_ids: Optional[bool] = None,
         headers: Optional[Dict[str, Any]] = None,
         other_params: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> Union[T_CogniteResourceList, Optional[T_CogniteResource]]:
         resource_path = resource_path or self._RESOURCE_PATH
 
         ignore_unknown_obj = {} if ignore_unknown_ids is None else {"ignoreUnknownIds": ignore_unknown_ids}
         tasks: List[Dict[str, Union[str, Dict[str, Any], None]]] = [
             {
                 "url_path": resource_path + "/byids",
@@ -320,15 +324,17 @@
                     **(other_params or {}),
                 },
                 "headers": headers,
                 "params": params,
             }
             for id_chunk in identifiers.chunked(self._RETRIEVE_LIMIT)
         ]
-        tasks_summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
+        tasks_summary = utils._concurrency.execute_tasks(
+            self._post, tasks, max_workers=self._config.max_workers, executor=executor
+        )
 
         if tasks_summary.exceptions:
             try:
                 utils._concurrency.collect_exc_info_and_raise(tasks_summary.exceptions)
             except CogniteNotFoundError:
                 if identifiers.is_singleton():
                     return None
@@ -604,14 +610,15 @@
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
         input_resource_cls: Optional[Type[CogniteResource]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> T_CogniteResourceList:
         ...
 
     @overload
     def _create_multiple(
         self,
         items: Union[CogniteResource, Dict[str, Any]],
@@ -619,43 +626,47 @@
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
         input_resource_cls: Optional[Type[CogniteResource]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> T_CogniteResource:
         ...
 
     def _create_multiple(
         self,
         items: Union[Sequence[CogniteResource], Sequence[Dict[str, Any]], CogniteResource, Dict[str, Any]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
         input_resource_cls: Optional[Type[CogniteResource]] = None,
+        executor: Optional[TaskExecutor] = None,
     ) -> Union[T_CogniteResourceList, T_CogniteResource]:
         resource_path = resource_path or self._RESOURCE_PATH
         input_resource_cls = input_resource_cls or resource_cls
         limit = limit or self._CREATE_LIMIT
         single_item = not isinstance(items, Sequence)
         if single_item:
             items = cast(Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]]], [items])
         else:
             items = cast(Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]]], items)
 
         tasks = [
             (resource_path, task_items, params, headers)
             for task_items in self._prepare_item_chunks(items, limit, extra_body_fields)
         ]
-        summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
+        summary = utils._concurrency.execute_tasks(
+            self._post, tasks, max_workers=self._config.max_workers, executor=executor
+        )
 
         def unwrap_element(el: T) -> Union[CogniteResource, T]:
             if isinstance(el, dict):
                 return input_resource_cls._load(el, cognite_client=self._cognite_client)  # type: ignore[union-attr]
             else:
                 return el
 
@@ -683,29 +694,32 @@
         identifiers: IdentifierSequenceCore,
         wrap_ids: bool,
         resource_path: Optional[str] = None,
         params: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, Any]] = None,
         extra_body_fields: Optional[Dict[str, Any]] = None,
         returns_items: bool = False,
+        executor: Optional[TaskExecutor] = None,
     ) -> list | None:
         resource_path = resource_path or self._RESOURCE_PATH
         tasks = [
             {
                 "url_path": resource_path + "/delete",
                 "json": {
                     "items": chunk.as_dicts() if wrap_ids else chunk.as_primitives(),
                     **(extra_body_fields or {}),
                 },
                 "params": params,
                 "headers": headers,
             }
             for chunk in identifiers.chunked(self._DELETE_LIMIT)
         ]
-        summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
+        summary = utils._concurrency.execute_tasks(
+            self._post, tasks, max_workers=self._config.max_workers, executor=executor
+        )
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"],
             task_list_element_unwrap_fn=identifiers.unwrap_identifier,
         )
         if returns_items:
             return summary.joined_results(lambda res: res.json()["items"])
         else:
```

### Comparing `cognite_sdk-6.8.3/cognite/client/_cognite_client.py` & `cognite_sdk-6.8.4/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_http_client.py` & `cognite_sdk-6.8.4/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.8.4/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/config.py` & `cognite_sdk-6.8.4/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/credentials.py` & `cognite_sdk-6.8.4/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/_base.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/assets.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/graphql.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/query.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/query.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/events.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/files.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/functions.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/iam.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/labels.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/raw.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/shared.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/templates.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/exceptions.py` & `cognite_sdk-6.8.4/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/testing.py` & `cognite_sdk-6.8.4/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/__init__.py` & `cognite_sdk-6.8.4/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.8.4/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.8.4/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_graph.py` & `cognite_sdk-6.8.4/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_identifier.py` & `cognite_sdk-6.8.4/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_logging.py` & `cognite_sdk-6.8.4/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.8.4/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.8.4/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.8.4/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_text.py` & `cognite_sdk-6.8.4/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_time.py` & `cognite_sdk-6.8.4/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_validation.py` & `cognite_sdk-6.8.4/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.8.4/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.3/pyproject.toml` & `cognite_sdk-6.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.8.3"
+version = "6.8.4"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.8.3/PKG-INFO` & `cognite_sdk-6.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.8.3
+Version: 6.8.4
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.8.3 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.8.4 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

