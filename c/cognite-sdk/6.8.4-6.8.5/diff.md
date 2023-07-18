# Comparing `tmp/cognite_sdk-6.8.4.tar.gz` & `tmp/cognite_sdk-6.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.8.4.tar", max compression
+gzip compressed data, was "cognite_sdk-6.8.5.tar", max compression
```

## Comparing `cognite_sdk-6.8.4.tar` & `cognite_sdk-6.8.5.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    11349 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/LICENSE
--rw-r--r--   0        0        0     3945 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/README.md
--rw-r--r--   0        0        0      574 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     8676 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49274 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1317 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     1156 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/_data_modeling_executor.py
--rw-r--r--   0        0        0     8425 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0    10061 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     3088 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/graphql.py
--rw-r--r--   0        0        0    43627 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6974 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     9126 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11115 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87544 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21384 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17504 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41590 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45636 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    50175 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9619 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6088 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24756 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22919 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    38200 2023-07-12 13:44:59.337119 cognite_sdk-6.8.4/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7936 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    28258 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19276 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    22021 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     5083 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4691 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9705 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1881 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38862 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_api_client.py
--rw-r--r--   0        0        0     9688 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/beta.py
--rw-r--r--   0        0        0     5675 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/config.py
--rw-r--r--   0        0        0    22326 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0    10425 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34417 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    34142 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     4207 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0     5154 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/aggregations.py
--rw-r--r--   0        0        0    11348 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7670 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4710 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0      693 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/graphql.py
--rw-r--r--   0        0        0     6968 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    31469 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0    13178 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/query.py
--rw-r--r--   0        0        0     2944 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14889 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-07-12 13:44:59.341119 cognite_sdk-6.8.4/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6349 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9968 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/py.typed
--rw-r--r--   0        0        0     9163 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     7559 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7748 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2222 2023-07-12 13:44:59.345119 cognite_sdk-6.8.4/pyproject.toml
--rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-07-18 11:26:22.680902 cognite_sdk-6.8.5/LICENSE
+-rw-r--r--   0        0        0     3945 2023-07-18 11:26:22.680902 cognite_sdk-6.8.5/README.md
+-rw-r--r--   0        0        0      574 2023-07-18 11:26:22.680902 cognite_sdk-6.8.5/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:26:22.680902 cognite_sdk-6.8.5/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     8676 2023-07-18 11:26:22.680902 cognite_sdk-6.8.5/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49782 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1317 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/_data_modeling_executor.py
+-rw-r--r--   0        0        0     8465 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0    10101 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3088 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/graphql.py
+-rw-r--r--   0        0        0    43715 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     7024 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     9176 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11245 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87617 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12419 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21848 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17568 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    42408 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45780 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50369 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6208 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24920 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    23339 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38715 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     8006 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32082 2023-07-18 11:26:22.684902 cognite_sdk-6.8.5/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28398 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19666 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22281 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4721 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9725 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5920 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38982 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     9843 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/beta.py
+-rw-r--r--   0        0        0     5685 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/config.py
+-rw-r--r--   0        0        0    22346 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19171 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0    10445 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34855 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    34655 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4207 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5154 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11498 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7750 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0      693 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/graphql.py
+-rw-r--r--   0        0        0     6968 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    31660 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0    13295 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/query.py
+-rw-r--r--   0        0        0     3014 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14999 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6861 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    34564 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11359 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14826 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    14081 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    17245 2023-07-18 11:26:22.688902 cognite_sdk-6.8.5/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16934 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6613 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     6050 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4328 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12557 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17955 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8789 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    17456 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    12235 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12390 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23398 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12226 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11713 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2497 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2545 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2941 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0    10211 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/py.typed
+-rw-r--r--   0        0        0     9163 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     7579 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7748 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-07-18 11:26:22.692903 cognite_sdk-6.8.5/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2222 2023-07-18 11:26:22.696903 cognite_sdk-6.8.5/pyproject.toml
+-rw-r--r--   0        0        0     5699 1970-01-01 00:00:00.000000 cognite_sdk-6.8.5/PKG-INFO
```

### Comparing `cognite_sdk-6.8.4/LICENSE` & `cognite_sdk-6.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/README.md` & `cognite_sdk-6.8.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/__init__.py` & `cognite_sdk-6.8.5/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/annotations.py` & `cognite_sdk-6.8.5/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/assets.py` & `cognite_sdk-6.8.5/cognite/client/_api/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,33 +56,33 @@
 
 
 class AssetsAPI(APIClient):
     _RESOURCE_PATH = "/assets"
 
     def __call__(
         self,
-        chunk_size: int = None,
-        name: str = None,
-        parent_ids: Sequence[int] = None,
-        parent_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        metadata: Dict[str, str] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        root: bool = None,
-        external_id_prefix: str = None,
-        aggregated_properties: Sequence[str] = None,
-        limit: int = None,
-        partitions: int = None,
+        chunk_size: Optional[int] = None,
+        name: Optional[str] = None,
+        parent_ids: Optional[Sequence[int]] = None,
+        parent_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        root: Optional[bool] = None,
+        external_id_prefix: Optional[str] = None,
+        aggregated_properties: Optional[Sequence[str]] = None,
+        limit: Optional[int] = None,
+        partitions: Optional[int] = None,
     ) -> Union[Iterator[Asset], Iterator[AssetList]]:
         """Iterate over assets
 
         Fetches assets as they are iterated over, so you keep a limited number of assets in memory.
 
         Args:
             chunk_size (int, optional): Number of assets to return in each chunk. Defaults to yielding one asset a time.
@@ -214,31 +214,31 @@
         identifiers = IdentifierSequence.load(ids=ids, external_ids=external_ids)
         return self._retrieve_multiple(
             list_cls=AssetList, resource_cls=Asset, identifiers=identifiers, ignore_unknown_ids=ignore_unknown_ids
         )
 
     def list(
         self,
-        name: str = None,
-        parent_ids: Sequence[int] = None,
-        parent_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        metadata: Dict[str, str] = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        root: bool = None,
-        external_id_prefix: str = None,
-        aggregated_properties: Sequence[str] = None,
-        partitions: int = None,
+        name: Optional[str] = None,
+        parent_ids: Optional[Sequence[int]] = None,
+        parent_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        root: Optional[bool] = None,
+        external_id_prefix: Optional[str] = None,
+        aggregated_properties: Optional[Sequence[str]] = None,
+        partitions: Optional[int] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> AssetList:
         """`List assets <https://developer.cognite.com/api#tag/Assets/operation/listAssets>`_
 
         Args:
             name (str): Name of asset. Often referred to as tag.
             parent_ids (Sequence[int]): Return only the direct descendants of the specified assets.
@@ -324,15 +324,15 @@
             method="POST",
             limit=limit,
             filter=filter,
             other_params={"aggregatedProperties": aggregated_properties} if aggregated_properties else {},
             partitions=partitions,
         )
 
-    def aggregate(self, filter: Union[AssetFilter, dict] = None) -> List[AssetAggregate]:
+    def aggregate(self, filter: Optional[Union[AssetFilter, dict]] = None) -> List[AssetAggregate]:
         """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Args:
             filter (Union[AssetFilter, Dict]): Filter on assets filter with exact match
 
         Returns:
             List[AssetAggregate]: List of asset aggregates
@@ -343,15 +343,17 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> aggregate_by_prefix = c.assets.aggregate(filter={"external_id_prefix": "prefix"})
         """
         return self._aggregate(filter=filter, cls=AssetAggregate)
 
-    def aggregate_metadata_keys(self, filter: Union[AssetFilter, dict] = None) -> Sequence[AggregateBucketResult]:
+    def aggregate_metadata_keys(
+        self, filter: Optional[Union[AssetFilter, dict]] = None
+    ) -> Sequence[AggregateBucketResult]:
         """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Note:
             In the case of text fields, the values are aggregated in a case-insensitive manner
 
         Args:
             filter (Union[AssetFilter, Dict]): Filter on assets filter with exact match
@@ -366,15 +368,15 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> aggregate_by_prefix = c.assets.aggregate_metadata_keys(filter={"external_id_prefix": "prefix"})
         """
         return self._aggregate(filter=filter, aggregate="metadataKeys", cls=AggregateBucketResult)
 
     def aggregate_metadata_values(
-        self, keys: Sequence[str], filter: Union[AssetFilter, dict] = None
+        self, keys: Sequence[str], filter: Optional[Union[AssetFilter, dict]] = None
     ) -> Sequence[AggregateBucketResult]:
         """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Note:
             In the case of text fields, the values are aggregated in a case-insensitive manner
 
         Args:
@@ -567,16 +569,16 @@
             utils._auxiliary.assert_type(assets, "assets", [Sequence])
             assets = AssetHierarchy(assets, ignore_orphans=True)
 
         return _AssetHierarchyCreator(assets, assets_api=self).create(upsert, upsert_mode)
 
     def delete(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         recursive: bool = False,
         ignore_unknown_ids: bool = False,
     ) -> None:
         """`Delete one or more assets <https://developer.cognite.com/api#tag/Assets/operation/deleteAssets>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
@@ -667,18 +669,18 @@
                 >>> my_update = AssetUpdate(id=1).labels.set("PUMP")
                 >>> res = c.assets.update(my_update)
         """
         return self._update_multiple(list_cls=AssetList, resource_cls=Asset, update_cls=AssetUpdate, items=item)
 
     def search(
         self,
-        name: str = None,
-        description: str = None,
-        query: str = None,
-        filter: Union[AssetFilter, Dict] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        query: Optional[str] = None,
+        filter: Optional[Union[AssetFilter, Dict]] = None,
         limit: int = 100,
     ) -> AssetList:
         """`Search for assets <https://developer.cognite.com/api#tag/Assets/operation/searchAssets>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str): Fuzzy match on name.
@@ -726,15 +728,17 @@
         return self._search(
             list_cls=AssetList,
             search={"name": name, "description": description, "query": query},
             filter=filter or {},
             limit=limit,
         )
 
-    def retrieve_subtree(self, id: int = None, external_id: str = None, depth: int = None) -> AssetList:
+    def retrieve_subtree(
+        self, id: Optional[int] = None, external_id: Optional[str] = None, depth: Optional[int] = None
+    ) -> AssetList:
         """Retrieve the subtree for this asset up to a specified depth.
 
         Args:
             id (int): Id of the root asset in the subtree.
             external_id (str): External id of the root asset in the subtree.
             depth (int): Retrieve assets up to this depth below the root asset in the subtree. Omit to get the entire
                 subtree.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/_data_modeling_executor.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/_data_modeling_executor.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Sequence, cast, overload
+from typing import Iterator, Optional, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.containers import (
     Container,
     ContainerApply,
     ContainerFilter,
@@ -24,34 +24,34 @@
 
     @overload
     def __call__(
         self,
         chunk_size: None = None,
         space: str | None = None,
         include_global: bool = False,
-        limit: int = None,
+        limit: Optional[int] = None,
     ) -> Iterator[Container]:
         ...
 
     @overload
     def __call__(
         self,
         chunk_size: int,
         space: str | None = None,
         include_global: bool = False,
-        limit: int = None,
+        limit: Optional[int] = None,
     ) -> Iterator[ContainerList]:
         ...
 
     def __call__(
         self,
         chunk_size: int | None = None,
         space: str | None = None,
         include_global: bool = False,
-        limit: int = None,
+        limit: Optional[int] = None,
     ) -> Iterator[Container] | Iterator[ContainerList]:
         """Iterate over containers
 
         Fetches containers as they are iterated over, so you keep a limited number of containers in memory.
 
         Args:
             chunk_size (int, optional): Number of containers to return in each chunk. Defaults to yielding one container a time.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Literal, Sequence, cast, overload
+from typing import Iterator, Literal, Optional, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.data_models import (
     DataModel,
     DataModelApply,
     DataModelFilter,
@@ -19,38 +19,38 @@
 class DataModelsAPI(APIClient):
     _RESOURCE_PATH = "/models/datamodels"
 
     @overload
     def __call__(
         self,
         chunk_size: None = None,
-        limit: int = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[DataModel]:
         ...
 
     @overload
     def __call__(
         self,
         chunk_size: int,
-        limit: int = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[DataModelList]:
         ...
 
     def __call__(
         self,
         chunk_size: int | None = None,
-        limit: int = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[DataModel] | Iterator[DataModelList]:
         """Iterate over data model
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/graphql.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Sequence, Type, Union, cast, overload
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Optional, Sequence, Type, Union, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import INSTANCES_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes._base import CogniteResourceList
 from cognite.client.data_classes.data_modeling.aggregations import (
     Aggregation,
     Histogram,
@@ -50,64 +50,68 @@
     from cognite.client import CogniteClient
 
 
 class _NodeOrEdgeList(CogniteResourceList):
     _RESOURCE = (Node, Edge)  # type: ignore[assignment]
 
     @classmethod
-    def _load(cls, resource_list: list[dict[str, Any]] | str, cognite_client: CogniteClient = None) -> _NodeOrEdgeList:
+    def _load(
+        cls, resource_list: list[dict[str, Any]] | str, cognite_client: Optional[CogniteClient] = None
+    ) -> _NodeOrEdgeList:
         resource_list = json.loads(resource_list) if isinstance(resource_list, str) else resource_list
         resources: list[Node | Edge] = [
             Node.load(data) if data["instanceType"] == "node" else Edge.load(data) for data in resource_list
         ]
         return cls(resources, None)
 
     def as_ids(self) -> list[NodeId | EdgeId]:
         return [instance.as_id() for instance in self]
 
 
 class _NodeOrEdgeResourceAdapter:
     @classmethod
-    def _load(cls, data: str | dict, cognite_client: CogniteClient = None) -> Node | Edge:
+    def _load(cls, data: str | dict, cognite_client: Optional[CogniteClient] = None) -> Node | Edge:
         data = json.loads(data) if isinstance(data, str) else data
         if data["instanceType"] == "node":
             return Node.load(data)
         return Edge.load(data)
 
 
 class _NodeOrEdgeApplyResultList(CogniteResourceList):
     _RESOURCE = (NodeApplyResult, EdgeApplyResult)  # type: ignore[assignment]
 
     @classmethod
     def _load(
-        cls, resource_list: list[dict[str, Any]] | str, cognite_client: CogniteClient = None
+        cls, resource_list: list[dict[str, Any]] | str, cognite_client: Optional[CogniteClient] = None
     ) -> _NodeOrEdgeApplyResultList:
         resource_list = json.loads(resource_list) if isinstance(resource_list, str) else resource_list
         resources: list[NodeApplyResult | EdgeApplyResult] = [
             NodeApplyResult.load(data) if data["instanceType"] == "node" else EdgeApplyResult.load(data)
             for data in resource_list
         ]
         return cls(resources, None)
 
     def as_ids(self) -> list[NodeId | EdgeId]:
         return [result.as_id() for result in self]
 
 
 class _NodeOrEdgeApplyResultAdapter:
     @classmethod
-    def _load(cls, data: str | dict, cognite_client: CogniteClient = None) -> NodeApplyResult | EdgeApplyResult:
+    def _load(
+        cls, data: str | dict, cognite_client: Optional[CogniteClient] = None
+    ) -> NodeApplyResult | EdgeApplyResult:
         data = json.loads(data) if isinstance(data, str) else data
         if data["instanceType"] == "node":
             return NodeApplyResult.load(data)
         return EdgeApplyResult.load(data)
 
 
 class _NodeOrEdgeApplyAdapter:
     @classmethod
-    def _load(cls, data: str | dict, cognite_client: CogniteClient = None) -> NodeApply | EdgeApply:
+    def _load(cls, data: str | dict, cognite_client: Optional[CogniteClient] = None) -> NodeApply | EdgeApply:
         data = json.loads(data) if isinstance(data, str) else data
         if data["instanceType"] == "node":
             return NodeApply.load(data)
         return EdgeApply.load(data)
 
 
 class InstancesAPI(APIClient):
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/spaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Sequence, cast, overload
+from typing import Iterator, Optional, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.ids import _load_space_identifier
 from cognite.client.data_classes.data_modeling.spaces import Space, SpaceApply, SpaceList
 
 from ._data_modeling_executor import get_data_modeling_executor
@@ -13,30 +13,30 @@
 class SpacesAPI(APIClient):
     _RESOURCE_PATH = "/models/spaces"
 
     @overload
     def __call__(
         self,
         chunk_size: None = None,
-        limit: int = None,
+        limit: Optional[int] = None,
     ) -> Iterator[Space]:
         ...
 
     @overload
     def __call__(
         self,
         chunk_size: int,
-        limit: int = None,
+        limit: Optional[int] = None,
     ) -> Iterator[SpaceList]:
         ...
 
     def __call__(
         self,
-        chunk_size: int = None,
-        limit: int = None,
+        chunk_size: Optional[int] = None,
+        limit: Optional[int] = None,
     ) -> Iterator[Space] | Iterator[SpaceList]:
         """Iterate over spaces
 
         Fetches spaces as they are iterated over, so you keep a limited number of spaces in memory.
 
         Args:
             chunk_size (int, optional): Number of spaces to return in each chunk. Defaults to yielding one space a time.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_modeling/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Iterator, Sequence, cast, overload
+from typing import Iterator, Optional, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.ids import (
     ViewId,
     ViewIdentifier,
     _load_identifier,
@@ -18,38 +18,38 @@
 class ViewsAPI(APIClient):
     _RESOURCE_PATH = "/models/views"
 
     @overload
     def __call__(
         self,
         chunk_size: None = None,
-        limit: int = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[View]:
         ...
 
     @overload
     def __call__(
         self,
         chunk_size: int,
-        limit: int = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[ViewList]:
         ...
 
     def __call__(
         self,
-        chunk_size: int = None,
-        limit: int = None,
+        chunk_size: Optional[int] = None,
+        limit: Optional[int] = None,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> Iterator[View] | Iterator[ViewList]:
         """Iterate over views
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/data_sets.py` & `cognite_sdk-6.8.5/cognite/client/_api/data_sets.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._CREATE_LIMIT = 10
 
     def __call__(
         self,
-        chunk_size: int = None,
-        metadata: Dict[str, str] = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        write_protected: bool = None,
-        limit: int = None,
+        chunk_size: Optional[int] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        write_protected: Optional[bool] = None,
+        limit: Optional[int] = None,
     ) -> Union[Iterator[DataSet], Iterator[DataSetList]]:
         """Iterate over data sets
 
         Fetches data sets as they are iterated over, so you keep a limited number of data sets in memory.
 
         Args:
             chunk_size (int, optional): Number of data sets to return in each chunk. Defaults to yielding one data set a time.
@@ -154,19 +154,19 @@
         identifiers = IdentifierSequence.load(ids=ids, external_ids=external_ids)
         return self._retrieve_multiple(
             list_cls=DataSetList, resource_cls=DataSet, identifiers=identifiers, ignore_unknown_ids=ignore_unknown_ids
         )
 
     def list(
         self,
-        metadata: Dict[str, str] = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        write_protected: bool = None,
+        metadata: Optional[Dict[str, str]] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        write_protected: Optional[bool] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> DataSetList:
         """`List data sets <https://developer.cognite.com/api#tag/Data-sets/operation/listDataSets>`_
 
         Args:
             metadata (Dict[str, str]): Custom, application-specific metadata. String key -> String value.
             created_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
@@ -207,15 +207,15 @@
             created_time=created_time,
             last_updated_time=last_updated_time,
             external_id_prefix=external_id_prefix,
             write_protected=write_protected,
         ).dump(camel_case=True)
         return self._list(list_cls=DataSetList, resource_cls=DataSet, method="POST", limit=limit, filter=filter)
 
-    def aggregate(self, filter: Union[DataSetFilter, Dict] = None) -> List[DataSetAggregate]:
+    def aggregate(self, filter: Optional[Union[DataSetFilter, Dict]] = None) -> List[DataSetAggregate]:
         """`Aggregate data sets <https://developer.cognite.com/api#tag/Data-sets/operation/aggregateDataSets>`_
 
         Args:
             filter (Union[DataSetFilter, Dict]): Filter on data set filter with exact match
 
         Returns:
             List[DataSetAggregate]: List of data set aggregates
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.8.5/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/datapoints.py` & `cognite_sdk-6.8.5/cognite/client/_api/datapoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1236,16 +1236,16 @@
 
     def insert(
         self,
         datapoints: Datapoints
         | DatapointsArray
         | Sequence[dict[str, int | float | str | datetime]]
         | Sequence[tuple[int | float | datetime, int | float | str]],
-        id: int = None,
-        external_id: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
     ) -> None:
         """Insert datapoints into a time series
 
         Timestamps can be represented as milliseconds since epoch or datetime objects.
 
         Args:
             datapoints(Union[Datapoints, DatapointsArray, List[Dict], List[Tuple]]): The datapoints you wish to insert. Can either be a list of tuples,
@@ -1343,15 +1343,19 @@
             # Extract data inplace for any Datapoints and/or DatapointsArray:
             if isinstance(dps_dct, Mapping) and isinstance(dps_dct["datapoints"], (Datapoints, DatapointsArray)):
                 dps_dct["datapoints"] = DatapointsPoster._extract_raw_data_from_dps_container(dps_dct["datapoints"])
         dps_poster = DatapointsPoster(self)
         dps_poster.insert(datapoints)
 
     def delete_range(
-        self, start: int | str | datetime, end: int | str | datetime, id: int = None, external_id: str = None
+        self,
+        start: int | str | datetime,
+        end: int | str | datetime,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
     ) -> None:
         """Delete a range of datapoints from a time series.
 
         Args:
             start (Union[int, str, datetime]): Inclusive start of delete range
             end (Union[int, str, datetime]): Exclusvie end of delete range
             id (int): Id of time series to delete data from
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/diagrams.py` & `cognite_sdk-6.8.5/cognite/client/_api/diagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,31 +33,31 @@
         self._DETECT_API_FILE_LIMIT = 50
         # https://docs.cognite.com/api/playground/#operation/diagramDetectMultipleResults
         self._DETECT_API_STATUS_JOB_LIMIT = 1000
 
     def _camel_post(
         self,
         context_path: str,
-        json: Dict[str, Any] = None,
-        params: Dict[str, Any] = None,
-        headers: Dict[str, Any] = None,
+        json: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, Any]] = None,
     ) -> Response:
         return self._post(
             self._RESOURCE_PATH + context_path,
             json={to_camel_case(k): v for k, v in (json or {}).items() if v is not None},
             params=params,
             headers=headers,
         )
 
     def _run_job(
         self,
         job_cls: Type[T_ContextualizationJob],
         job_path: str,
-        status_path: str = None,
-        headers: Dict[str, Any] = None,
+        status_path: Optional[str] = None,
+        headers: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> T_ContextualizationJob:
         if status_path is None:
             status_path = job_path + "/"
         response = self._camel_post(job_path, json=kwargs, headers=headers)
         return job_cls._load_with_status(
             data=response.json(),
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.8.5/cognite/client/_api/entity_matching.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def _run_job(
         self,
         job_path: str,
         job_cls: Type[T_ContextualizationJob],
         json: Dict[str, Any],
         status_path: Optional[str] = None,
-        headers: Dict = None,
+        headers: Optional[Dict] = None,
     ) -> T_ContextualizationJob:
         if status_path is None:
             status_path = job_path + "/"
         response = self._post(self._RESOURCE_PATH + job_path, json=json, headers=headers)
 
         return job_cls._load_with_status(
             data=response.json(),
@@ -87,19 +87,19 @@
             resource_cls=EntityMatchingModel,
             update_cls=EntityMatchingModelUpdate,
             items=item,
         )
 
     def list(
         self,
-        name: str = None,
-        description: str = None,
-        original_id: int = None,
-        feature_type: str = None,
-        classifier: str = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        original_id: Optional[int] = None,
+        feature_type: Optional[str] = None,
+        classifier: Optional[str] = None,
         limit: int = 100,
     ) -> EntityMatchingModelList:
         """List models
 
         Args:
             name (str): Optional user-defined name of model.
             description (str): Optional user-defined description of model.
@@ -131,35 +131,37 @@
 
         Returns:
             ContextualizationJobList: List of jobs."""
         return ContextualizationJobList._load(
             self._get(self._RESOURCE_PATH + "/jobs").json()["items"], cognite_client=self._cognite_client
         )
 
-    def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete(
+        self, id: Optional[Union[int, Sequence[int]]] = None, external_id: Optional[Union[str, Sequence[str]]] = None
+    ) -> None:
         """Delete models
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids"""
 
         self._delete_multiple(identifiers=IdentifierSequence.load(ids=id, external_ids=external_id), wrap_ids=True)
 
     def fit(
         self,
         sources: Sequence[Union[Dict, CogniteResource]],
         targets: Sequence[Union[Dict, CogniteResource]],
-        true_matches: Sequence[Union[Dict, Tuple[Union[int, str], Union[int, str]]]] = None,
-        match_fields: Union[Dict, Sequence[Tuple[str, str]]] = None,
-        feature_type: str = None,
-        classifier: str = None,
+        true_matches: Optional[Sequence[Union[Dict, Tuple[Union[int, str], Union[int, str]]]]] = None,
+        match_fields: Optional[Union[Dict, Sequence[Tuple[str, str]]]] = None,
+        feature_type: Optional[str] = None,
+        classifier: Optional[str] = None,
         ignore_missing_fields: bool = False,
-        name: str = None,
-        description: str = None,
-        external_id: str = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        external_id: Optional[str] = None,
     ) -> EntityMatchingModel:
         """Fit entity matching model.
 
         Note:
             All users on this CDF subscription with assets read-all and entitymatching read-all and write-all
             capabilities in the project, are able to access the data sent to this endpoint.
 
@@ -204,15 +206,15 @@
         return EntityMatchingModel._load(response.json(), cognite_client=self._cognite_client)
 
     def predict(
         self,
         sources: Optional[Sequence[Dict]] = None,
         targets: Optional[Sequence[Dict]] = None,
         num_matches: int = 1,
-        score_threshold: float = None,
+        score_threshold: Optional[float] = None,
         id: Optional[int] = None,
         external_id: Optional[str] = None,
     ) -> ContextualizationJob:
         """Predict entity matching.
 
         Warning:
             Blocks and waits for the model to be ready if it has been recently created.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/events.py` & `cognite_sdk-6.8.5/cognite/client/_api/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 
 class EventsAPI(APIClient):
     _RESOURCE_PATH = "/events"
 
     def __call__(
         self,
-        chunk_size: int = None,
-        start_time: Union[Dict[str, Any], TimestampRange] = None,
-        end_time: Union[Dict[str, Any], EndTimeFilter] = None,
-        active_at_time: Union[Dict[str, Any], TimestampRange] = None,
-        type: str = None,
-        subtype: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        sort: Sequence[str] = None,
-        limit: int = None,
-        partitions: int = None,
+        chunk_size: Optional[int] = None,
+        start_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        end_time: Optional[Union[Dict[str, Any], EndTimeFilter]] = None,
+        active_at_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        type: Optional[str] = None,
+        subtype: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        sort: Optional[Sequence[str]] = None,
+        limit: Optional[int] = None,
+        partitions: Optional[int] = None,
     ) -> Union[Iterator[Event], Iterator[EventList]]:
         """Iterate over events
 
         Fetches events as they are iterated over, so you keep a limited number of events in memory.
 
         Args:
             chunk_size (int, optional): Number of events to return in each chunk. Defaults to yielding one event a time.
@@ -176,32 +176,32 @@
         identifiers = IdentifierSequence.load(ids=ids, external_ids=external_ids)
         return self._retrieve_multiple(
             list_cls=EventList, resource_cls=Event, identifiers=identifiers, ignore_unknown_ids=ignore_unknown_ids
         )
 
     def list(
         self,
-        start_time: Union[Dict[str, Any], TimestampRange] = None,
-        end_time: Union[Dict[str, Any], EndTimeFilter] = None,
-        active_at_time: Union[Dict[str, Any], TimestampRange] = None,
-        type: str = None,
-        subtype: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        sort: Sequence[str] = None,
-        partitions: int = None,
+        start_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        end_time: Optional[Union[Dict[str, Any], EndTimeFilter]] = None,
+        active_at_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        type: Optional[str] = None,
+        subtype: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        sort: Optional[Sequence[str]] = None,
+        partitions: Optional[int] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> EventList:
         """`List events <https://developer.cognite.com/api#tag/Events/operation/advancedListEvents>`_
 
         Args:
             start_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
             end_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
@@ -280,15 +280,15 @@
             method="POST",
             limit=limit,
             filter=filter,
             partitions=partitions,
             sort=sort,
         )
 
-    def aggregate(self, filter: Union[EventFilter, Dict] = None) -> List[AggregateResult]:
+    def aggregate(self, filter: Optional[Union[EventFilter, Dict]] = None) -> List[AggregateResult]:
         """`Aggregate events <https://developer.cognite.com/api#tag/Events/operation/aggregateEvents>`_
 
         Args:
             filter (Union[EventFilter, Dict]): Filter on events filter with exact match
 
         Returns:
             List[AggregateResult]: List of event aggregates
@@ -301,15 +301,15 @@
                 >>> c = CogniteClient()
                 >>> aggregate_type = c.events.aggregate(filter={"type": "failure"})
         """
 
         return self._aggregate(filter=filter, cls=AggregateResult)
 
     def aggregate_unique_values(
-        self, filter: Union[EventFilter, Dict] = None, fields: Sequence[str] = None
+        self, filter: Optional[Union[EventFilter, Dict]] = None, fields: Optional[Sequence[str]] = None
     ) -> List[AggregateUniqueValuesResult]:
         """`Aggregate unique values for events <https://developer.cognite.com/api#tag/Events/operation/aggregateEvents>`_
 
         Args:
             filter (Union[EventFilter, Dict]): Filter on events filter with exact match
             fields (Sequence[str]): The field name(s) to apply the aggregation on. Currently limited to one field.
 
@@ -354,16 +354,16 @@
                 >>> events = [Event(start_time=0, end_time=1), Event(start_time=2, end_time=3)]
                 >>> res = c.events.create(events)
         """
         return self._create_multiple(list_cls=EventList, resource_cls=Event, items=event)
 
     def delete(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
         """`Delete one or more events <https://developer.cognite.com/api#tag/Events/operation/deleteEvents>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
@@ -418,15 +418,17 @@
                 >>> from cognite.client.data_classes import EventUpdate
                 >>> c = CogniteClient()
                 >>> my_update = EventUpdate(id=1).description.set("New description").metadata.add({"key": "value"})
                 >>> res = c.events.update(my_update)
         """
         return self._update_multiple(list_cls=EventList, resource_cls=Event, update_cls=EventUpdate, items=item)
 
-    def search(self, description: str = None, filter: Union[EventFilter, Dict] = None, limit: int = 100) -> EventList:
+    def search(
+        self, description: Optional[str] = None, filter: Optional[Union[EventFilter, Dict]] = None, limit: int = 100
+    ) -> EventList:
         """`Search for events <https://developer.cognite.com/api#tag/Events/operation/searchEvents>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             description (str): Fuzzy match on description.
             filter (Union[EventFilter, Dict]): Filter to apply. Performs exact match on these fields.
             limit (int): Maximum number of results to return.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.8.5/cognite/client/_api/extractionpipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,15 +153,17 @@
                 >>> res = c.extraction_pipelines.create(extpipes)
         """
         utils._auxiliary.assert_type(extraction_pipeline, "extraction_pipeline", [ExtractionPipeline, Sequence])
         return self._create_multiple(
             list_cls=ExtractionPipelineList, resource_cls=ExtractionPipeline, items=extraction_pipeline
         )
 
-    def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete(
+        self, id: Optional[Union[int, Sequence[int]]] = None, external_id: Optional[Union[str, Sequence[str]]] = None
+    ) -> None:
         """`Delete one or more extraction pipelines <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/deleteExtPipes>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
 
         Returns:
@@ -219,17 +221,17 @@
 
 class ExtractionPipelineRunsAPI(APIClient):
     _RESOURCE_PATH = "/extpipes/runs"
 
     def list(
         self,
         external_id: str,
-        statuses: Sequence[str] = None,
-        message_substring: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
+        statuses: Optional[Sequence[str]] = None,
+        message_substring: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ExtractionPipelineRunList:
         """`List runs for an extraction pipeline with given external_id <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/filterRuns>`_
 
         Args:
             external_id (str): Extraction pipeline external Id.
             statuses (Sequence[str]): One or more among "success" / "failure" / "seen".
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/files.py` & `cognite_sdk-6.8.5/cognite/client/_api/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,36 +42,36 @@
 
 
 class FilesAPI(APIClient):
     _RESOURCE_PATH = "/files"
 
     def __call__(
         self,
-        chunk_size: int = None,
-        name: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        source_created_time: Union[Dict[str, Any], TimestampRange] = None,
-        source_modified_time: Union[Dict[str, Any], TimestampRange] = None,
-        uploaded_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        directory_prefix: str = None,
-        uploaded: bool = None,
-        limit: int = None,
+        chunk_size: Optional[int] = None,
+        name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        source_created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        source_modified_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        uploaded_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        directory_prefix: Optional[str] = None,
+        uploaded: Optional[bool] = None,
+        limit: Optional[int] = None,
     ) -> Union[Iterator[FileMetadata], Iterator[FileMetadataList]]:
         """Iterate over files
 
         Fetches file metadata objects as they are iterated over, so you keep a limited number of metadata objects in memory.
 
         Args:
             chunk_size (int, optional): Number of files to return in each chunk. Defaults to yielding one event a time.
@@ -240,34 +240,34 @@
             resource_cls=FileMetadata,
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
     def list(
         self,
-        name: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        source_created_time: Union[Dict[str, Any], TimestampRange] = None,
-        source_modified_time: Union[Dict[str, Any], TimestampRange] = None,
-        uploaded_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        directory_prefix: str = None,
-        uploaded: bool = None,
+        name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        source_created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        source_modified_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        uploaded_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        directory_prefix: Optional[str] = None,
+        uploaded: Optional[bool] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> FileMetadataList:
         """`List files <https://developer.cognite.com/api#tag/Files/operation/advancedListFiles>`_
 
         Args:
             name (str): Name of the file.
             mime_type (str): File type. E.g. text/plain, application/pdf, ..
@@ -357,15 +357,15 @@
             data_set_ids=data_set_ids_processed,
         ).dump(camel_case=True)
 
         return self._list(
             list_cls=FileMetadataList, resource_cls=FileMetadata, method="POST", limit=limit, filter=filter
         )
 
-    def aggregate(self, filter: Union[FileMetadataFilter, Dict] = None) -> List[FileAggregate]:
+    def aggregate(self, filter: Optional[Union[FileMetadataFilter, Dict]] = None) -> List[FileAggregate]:
         """`Aggregate files <https://developer.cognite.com/api#tag/Files/operation/aggregateFiles>`_
 
         Args:
             filter (Union[FileMetadataFilter, Dict]): Filter on file metadata filter with exact match
 
         Returns:
             List[FileAggregate]: List of file aggregates
@@ -377,15 +377,17 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> aggregate_uploaded = c.files.aggregate(filter={"uploaded": True})
         """
 
         return self._aggregate(filter=filter, cls=FileAggregate)
 
-    def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete(
+        self, id: Optional[Union[int, Sequence[int]]] = None, external_id: Optional[Union[str, Sequence[str]]] = None
+    ) -> None:
         """`Delete files <https://developer.cognite.com/api#tag/Files/operation/deleteFiles>`_
 
         Args:
             id (Union[int, Sequence[int]]): Id or list of ids
             external_id (Union[str, Sequence[str]]): str or list of str
 
         Returns:
@@ -460,15 +462,15 @@
             resource_cls=FileMetadata,
             update_cls=FileMetadataUpdate,
             resource_path=self._RESOURCE_PATH,
             items=item,
         )
 
     def search(
-        self, name: str = None, filter: Optional[Union[FileMetadataFilter, dict]] = None, limit: int = 100
+        self, name: Optional[str] = None, filter: Optional[Union[FileMetadataFilter, dict]] = None, limit: int = 100
     ) -> FileMetadataList:
         """`Search for files. <https://developer.cognite.com/api#tag/Files/operation/searchFiles>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
             filter (Union[FileMetadataFilter, dict], optional): Filter to apply. Performs exact match on these fields.
@@ -493,27 +495,27 @@
                 >>> res = c.assets.search(name="xyz",filter=FileMetadataFilter(labels=my_label_filter))
         """
         return self._search(list_cls=FileMetadataList, search={"name": name}, filter=filter or {}, limit=limit)
 
     def upload(
         self,
         path: str,
-        external_id: str = None,
-        name: str = None,
-        source: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        directory: str = None,
-        asset_ids: Sequence[int] = None,
-        source_created_time: int = None,
-        source_modified_time: int = None,
-        data_set_id: int = None,
-        labels: Sequence[Label] = None,
-        geo_location: GeoLocation = None,
-        security_categories: Sequence[int] = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        source: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        directory: Optional[str] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        source_created_time: Optional[int] = None,
+        source_modified_time: Optional[int] = None,
+        data_set_id: Optional[int] = None,
+        labels: Optional[Sequence[Label]] = None,
+        geo_location: Optional[GeoLocation] = None,
+        security_categories: Optional[Sequence[int]] = None,
         recursive: bool = False,
         overwrite: bool = False,
     ) -> Union[FileMetadata, FileMetadataList]:
         """`Upload a file <https://developer.cognite.com/api#tag/Files/operation/initFileUpload>`_
 
         Args:
             path (str): Path to the file you wish to upload. If path is a directory, this method will upload all files in that directory.
@@ -626,26 +628,26 @@
             file_metadata = self.upload_bytes(fh, overwrite=overwrite, **file.dump())
         return file_metadata
 
     def upload_bytes(
         self,
         content: Union[str, bytes, TextIO, BinaryIO],
         name: str,
-        external_id: str = None,
-        source: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        directory: str = None,
-        asset_ids: Sequence[int] = None,
-        data_set_id: int = None,
-        labels: Sequence[Label] = None,
-        geo_location: GeoLocation = None,
-        source_created_time: int = None,
-        source_modified_time: int = None,
-        security_categories: Sequence[int] = None,
+        external_id: Optional[str] = None,
+        source: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        directory: Optional[str] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        data_set_id: Optional[int] = None,
+        labels: Optional[Sequence[Label]] = None,
+        geo_location: Optional[GeoLocation] = None,
+        source_created_time: Optional[int] = None,
+        source_modified_time: Optional[int] = None,
+        security_categories: Optional[Sequence[int]] = None,
         overwrite: bool = False,
     ) -> FileMetadata:
         """Upload bytes or string.
 
         You can also pass a file handle to content.
 
         Args:
@@ -705,16 +707,16 @@
         self._http_client_with_retry.request(
             "PUT", upload_url, data=content, timeout=self._config.file_transfer_timeout, headers=headers
         )
         return FileMetadata._load(returned_file_metadata)
 
     def retrieve_download_urls(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         extended_expiration: bool = False,
     ) -> Dict[Union[int, str], str]:
         """Get download links by id or external id
 
         Args:
             id (Union[int, Sequence[int]]): Id or list of ids.
             external_id (Union[str, Sequence[str]]): External id or list of external ids.
@@ -736,16 +738,16 @@
         tasks_summary.raise_compound_exception_if_failed_tasks()
         results = tasks_summary.joined_results(unwrap_fn=lambda res: res.json()["items"])
         return {result.get("id") or result["externalId"]: result["downloadUrl"] for result in results}
 
     def download(
         self,
         directory: Union[str, Path],
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
     ) -> None:
         """`Download files by id or external id. <https://developer.cognite.com/api#tag/Files/operation/downloadLinks>`_
 
         This method will stream all files to disk, never keeping more than 2MB in memory per worker.
         The files will be stored in the provided directory using the name retrieved from the file metadata in CDF.
 
 
@@ -827,15 +829,17 @@
         ) as r:
             r = cast("Response", r)
             with path.open("wb") as f:
                 for chunk in r.iter_content(chunk_size=chunk_size):
                     if chunk:  # filter out keep-alive new chunks
                         f.write(chunk)
 
-    def download_to_path(self, path: Union[Path, str], id: int = None, external_id: str = None) -> None:
+    def download_to_path(
+        self, path: Union[Path, str], id: Optional[int] = None, external_id: Optional[str] = None
+    ) -> None:
         """Download a file to a specific target.
 
         Args:
             path (str): The path in which to place the file.
             id (int): Id of of the file to download.
             external_id (str): External id of the file to download.
 
@@ -852,15 +856,15 @@
         if isinstance(path, str):
             path = Path(path)
         assert path.parent.is_dir(), f"{path.parent} is not a directory"
         identifier = Identifier.of_either(id, external_id).as_dict()
         download_link = self._get_download_link(identifier)
         self._download_file_to_path(download_link, path)
 
-    def download_bytes(self, id: int = None, external_id: str = None) -> bytes:
+    def download_bytes(self, id: Optional[int] = None, external_id: Optional[str] = None) -> bytes:
         """Download a file as bytes.
 
         Args:
             id (int, optional): Id of the file
             external_id (str, optional): External id of the file
 
         Examples:
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/functions.py` & `cognite_sdk-6.8.5/cognite/client/_api/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,17 @@
         if index_url:
             function["indexUrl"] = index_url
 
         body = {"items": [function]}
         res = self._post(url, json=body)
         return Function._load(res.json()["items"][0], cognite_client=self._cognite_client)
 
-    def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete(
+        self, id: Optional[Union[int, Sequence[int]]] = None, external_id: Optional[Union[str, Sequence[str]]] = None
+    ) -> None:
         """`Delete one or more functions. <https://developer.cognite.com/api#tag/Functions/operation/deleteFunctions>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids.
             external_id (Union[str, Sequence[str]]): External ID or list of external ids.
 
         Returns:
@@ -235,20 +237,20 @@
                 >>> c = CogniteClient()
                 >>> c.functions.delete(id=[1,2,3], external_id="function3")
         """
         self._delete_multiple(identifiers=IdentifierSequence.load(ids=id, external_ids=external_id), wrap_ids=True)
 
     def list(
         self,
-        name: str = None,
-        owner: str = None,
-        file_id: int = None,
-        status: str = None,
-        external_id_prefix: str = None,
-        created_time: Union[Dict[str, int], TimestampRange] = None,
+        name: Optional[str] = None,
+        owner: Optional[str] = None,
+        file_id: Optional[int] = None,
+        status: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> FunctionList:
         """`List all functions. <https://developer.cognite.com/api#tag/Functions/operation/listFunctions>`_
 
         Args:
             name (str): The name of the function.
             owner (str): Owner of the function.
@@ -856,19 +858,19 @@
         """
         return self._retrieve_multiple(
             identifiers=IdentifierSequence.load(ids=id), resource_cls=FunctionSchedule, list_cls=FunctionSchedulesList
         )
 
     def list(
         self,
-        name: str = None,
-        function_id: int = None,
-        function_external_id: str = None,
-        created_time: Union[Dict[str, int], TimestampRange] = None,
-        cron_expression: str = None,
+        name: Optional[str] = None,
+        function_id: Optional[int] = None,
+        function_external_id: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
+        cron_expression: Optional[str] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> FunctionSchedulesList:
         """`List all schedules associated with a specific project. <https://developer.cognite.com/api#tag/Function-schedules/operation/listFunctionSchedules>`_
 
         Args:
             name (str): Name of the function schedule.
             function_id (int): ID of the function the schedules are linked to.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/geospatial.py` & `cognite_sdk-6.8.5/cognite/client/_api/geospatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,34 +292,34 @@
 
     @overload
     def create_features(
         self,
         feature_type_external_id: str,
         feature: Feature,
         allow_crs_transformation: bool = False,
-        chunk_size: int = None,
+        chunk_size: Optional[int] = None,
     ) -> Feature:
         ...
 
     @overload
     def create_features(
         self,
         feature_type_external_id: str,
         feature: Union[Sequence[Feature], FeatureList],
         allow_crs_transformation: bool = False,
-        chunk_size: int = None,
+        chunk_size: Optional[int] = None,
     ) -> FeatureList:
         ...
 
     def create_features(
         self,
         feature_type_external_id: str,
         feature: Union[Feature, Sequence[Feature], FeatureList],
         allow_crs_transformation: bool = False,
-        chunk_size: int = None,
+        chunk_size: Optional[int] = None,
     ) -> Union[Feature, FeatureList]:
         """`Creates features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/createFeatures>
 
         Args:
             feature_type_external_id: Feature type definition for the features to create.
             feature: one feature or a list of features to create or a FeatureList object
@@ -368,15 +368,17 @@
             resource_cls=Feature,
             items=feature,
             resource_path=resource_path,
             extra_body_fields=extra_body_fields,
             limit=chunk_size,
         )
 
-    def delete_features(self, feature_type_external_id: str, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete_features(
+        self, feature_type_external_id: str, external_id: Optional[Union[str, Sequence[str]]] = None
+    ) -> None:
         """`Delete one or more feature`
         <https://developer.cognite.com/api#tag/Geospatial/operation/deleteFeatures>
 
         Args:
             feature_type_external_id : Feature type external id for the features to delete.
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
 
@@ -400,32 +402,32 @@
         )
 
     @overload
     def retrieve_features(
         self,
         feature_type_external_id: str,
         external_id: str,
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
     ) -> Feature:
         ...
 
     @overload
     def retrieve_features(
         self,
         feature_type_external_id: str,
         external_id: List[str],
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
     ) -> FeatureList:
         ...
 
     def retrieve_features(
         self,
         feature_type_external_id: str,
         external_id: Union[str, List[str]],
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
     ) -> Union[FeatureList, Feature]:
         """`Retrieve features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/getFeaturesByIds>
 
         Args:
             feature_type_external_id : Feature type external id for the features to retrieve.
             external_id (Union[str, List[str]]): External ID or list of external ids
@@ -456,15 +458,15 @@
         )
 
     def update_features(
         self,
         feature_type_external_id: str,
         feature: Union[Feature, Sequence[Feature]],
         allow_crs_transformation: bool = False,
-        chunk_size: int = None,
+        chunk_size: Optional[int] = None,
     ) -> FeatureList:
         """`Update features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/updateFeatures>
 
         Args:
             feature_type_external_id : Feature type definition for the features to update.
             feature (Union[Feature, Sequence[Feature]]): feature or list of features.
@@ -512,15 +514,15 @@
             ),
         )
 
     def list_features(
         self,
         feature_type_external_id: str,
         filter: Optional[Dict[str, Any]] = None,
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
         limit: int = 100,
         allow_crs_transformation: bool = False,
     ) -> FeatureList:
         """`List features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/listFeatures>
 
         This method allows to filter all features.
@@ -594,17 +596,17 @@
             },
         )
 
     def search_features(
         self,
         feature_type_external_id: str,
         filter: Optional[Dict[str, Any]] = None,
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
         limit: int = 100,
-        order_by: Sequence[OrderSpec] = None,
+        order_by: Optional[Sequence[OrderSpec]] = None,
         allow_crs_transformation: bool = False,
     ) -> FeatureList:
         """`Search for features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/searchFeatures>
 
         This method allows to order the result by one or more of the properties of the feature type.
         However, the number of items returned is  limited to 1000 and there is no support for cursors yet.
@@ -715,15 +717,15 @@
         )
         return cls._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def stream_features(
         self,
         feature_type_external_id: str,
         filter: Optional[Dict[str, Any]] = None,
-        properties: Dict[str, Any] = None,
+        properties: Optional[Dict[str, Any]] = None,
         allow_crs_transformation: bool = False,
     ) -> Generator[Feature, None, None]:
         """`Stream features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/searchFeaturesStreaming>
 
         This method allows to return any number of items until the underlying
         api calls times out. The order of the result items is not deterministic.
@@ -781,20 +783,20 @@
                 yield Feature._load(complexjson.loads(line))
         except (ChunkedEncodingError, ConnectionError) as e:
             raise CogniteConnectionError(e)
 
     def aggregate_features(
         self,
         feature_type_external_id: str,
-        property: str = None,
-        aggregates: Sequence[str] = None,
+        property: Optional[str] = None,
+        aggregates: Optional[Sequence[str]] = None,
         filter: Optional[Dict[str, Any]] = None,
-        group_by: Sequence[str] = None,
-        order_by: Sequence[OrderSpec] = None,
-        output: Dict[str, Any] = None,
+        group_by: Optional[Sequence[str]] = None,
+        order_by: Optional[Sequence[OrderSpec]] = None,
+        output: Optional[Dict[str, Any]] = None,
     ) -> FeatureAggregateList:
         """`Aggregate filtered features`
         <https://developer.cognite.com/api#tag/Geospatial/operation/aggregateFeatures>
 
         Args:
             feature_type_external_id: the feature type to filter features from
             filter (Dict[str, Any]): the search filter
@@ -1091,15 +1093,15 @@
 
     def get_raster(
         self,
         feature_type_external_id: str,
         feature_external_id: str,
         raster_property_name: str,
         raster_format: str,
-        raster_options: Dict[str, Any] = None,
+        raster_options: Optional[Dict[str, Any]] = None,
         raster_srid: Optional[int] = None,
         raster_scale_x: Optional[float] = None,
         raster_scale_y: Optional[float] = None,
         allow_crs_transformation: bool = False,
     ) -> bytes:
         """`Get raster <https://developer.cognite.com/api#tag/Geospatial/operation/getRaster>`
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/iam.py` & `cognite_sdk-6.8.5/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/labels.py` & `cognite_sdk-6.8.5/cognite/client/_api/labels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Iterator, Sequence, Union, cast
+from typing import Iterator, Optional, Sequence, Union, cast
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import LIST_LIMIT_DEFAULT
 from cognite.client.data_classes import LabelDefinition, LabelDefinitionFilter, LabelDefinitionList
 from cognite.client.utils._identifier import IdentifierSequence
 from cognite.client.utils._validation import process_data_set_ids
 
@@ -20,20 +20,20 @@
         Yields:
             LabelDefinition: yields Labels one by one.
         """
         return cast(Iterator[LabelDefinition], self())
 
     def __call__(
         self,
-        name: str = None,
-        external_id_prefix: str = None,
-        limit: int = None,
-        chunk_size: int = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        limit: Optional[int] = None,
+        chunk_size: Optional[int] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
     ) -> Union[Iterator[LabelDefinition], Iterator[LabelDefinitionList]]:
         data_set_ids_processed = process_data_set_ids(data_set_ids, data_set_external_ids)
 
         filter = LabelDefinitionFilter(
             name=name, external_id_prefix=external_id_prefix, data_set_ids=data_set_ids_processed
         ).dump(camel_case=True)
         return self._list_generator(
@@ -43,18 +43,18 @@
             limit=limit,
             filter=filter,
             chunk_size=chunk_size,
         )
 
     def list(
         self,
-        name: str = None,
-        external_id_prefix: str = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> LabelDefinitionList:
         """`List Labels <https://developer.cognite.com/api#tag/Labels/operation/listLabels>`_
 
         Args:
             name (str): returns the label definitions matching that name
             data_set_ids (Union[int, Sequence[int]]): return only labels in the data sets with this id / these ids.
@@ -120,15 +120,15 @@
         if isinstance(label, Sequence):
             if len(label) > 0 and not isinstance(label[0], LabelDefinition):
                 raise TypeError("'label' must be of type LabelDefinition or Sequence[LabelDefinition]")
         elif not isinstance(label, LabelDefinition):
             raise TypeError("'label' must be of type LabelDefinition or Sequence[LabelDefinition]")
         return self._create_multiple(list_cls=LabelDefinitionList, resource_cls=LabelDefinition, items=label)
 
-    def delete(self, external_id: Union[str, Sequence[str]] = None) -> None:
+    def delete(self, external_id: Optional[Union[str, Sequence[str]]] = None) -> None:
         """`Delete one or more label definitions <https://developer.cognite.com/api#tag/Labels/operation/deleteLabels>`_
 
         Args:
             external_id (Union[str, Sequence[str]]): One or more label external ids
 
         Returns:
             None
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/raw.py` & `cognite_sdk-6.8.5/cognite/client/_api/raw.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
         self.tables = RawTablesAPI(config, api_version, cognite_client)
         self.rows = RawRowsAPI(config, api_version, cognite_client)
 
 
 class RawDatabasesAPI(APIClient):
     _RESOURCE_PATH = "/raw/dbs"
 
-    def __call__(self, chunk_size: int = None, limit: int = None) -> Union[Iterator[Database], Iterator[DatabaseList]]:
+    def __call__(
+        self, chunk_size: Optional[int] = None, limit: Optional[int] = None
+    ) -> Union[Iterator[Database], Iterator[DatabaseList]]:
         """Iterate over databases
 
         Fetches dbs as they are iterated over, so you keep a limited number of dbs in memory.
 
         Args:
             chunk_size (int, optional): Number of dbs to return in each chunk. Defaults to yielding one db a time.
             limit (int, optional): Maximum number of dbs to return. Defaults to return all items.
@@ -142,15 +144,15 @@
         return self._list(list_cls=DatabaseList, resource_cls=Database, method="GET", limit=limit)
 
 
 class RawTablesAPI(APIClient):
     _RESOURCE_PATH = "/raw/dbs/{}/tables"
 
     def __call__(
-        self, db_name: str, chunk_size: int = None, limit: int = None
+        self, db_name: str, chunk_size: Optional[int] = None, limit: Optional[int] = None
     ) -> Union[Iterator[Table], Iterator[TableList]]:
         """Iterate over tables
 
         Fetches tables as they are iterated over, so you keep a limited number of tables in memory.
 
         Args:
             db_name (str): Name of the database to iterate over tables for
@@ -302,19 +304,19 @@
         self._CREATE_LIMIT = 5000
         self._LIST_LIMIT = 10000
 
     def __call__(
         self,
         db_name: str,
         table_name: str,
-        chunk_size: int = None,
-        limit: int = None,
-        min_last_updated_time: int = None,
-        max_last_updated_time: int = None,
-        columns: List[str] = None,
+        chunk_size: Optional[int] = None,
+        limit: Optional[int] = None,
+        min_last_updated_time: Optional[int] = None,
+        max_last_updated_time: Optional[int] = None,
+        columns: Optional[List[str]] = None,
     ) -> Union[Iterator[Row], Iterator[RowList]]:
         """Iterate over rows.
 
         Fetches rows as they are iterated over, so you keep a limited number of rows in memory.
 
         Args:
             db_name (str): Name of the database
@@ -487,17 +489,17 @@
             identifier=Identifier(key),
         )
 
     def list(
         self,
         db_name: str,
         table_name: str,
-        min_last_updated_time: int = None,
-        max_last_updated_time: int = None,
-        columns: List[str] = None,
+        min_last_updated_time: Optional[int] = None,
+        max_last_updated_time: Optional[int] = None,
+        columns: Optional[List[str]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> RowList:
         """`List rows in a table. <https://developer.cognite.com/api#tag/Raw/operation/getRows>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
@@ -575,17 +577,17 @@
         else:
             return ",".join([str(x) for x in columns])
 
     def retrieve_dataframe(
         self,
         db_name: str,
         table_name: str,
-        min_last_updated_time: int = None,
-        max_last_updated_time: int = None,
-        columns: List[str] = None,
+        min_last_updated_time: Optional[int] = None,
+        max_last_updated_time: Optional[int] = None,
+        columns: Optional[List[str]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> pandas.DataFrame:
         """`Retrieve rows in a table as a pandas dataframe. <https://developer.cognite.com/api#tag/Raw/operation/getRows>`_
 
         Rowkeys are used as the index.
 
         Args:
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/relationships.py` & `cognite_sdk-6.8.5/cognite/client/_api/relationships.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._LIST_SUBQUERY_LIMIT = 1000
 
     def _create_filter(
         self,
-        source_external_ids: Sequence[str] = None,
-        source_types: Sequence[str] = None,
-        target_external_ids: Sequence[str] = None,
-        target_types: Sequence[str] = None,
-        data_set_ids: Sequence[Dict[str, Any]] = None,
-        start_time: Dict[str, int] = None,
-        end_time: Dict[str, int] = None,
-        confidence: Dict[str, int] = None,
-        last_updated_time: Dict[str, int] = None,
-        created_time: Dict[str, int] = None,
-        active_at_time: Dict[str, int] = None,
-        labels: LabelFilter = None,
+        source_external_ids: Optional[Sequence[str]] = None,
+        source_types: Optional[Sequence[str]] = None,
+        target_external_ids: Optional[Sequence[str]] = None,
+        target_types: Optional[Sequence[str]] = None,
+        data_set_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        start_time: Optional[Dict[str, int]] = None,
+        end_time: Optional[Dict[str, int]] = None,
+        confidence: Optional[Dict[str, int]] = None,
+        last_updated_time: Optional[Dict[str, int]] = None,
+        created_time: Optional[Dict[str, int]] = None,
+        active_at_time: Optional[Dict[str, int]] = None,
+        labels: Optional[LabelFilter] = None,
     ) -> Dict[str, Any]:
         return RelationshipFilter(
             source_external_ids=source_external_ids,
             source_types=source_types,
             target_external_ids=target_external_ids,
             target_types=target_types,
             data_set_ids=data_set_ids,
@@ -51,31 +51,31 @@
             created_time=created_time,
             active_at_time=active_at_time,
             labels=labels,
         ).dump(camel_case=True)
 
     def __call__(
         self,
-        source_external_ids: Sequence[str] = None,
-        source_types: Sequence[str] = None,
-        target_external_ids: Sequence[str] = None,
-        target_types: Sequence[str] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        start_time: Dict[str, int] = None,
-        end_time: Dict[str, int] = None,
-        confidence: Dict[str, int] = None,
-        last_updated_time: Dict[str, int] = None,
-        created_time: Dict[str, int] = None,
-        active_at_time: Dict[str, int] = None,
-        labels: LabelFilter = None,
-        limit: int = None,
+        source_external_ids: Optional[Sequence[str]] = None,
+        source_types: Optional[Sequence[str]] = None,
+        target_external_ids: Optional[Sequence[str]] = None,
+        target_types: Optional[Sequence[str]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        start_time: Optional[Dict[str, int]] = None,
+        end_time: Optional[Dict[str, int]] = None,
+        confidence: Optional[Dict[str, int]] = None,
+        last_updated_time: Optional[Dict[str, int]] = None,
+        created_time: Optional[Dict[str, int]] = None,
+        active_at_time: Optional[Dict[str, int]] = None,
+        labels: Optional[LabelFilter] = None,
+        limit: Optional[int] = None,
         fetch_resources: bool = False,
-        chunk_size: int = None,
-        partitions: int = None,
+        chunk_size: Optional[int] = None,
+        partitions: Optional[int] = None,
     ) -> Union[Iterator[Relationship], Iterator[RelationshipList]]:
         """Iterate over relationships
 
         Fetches relationships as they are iterated over, so you keep a limited number of relationships in memory.
 
         Args:
             source_external_ids (Sequence[str]): Include relationships that have any of these values in their source External Id field
@@ -195,29 +195,29 @@
             resource_cls=Relationship,
             identifiers=identifiers,
             other_params={"fetchResources": fetch_resources},
         )
 
     def list(
         self,
-        source_external_ids: Sequence[str] = None,
-        source_types: Sequence[str] = None,
-        target_external_ids: Sequence[str] = None,
-        target_types: Sequence[str] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        start_time: Dict[str, int] = None,
-        end_time: Dict[str, int] = None,
-        confidence: Dict[str, int] = None,
-        last_updated_time: Dict[str, int] = None,
-        created_time: Dict[str, int] = None,
-        active_at_time: Dict[str, int] = None,
-        labels: LabelFilter = None,
+        source_external_ids: Optional[Sequence[str]] = None,
+        source_types: Optional[Sequence[str]] = None,
+        target_external_ids: Optional[Sequence[str]] = None,
+        target_types: Optional[Sequence[str]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        start_time: Optional[Dict[str, int]] = None,
+        end_time: Optional[Dict[str, int]] = None,
+        confidence: Optional[Dict[str, int]] = None,
+        last_updated_time: Optional[Dict[str, int]] = None,
+        created_time: Optional[Dict[str, int]] = None,
+        active_at_time: Optional[Dict[str, int]] = None,
+        labels: Optional[LabelFilter] = None,
         limit: int = 100,
-        partitions: int = None,
+        partitions: Optional[int] = None,
         fetch_resources: bool = False,
     ) -> RelationshipList:
         """`Lists relationships stored in the project based on a query filter given in the payload of this request. Up to 1000 relationships can be retrieved in one operation.  <https://developer.cognite.com/api#tag/Relationships/operation/listRelationships>`_
 
         Args:
             source_external_ids (Sequence[str]): Include relationships that have any of these values in their source External Id field
             source_types (Sequence[str]): Include relationships that have any of these values in their source Type field
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/sequences.py` & `cognite_sdk-6.8.5/cognite/client/_api/sequences.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,26 +34,26 @@
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.data = SequencesDataAPI(config, api_version, cognite_client)
 
     def __call__(
         self,
-        chunk_size: int = None,
-        name: str = None,
-        external_id_prefix: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: SequenceType[int] = None,
-        asset_subtree_ids: Union[int, SequenceType[int]] = None,
-        asset_subtree_external_ids: Union[str, SequenceType[str]] = None,
-        data_set_ids: Union[int, SequenceType[int]] = None,
-        data_set_external_ids: Union[str, SequenceType[str]] = None,
-        created_time: Dict[str, Any] = None,
-        last_updated_time: Dict[str, Any] = None,
-        limit: int = None,
+        chunk_size: Optional[int] = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[SequenceType[int]] = None,
+        asset_subtree_ids: Optional[Union[int, SequenceType[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, SequenceType[str]]] = None,
+        data_set_ids: Optional[Union[int, SequenceType[int]]] = None,
+        data_set_external_ids: Optional[Union[str, SequenceType[str]]] = None,
+        created_time: Optional[Dict[str, Any]] = None,
+        last_updated_time: Optional[Dict[str, Any]] = None,
+        limit: Optional[int] = None,
     ) -> Union[Iterator[Sequence], Iterator[SequenceList]]:
         """Iterate over sequences
 
         Fetches sequences as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
             chunk_size (int, optional): Number of sequences to return in each chunk. Defaults to yielding one event a time.
@@ -164,24 +164,24 @@
         identifiers = IdentifierSequence.load(ids=ids, external_ids=external_ids)
         return self._retrieve_multiple(
             list_cls=SequenceList, resource_cls=Sequence, identifiers=identifiers, ignore_unknown_ids=ignore_unknown_ids
         )
 
     def list(
         self,
-        name: str = None,
-        external_id_prefix: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: SequenceType[int] = None,
-        asset_subtree_ids: Union[int, SequenceType[int]] = None,
-        asset_subtree_external_ids: Union[str, SequenceType[str]] = None,
-        data_set_ids: Union[int, SequenceType[int]] = None,
-        data_set_external_ids: Union[str, SequenceType[str]] = None,
-        created_time: (Union[Dict[str, Any], TimestampRange]) = None,
-        last_updated_time: (Union[Dict[str, Any], TimestampRange]) = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[SequenceType[int]] = None,
+        asset_subtree_ids: Optional[Union[int, SequenceType[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, SequenceType[str]]] = None,
+        data_set_ids: Optional[Union[int, SequenceType[int]]] = None,
+        data_set_external_ids: Optional[Union[str, SequenceType[str]]] = None,
+        created_time: Optional[(Union[Dict[str, Any], TimestampRange])] = None,
+        last_updated_time: Optional[(Union[Dict[str, Any], TimestampRange])] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> SequenceList:
         """`Iterate over sequences <https://developer.cognite.com/api#tag/Sequences/operation/advancedListSequences>`_
 
         Fetches sequences as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
@@ -234,15 +234,15 @@
             asset_subtree_ids=asset_subtree_ids_processed,
             created_time=created_time,
             last_updated_time=last_updated_time,
             data_set_ids=data_set_ids_processed,
         ).dump(camel_case=True)
         return self._list(list_cls=SequenceList, resource_cls=Sequence, method="POST", filter=filter, limit=limit)
 
-    def aggregate(self, filter: Union[SequenceFilter, Dict] = None) -> List[SequenceAggregate]:
+    def aggregate(self, filter: Optional[Union[SequenceFilter, Dict]] = None) -> List[SequenceAggregate]:
         """`Aggregate sequences <https://developer.cognite.com/api#tag/Sequences/operation/aggregateSequences>`_
 
         Args:
             filter (Union[SequenceFilter, Dict]): Filter on sequence filter with exact match
 
         Returns:
             List[SequenceAggregate]: List of sequence aggregates
@@ -316,15 +316,17 @@
             if not sequence.columns[i].get("externalId"):
                 sequence.columns[i]["externalId"] = "column" + str(i)
             if sequence.columns[i].get("valueType"):
                 sequence.columns[i]["valueType"] = sequence.columns[i]["valueType"].upper()
         return sequence
 
     def delete(
-        self, id: Union[int, SequenceType[int]] = None, external_id: Union[str, SequenceType[str]] = None
+        self,
+        id: Optional[Union[int, SequenceType[int]]] = None,
+        external_id: Optional[Union[str, SequenceType[str]]] = None,
     ) -> None:
         """`Delete one or more sequences. <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequences>`_
 
         Args:
             id (Union[int, SequenceType[int]): Id or list of ids
             external_id (Union[str, SequenceType[str]]): External ID or list of external ids
 
@@ -434,18 +436,18 @@
         """
         return self._update_multiple(
             list_cls=SequenceList, resource_cls=Sequence, update_cls=SequenceUpdate, items=item
         )
 
     def search(
         self,
-        name: str = None,
-        description: str = None,
-        query: str = None,
-        filter: Union[SequenceFilter, Dict] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        query: Optional[str] = None,
+        filter: Optional[Union[SequenceFilter, Dict]] = None,
         limit: int = 100,
     ) -> SequenceList:
         """`Search for sequences. <https://developer.cognite.com/api#tag/Sequences/operation/searchSequences>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
@@ -488,16 +490,16 @@
         rows: Union[
             Dict[int, SequenceType[Union[int, float, str]]],
             SequenceType[Tuple[int, SequenceType[Union[int, float, str]]]],
             SequenceType[Dict[str, Any]],
             SequenceData,
         ],
         column_external_ids: Optional[SequenceType[str]],
-        id: int = None,
-        external_id: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
     ) -> None:
         """`Insert rows into a sequence <https://developer.cognite.com/api#tag/Sequences/operation/postSequenceData>`_
 
         Args:
             column_external_ids (Optional[SequenceType[str]]): List of external id for the columns of the sequence.
             rows (Union[ Dict[int, SequenceType[Union[int, float, str]]], SequenceType[Tuple[int, SequenceType[Union[int, float, str]]]], SequenceType[Dict[str,Any]], SequenceData]):  The rows you wish to insert.
                 Can either be a list of tuples, a list of {"rowNumber":... ,"values": ...} objects, a dictionary of rowNumber: data, or a SequenceData object. See examples below.
@@ -561,15 +563,17 @@
             rows_per_request = self._SEQ_POST_LIMIT_ROWS
 
         row_objs = [{"rows": all_rows[i : i + rows_per_request]} for i in range(0, len(all_rows), rows_per_request)]
         tasks = [({**base_obj, **rows},) for rows in row_objs]  # type: ignore
         summary = utils._concurrency.execute_tasks(self._insert_data, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks()
 
-    def insert_dataframe(self, dataframe: pandas.DataFrame, id: int = None, external_id: str = None) -> None:
+    def insert_dataframe(
+        self, dataframe: pandas.DataFrame, id: Optional[int] = None, external_id: Optional[str] = None
+    ) -> None:
         """`Insert a Pandas dataframe. <https://developer.cognite.com/api#tag/Sequences/operation/postSequenceData>`_
 
         The index of the dataframe must contain the row numbers. The names of the remaining columns specify the column external ids.
         The sequence and columns must already exist.
 
         Args:
             dataframe (pandas.DataFrame):  Pandas DataFrame object containing the sequence data.
@@ -591,15 +595,15 @@
         data = [(v[0], list(v[1:])) for v in dataframe.itertuples()]
         column_external_ids = [str(s) for s in dataframe.columns]
         self.insert(rows=data, column_external_ids=column_external_ids, id=id, external_id=external_id)
 
     def _insert_data(self, task: Dict[str, Any]) -> None:
         self._post(url_path=self._DATA_PATH, json={"items": [task]})
 
-    def delete(self, rows: SequenceType[int], id: int = None, external_id: str = None) -> None:
+    def delete(self, rows: SequenceType[int], id: Optional[int] = None, external_id: Optional[str] = None) -> None:
         """`Delete rows from a sequence <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequenceData>`_
 
         Args:
             rows (SequenceType[int]): List of row numbers.
             id (int): Id of sequence to delete rows from.
             external_id (str): External id of sequence to delete rows from.
 
@@ -613,15 +617,17 @@
                 >>> c.sequences.data.delete(id=0, rows=[1,2,42])
         """
         post_obj = Identifier.of_either(id, external_id).as_dict()
         post_obj["rows"] = rows
 
         self._post(url_path=self._DATA_PATH + "/delete", json={"items": [post_obj]})
 
-    def delete_range(self, start: int, end: Union[int, None], id: int = None, external_id: str = None) -> None:
+    def delete_range(
+        self, start: int, end: Union[int, None], id: Optional[int] = None, external_id: Optional[str] = None
+    ) -> None:
         """`Delete a range of rows from a sequence. Note this operation is potentially slow, as retrieves each row before deleting. <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequenceData>`_
 
         Args:
             start (int): Row number to start from (inclusive).
             end (Union[int, None]): Upper limit on the row number (exclusive).
                 Set to None or -1 to delete all rows until end of sequence.
             id (int): Id of sequence to delete rows from.
@@ -646,17 +652,17 @@
                 self.delete(rows=[r["rowNumber"] for r in data], external_id=external_id, id=id)
 
     def retrieve(
         self,
         start: int,
         end: Union[int, None],
         column_external_ids: Optional[SequenceType[str]] = None,
-        external_id: Union[str, SequenceType[str]] = None,
-        id: Union[int, SequenceType[int]] = None,
-        limit: int = None,
+        external_id: Optional[Union[str, SequenceType[str]]] = None,
+        id: Optional[Union[int, SequenceType[int]]] = None,
+        limit: Optional[int] = None,
     ) -> Union[SequenceData, SequenceDataList]:
         """`Retrieve data from a sequence <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceData>`_
 
         Args:
             start (int): Row number to start from (inclusive).
             end (Union[int, None]): Upper limit on the row number (exclusive). Set to None or -1 to get all rows
                 until end of sequence.
@@ -701,18 +707,18 @@
         if len(post_objs) == 1:
             return results[0]
         else:
             return SequenceDataList(results)
 
     def retrieve_latest(
         self,
-        id: int = None,
-        external_id: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
         column_external_ids: Optional[SequenceType[str]] = None,
-        before: int = None,
+        before: Optional[int] = None,
     ) -> SequenceData:
         """`Retrieves the last row (i.e the row with the highest row number) in a sequence. <https://developer.cognite.com/api#tag/Sequences/operation/getLatestSequenceRow>`_
 
         Args:
             id (optional, int): Id or list of ids.
             external_id (optional, str): External id or list of external ids.
             column_external_ids: (optional, SequenceType[str]): external ids of columns to include. Omitting wil return all columns.
@@ -736,18 +742,18 @@
         return SequenceData(id=res["id"], external_id=res.get("external_id"), rows=res["rows"], columns=res["columns"])
 
     def retrieve_dataframe(
         self,
         start: int,
         end: Union[int, None],
         column_external_ids: Optional[List[str]] = None,
-        external_id: str = None,
-        column_names: str = None,
-        id: int = None,
-        limit: int = None,
+        external_id: Optional[str] = None,
+        column_names: Optional[str] = None,
+        id: Optional[int] = None,
+        limit: Optional[int] = None,
     ) -> pandas.DataFrame:
         """`Retrieve data from a sequence as a pandas dataframe <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceData>`_
 
         Args:
             start (int): (inclusive) row number to start from.
             end (Union[int, None]): (exclusive) upper limit on the row number. Set to None or -1 to get all rows
                 until end of sequence.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.8.5/cognite/client/_api/synthetic_time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
         self._DPS_LIMIT_SYNTH = 10_000
 
     def query(
         self,
         expressions: Union[str, sympy.Expr, Sequence[Union[str, sympy.Expr]]],
         start: Union[int, str, datetime],
         end: Union[int, str, datetime],
-        limit: int = None,
-        variables: Dict[str, Union[str, TimeSeries]] = None,
-        aggregate: str = None,
-        granularity: str = None,
+        limit: Optional[int] = None,
+        variables: Optional[Dict[str, Union[str, TimeSeries]]] = None,
+        aggregate: Optional[str] = None,
+        granularity: Optional[str] = None,
     ) -> Union[Datapoints, DatapointsList]:
         """`Calculate the result of a function on time series. <https://developer.cognite.com/api#tag/Synthetic-Time-Series/operation/querySyntheticTimeseries>`_
 
         Args:
             expressions (Union[str, sympy.Expr, Sequence[Union[str, sympy.Expr]]]): Functions to be calculated. Supports both strings and sympy expressions. Strings can have either the API `ts{}` syntax, or contain variable names to be replaced using the `variables` parameter.
             start (Union[int, str, datetime]): Inclusive start.
             end (Union[int, str, datetime]): Exclusive end
@@ -113,17 +113,17 @@
                 break
             query["start"] = data["datapoints"][-1]["timestamp"] + 1
         return datapoints
 
     @staticmethod
     def _build_expression(
         expression: Union[str, sympy.Expr],
-        variables: Dict[str, Any] = None,
-        aggregate: str = None,
-        granularity: str = None,
+        variables: Optional[Dict[str, Any]] = None,
+        aggregate: Optional[str] = None,
+        granularity: Optional[str] = None,
     ) -> Tuple[str, str]:
         if expression.__class__.__module__.startswith("sympy."):
             expression_str = SyntheticDatapointsAPI._sympy_to_sts(expression)
             if not variables:
                 raise ValueError(
                     "sympy expressions are only supported in combination with the `variables` parameter to map symbols to time series."
                 )
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/templates.py` & `cognite_sdk-6.8.5/cognite/client/_api/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         return self._retrieve_multiple(
             list_cls=TemplateGroupList,
             resource_cls=TemplateGroup,
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
-    def list(self, limit: int = LIST_LIMIT_DEFAULT, owners: Sequence[str] = None) -> TemplateGroupList:
+    def list(self, limit: int = LIST_LIMIT_DEFAULT, owners: Optional[Sequence[str]] = None) -> TemplateGroupList:
         """`Lists template groups stored in the project based on a query filter given in the payload of this request.`
         Up to 1000 template groups can be retrieved in one operation.
 
         Args:
             owners (Sequence[str]): Include template groups that have any of these values in their `owner` field.
             limit (int): Maximum number of template groups to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/three_d.py` & `cognite_sdk-6.8.5/cognite/client/_api/three_d.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.asset_mappings = ThreeDAssetMappingAPI(config, api_version, cognite_client)
 
 
 class ThreeDModelsAPI(APIClient):
     _RESOURCE_PATH = "/3d/models"
 
     def __call__(
-        self, chunk_size: int = None, published: bool = None, limit: int = None
+        self, chunk_size: Optional[int] = None, published: Optional[bool] = None, limit: Optional[int] = None
     ) -> Union[Iterator[ThreeDModel], Iterator[ThreeDModelList]]:
         """Iterate over 3d models
 
         Fetches 3d models as they are iterated over, so you keep a limited number of 3d models in memory.
 
         Args:
             chunk_size (int, optional): Number of 3d models to return in each chunk. Defaults to yielding one model a time.
@@ -85,15 +85,15 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.three_d.models.retrieve(id=1)
         """
         return self._retrieve(cls=ThreeDModel, identifier=InternalId(id))
 
-    def list(self, published: bool = None, limit: int = LIST_LIMIT_DEFAULT) -> ThreeDModelList:
+    def list(self, published: Optional[bool] = None, limit: int = LIST_LIMIT_DEFAULT) -> ThreeDModelList:
         """`List 3d models. <https://developer.cognite.com/api#tag/3D-Models/operation/get3DModels>`_
 
         Args:
             published (bool): Filter based on whether or not the model has published revisions.
             limit (int): Maximum number of models to retrieve. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
@@ -208,15 +208,15 @@
         self._delete_multiple(identifiers=IdentifierSequence.load(ids=id), wrap_ids=True)
 
 
 class ThreeDRevisionsAPI(APIClient):
     _RESOURCE_PATH = "/3d/models/{}/revisions"
 
     def __call__(
-        self, model_id: int, chunk_size: int = None, published: bool = False, limit: int = None
+        self, model_id: int, chunk_size: Optional[int] = None, published: bool = False, limit: Optional[int] = None
     ) -> Union[Iterator[ThreeDModelRevision], Iterator[ThreeDModelRevisionList]]:
         """Iterate over 3d model revisions
 
         Fetches 3d model revisions as they are iterated over, so you keep a limited number of 3d model revisions in memory.
 
         Args:
             model_id (int): Iterate over revisions for the model with this id.
@@ -414,18 +414,18 @@
         body = {"fileId": file_id}
         self._post(resource_path, json=body)
 
     def list_nodes(
         self,
         model_id: int,
         revision_id: int,
-        node_id: int = None,
-        depth: int = None,
+        node_id: Optional[int] = None,
+        depth: Optional[int] = None,
         sort_by_node_id: bool = False,
-        partitions: int = None,
+        partitions: Optional[int] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ThreeDNodeList:
         """`Retrieves a list of nodes from the hierarchy in the 3D Model. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DNodes>`_
 
         You can also request a specific subtree with the 'nodeId' query parameter and limit the depth of
         the resulting subtree with the 'depth' query parameter.
 
@@ -464,17 +464,17 @@
             other_params={"sortByNodeId": sort_by_node_id},
         )
 
     def filter_nodes(
         self,
         model_id: int,
         revision_id: int,
-        properties: Dict[str, Dict[str, Sequence[str]]] = None,
+        properties: Optional[Dict[str, Dict[str, Sequence[str]]]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
-        partitions: int = None,
+        partitions: Optional[int] = None,
     ) -> ThreeDNodeList:
         """`List nodes in a revision, filtered by node property values. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/filter3DNodes>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             properties (Dict[str, Dict[str, Sequence[str]]]): Properties for filtering. The object contains one or more category. Each category references one or more properties. Each property is associated with a list of values. For a node to satisfy the filter, it must, for each category/property in the filter, contain the catogery+property combination with a value that is contained within the corresponding list in the filter.
@@ -503,15 +503,15 @@
             method="POST",
             limit=limit,
             filter={"properties": properties},
             partitions=partitions,
         )
 
     def list_ancestor_nodes(
-        self, model_id: int, revision_id: int, node_id: int = None, limit: int = LIST_LIMIT_DEFAULT
+        self, model_id: int, revision_id: int, node_id: Optional[int] = None, limit: int = LIST_LIMIT_DEFAULT
     ) -> ThreeDNodeList:
         """`Retrieves a list of ancestor nodes of a given node, including itself, in the hierarchy of the 3D model <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DNodeAncestors>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             node_id (int): ID of the node to get the ancestors of.
@@ -569,16 +569,16 @@
 class ThreeDAssetMappingAPI(APIClient):
     _RESOURCE_PATH = "/3d/models/{}/revisions/{}/mappings"
 
     def list(
         self,
         model_id: int,
         revision_id: int,
-        node_id: int = None,
-        asset_id: int = None,
+        node_id: Optional[int] = None,
+        asset_id: Optional[int] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ThreeDAssetMappingList:
         """`List 3D node asset mappings. <https://developer.cognite.com/api#tag/3D-Asset-Mapping/operation/get3DMappings>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/time_series.py` & `cognite_sdk-6.8.5/cognite/client/_api/time_series.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,31 +25,31 @@
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.data = DatapointsAPI(config, api_version, cognite_client)
 
     def __call__(
         self,
-        chunk_size: int = None,
-        name: str = None,
-        unit: str = None,
-        is_string: bool = None,
-        is_step: bool = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        metadata: Dict[str, Any] = None,
-        external_id_prefix: str = None,
-        created_time: Dict[str, Any] = None,
-        last_updated_time: Dict[str, Any] = None,
-        limit: int = None,
-        partitions: int = None,
+        chunk_size: Optional[int] = None,
+        name: Optional[str] = None,
+        unit: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        is_step: Optional[bool] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        external_id_prefix: Optional[str] = None,
+        created_time: Optional[Dict[str, Any]] = None,
+        last_updated_time: Optional[Dict[str, Any]] = None,
+        limit: Optional[int] = None,
+        partitions: Optional[int] = None,
     ) -> Union[Iterator[TimeSeries], Iterator[TimeSeriesList]]:
         """Iterate over time series
 
         Fetches time series as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
             chunk_size (int, optional): Number of time series to return in each chunk. Defaults to yielding one time series a time.
@@ -173,29 +173,29 @@
             resource_cls=TimeSeries,
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
     def list(
         self,
-        name: str = None,
-        unit: str = None,
-        is_string: bool = None,
-        is_step: bool = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Union[int, Sequence[int]] = None,
-        asset_subtree_external_ids: Union[str, Sequence[str]] = None,
-        data_set_ids: Union[int, Sequence[int]] = None,
-        data_set_external_ids: Union[str, Sequence[str]] = None,
-        metadata: Dict[str, Any] = None,
-        external_id_prefix: str = None,
-        created_time: Dict[str, Any] = None,
-        last_updated_time: Dict[str, Any] = None,
-        partitions: int = None,
+        name: Optional[str] = None,
+        unit: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        is_step: Optional[bool] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Union[int, Sequence[int]]] = None,
+        asset_subtree_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        data_set_ids: Optional[Union[int, Sequence[int]]] = None,
+        data_set_external_ids: Optional[Union[str, Sequence[str]]] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        external_id_prefix: Optional[str] = None,
+        created_time: Optional[Dict[str, Any]] = None,
+        last_updated_time: Optional[Dict[str, Any]] = None,
+        partitions: Optional[int] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> TimeSeriesList:
         """`List over time series <https://developer.cognite.com/api#tag/Time-series/operation/listTimeSeries>`_
 
         Fetches time series as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
@@ -264,15 +264,15 @@
             resource_cls=TimeSeries,
             method="POST",
             filter=filter,
             limit=limit,
             partitions=partitions,
         )
 
-    def aggregate(self, filter: Union[TimeSeriesFilter, Dict] = None) -> List[TimeSeriesAggregate]:
+    def aggregate(self, filter: Optional[Union[TimeSeriesFilter, Dict]] = None) -> List[TimeSeriesAggregate]:
         """`Aggregate time series <https://developer.cognite.com/api#tag/Time-series/operation/aggregateTimeSeries>`_
 
         Args:
             filter (Union[TimeSeriesFilter, Dict]): Filter on time series filter with exact match
 
         Returns:
             List[TimeSeriesAggregate]: List of sequence aggregates
@@ -314,16 +314,16 @@
                 >>> c = CogniteClient()
                 >>> ts = c.time_series.create(TimeSeries(name="my ts"))
         """
         return self._create_multiple(list_cls=TimeSeriesList, resource_cls=TimeSeries, items=time_series)
 
     def delete(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
         """`Delete one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/deleteTimeSeries>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
@@ -385,18 +385,18 @@
         """
         return self._update_multiple(
             list_cls=TimeSeriesList, resource_cls=TimeSeries, update_cls=TimeSeriesUpdate, items=item
         )
 
     def search(
         self,
-        name: str = None,
-        description: str = None,
-        query: str = None,
-        filter: Union[TimeSeriesFilter, Dict] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        query: Optional[str] = None,
+        filter: Optional[Union[TimeSeriesFilter, Dict]] = None,
         limit: int = 100,
     ) -> TimeSeriesList:
         """`Search for time series. <https://developer.cognite.com/api#tag/Time-series/operation/searchTimeSeries>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.8.5/cognite/client/_api/transformations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         else:
             raise TypeError("transformation must be Sequence[Transformation] or Transformation")
 
         return self._create_multiple(list_cls=TransformationList, resource_cls=Transformation, items=transformation)
 
     def delete(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
         """`Delete one or more transformations. <https://developer.cognite.com/api#tag/Transformations/operation/deleteTransformations>`_
 
         Args:
             id (Union[int, List[int]): Id or list of ids.
             external_id (Union[str, List[str]]): External ID or list of external ids.
@@ -143,24 +143,24 @@
             wrap_ids=True,
             extra_body_fields={"ignoreUnknownIds": ignore_unknown_ids},
         )
 
     def list(
         self,
         include_public: bool = True,
-        name_regex: str = None,
-        query_regex: str = None,
-        destination_type: str = None,
-        conflict_mode: str = None,
-        cdf_project_name: str = None,
-        has_blocked_error: bool = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        data_set_ids: List[int] = None,
-        data_set_external_ids: List[str] = None,
+        name_regex: Optional[str] = None,
+        query_regex: Optional[str] = None,
+        destination_type: Optional[str] = None,
+        conflict_mode: Optional[str] = None,
+        cdf_project_name: Optional[str] = None,
+        has_blocked_error: Optional[bool] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        data_set_ids: Optional[List[int]] = None,
+        data_set_external_ids: Optional[List[str]] = None,
         tags: Optional[TagsFilter] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> TransformationList:
         """`List all transformations. <https://developer.cognite.com/api#tag/Transformations/operation/getTransformations>`_
 
         Args:
             include_public (bool): Whether public transformations should be included in the results. (default true).
@@ -245,15 +245,18 @@
         return self._retrieve_multiple(
             list_cls=TransformationList,
             resource_cls=Transformation,
             identifiers=identifiers,
         )
 
     def retrieve_multiple(
-        self, ids: Sequence[int] = None, external_ids: Sequence[str] = None, ignore_unknown_ids: bool = False
+        self,
+        ids: Optional[Sequence[int]] = None,
+        external_ids: Optional[Sequence[str]] = None,
+        ignore_unknown_ids: bool = False,
     ) -> TransformationList:
         """`Retrieve multiple transformations. <https://developer.cognite.com/api#tag/Transformations/operation/getTransformationsByIds>`_
 
         Args:
             ids (List[int]): List of ids to retrieve.
             external_ids (List[str]): List of external ids to retrieve.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
@@ -327,16 +330,16 @@
 
         return self._update_multiple(
             list_cls=TransformationList, resource_cls=Transformation, update_cls=TransformationUpdate, items=item
         )
 
     def run(
         self,
-        transformation_id: int = None,
-        transformation_external_id: str = None,
+        transformation_id: Optional[int] = None,
+        transformation_external_id: Optional[str] = None,
         wait: bool = True,
         timeout: Optional[float] = None,
     ) -> TransformationJob:
         """`Run a transformation. <https://developer.cognite.com/api#tag/Transformations/operation/runTransformation>`_
 
         Args:
             transformation_id (int): Transformation internal id
@@ -372,15 +375,18 @@
 
         if wait:
             return job.wait(timeout=timeout)
 
         return job
 
     async def run_async(
-        self, transformation_id: int = None, transformation_external_id: str = None, timeout: Optional[float] = None
+        self,
+        transformation_id: Optional[int] = None,
+        transformation_external_id: Optional[str] = None,
+        timeout: Optional[float] = None,
     ) -> TransformationJob:
         """`Run a transformation to completion asynchronously. <https://developer.cognite.com/api#tag/Transformations/operation/runTransformation>`_
 
         Args:
             transformation_id (int): internal Transformation id
             transformation_external_id (str): external Transformation id
             timeout (Optional[float]): maximum time (s) to wait, default is None (infinite time). Once the timeout is reached, it returns with the current status.
@@ -406,15 +412,15 @@
         """
 
         job = self.run(
             transformation_id=transformation_id, transformation_external_id=transformation_external_id, wait=False
         )
         return await job.wait_async(timeout=timeout)
 
-    def cancel(self, transformation_id: int = None, transformation_external_id: str = None) -> None:
+    def cancel(self, transformation_id: Optional[int] = None, transformation_external_id: Optional[str] = None) -> None:
         """`Cancel a running transformation. <https://developer.cognite.com/api#tag/Transformations/operation/cancelTransformation>`_
 
         Args:
             transformation_id (int): Transformation internal id
             transformation_external_id (str): Transformation external id
 
         Examples:
@@ -433,15 +439,15 @@
 
         id = {"externalId": transformation_external_id, "id": transformation_id}
 
         self._post(json=id, url_path=self._RESOURCE_PATH + "/cancel")
 
     def preview(
         self,
-        query: str = None,
+        query: Optional[str] = None,
         convert_to_string: bool = False,
         limit: int = 100,
         source_limit: Optional[int] = 100,
         infer_schema_limit: Optional[int] = 1000,
     ) -> TransformationPreviewResult:
         """`Preview the result of a query. <https://developer.cognite.com/api#tag/Transformations/operation/runPreview>`_
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.8.5/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.8.5/cognite/client/_api/transformations/notifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         return self._create_multiple(
             list_cls=TransformationNotificationList, resource_cls=TransformationNotification, items=notification
         )
 
     def list(
         self,
         transformation_id: Optional[int] = None,
-        transformation_external_id: str = None,
-        destination: str = None,
+        transformation_external_id: Optional[str] = None,
+        destination: Optional[str] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> TransformationNotificationList:
         """`List notification subscriptions. <https://developer.cognite.com/api#tag/Transformation-Notifications/operation/getTransformationNotifications>`_
 
         Args:
             transformation_id (Optional[int]): Filter by transformation internal numeric ID.
             transformation_external_id (str): Filter by transformation externalId.
@@ -81,15 +81,15 @@
             list_cls=TransformationNotificationList,
             resource_cls=TransformationNotification,
             method="GET",
             limit=limit,
             filter=filter,
         )
 
-    def delete(self, id: Union[int, Sequence[int]] = None) -> None:
+    def delete(self, id: Optional[Union[int, Sequence[int]]] = None) -> None:
         """`Deletes the specified notification subscriptions on the transformation. Does nothing when the subscriptions already don't exist <https://developer.cognite.com/api#tag/Transformation-Notifications/operation/deleteTransformationNotifications>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of transformation notification ids
 
         Returns:
             None
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.8.5/cognite/client/_api/transformations/schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,16 @@
             method="GET",
             limit=limit,
             filter=filter,
         )
 
     def delete(
         self,
-        id: Union[int, Sequence[int]] = None,
-        external_id: Union[str, Sequence[str]] = None,
+        id: Optional[Union[int, Sequence[int]]] = None,
+        external_id: Optional[Union[str, Sequence[str]]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
         """`Unschedule one or more transformations <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/deleteTransformationSchedules>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.8.5/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_api/vision.py` & `cognite_sdk-6.8.5/cognite/client/_api/vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         return [*id_objs, *external_id_objs]
 
     def _run_job(
         self,
         job_path: str,
         job_cls: Type[T_ContextualizationJob],
         status_path: Optional[str] = None,
-        headers: Dict[str, Any] = None,
+        headers: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> T_ContextualizationJob:
         if status_path is None:
             status_path = job_path + "/"
         res = self._post(
             self._RESOURCE_PATH + job_path,
             json={to_camel_case(k): v for k, v in (kwargs or {}).items() if v is not None},
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_api_client.py` & `cognite_sdk-6.8.5/cognite/client/_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,17 +247,17 @@
                 return True
         return False
 
     def _retrieve(
         self,
         identifier: IdentifierCore,
         cls: Type[T_CogniteResource],
-        resource_path: str = None,
-        params: Dict = None,
-        headers: Dict = None,
+        resource_path: Optional[str] = None,
+        params: Optional[Dict] = None,
+        headers: Optional[Dict] = None,
     ) -> Optional[T_CogniteResource]:
         resource_path = resource_path or self._RESOURCE_PATH
         try:
             res = self._get(
                 url_path=utils._auxiliary.interpolate_and_url_encode(
                     resource_path + "/{}", str(identifier.as_primitive())
                 ),
@@ -728,42 +728,42 @@
     @overload
     def _update_multiple(
         self,
         items: Union[CogniteResource, CogniteUpdate],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         update_cls: Type[CogniteUpdate],
-        resource_path: str = None,
-        params: Dict = None,
-        headers: Dict = None,
+        resource_path: Optional[str] = None,
+        params: Optional[Dict] = None,
+        headers: Optional[Dict] = None,
     ) -> T_CogniteResource:
         ...
 
     @overload
     def _update_multiple(
         self,
         items: Sequence[Union[CogniteResource, CogniteUpdate]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         update_cls: Type[CogniteUpdate],
-        resource_path: str = None,
-        params: Dict = None,
-        headers: Dict = None,
+        resource_path: Optional[str] = None,
+        params: Optional[Dict] = None,
+        headers: Optional[Dict] = None,
     ) -> T_CogniteResourceList:
         ...
 
     def _update_multiple(
         self,
         items: Union[Sequence[Union[CogniteResource, CogniteUpdate]], CogniteResource, CogniteUpdate],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         update_cls: Type[CogniteUpdate],
-        resource_path: str = None,
-        params: Dict = None,
-        headers: Dict = None,
+        resource_path: Optional[str] = None,
+        params: Optional[Dict] = None,
+        headers: Optional[Dict] = None,
     ) -> Union[T_CogniteResourceList, T_CogniteResource]:
         resource_path = resource_path or self._RESOURCE_PATH
         patch_objects = []
         single_item = not isinstance(items, (Sequence, UserList))
         if single_item:
             item_list = cast(Union[Sequence[CogniteResource], Sequence[CogniteUpdate]], [items])
         else:
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_cognite_client.py` & `cognite_sdk-6.8.5/cognite/client/_cognite_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,29 +73,39 @@
         self.annotations = AnnotationsAPI(self._config, self._API_VERSION, self)
         self.functions = FunctionsAPI(self._config, self._API_VERSION, self)
         self.data_modeling = DataModelingAPI(self._config, self._API_VERSION, self)
 
         # APIs just using base_url:
         self._api_client = APIClient(self._config, api_version=None, cognite_client=self)
 
-    def get(self, url: str, params: Dict[str, Any] = None, headers: Dict[str, Any] = None) -> Response:
+    def get(
+        self, url: str, params: Optional[Dict[str, Any]] = None, headers: Optional[Dict[str, Any]] = None
+    ) -> Response:
         """Perform a GET request to an arbitrary path in the API."""
         return self._api_client._get(url, params=params, headers=headers)
 
     def post(
-        self, url: str, json: Dict[str, Any], params: Dict[str, Any] = None, headers: Dict[str, Any] = None
+        self,
+        url: str,
+        json: Dict[str, Any],
+        params: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, Any]] = None,
     ) -> Response:
         """Perform a POST request to an arbitrary path in the API."""
         return self._api_client._post(url, json=json, params=params, headers=headers)
 
-    def put(self, url: str, json: Dict[str, Any] = None, headers: Dict[str, Any] = None) -> Response:
+    def put(
+        self, url: str, json: Optional[Dict[str, Any]] = None, headers: Optional[Dict[str, Any]] = None
+    ) -> Response:
         """Perform a PUT request to an arbitrary path in the API."""
         return self._api_client._put(url, json=json, headers=headers)
 
-    def delete(self, url: str, params: Dict[str, Any] = None, headers: Dict[str, Any] = None) -> Response:
+    def delete(
+        self, url: str, params: Optional[Dict[str, Any]] = None, headers: Optional[Dict[str, Any]] = None
+    ) -> Response:
         """Perform a DELETE request to an arbitrary path in the API."""
         return self._api_client._delete(url, params=params, headers=headers)
 
     @property
     def version(self) -> str:
         """Returns the current SDK version.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/_http_client.py` & `cognite_sdk-6.8.5/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.8.5/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.8.5/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.8.5/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.8.5/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.8.5/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/config.py` & `cognite_sdk-6.8.5/cognite/client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         return pprint.pformat(self.__dict__, indent=4)
 
     def _repr_html_(self) -> str:
         return str(self)
 
     @classmethod
     def default(
-        cls, project: str, cdf_cluster: str, credentials: CredentialProvider, client_name: str = None
+        cls, project: str, cdf_cluster: str, credentials: CredentialProvider, client_name: Optional[str] = None
     ) -> ClientConfig:
         """
         Create a default client config object.
 
         Args:
             project: CDF Project name.
             cdf_cluster: The CDF cluster where the CDF project is located.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/credentials.py` & `cognite_sdk-6.8.5/cognite/client/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     """
 
     def __init__(
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
-        token_cache_path: Path = None,
+        token_cache_path: Optional[Path] = None,
         token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
     ) -> None:
         super().__init__(token_expiry_leeway_seconds)
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
 
@@ -246,15 +246,15 @@
 
     def __init__(
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
         redirect_port: int = 53000,
-        token_cache_path: Path = None,
+        token_cache_path: Optional[Path] = None,
         token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
     ) -> None:
 
         super().__init__(token_expiry_leeway_seconds)
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/_base.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,29 +116,29 @@
         Returns:
             Dict[str, Any]: A dictionary representation of the instance.
         """
         return basic_instance_dump(self, camel_case=camel_case)
 
     @classmethod
     def _load(
-        cls: Type[T_CogniteResource], resource: Union[Dict, str], cognite_client: CogniteClient = None
+        cls: Type[T_CogniteResource], resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None
     ) -> T_CogniteResource:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         elif isinstance(resource, Dict):
             instance = cls(cognite_client=cognite_client)
             for key, value in resource.items():
                 snake_case_key = to_snake_case(key)
                 if hasattr(instance, snake_case_key):
                     setattr(instance, snake_case_key, value)
             return instance
         raise TypeError(f"Resource must be json str or dict, not {type(resource)}")
 
     def to_pandas(
-        self, expand: Sequence[str] = ("metadata",), ignore: List[str] = None, camel_case: bool = False
+        self, expand: Sequence[str] = ("metadata",), ignore: Optional[List[str]] = None, camel_case: bool = False
     ) -> pandas.DataFrame:
         """Convert the instance into a pandas DataFrame.
 
         Args:
             expand (List[str]): List of row keys to expand, only works if the value is a Dict.
                 Will expand metadata by default.
             ignore (List[str]): List of row keys to not include when converting to a data frame.
@@ -188,15 +188,15 @@
         else:
             self[schema_name] = value
 
 
 class CogniteResourceList(UserList, Generic[T_CogniteResource]):
     _RESOURCE: Type[CogniteResource]
 
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         for resource in resources:
             if not isinstance(resource, self._RESOURCE):
                 raise TypeError(
                     f"All resources for class '{self.__class__.__name__}' must be of type "
                     f"'{self._RESOURCE.__name__}', not '{type(resource)}'."
                 )
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -260,15 +260,15 @@
             camel_case (bool): Use camelCase for attribute names. Defaults to False.
 
         Returns:
             List[Dict[str, Any]]: A list of dicts representing the instance.
         """
         return [resource.dump(camel_case) for resource in self.data]
 
-    def get(self, id: int = None, external_id: str = None) -> Optional[T_CogniteResource]:
+    def get(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[T_CogniteResource]:
         """Get an item from this list by id or exernal_id.
 
         Args:
             id (int): The id of the item to get.
             external_id (str): The external_id of the item to get.
 
         Returns:
@@ -290,28 +290,30 @@
         return convert_nullable_int_cols(df, camel_case)
 
     def _repr_html_(self) -> str:
         return notebook_display_with_fallback(self)
 
     @classmethod
     def _load(
-        cls: Type[T_CogniteResourceList], resource_list: Union[List, str], cognite_client: CogniteClient = None
+        cls: Type[T_CogniteResourceList],
+        resource_list: Union[List, str],
+        cognite_client: Optional[CogniteClient] = None,
     ) -> T_CogniteResourceList:
         if isinstance(resource_list, str):
             return cls._load(json.loads(resource_list), cognite_client=cognite_client)
         elif isinstance(resource_list, List):
             resources = [cls._RESOURCE._load(resource, cognite_client=cognite_client) for resource in resource_list]
             return cls(resources, cognite_client=cognite_client)
 
 
 T_CogniteResourceList = TypeVar("T_CogniteResourceList", bound=CogniteResourceList)
 
 
 class CogniteUpdate:
-    def __init__(self, id: int = None, external_id: str = None):
+    def __init__(self, id: Optional[int] = None, external_id: Optional[str] = None):
         self._id = id
         self._external_id = external_id
         self._update_object: Dict[str, Any] = {}
 
     def __eq__(self, other: Any) -> bool:
         return type(self) == type(other) and self.dump() == other.dump()
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,23 +60,23 @@
         self.annotated_resource_id = annotated_resource_id
         self.id: Optional[int] = None  # Read only
         self.created_time: Optional[int] = None  # Read only
         self.last_updated_time: Optional[int] = None  # Read only
         self._cognite_client: CogniteClient = cast("CogniteClient", None)  # Read only
 
     @classmethod
-    def _load(cls, resource: Union[Dict[str, Any], str], cognite_client: CogniteClient = None) -> Annotation:
+    def _load(cls, resource: Union[Dict[str, Any], str], cognite_client: Optional[CogniteClient] = None) -> Annotation:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         elif isinstance(resource, dict):
             return cls.from_dict(resource, cognite_client=cognite_client)
         raise TypeError(f"Resource must be json str or dict, not {type(resource)}")
 
     @classmethod
-    def from_dict(cls, resource: Dict[str, Any], cognite_client: CogniteClient = None) -> Annotation:
+    def from_dict(cls, resource: Dict[str, Any], cognite_client: Optional[CogniteClient] = None) -> Annotation:
         # Create base annotation
         data = {to_snake_case(key): val for key, val in resource.items()}
         annotation = Annotation(
             annotation_type=data["annotation_type"],
             data=data["data"],
             status=data.get("status", "suggested"),
             creating_app=data["creating_app"],
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/assets.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class AssetAggregate(dict):
     """Aggregation group of assets
 
     Args:
         count (int): Size of the aggregation group
     """
 
-    def __init__(self, count: int = None, **kwargs: Any) -> None:
+    def __init__(self, count: Optional[int] = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
 class AggregateResultItem(dict):
@@ -75,15 +75,19 @@
     Args:
         child_count (int): Number of direct descendants for the asset
         depth (int): Asset path depth (number of levels below root node).
         path (List[Dict[str, Any]]): IDs of assets on the path to the asset.
     """
 
     def __init__(
-        self, child_count: int = None, depth: int = None, path: List[Dict[str, Any]] = None, **kwargs: Any
+        self,
+        child_count: Optional[int] = None,
+        depth: Optional[int] = None,
+        path: Optional[List[Dict[str, Any]]] = None,
+        **kwargs: Any,
     ) -> None:
         self.child_count = child_count
         self.depth = depth
         self.path = path
         self.update(kwargs)
 
     child_count = CognitePropertyClassUtil.declare_property("childCount")
@@ -111,30 +115,30 @@
         root_id (int): ID of the root asset.
         aggregates (Union[Dict[str, Any], AggregateResultItem]): Aggregated metrics of the asset
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        name: str = None,
-        parent_id: int = None,
-        parent_external_id: str = None,
-        description: str = None,
-        data_set_id: int = None,
-        metadata: Dict[str, str] = None,
-        source: str = None,
-        labels: List[Union[Label, str, LabelDefinition, dict]] = None,
-        geo_location: GeoLocation = None,
-        id: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        root_id: int = None,
-        aggregates: Union[Dict[str, Any], AggregateResultItem] = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        parent_id: Optional[int] = None,
+        parent_external_id: Optional[str] = None,
+        description: Optional[str] = None,
+        data_set_id: Optional[int] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        source: Optional[str] = None,
+        labels: Optional[List[Union[Label, str, LabelDefinition, dict]]] = None,
+        geo_location: Optional[GeoLocation] = None,
+        id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        root_id: Optional[int] = None,
+        aggregates: Optional[Union[Dict[str, Any], AggregateResultItem]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         if geo_location is not None and not isinstance(geo_location, GeoLocation):
             raise TypeError("Asset.geo_location should be of type GeoLocation")
         self.external_id = external_id
         self.name = name
         self.parent_id = parent_id
         self.parent_external_id = parent_external_id
@@ -148,15 +152,15 @@
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self.root_id = root_id
         self.aggregates = aggregates
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> Asset:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> Asset:
         instance = super()._load(resource, cognite_client)
         if isinstance(resource, Dict):
             if instance.aggregates is not None:
                 instance.aggregates = AggregateResultItem(**instance.aggregates)
         instance.labels = Label._load_list(instance.labels)
         if instance.geo_location is not None:
             instance.geo_location = GeoLocation._load(instance.geo_location)
@@ -179,15 +183,15 @@
         """Returns the children of this asset.
 
         Returns:
             AssetList: The requested assets
         """
         return self._cognite_client.assets.list(parent_ids=[self.id], limit=None)
 
-    def subtree(self, depth: int = None) -> AssetList:
+    def subtree(self, depth: Optional[int] = None) -> AssetList:
         """Returns the subtree of this asset up to a specified depth.
 
         Args:
             depth (int, optional): Retrieve assets up to this depth below the asset.
 
         Returns:
             AssetList: The requested assets sorted topologically.
@@ -230,15 +234,18 @@
     def dump(self, camel_case: bool = False) -> Dict[str, Any]:
         result = super().dump(camel_case)
         if self.labels is not None:
             result["labels"] = [label.dump(camel_case) for label in self.labels]
         return result
 
     def to_pandas(
-        self, expand: Sequence[str] = ("metadata", "aggregates"), ignore: List[str] = None, camel_case: bool = False
+        self,
+        expand: Sequence[str] = ("metadata", "aggregates"),
+        ignore: Optional[List[str]] = None,
+        camel_case: bool = False,
     ) -> pandas.DataFrame:
         """Convert the instance into a pandas DataFrame.
 
         Args:
             expand (List[str]): List of row keys to expand, only works if the value is a Dict.
             ignore (List[str]): List of row keys to not include when converting to a data frame.
             camel_case (bool): Convert column names to camel case (e.g. `externalId` instead of `external_id`)
@@ -331,15 +338,15 @@
     def geo_location(self) -> _PrimitiveAssetUpdate:
         return AssetUpdate._PrimitiveAssetUpdate(self, "geoLocation")
 
 
 class AssetList(CogniteResourceList[Asset]):
     _RESOURCE = Asset
 
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         super().__init__(resources, cognite_client)
         self._retrieve_chunk_size = 100
 
     def time_series(self) -> TimeSeriesList:
         """Retrieve all time series related to these assets.
 
         Returns:
@@ -415,28 +422,28 @@
         labels (LabelFilter): Return only the resource matching the specified label constraints.
         geo_location (GeoLocationFilter): Only include files matching the specified geographic relation.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        parent_ids: Sequence[int] = None,
-        parent_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Sequence[Dict[str, Any]] = None,
-        data_set_ids: Sequence[Dict[str, Any]] = None,
-        metadata: Dict[str, str] = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        root: bool = None,
-        external_id_prefix: str = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        parent_ids: Optional[Sequence[int]] = None,
+        parent_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        data_set_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        root: Optional[bool] = None,
+        external_id_prefix: Optional[str] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.parent_ids = parent_ids
         self.parent_external_ids = parent_external_ids
         self.asset_subtree_ids = asset_subtree_ids
         self.data_set_ids = data_set_ids
         self.metadata = metadata
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/contextualization.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,24 +72,24 @@
             "jobToken",
         }
     )
     _JOB_TYPE = ContextualizationJobType.ENTITY_MATCHING
 
     def __init__(
         self,
-        job_id: int = None,
-        model_id: int = None,
-        status: str = None,
-        error_message: str = None,
-        created_time: int = None,
-        start_time: int = None,
-        status_time: int = None,
-        status_path: str = None,
-        job_token: str = None,
-        cognite_client: CogniteClient = None,
+        job_id: Optional[int] = None,
+        model_id: Optional[int] = None,
+        status: Optional[str] = None,
+        error_message: Optional[str] = None,
+        created_time: Optional[int] = None,
+        start_time: Optional[int] = None,
+        status_time: Optional[int] = None,
+        status_path: Optional[str] = None,
+        job_token: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         """Data class for the result of a contextualization job."""
         self.job_id = job_id
         self.model_id = model_id
         self.status = status
         self.created_time = created_time
         self.start_time = start_time
@@ -113,15 +113,15 @@
         self.start_time = data.get("startTime")
         self.created_time = self.created_time or data.get("createdTime")
         self.error_message = data.get("errorMessage")
         self._result = {k: v for k, v in data.items() if k not in self._COMMON_FIELDS}
         assert self.status is not None
         return self.status
 
-    def wait_for_completion(self, timeout: int = None, interval: int = 1) -> None:
+    def wait_for_completion(self, timeout: Optional[int] = None, interval: int = 1) -> None:
         """Waits for job completion. This is generally not needed to call directly, as `.result` will do so automatically.
 
         Args:
             timeout (int): Time out after this many seconds. (None means wait indefinitely)
             interval (int): Poll status every this many seconds.
 
         Raises:
@@ -170,28 +170,28 @@
 
 class EntityMatchingModel(CogniteResource):
     _RESOURCE_PATH = "/context/entitymatching"
     _STATUS_PATH = _RESOURCE_PATH + "/"
 
     def __init__(
         self,
-        id: int = None,
-        status: str = None,
-        error_message: str = None,
-        created_time: int = None,
-        start_time: int = None,
-        status_time: int = None,
-        classifier: str = None,
-        feature_type: str = None,
-        match_fields: List[str] = None,
-        model_type: str = None,
-        name: str = None,
-        description: str = None,
-        external_id: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        status: Optional[str] = None,
+        error_message: Optional[str] = None,
+        created_time: Optional[int] = None,
+        start_time: Optional[int] = None,
+        status_time: Optional[int] = None,
+        classifier: Optional[str] = None,
+        feature_type: Optional[str] = None,
+        match_fields: Optional[List[str]] = None,
+        model_type: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        external_id: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         """Entity matching model. See the `fit` method for the meaning of these fields."""
         self.id = id
         self.status = status
         self.created_time = created_time
         self.start_time = start_time
         self.status_time = status_time
@@ -215,15 +215,15 @@
         self.status_time = data.get("statusTime")
         self.start_time = data.get("startTime")
         self.created_time = self.created_time or data.get("createdTime")
         self.error_message = data.get("errorMessage")
         assert self.status is not None
         return self.status
 
-    def wait_for_completion(self, timeout: int = None, interval: int = 1) -> None:
+    def wait_for_completion(self, timeout: Optional[int] = None, interval: int = 1) -> None:
         """Waits for model completion. This is generally not needed to call directly, as `.result` will do so automatically.
 
         Args:
             timeout: Time out after this many seconds. (None means wait indefinitely)
             interval: Poll status every this many seconds.
 
         Raises:
@@ -241,15 +241,15 @@
             raise ModelFailedException(self.__class__.__name__, self.id, self.error_message)
 
     def predict(
         self,
         sources: Optional[List[Dict]] = None,
         targets: Optional[List[Dict]] = None,
         num_matches: int = 1,
-        score_threshold: float = None,
+        score_threshold: Optional[float] = None,
     ) -> ContextualizationJob:
         """Predict entity matching. NB. blocks and waits for the model to be ready if it has been recently created.
 
         Args:
             sources: entities to match from, does not need an 'id' field. Tolerant to passing more than is needed or used (e.g. json dump of time series list). If omitted, will use data from fit.
             targets: entities to match to, does not need an 'id' field.  Tolerant to passing more than is needed or used. If omitted, will use data from fit.
             num_matches (int): number of matches to return for each item.
@@ -356,33 +356,37 @@
         if self.first_page is not None and self.last_page is not None:
             item["pageRange"] = {"begin": self.first_page, "end": self.last_page}
         return item
 
 
 class DiagramConvertPage(CogniteResource):
     def __init__(
-        self, page: int = None, png_url: str = None, svg_url: str = None, cognite_client: CogniteClient = None
+        self,
+        page: Optional[int] = None,
+        png_url: Optional[str] = None,
+        svg_url: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.page = page
         self.png_url = png_url
         self.svg_url = svg_url
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class DiagramConvertPageList(CogniteResourceList[DiagramConvertPage]):
     _RESOURCE = DiagramConvertPage
 
 
 class DiagramConvertItem(CogniteResource):
     def __init__(
         self,
-        file_id: int = None,
-        file_external_id: str = None,
-        results: list = None,
-        cognite_client: CogniteClient = None,
+        file_id: Optional[int] = None,
+        file_external_id: Optional[str] = None,
+        results: Optional[list] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.file_id = file_id
         self.file_external_id = file_external_id
         self.results = results
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     def __len__(self) -> int:
@@ -441,19 +445,19 @@
     def items(self, items: list) -> None:
         self._items = items
 
 
 class DiagramDetectItem(CogniteResource):
     def __init__(
         self,
-        file_id: int = None,
-        file_external_id: str = None,
-        annotations: list = None,
-        error_message: str = None,
-        cognite_client: CogniteClient = None,
+        file_id: Optional[int] = None,
+        file_external_id: Optional[str] = None,
+        annotations: Optional[list] = None,
+        error_message: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
         page_range: Optional[Dict[str, int]] = None,
         page_count: Optional[int] = None,
     ):
         self.file_id = file_id
         self.file_external_id = file_external_id
         self.annotations = annotations
         self.error_message = error_message
@@ -595,15 +599,15 @@
 
 
 class DetectJobBundle:
     _RESOURCE_PATH = "/context/diagram/detect/"
     _STATUS_PATH = "/context/diagram/detect/status"
     _WAIT_TIME = 2
 
-    def __init__(self, job_ids: List[int], cognite_client: CogniteClient = None):
+    def __init__(self, job_ids: List[int], cognite_client: Optional[CogniteClient] = None):
         warnings.warn(
             "DetectJobBundle.result is calling a beta endpoint which is still in development. "
             "Breaking changes can happen in between patch versions."
         )
 
         self._cognite_client = cast("CogniteClient", cognite_client)
         if not job_ids:
@@ -623,15 +627,15 @@
         Linear back off, in order to limit load on our API.
         Starts at _WAIT_TIME and goes to 10 seconds.
         """
         time.sleep(self._WAIT_TIME)
         if self._WAIT_TIME < 10:
             self._WAIT_TIME += 2
 
-    def wait_for_completion(self, timeout: int = None) -> None:
+    def wait_for_completion(self, timeout: Optional[int] = None) -> None:
         """Waits for all jobs to complete, generally not needed to call as it is called by result.
 
         Args:
             timeout (int): Time out after this many seconds. (None means wait indefinitely)
             interval (int): Poll status every this many seconds.
         """
         start = time.time()
@@ -701,31 +705,31 @@
         assert self.status is not None
         return self.status
 
 
 class VisionExtractItem(CogniteResource):
     def __init__(
         self,
-        file_id: int = None,
-        predictions: Dict[str, Any] = None,
-        file_external_id: str = None,
-        error_message: str = None,
-        cognite_client: CogniteClient = None,
+        file_id: Optional[int] = None,
+        predictions: Optional[Dict[str, Any]] = None,
+        file_external_id: Optional[str] = None,
+        error_message: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         """Data class for storing predictions for a single image file"""
         self.file_id = file_id
         self.file_external_id = file_external_id
         self.error_message = error_message
         self.predictions = self._process_predictions_dict(predictions) if isinstance(predictions, Dict) else predictions
 
         self._predictions_dict = predictions  # The "raw" predictions dict returned by the endpoint
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> VisionExtractItem:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> VisionExtractItem:
         """Override CogniteResource._load so that we can convert the dicts returned by the API to data classes"""
         extracted_item = super()._load(resource, cognite_client=cognite_client)
         if isinstance(extracted_item.predictions, dict):
             extracted_item._predictions_dict = extracted_item.predictions
             extracted_item.predictions = cls._process_predictions_dict(extracted_item._predictions_dict)
         return extracted_item
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Type, TypeVar
+from typing import TYPE_CHECKING, Optional, Type, TypeVar
 
 from cognite.client.data_classes._base import CogniteResource
 from cognite.client.utils._text import convert_all_keys_to_snake_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
@@ -25,13 +25,13 @@
     @classmethod
     def load(cls: Type[T_DataModelingResource], data: dict | str) -> T_DataModelingResource:
         data = json.loads(data) if isinstance(data, str) else data
         return cls(**convert_all_keys_to_snake_case(data))
 
     @classmethod
     def _load(
-        cls: Type[T_DataModelingResource], resource: dict | str, cognite_client: CogniteClient = None
+        cls: Type[T_DataModelingResource], resource: dict | str, cognite_client: Optional[CogniteClient] = None
     ) -> T_DataModelingResource:
         return cls.load(resource)
 
 
 T_DataModelingResource = TypeVar("T_DataModelingResource", bound=DataModelingResource)
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/aggregations.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/aggregations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         properties: dict[str, ContainerProperty],
-        description: str = None,
-        name: str = None,
-        used_for: Literal["node", "edge", "all"] = None,
-        constraints: dict[str, Constraint] = None,
-        indexes: dict[str, Index] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        used_for: Optional[Literal["node", "edge", "all"]] = None,
+        constraints: Optional[dict[str, Constraint]] = None,
+        indexes: Optional[dict[str, Index]] = None,
         **_: dict,
     ):
         self.space = space
         self.external_id = external_id
         self.description = description
         self.name = name
         self.used_for = used_for
@@ -96,19 +96,19 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         properties: dict[str, ContainerProperty],
-        description: str = None,
-        name: str = None,
-        used_for: Literal["node", "edge", "all"] = None,
-        constraints: dict[str, Constraint] = None,
-        indexes: dict[str, Index] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        used_for: Optional[Literal["node", "edge", "all"]] = None,
+        constraints: Optional[dict[str, Constraint]] = None,
+        indexes: Optional[dict[str, Index]] = None,
     ):
         validate_data_modeling_identifier(space, external_id)
         super().__init__(space, external_id, properties, description, name, used_for, constraints, indexes)
 
 
 class Container(ContainerCore):
     """Represent the physical storage of data. This is the read format of the container
@@ -131,19 +131,19 @@
         self,
         space: str,
         external_id: str,
         properties: dict[str, ContainerProperty],
         is_global: bool,
         last_updated_time: int,
         created_time: int,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         used_for: Literal["node", "edge", "all"] = "node",
-        constraints: dict[str, Constraint] = None,
-        indexes: dict[str, Index] = None,
+        constraints: Optional[dict[str, Constraint]] = None,
+        indexes: Optional[dict[str, Index]] = None,
     ):
         super().__init__(space, external_id, properties, description, name, used_for, constraints, indexes)
         self.is_global = is_global
         self.last_updated_time = last_updated_time
         self.created_time = created_time
 
     def as_apply(self) -> ContainerApply:
@@ -179,15 +179,15 @@
     """Represent the filter arguments for the list endpoint.
 
     Args:
         space (str): The space to query
         include_global (bool): Whether the global containers should be included.
     """
 
-    def __init__(self, space: str = None, include_global: bool = False):
+    def __init__(self, space: Optional[str] = None, include_global: bool = False):
         self.space = space
         self.include_global = include_global
 
 
 @dataclass
 class ContainerProperty:
     type: PropertyType
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         **_: dict,
     ):
         self.space = space
         self.external_id = external_id
         self.description = description
         self.name = name
         self.version = version
@@ -56,17 +56,17 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
-        description: str = None,
-        name: str = None,
-        views: list[ViewId | ViewApply] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        views: Optional[list[ViewId | ViewApply]] = None,
     ):
         validate_data_modeling_identifier(space, external_id)
         super().__init__(space, external_id, version, description, name)
         self.views = views
 
     @classmethod
     def _load_view(cls, view_data: dict) -> ViewId | ViewApply:
@@ -114,16 +114,16 @@
         self,
         space: str,
         external_id: str,
         version: str,
         is_global: bool,
         last_updated_time: int,
         created_time: int,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         views: Optional[list[T_View]] = None,
         **_: dict,
     ):
         super().__init__(space, external_id, version, description, name)
         self.views: list[T_View] = views or []
         self.is_global = is_global
         self.last_updated_time = last_updated_time
@@ -192,15 +192,15 @@
         all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
                              which is determined based on the 'createdTime' field.
         include_global (bool): Whether to include global views.
     """
 
     def __init__(
         self,
-        space: str = None,
+        space: Optional[str] = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ):
         self.space = space
         self.inline_views = inline_views
         self.all_versions = all_versions
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/graphql.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,16 +113,16 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         instance_type: Literal["node", "edge"] = "node",
-        existing_version: int = None,
-        sources: list[NodeOrEdgeData] = None,
+        existing_version: Optional[int] = None,
+        sources: Optional[list[NodeOrEdgeData]] = None,
     ):
         validate_data_modeling_identifier(space, external_id)
         super().__init__(space, external_id, instance_type)
         self.existing_version = existing_version
         self.sources = sources
 
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
@@ -201,15 +201,17 @@
     @overload
     def get(
         self, view: ViewIdentifier, default: MutableMapping[PropertyIdentifier, PropertyValue] | _T
     ) -> MutableMapping[PropertyIdentifier, PropertyValue] | _T:
         ...
 
     def get(
-        self, view: ViewIdentifier, default: Optional[MutableMapping[PropertyIdentifier, PropertyValue]] | _T = None
+        self,
+        view: ViewIdentifier,
+        default: Optional[Optional[MutableMapping[PropertyIdentifier, PropertyValue]] | _T] = None,
     ) -> Optional[MutableMapping[PropertyIdentifier, PropertyValue]] | _T:
         view_id = ViewId.load(view)
         return self.data.get(view_id, default)
 
     def __len__(self) -> int:
         return len(self.data)
 
@@ -244,16 +246,16 @@
         self,
         space: str,
         external_id: str,
         version: str,
         last_updated_time: int,
         created_time: int,
         instance_type: Literal["node", "edge"] = "node",
-        deleted_time: int = None,
-        properties: Properties = None,
+        deleted_time: Optional[int] = None,
+        properties: Optional[Properties] = None,
         **_: dict,
     ):
         super().__init__(space, external_id, instance_type)
         self.version = version
         self.last_updated_time = last_updated_time
         self.created_time = created_time
         self.deleted_time = deleted_time
@@ -378,16 +380,16 @@
                         container the container(s) making up this node.
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
-        existing_version: int = None,
-        sources: list[NodeOrEdgeData] = None,
+        existing_version: Optional[int] = None,
+        sources: Optional[list[NodeOrEdgeData]] = None,
     ):
         super().__init__(space, external_id, "node", existing_version, sources)
 
     def as_id(self) -> NodeId:
         return NodeId(space=self.space, external_id=self.external_id)
 
 
@@ -408,16 +410,16 @@
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
         last_updated_time: int,
         created_time: int,
-        deleted_time: int = None,
-        properties: Properties = None,
+        deleted_time: Optional[int] = None,
+        properties: Optional[Properties] = None,
         **_: dict,
     ):
         super().__init__(space, external_id, version, last_updated_time, created_time, "node", deleted_time, properties)
 
     def as_apply(self, source: ViewIdentifier | ContainerIdentifier, existing_version: int) -> NodeApply:
         """
         This is a convenience function for converting the read to a write node.
@@ -511,16 +513,16 @@
     def __init__(
         self,
         space: str,
         external_id: str,
         type: DirectRelationReference | tuple[str, str],
         start_node: DirectRelationReference | tuple[str, str],
         end_node: DirectRelationReference | tuple[str, str],
-        existing_version: int = None,
-        sources: list[NodeOrEdgeData] = None,
+        existing_version: Optional[int] = None,
+        sources: Optional[list[NodeOrEdgeData]] = None,
     ):
         super().__init__(space, external_id, "edge", existing_version, sources)
         self.type = type if isinstance(type, DirectRelationReference) else DirectRelationReference.load(type)
         self.start_node = (
             start_node if isinstance(start_node, DirectRelationReference) else DirectRelationReference.load(start_node)
         )
         self.end_node = (
@@ -573,24 +575,26 @@
         external_id: str,
         version: str,
         type: DirectRelationReference,
         last_updated_time: int,
         created_time: int,
         start_node: DirectRelationReference,
         end_node: DirectRelationReference,
-        deleted_time: int = None,
-        properties: Properties = None,
+        deleted_time: Optional[int] = None,
+        properties: Optional[Properties] = None,
         **_: dict,
     ):
         super().__init__(space, external_id, version, last_updated_time, created_time, "edge", deleted_time, properties)
         self.type = type
         self.start_node = start_node
         self.end_node = end_node
 
-    def as_apply(self, source: ViewIdentifier | ContainerIdentifier, existing_version: int = None) -> EdgeApply:
+    def as_apply(
+        self, source: ViewIdentifier | ContainerIdentifier, existing_version: Optional[int] = None
+    ) -> EdgeApply:
         """
         This is a convenience function for converting the read to a write edge.
 
         It makes the simplifying assumption that all properties are from the same view. Note that this
         is not true in general.
 
         Args:
@@ -689,15 +693,15 @@
     _RESOURCE = Node
 
     def as_ids(self) -> list[NodeId]:
         return [node.as_id() for node in self]
 
 
 class NodeListWithCursor(NodeList):
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         super().__init__(resources, cognite_client)
         self.cursor: str | None = None
 
 
 class EdgeApplyResultList(CogniteResourceList[EdgeApplyResult]):
     _RESOURCE = EdgeApplyResult
 
@@ -709,15 +713,15 @@
     _RESOURCE = Edge
 
     def as_ids(self) -> list[EdgeId]:
         return [edge.as_id() for edge in self]
 
 
 class EdgeListWithCursor(EdgeList):
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         super().__init__(resources, cognite_client)
         self.cursor: str | None = None
 
 
 class InstanceSort(CogniteFilter):
     def __init__(
         self,
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/query.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,21 @@
             raise NotImplementedError(f"Unknown query type: {query}")
 
     def __eq__(self, other: Any) -> bool:
         return type(other) == type(self) and self.dump() == other.dump()
 
 
 class NodeResultSetExpression(ResultSetExpression):
-    def __init__(self, from_: str = None, filter: Filter = None, sort: list[InstanceSort] = None, limit: int = None):
+    def __init__(
+        self,
+        from_: Optional[str] = None,
+        filter: Optional[Filter] = None,
+        sort: Optional[list[InstanceSort]] = None,
+        limit: Optional[int] = None,
+    ):
         self.from_ = from_
         self.filter = filter
         self.sort = sort
         self.limit = limit
 
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output: Dict[str, Any] = {"nodes": {}}
@@ -212,17 +218,17 @@
         from_: Optional[str] = None,
         max_distance: Optional[int] = None,
         direction: Literal["outwards", "inwards"] = "outwards",
         filter: Optional[Filter] = None,
         node_filter: Optional[Filter] = None,
         termination_filter: Optional[Filter] = None,
         limit_each: Optional[int] = None,
-        sort: list[InstanceSort] = None,
-        post_sort: list[InstanceSort] = None,
-        limit: int = None,
+        sort: Optional[list[InstanceSort]] = None,
+        post_sort: Optional[list[InstanceSort]] = None,
+        limit: Optional[int] = None,
     ):
         self.from_ = from_
         self.max_distance = max_distance
         self.direction = direction
         self.filter = filter
         self.node_filter = node_filter
         self.termination_filter = termination_filter
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Optional
 
 from cognite.client.data_classes._base import (
     CogniteResourceList,
 )
 from cognite.client.data_classes.data_modeling._core import DataModelingResource
 from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
 
@@ -14,15 +14,15 @@
 
     Args:
         space (str): A unique identifier for space.
         description (str): Textual description of the space
         name (str): Human readable name for the space.
     """
 
-    def __init__(self, space: str, description: str = None, name: str = None):
+    def __init__(self, space: str, description: Optional[str] = None, name: Optional[str] = None):
         self.space = space
         self.description = description
         self.name = name
 
     def as_id(self) -> str:
         return self.space
 
@@ -35,16 +35,16 @@
         description (str): Textual description of the space
         name (str): Human readable name for the space.
     """
 
     def __init__(
         self,
         space: str,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         **_: Any,
     ):
         validate_data_modeling_identifier(space)
         super().__init__(space, description, name)
 
 
 class Space(SpaceCore):
@@ -61,16 +61,16 @@
 
     def __init__(
         self,
         space: str,
         is_global: bool,
         last_updated_time: int,
         created_time: int,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         **_: Any,
     ):
         super().__init__(space, description, name)
         self.is_global = is_global
         self.last_updated_time = last_updated_time
         self.created_time = created_time
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_modeling/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 class ViewCore(DataModelingResource):
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         filter: Filter | None = None,
-        implements: list[ViewId] = None,
+        implements: Optional[list[ViewId]] = None,
         **_: dict,
     ):
         self.space = space
         self.external_id = external_id
         self.description = description
         self.name = name
         self.filter = filter
@@ -86,19 +86,19 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         filter: Filter | None = None,
-        implements: list[ViewId] = None,
-        properties: dict[str, MappedPropertyApply | ConnectionDefinition] = None,
+        implements: Optional[list[ViewId]] = None,
+        properties: Optional[dict[str, MappedPropertyApply | ConnectionDefinition]] = None,
     ):
         validate_data_modeling_identifier(space, external_id)
         super().__init__(space, external_id, version, description, name, filter, implements)
         self.properties = properties
 
     @classmethod
     def load(cls, resource: dict | str) -> ViewApply:
@@ -139,18 +139,18 @@
         self,
         space: str,
         external_id: str,
         version: str,
         properties: dict[str, MappedProperty | ConnectionDefinition],
         last_updated_time: int,
         created_time: int,
-        description: str = None,
-        name: str = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
         filter: Filter | None = None,
-        implements: list[ViewId] = None,
+        implements: Optional[list[ViewId]] = None,
         writable: bool = False,
         used_for: Literal["node", "edge", "all"] = "node",
         is_global: bool = False,
         **_: dict,
     ):
         super().__init__(
             space,
@@ -230,15 +230,15 @@
         all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
                              which is determined based on the 'createdTime' field.
         include_global (bool): Whether to include global views.
     """
 
     def __init__(
         self,
-        space: str = None,
+        space: Optional[str] = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ):
         self.space = space
         self.include_inherited_properties = include_inherited_properties
         self.all_versions = all_versions
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/data_sets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
@@ -32,23 +32,23 @@
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        name: str = None,
-        description: str = None,
-        metadata: Dict[str, str] = None,
-        write_protected: bool = None,
-        id: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        write_protected: Optional[bool] = None,
+        id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.name = name
         self.description = description
         self.metadata = metadata
         self.write_protected = write_protected
         self.id = id
@@ -67,20 +67,20 @@
         external_id_prefix (str): Filter by this (case-sensitive) prefix for the external ID.
         write_protected (bool): No description.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        metadata: Dict[str, str] = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        write_protected: bool = None,
-        cognite_client: CogniteClient = None,
+        metadata: Optional[Dict[str, str]] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        write_protected: Optional[bool] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.metadata = metadata
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self.external_id_prefix = external_id_prefix
         self.write_protected = write_protected
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -159,15 +159,15 @@
 class DataSetAggregate(dict):
     """Aggregation group of data sets
 
     Args:
         count (int): Size of the aggregation group
     """
 
-    def __init__(self, count: int = None, **kwargs: Any) -> None:
+    def __init__(self, count: Optional[int] = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
 class DataSetList(CogniteResourceList[DataSet]):
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/datapoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,26 +114,26 @@
         continuous_variance (float): The variance of the interpolated underlying function.
         discrete_variance (float): The variance of the datapoint values.
         total_variation (float): The total variation of the interpolated underlying function.
     """
 
     def __init__(
         self,
-        timestamp: int = None,
-        value: Union[str, float] = None,
-        average: float = None,
-        max: float = None,
-        min: float = None,
-        count: int = None,
-        sum: float = None,
-        interpolation: float = None,
-        step_interpolation: float = None,
-        continuous_variance: float = None,
-        discrete_variance: float = None,
-        total_variation: float = None,
+        timestamp: Optional[int] = None,
+        value: Optional[Union[str, float]] = None,
+        average: Optional[float] = None,
+        max: Optional[float] = None,
+        min: Optional[float] = None,
+        count: Optional[int] = None,
+        sum: Optional[float] = None,
+        interpolation: Optional[float] = None,
+        step_interpolation: Optional[float] = None,
+        continuous_variance: Optional[float] = None,
+        discrete_variance: Optional[float] = None,
+        total_variation: Optional[float] = None,
     ):
         self.timestamp = timestamp
         self.value = value
         self.average = average
         self.max = max
         self.min = min
         self.count = count
@@ -162,32 +162,32 @@
 
 
 class DatapointsArray(CogniteResource):
     """An object representing datapoints using numpy arrays."""
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        is_string: bool = None,
-        is_step: bool = None,
-        unit: str = None,
-        granularity: str = None,
-        timestamp: NumpyDatetime64NSArray = None,
-        value: Union[NumpyFloat64Array, NumpyObjArray] = None,
-        average: NumpyFloat64Array = None,
-        max: NumpyFloat64Array = None,
-        min: NumpyFloat64Array = None,
-        count: NumpyInt64Array = None,
-        sum: NumpyFloat64Array = None,
-        interpolation: NumpyFloat64Array = None,
-        step_interpolation: NumpyFloat64Array = None,
-        continuous_variance: NumpyFloat64Array = None,
-        discrete_variance: NumpyFloat64Array = None,
-        total_variation: NumpyFloat64Array = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        is_step: Optional[bool] = None,
+        unit: Optional[str] = None,
+        granularity: Optional[str] = None,
+        timestamp: Optional[NumpyDatetime64NSArray] = None,
+        value: Optional[Union[NumpyFloat64Array, NumpyObjArray]] = None,
+        average: Optional[NumpyFloat64Array] = None,
+        max: Optional[NumpyFloat64Array] = None,
+        min: Optional[NumpyFloat64Array] = None,
+        count: Optional[NumpyInt64Array] = None,
+        sum: Optional[NumpyFloat64Array] = None,
+        interpolation: Optional[NumpyFloat64Array] = None,
+        step_interpolation: Optional[NumpyFloat64Array] = None,
+        continuous_variance: Optional[NumpyFloat64Array] = None,
+        discrete_variance: Optional[NumpyFloat64Array] = None,
+        total_variation: Optional[NumpyFloat64Array] = None,
     ):
         self.id = id
         self.external_id = external_id
         self.is_string = is_string
         self.is_step = is_step
         self.unit = unit
         self.granularity = granularity
@@ -404,33 +404,33 @@
         continuous_variance (List[float]): The variance of the interpolated underlying function.
         discrete_variance (List[float]): The variance of the datapoint values.
         total_variation (List[float]): The total variation of the interpolated underlying function.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        is_string: bool = None,
-        is_step: bool = None,
-        unit: str = None,
-        granularity: str = None,
-        timestamp: Sequence[int] = None,
-        value: Union[Sequence[str], Sequence[float]] = None,
-        average: List[float] = None,
-        max: List[float] = None,
-        min: List[float] = None,
-        count: List[int] = None,
-        sum: List[float] = None,
-        interpolation: List[float] = None,
-        step_interpolation: List[float] = None,
-        continuous_variance: List[float] = None,
-        discrete_variance: List[float] = None,
-        total_variation: List[float] = None,
-        error: List[Union[None, str]] = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        is_step: Optional[bool] = None,
+        unit: Optional[str] = None,
+        granularity: Optional[str] = None,
+        timestamp: Optional[Sequence[int]] = None,
+        value: Optional[Union[Sequence[str], Sequence[float]]] = None,
+        average: Optional[List[float]] = None,
+        max: Optional[List[float]] = None,
+        min: Optional[List[float]] = None,
+        count: Optional[List[int]] = None,
+        sum: Optional[List[float]] = None,
+        interpolation: Optional[List[float]] = None,
+        step_interpolation: Optional[List[float]] = None,
+        continuous_variance: Optional[List[float]] = None,
+        discrete_variance: Optional[List[float]] = None,
+        total_variation: Optional[List[float]] = None,
+        error: Optional[List[Union[None, str]]] = None,
     ):
         self.id = id
         self.external_id = external_id
         self.is_string = is_string
         self.is_step = is_step
         self.unit = unit
         self.granularity = granularity
@@ -564,15 +564,18 @@
 
         idx = pd.to_datetime(self.timestamp, unit="ms")
         (df := pd.DataFrame(dict(enumerate(data_lists)), index=idx)).columns = field_names
         return df
 
     @classmethod
     def _load(  # type: ignore [override]
-        cls, dps_object: Dict[str, Any], expected_fields: List[str] = None, cognite_client: CogniteClient = None
+        cls,
+        dps_object: Dict[str, Any],
+        expected_fields: Optional[List[str]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> Datapoints:
         del cognite_client  # just needed for signature
         instance = cls(
             id=dps_object.get("id"),
             external_id=dps_object.get("externalId"),
             is_string=dps_object["isString"],
             is_step=dps_object.get("isStep"),
@@ -640,15 +643,15 @@
         is_synthetic_dps = self.error is not None
         return notebook_display_with_fallback(self, include_errors=is_synthetic_dps)
 
 
 class DatapointsArrayList(CogniteResourceList[DatapointsArray]):
     _RESOURCE = DatapointsArray
 
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         super().__init__(resources, cognite_client)
 
         # Fix what happens for duplicated identifiers:
         ids = [dps.id for dps in self if dps.id is not None]
         xids = [dps.external_id for dps in self if dps.external_id is not None]
         dupe_ids, id_dct = find_duplicates(ids), defaultdict(list)
         dupe_xids, xid_dct = find_duplicates(xids), defaultdict(list)
@@ -700,16 +703,16 @@
                 continue
             concatenated = DatapointsArray.create_from_arrays(*items)
             self._id_to_item[id_] = concatenated
             self.data.append(concatenated)
 
     def get(  # type: ignore [override]
         self,
-        id: int = None,
-        external_id: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
     ) -> Union[None, DatapointsArray, List[DatapointsArray]]:
         """Get a specific DatapointsArray from this list by id or exernal_id.
 
         Note: For duplicated time series, returns a list of DatapointsArray.
 
         Args:
             id (int): The id of the item(s) to get.
@@ -759,15 +762,15 @@
         """
         return [dps.dump(camel_case, convert_timestamps) for dps in self]
 
 
 class DatapointsList(CogniteResourceList[Datapoints]):
     _RESOURCE = Datapoints
 
-    def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
+    def __init__(self, resources: Collection[Any], cognite_client: Optional[CogniteClient] = None):
         super().__init__(resources, cognite_client)
 
         # Fix what happens for duplicated identifiers:
         ids = [dps.id for dps in self if dps.id is not None]
         xids = [dps.external_id for dps in self if dps.external_id is not None]
         dupe_ids, id_dct = find_duplicates(ids), defaultdict(list)
         dupe_xids, xid_dct = find_duplicates(xids), defaultdict(list)
@@ -779,16 +782,16 @@
                 xid_dct[xid].append(dps)
 
         self._id_to_item.update(id_dct)
         self._external_id_to_item.update(xid_dct)
 
     def get(  # type: ignore [override]
         self,
-        id: int = None,
-        external_id: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
     ) -> Union[None, Datapoints, List[Datapoints]]:
         """Get a specific Datapoints from this list by id or exernal_id.
 
         Note: For duplicated time series, returns a list of Datapoints.
 
         Args:
             id (int): The id of the item(s) to get.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/events.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
@@ -24,15 +24,17 @@
 
     Args:
         max (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         min (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         is_null (bool): Set to true if you want to search for data with field value not set, false to search for cases where some value is present.
     """
 
-    def __init__(self, max: int = None, min: int = None, is_null: bool = None, **kwargs: Any) -> None:
+    def __init__(
+        self, max: Optional[int] = None, min: Optional[int] = None, is_null: Optional[bool] = None, **kwargs: Any
+    ) -> None:
         self.max = max
         self.min = min
         self.is_null = is_null
         self.update(kwargs)
 
     max = CognitePropertyClassUtil.declare_property("max")
     min = CognitePropertyClassUtil.declare_property("min")
@@ -57,28 +59,28 @@
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        data_set_id: int = None,
-        start_time: int = None,
-        end_time: int = None,
-        type: str = None,
-        subtype: str = None,
-        description: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        source: str = None,
-        id: int = None,
-        last_updated_time: int = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        data_set_id: Optional[int] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        type: Optional[str] = None,
+        subtype: Optional[str] = None,
+        description: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        source: Optional[str] = None,
+        id: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.data_set_id = data_set_id
         self.start_time = start_time
         self.end_time = end_time
         self.type = type
         self.subtype = subtype
@@ -111,29 +113,29 @@
         last_updated_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
         external_id_prefix (str): Filter by this (case-sensitive) prefix for the external ID.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        start_time: Union[Dict[str, Any], TimestampRange] = None,
-        end_time: Union[Dict[str, Any], EndTimeFilter] = None,
-        active_at_time: Union[Dict[str, Any], TimestampRange] = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Sequence[Dict[str, Any]] = None,
-        data_set_ids: Sequence[Dict[str, Any]] = None,
-        source: str = None,
-        type: str = None,
-        subtype: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        external_id_prefix: str = None,
-        cognite_client: CogniteClient = None,
+        start_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        end_time: Optional[Union[Dict[str, Any], EndTimeFilter]] = None,
+        active_at_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        data_set_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        source: Optional[str] = None,
+        type: Optional[str] = None,
+        subtype: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        external_id_prefix: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.start_time = start_time
         self.end_time = end_time
         self.active_at_time = active_at_time
         self.metadata = metadata
         self.asset_ids = asset_ids
         self.asset_external_ids = asset_external_ids
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/extractionpipelines.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
     CognitePropertyClassUtil,
@@ -67,33 +67,33 @@
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         created_by (str): Extraction pipeline creator, usually an email.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        name: str = None,
-        description: str = None,
-        data_set_id: int = None,
-        raw_tables: List[Dict[str, str]] = None,
-        last_success: int = None,
-        last_failure: int = None,
-        last_message: str = None,
-        last_seen: int = None,
-        schedule: str = None,
-        contacts: List[ExtractionPipelineContact] = None,
-        metadata: Dict[str, str] = None,
-        source: str = None,
-        documentation: str = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        created_by: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        data_set_id: Optional[int] = None,
+        raw_tables: Optional[List[Dict[str, str]]] = None,
+        last_success: Optional[int] = None,
+        last_failure: Optional[int] = None,
+        last_message: Optional[str] = None,
+        last_seen: Optional[int] = None,
+        schedule: Optional[str] = None,
+        contacts: Optional[List[ExtractionPipelineContact]] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        source: Optional[str] = None,
+        documentation: Optional[str] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        created_by: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.external_id = external_id
         self.name = name
         self.description = description
         self.data_set_id = data_set_id
         self.raw_tables = raw_tables
@@ -108,15 +108,15 @@
         self.last_seen = last_seen
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self.created_by = created_by
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> ExtractionPipeline:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> ExtractionPipeline:
         instance = super()._load(resource, cognite_client)
         return instance
 
     def __hash__(self) -> int:
         return hash(self.external_id)
 
 
@@ -207,30 +207,30 @@
         message (str): Optional status message.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        extpipe_external_id: str = None,
-        status: str = None,
-        message: str = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
-        id: int = None,
+        extpipe_external_id: Optional[str] = None,
+        status: Optional[str] = None,
+        message: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
+        id: Optional[int] = None,
     ):
         self.id = id
         self.extpipe_external_id = extpipe_external_id
         self.status = status
         self.message = message
         self.created_time = created_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> ExtractionPipelineRun:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> ExtractionPipelineRun:
         obj = super()._load(resource, cognite_client)
         # Note: The API ONLY returns IDs, but if they chose to change this, we're ready:
         if isinstance(resource, dict):
             obj.extpipe_external_id = resource.get("externalId")
         return obj
 
     def dump(self, camel_case: bool = False) -> Dict[str, Any]:
@@ -255,15 +255,15 @@
 class StringFilter(CogniteFilter):
     """Filter runs on substrings of the message
 
     Args:
         substring (str): Part of message
     """
 
-    def __init__(self, substring: str = None):
+    def __init__(self, substring: Optional[str] = None):
         self.substring = substring
 
 
 class ExtractionPipelineRunFilter(CogniteFilter):
     """Filter runs with exact matching
 
     Args:
@@ -272,19 +272,19 @@
         message (StringFilter): message filter.
         created_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        statuses: Sequence[str] = None,
-        message: StringFilter = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        statuses: Optional[Sequence[str]] = None,
+        message: Optional[StringFilter] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.statuses = statuses
         self.message = message
         self.created_time = created_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
@@ -306,19 +306,19 @@
         description (str): Short description of this configuration revision.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        revision: int = None,
-        description: str = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        revision: Optional[int] = None,
+        description: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.revision = revision
         self.description = description
         self.created_time = created_time
         self._cognite_client = cognite_client
 
@@ -333,20 +333,20 @@
         description (str): Short description of this configuration revision.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        config: str = None,
-        revision: int = None,
-        description: str = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        config: Optional[str] = None,
+        revision: Optional[int] = None,
+        description: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         super().__init__(
             external_id=external_id,
             revision=revision,
             description=description,
             created_time=created_time,
             cognite_client=cognite_client,
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/files.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
@@ -43,33 +43,33 @@
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        name: str = None,
-        source: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        directory: str = None,
-        asset_ids: Sequence[int] = None,
-        data_set_id: int = None,
-        labels: Sequence[Label] = None,
-        geo_location: GeoLocation = None,
-        source_created_time: int = None,
-        source_modified_time: int = None,
-        security_categories: Sequence[int] = None,
-        id: int = None,
-        uploaded: bool = None,
-        uploaded_time: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        source: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        directory: Optional[str] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        data_set_id: Optional[int] = None,
+        labels: Optional[Sequence[Label]] = None,
+        geo_location: Optional[GeoLocation] = None,
+        source_created_time: Optional[int] = None,
+        source_modified_time: Optional[int] = None,
+        security_categories: Optional[Sequence[int]] = None,
+        id: Optional[int] = None,
+        uploaded: Optional[bool] = None,
+        uploaded_time: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         if geo_location is not None and not isinstance(geo_location, GeoLocation):
             raise TypeError("FileMetadata.geo_location should be of type GeoLocation")
         self.external_id = external_id
         self.name = name
         self.directory = directory
         self.source = source
@@ -86,15 +86,15 @@
         self.uploaded = uploaded
         self.uploaded_time = uploaded_time
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> FileMetadata:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> FileMetadata:
         instance = super()._load(resource, cognite_client)
         instance.labels = Label._load_list(instance.labels)
         if instance.geo_location is not None:
             instance.geo_location = GeoLocation._load(instance.geo_location)
         return instance
 
 
@@ -121,33 +121,33 @@
         directory_prefix (str): Filter by this (case-sensitive) prefix for the directory provided by the client.
         uploaded (bool): Whether or not the actual file is uploaded. This field is returned only by the API, it has no effect in a post body.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        mime_type: str = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        data_set_ids: Sequence[Dict[str, Any]] = None,
-        labels: LabelFilter = None,
-        geo_location: GeoLocationFilter = None,
-        asset_subtree_ids: Sequence[Dict[str, Any]] = None,
-        source: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        uploaded_time: Union[Dict[str, Any], TimestampRange] = None,
-        source_created_time: Dict[str, Any] = None,
-        source_modified_time: Dict[str, Any] = None,
-        external_id_prefix: str = None,
-        directory_prefix: str = None,
-        uploaded: bool = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        mime_type: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        data_set_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        labels: Optional[LabelFilter] = None,
+        geo_location: Optional[GeoLocationFilter] = None,
+        asset_subtree_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        source: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        uploaded_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        source_created_time: Optional[Dict[str, Any]] = None,
+        source_modified_time: Optional[Dict[str, Any]] = None,
+        external_id_prefix: Optional[str] = None,
+        directory_prefix: Optional[str] = None,
+        uploaded: Optional[bool] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.mime_type = mime_type
         self.metadata = metadata
         self.asset_ids = asset_ids
         self.asset_external_ids = asset_external_ids
         self.data_set_ids = data_set_ids
@@ -284,15 +284,15 @@
 class FileAggregate(dict):
     """Aggregation results for files
 
     Args:
         count (int): Number of filtered items included in aggregation
     """
 
-    def __init__(self, count: int = None, **kwargs: Any) -> None:
+    def __init__(self, count: Optional[int] = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
 class FileMetadataList(CogniteResourceList[FileMetadata]):
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/functions.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,32 +35,32 @@
         metadata(Dict[str, str): Metadata associated with a function as a set of key:value pairs.
         error(Dict[str, str]): Dictionary with keys "message" and "trace", which is populated if deployment fails.
         cognite_client (CogniteClient): An optional CogniteClient to associate with this data class.
     """
 
     def __init__(
         self,
-        id: int = None,
-        name: str = None,
-        external_id: str = None,
-        description: str = None,
-        owner: str = None,
-        status: str = None,
-        file_id: int = None,
-        function_path: str = None,
-        created_time: int = None,
-        secrets: Dict = None,
-        env_vars: Dict = None,
-        cpu: Number = None,
-        memory: Number = None,
-        runtime: str = None,
-        runtime_version: str = None,
-        metadata: Dict = None,
-        error: Dict = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        name: Optional[str] = None,
+        external_id: Optional[str] = None,
+        description: Optional[str] = None,
+        owner: Optional[str] = None,
+        status: Optional[str] = None,
+        file_id: Optional[int] = None,
+        function_path: Optional[str] = None,
+        created_time: Optional[int] = None,
+        secrets: Optional[Dict] = None,
+        env_vars: Optional[Dict] = None,
+        cpu: Optional[Number] = None,
+        memory: Optional[Number] = None,
+        runtime: Optional[str] = None,
+        runtime_version: Optional[str] = None,
+        metadata: Optional[Dict] = None,
+        error: Optional[Dict] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.id = cast(int, id)
         self.name = cast(str, name)
         self.external_id = external_id
         self.description = description
         self.owner = owner
         self.status = status
@@ -164,36 +164,36 @@
             latest_value = getattr(latest, attribute)
             setattr(self, attribute, latest_value)
 
 
 class FunctionFilter(CogniteFilter):
     def __init__(
         self,
-        name: str = None,
-        owner: str = None,
-        file_id: int = None,
-        status: str = None,
-        external_id_prefix: str = None,
-        created_time: Union[Dict[str, int], TimestampRange] = None,
+        name: Optional[str] = None,
+        owner: Optional[str] = None,
+        file_id: Optional[int] = None,
+        status: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
     ) -> None:
         self.name = name
         self.owner = owner
         self.file_id = file_id
         self.status = status
         self.external_id_prefix = external_id_prefix
         self.created_time = created_time
 
 
 class FunctionCallsFilter(CogniteFilter):
     def __init__(
         self,
-        status: str = None,
-        schedule_id: int = None,
-        start_time: Union[Dict[str, int], TimestampRange] = None,
-        end_time: Union[Dict[str, int], TimestampRange] = None,
+        status: Optional[str] = None,
+        schedule_id: Optional[int] = None,
+        start_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
+        end_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
     ) -> None:
         self.status = status
         self.schedule_id = schedule_id
         self.start_time = start_time
         self.end_time = end_time
 
 
@@ -211,24 +211,24 @@
         session_id (int): ID of the session running with the schedule.
         when (str): When the schedule will trigger, in human readable text (server generated from cron_expression).
         cognite_client (CogniteClient): An optional CogniteClient to associate with this data class.
     """
 
     def __init__(
         self,
-        id: int = None,
-        name: str = None,
-        function_id: str = None,
-        function_external_id: str = None,
-        description: str = None,
-        created_time: int = None,
-        cron_expression: str = None,
-        session_id: int = None,
-        when: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        name: Optional[str] = None,
+        function_id: Optional[str] = None,
+        function_external_id: Optional[str] = None,
+        description: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cron_expression: Optional[str] = None,
+        session_id: Optional[int] = None,
+        when: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.id = id
         self.name = name
         self.function_id = function_id
         self.function_external_id = function_external_id
         self.description = description
         self.cron_expression = cron_expression
@@ -247,19 +247,19 @@
         """
         return self._cognite_client.functions.schedules.get_input_data(id=self.id)
 
 
 class FunctionSchedulesFilter(CogniteFilter):
     def __init__(
         self,
-        name: str = None,
-        function_id: int = None,
-        function_external_id: str = None,
-        created_time: Union[Dict[str, int], TimestampRange] = None,
-        cron_expression: str = None,
+        name: Optional[str] = None,
+        function_id: Optional[int] = None,
+        function_external_id: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, int], TimestampRange]] = None,
+        cron_expression: Optional[str] = None,
     ) -> None:
         self.name = name
         self.function_id = function_id
         self.function_external_id = function_external_id
         self.created_time = created_time
         self.cron_expression = cron_expression
 
@@ -284,23 +284,23 @@
         schedule_id (int): The schedule id belonging to the call.
         error (dict): Error from the function call. It contains an error message and the stack trace.
         cognite_client (CogniteClient): An optional CogniteClient to associate with this data class.
     """
 
     def __init__(
         self,
-        id: int = None,
-        start_time: int = None,
-        end_time: int = None,
-        scheduled_time: int = None,
-        status: str = None,
-        schedule_id: int = None,
-        error: dict = None,
-        function_id: int = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        scheduled_time: Optional[int] = None,
+        status: Optional[str] = None,
+        schedule_id: Optional[int] = None,
+        error: Optional[dict] = None,
+        function_id: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.id = id
         self.start_time = start_time
         self.end_time = end_time
         self.scheduled_time = scheduled_time
         self.status = status
         self.schedule_id = schedule_id
@@ -351,17 +351,17 @@
     Args:
         timestamp (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         message (str): Single line from stdout / stderr.
     """
 
     def __init__(
         self,
-        timestamp: int = None,
-        message: str = None,
-        cognite_client: CogniteClient = None,
+        timestamp: Optional[int] = None,
+        message: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.timestamp = timestamp
         self.message = message
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class FunctionCallLog(CogniteResourceList[FunctionCallLogEntry]):
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/geospatial.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 
 
 class FeatureType(CogniteResource):
     """A representation of a feature type in the geospatial api."""
 
     def __init__(
         self,
-        external_id: str = None,
-        data_set_id: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        properties: Dict[str, Any] = None,
-        search_spec: Dict[str, Any] = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        data_set_id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        properties: Optional[Dict[str, Any]] = None,
+        search_spec: Optional[Dict[str, Any]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.data_set_id = data_set_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self.properties = properties
         self.search_spec = search_spec
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None) -> FeatureType:
+    def _load(cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None) -> FeatureType:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
@@ -53,29 +53,31 @@
     _RESOURCE = FeatureType
 
 
 class PropertyAndSearchSpec:
     """A representation of a feature type property and search spec."""
 
     def __init__(
-        self, properties: Union[Dict[str, Any], List[str]] = None, search_spec: Union[Dict[str, Any], List[str]] = None
+        self,
+        properties: Optional[Union[Dict[str, Any], List[str]]] = None,
+        search_spec: Optional[Union[Dict[str, Any], List[str]]] = None,
     ):
         self.properties = properties
         self.search_spec = search_spec
 
 
 class FeatureTypeUpdate:
     """A representation of a feature type update in the geospatial api."""
 
     def __init__(
         self,
-        external_id: str = None,
-        add: PropertyAndSearchSpec = None,
-        remove: PropertyAndSearchSpec = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        add: Optional[PropertyAndSearchSpec] = None,
+        remove: Optional[PropertyAndSearchSpec] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.add = add if add is not None else PropertyAndSearchSpec()
         self.remove = remove if remove is not None else PropertyAndSearchSpec()
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
@@ -97,22 +99,24 @@
 
 
 class Feature(CogniteResource):
     """A representation of a feature in the geospatial api."""
 
     PRE_DEFINED_SNAKE_CASE_NAMES = {to_snake_case(key) for key in RESERVED_PROPERTIES}
 
-    def __init__(self, external_id: str = None, cognite_client: CogniteClient = None, **properties: Any):
+    def __init__(
+        self, external_id: Optional[str] = None, cognite_client: Optional[CogniteClient] = None, **properties: Any
+    ):
         self.external_id = external_id
         for key in properties:
             setattr(self, key, properties[key])
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None) -> Feature:
+    def _load(cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None) -> Feature:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             # Keep properties defined in Feature Type as is
             normalized_key = _to_feature_property_name(key)
             setattr(instance, normalized_key, value)
@@ -207,15 +211,15 @@
         return geopandas.GeoDataFrame(df, geometry=geometry)
 
     @staticmethod
     def from_geopandas(
         feature_type: FeatureType,
         geodataframe: geopandas.GeoDataFrame,
         external_id_column: str = "externalId",
-        property_column_mapping: Dict[str, str] = None,
+        property_column_mapping: Optional[Dict[str, str]] = None,
         data_set_id_column: str = "dataSetId",
     ) -> FeatureList:
         """Convert a GeoDataFrame instance into a FeatureList.
 
         Args:
             feature_type (FeatureType): The feature type the features will conform to
             geodataframe (GeoDataFrame): the geodataframe instance to convert into features
@@ -283,19 +287,21 @@
 
     return None if is_scalar(column_value) and isna(column_value) else column_value
 
 
 class FeatureAggregate(CogniteResource):
     """A result of aggregating features in geospatial api."""
 
-    def __init__(self, cognite_client: CogniteClient = None):
+    def __init__(self, cognite_client: Optional[CogniteClient] = None):
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None) -> FeatureAggregate:
+    def _load(
+        cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None
+    ) -> FeatureAggregate:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
@@ -305,24 +311,28 @@
     _RESOURCE = FeatureAggregate
 
 
 class CoordinateReferenceSystem(CogniteResource):
     """A representation of a feature in the geospatial api."""
 
     def __init__(
-        self, srid: int = None, wkt: str = None, proj_string: str = None, cognite_client: CogniteClient = None
+        self,
+        srid: Optional[int] = None,
+        wkt: Optional[str] = None,
+        proj_string: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.srid = srid
         self.wkt = wkt
         self.proj_string = proj_string
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
     def _load(
-        cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None
+        cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None
     ) -> CoordinateReferenceSystem:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
@@ -345,15 +355,15 @@
     """Raster metadata"""
 
     def __init__(self, **properties: Any):
         for key in properties:
             setattr(self, key, properties[key])
 
     @classmethod
-    def _load(cls, resource: Dict, cognite_client: CogniteClient = None) -> RasterMetadata:
+    def _load(cls, resource: Dict, cognite_client: Optional[CogniteClient] = None) -> RasterMetadata:
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
 
 
@@ -395,21 +405,21 @@
             "ewkt": self.ewkt,
         }
 
 
 class GeospatialComputedItem(CogniteResource):
     """A representation of an item computed from geospatial."""
 
-    def __init__(self, resource: Dict[str, Any], cognite_client: CogniteClient = None):
+    def __init__(self, resource: Dict[str, Any], cognite_client: Optional[CogniteClient] = None):
         self.resource = resource
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
     def _load(
-        cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None
+        cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None
     ) -> GeospatialComputedItem:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         instance = cls(resource=resource, cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
@@ -420,21 +430,21 @@
     "A list of items computed from geospatial."
     _RESOURCE = GeospatialComputedItem
 
 
 class GeospatialComputedResponse(CogniteResource):
     "The geospatial compute response."
 
-    def __init__(self, computed_item_list: GeospatialComputedItemList, cognite_client: CogniteClient = None):
+    def __init__(self, computed_item_list: GeospatialComputedItemList, cognite_client: Optional[CogniteClient] = None):
         self.items = computed_item_list
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
     def _load(
-        cls, resource: Union[str, Dict[str, Any]], cognite_client: CogniteClient = None
+        cls, resource: Union[str, Dict[str, Any]], cognite_client: Optional[CogniteClient] = None
     ) -> GeospatialComputedResponse:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         item_list = GeospatialComputedItemList._load(
             cast("List[Any]", resource.get("items")), cognite_client=cognite_client
         )
         instance = cls(item_list, cognite_client=cognite_client)
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/iam.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/iam.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, cast
 
 from cognite.client.data_classes._base import CogniteResource, CogniteResourceList, CogniteResponse
 from cognite.client.utils._text import convert_all_keys_to_camel_case
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
 
@@ -22,22 +22,22 @@
         metadata (Dict[str, Any]): Custom, immutable application specific metadata. String key -> String value. Limits:
         Key are at most 32 bytes. Values are at most 512 bytes. Up to 16 key-value pairs. Total size is at most 4096.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        source_id: str = None,
-        capabilities: List[Dict[str, Any]] = None,
-        id: int = None,
-        is_deleted: bool = None,
-        deleted_time: int = None,
-        metadata: Dict[str, Any] = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        source_id: Optional[str] = None,
+        capabilities: Optional[List[Dict[str, Any]]] = None,
+        id: Optional[int] = None,
+        is_deleted: Optional[bool] = None,
+        deleted_time: Optional[int] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.source_id = source_id
         self.capabilities = capabilities
         self.id = id
         self.is_deleted = is_deleted
         self.deleted_time = deleted_time
@@ -54,15 +54,17 @@
 
     Args:
         name (str): Name of the security category
         id (int): Id of the security category
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
-    def __init__(self, name: str = None, id: int = None, cognite_client: CogniteClient = None):
+    def __init__(
+        self, name: Optional[str] = None, id: Optional[int] = None, cognite_client: Optional[CogniteClient] = None
+    ):
         self.name = name
         self.id = id
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class SecurityCategoryList(CogniteResourceList[SecurityCategory]):
     _RESOURCE = SecurityCategory
@@ -127,20 +129,20 @@
         status (str): Current status of the session.
         nonce (str): Nonce to be passed to the internal service that will bind the session
         client_id (str): Client ID in identity provider. Returned only if the session was created using client credentials
     """
 
     def __init__(
         self,
-        id: int = None,
-        type: str = None,
-        status: str = None,
-        nonce: str = None,
-        client_id: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        type: Optional[str] = None,
+        status: Optional[str] = None,
+        nonce: Optional[str] = None,
+        client_id: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.type = type
         self.status = status
         self.nonce = nonce
         self.client_id = client_id
 
@@ -155,21 +157,21 @@
         creation_time (int): Session creation time, in milliseconds since 1970
         expiration_time (int): Session expiry time, in milliseconds since 1970. This value is updated on refreshing a token
         client_id (str): Client ID in identity provider. Returned only if the session was created using client credentials
     """
 
     def __init__(
         self,
-        id: int = None,
-        type: str = None,
-        status: str = None,
-        creation_time: int = None,
-        expiration_time: int = None,
-        client_id: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        type: Optional[str] = None,
+        status: Optional[str] = None,
+        creation_time: Optional[int] = None,
+        expiration_time: Optional[int] = None,
+        client_id: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.type = type
         self.status = status
         self.creation_time = creation_time
         self.expiration_time = expiration_time
         self.client_id = client_id
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/labels.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/labels.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         data_set_id (int): The id of the dataset this label belongs to.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        name: str = None,
-        description: str = None,
-        created_time: int = None,
-        data_set_id: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        created_time: Optional[int] = None,
+        data_set_id: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.name = name
         self.description = description
         self.created_time = created_time
         self.data_set_id = data_set_id
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -51,18 +51,18 @@
         external_id_prefix (str): filter label definitions with external ids starting with the prefix specified
         data_set_ids (List[Dict[str, Any]]): Only include labels that belong to these datasets.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        external_id_prefix: str = None,
-        data_set_ids: List[Dict[str, Any]] = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        data_set_ids: Optional[List[Dict[str, Any]]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.external_id_prefix = external_id_prefix
         self.data_set_ids = data_set_ids
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
@@ -73,15 +73,15 @@
 class Label(dict):
     """A label assigned to a resource.
 
     Args:
         external_id (str): The external id to the attached label.
     """
 
-    def __init__(self, external_id: str = None, **kwargs: Any):
+    def __init__(self, external_id: Optional[str] = None, **kwargs: Any):
         self.external_id = external_id
         self.update(kwargs)
 
     external_id = CognitePropertyClassUtil.declare_property("externalId")
 
     @classmethod
     def _load_list(cls, labels: Optional[Sequence[Union[str, dict, LabelDefinition, Label]]]) -> Optional[List[Label]]:
@@ -127,15 +127,18 @@
             List only resources marked as a PUMP or as a VALVE::
 
                 >>> from cognite.client.data_classes import LabelFilter
                 >>> my_label_filter = LabelFilter(contains_any=["PUMP", "VALVE"])
     """
 
     def __init__(
-        self, contains_any: List[str] = None, contains_all: List[str] = None, cognite_client: CogniteClient = None
+        self,
+        contains_any: Optional[List[str]] = None,
+        contains_all: Optional[List[str]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.contains_any = contains_any
         self.contains_all = contains_all
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @staticmethod
     def _wrap_labels(values: Optional[List[str]]) -> Optional[List[Dict[str, str]]]:
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/raw.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,18 +20,18 @@
         columns (Dict[str, Any]): Row data stored as a JSON object.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        key: str = None,
-        columns: Dict[str, Any] = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        key: Optional[str] = None,
+        columns: Optional[Dict[str, Any]] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.key = key
         self.columns = columns
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     def to_pandas(self) -> pandas.DataFrame:  # type: ignore[override]
@@ -62,22 +62,27 @@
 
     Args:
         name (str): Unique name of the table
         created_time (int): Time the table was created.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
-    def __init__(self, name: str = None, created_time: int = None, cognite_client: CogniteClient = None):
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
+    ):
         self.name = name
         self.created_time = created_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
         self._db_name: Optional[str] = None
 
-    def rows(self, key: str = None, limit: int = None) -> Union[Row, RowList]:
+    def rows(self, key: Optional[str] = None, limit: Optional[int] = None) -> Union[Row, RowList]:
         """Get the rows in this table.
 
         Args:
             key (str): Specify a key to return only that row.
             limit (int): The number of rows to return.
 
         Returns:
@@ -97,20 +102,25 @@
 
     Args:
         name (str): Unique name of a database.
         created_time (int): Time the database was created.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
-    def __init__(self, name: str = None, created_time: int = None, cognite_client: CogniteClient = None):
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
+    ):
         self.name = name
         self.created_time = created_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
-    def tables(self, limit: int = None) -> TableList:
+    def tables(self, limit: Optional[int] = None) -> TableList:
         """Get the tables in this database.
 
         Args:
             limit (int): The number of tables to return.
 
         Returns:
             TableList: List of tables in this database.
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/relationships.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     _RESOURCE_TYPES = frozenset({"asset", "timeseries", "file", "event", "sequence"})
 
     def __init__(
         self,
-        external_id: str = None,
-        source_external_id: str = None,
-        source_type: str = None,
-        source: Union[Asset, TimeSeries, FileMetadata, Sequence, Event, Dict] = None,
-        target_external_id: str = None,
-        target_type: str = None,
-        target: Union[Asset, TimeSeries, FileMetadata, Sequence, Event, Dict] = None,
-        start_time: int = None,
-        end_time: int = None,
-        confidence: float = None,
-        data_set_id: int = None,
-        labels: SequenceType[Union[Label, str, LabelDefinition, dict]] = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        external_id: Optional[str] = None,
+        source_external_id: Optional[str] = None,
+        source_type: Optional[str] = None,
+        source: Optional[Union[Asset, TimeSeries, FileMetadata, Sequence, Event, Dict]] = None,
+        target_external_id: Optional[str] = None,
+        target_type: Optional[str] = None,
+        target: Optional[Union[Asset, TimeSeries, FileMetadata, Sequence, Event, Dict]] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+        confidence: Optional[float] = None,
+        data_set_id: Optional[int] = None,
+        labels: Optional[SequenceType[Union[Label, str, LabelDefinition, dict]]] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.source_external_id = source_external_id
         self.source_type = source_type
         self.source = source
         self.target_external_id = target_external_id
         self.target_type = target_type
@@ -87,15 +87,15 @@
         return rel
 
     def _validate_resource_type(self, resource_type: Optional[str]) -> None:
         if resource_type is None or resource_type.lower() not in self._RESOURCE_TYPES:
             raise TypeError(f"Invalid source or target '{resource_type}' in relationship")
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> Relationship:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> Relationship:
         instance = super()._load(resource, cognite_client)
         if instance.source is not None:
             instance.source = instance._convert_resource(instance.source, instance.source_type)  # type: ignore
         if instance.target is not None:
             instance.target = instance._convert_resource(instance.target, instance.target_type)  # type: ignore
         instance.labels = Label._load_list(instance.labels)
         return instance
@@ -132,27 +132,27 @@
         active_at_time (Dict[str, int]): Limits results to those active at any point within the given time range, i.e. if there is any overlap in the intervals [activeAtTime.min, activeAtTime.max] and [startTime, endTime], where both intervals are inclusive. If a relationship does not have a startTime, it is regarded as active from the begining of time by this filter. If it does not have an endTime is will be regarded as active until the end of time. Similarly, if a min is not supplied to the filter, the min will be implicitly set to the beginning of time, and if a max is not supplied, the max will be implicitly set to the end of time.
         labels (LabelFilter): Return only the resource matching the specified label constraints.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        source_external_ids: SequenceType[str] = None,
-        source_types: SequenceType[str] = None,
-        target_external_ids: SequenceType[str] = None,
-        target_types: SequenceType[str] = None,
-        data_set_ids: SequenceType[Dict[str, Any]] = None,
-        start_time: Dict[str, int] = None,
-        end_time: Dict[str, int] = None,
-        confidence: Dict[str, int] = None,
-        last_updated_time: Dict[str, int] = None,
-        created_time: Dict[str, int] = None,
-        active_at_time: Dict[str, int] = None,
-        labels: LabelFilter = None,
-        cognite_client: CogniteClient = None,
+        source_external_ids: Optional[SequenceType[str]] = None,
+        source_types: Optional[SequenceType[str]] = None,
+        target_external_ids: Optional[SequenceType[str]] = None,
+        target_types: Optional[SequenceType[str]] = None,
+        data_set_ids: Optional[SequenceType[Dict[str, Any]]] = None,
+        start_time: Optional[Dict[str, int]] = None,
+        end_time: Optional[Dict[str, int]] = None,
+        confidence: Optional[Dict[str, int]] = None,
+        last_updated_time: Optional[Dict[str, int]] = None,
+        created_time: Optional[Dict[str, int]] = None,
+        active_at_time: Optional[Dict[str, int]] = None,
+        labels: Optional[LabelFilter] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.source_external_ids = source_external_ids
         self.source_types = source_types
         self.target_external_ids = target_external_ids
         self.target_types = target_types
         self.data_set_ids = data_set_ids
         self.start_time = start_time
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/sequences.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import json
 import math
-from typing import TYPE_CHECKING, Any, Dict, Generator, List, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple, Union, cast
 from typing import Sequence as SequenceType
 
 from cognite.client import utils
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteLabelUpdate,
     CogniteListUpdate,
@@ -42,25 +42,25 @@
         last_updated_time (int): The last time this sequence was updated in CDF, in milliseconds since Jan 1, 1970.
         data_set_id (int): Data set that this sequence belongs to
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        name: str = None,
-        description: str = None,
-        asset_id: int = None,
-        external_id: str = None,
-        metadata: Dict[str, Any] = None,
-        columns: SequenceType[Dict[str, Any]] = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        data_set_id: int = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        asset_id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        columns: Optional[SequenceType[Dict[str, Any]]] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        data_set_id: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.name = name
         self.description = description
         self.asset_id = asset_id
         self.external_id = external_id
         self.metadata = metadata
@@ -113,23 +113,23 @@
         last_updated_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
         data_set_ids (SequenceType[Dict[str, Any]]): Only include sequences that belong to these datasets.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        external_id_prefix: str = None,
-        metadata: Dict[str, Any] = None,
-        asset_ids: SequenceType[int] = None,
-        asset_subtree_ids: SequenceType[Dict[str, Any]] = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        data_set_ids: SequenceType[Dict[str, Any]] = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        external_id_prefix: Optional[str] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        asset_ids: Optional[SequenceType[int]] = None,
+        asset_subtree_ids: Optional[SequenceType[Dict[str, Any]]] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        data_set_ids: Optional[SequenceType[Dict[str, Any]]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.external_id_prefix = external_id_prefix
         self.metadata = metadata
         self.asset_ids = asset_ids
         self.asset_subtree_ids = asset_subtree_ids
         self.created_time = created_time
@@ -279,15 +279,15 @@
 class SequenceAggregate(dict):
     """No description.
 
     Args:
         count (int): No description.
     """
 
-    def __init__(self, count: int = None, **kwargs: Any):
+    def __init__(self, count: Optional[int] = None, **kwargs: Any):
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
 class SequenceList(CogniteResourceList[Sequence]):
@@ -304,20 +304,20 @@
         row_numbers (SequenceType[int]): The data row numbers.
         values (SequenceType[SequenceType[ Union[int, str, float]]]): The data values, one row at a time.
         columns: SequenceType[dict]: The column information, in the format returned by the API.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        rows: SequenceType[dict] = None,
-        row_numbers: SequenceType[int] = None,
-        values: SequenceType[SequenceType[Union[int, str, float]]] = None,
-        columns: SequenceType[Dict[str, Any]] = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        rows: Optional[SequenceType[dict]] = None,
+        row_numbers: Optional[SequenceType[int]] = None,
+        values: Optional[SequenceType[SequenceType[Union[int, str, float]]]] = None,
+        columns: Optional[SequenceType[Dict[str, Any]]] = None,
     ):
         if rows:
             row_numbers = [r["rowNumber"] for r in rows]
             values = [r["values"] for r in rows]
         self.id = id
         self.external_id = external_id
         self.row_numbers = row_numbers or []
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/shared.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Literal, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 from cognite.client.data_classes._base import CognitePropertyClassUtil
 from cognite.client.utils._text import convert_all_keys_to_camel_case
 
 
 class TimestampRange(dict):
     """Range between two timestamps.
 
     Args:
         max (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         min (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
     """
 
-    def __init__(self, max: int = None, min: int = None, **kwargs: Any):
+    def __init__(self, max: Optional[int] = None, min: Optional[int] = None, **kwargs: Any):
         self.max = max
         self.min = min
         self.update(kwargs)
 
     max = CognitePropertyClassUtil.declare_property("max")
     min = CognitePropertyClassUtil.declare_property("min")
 
@@ -26,41 +26,41 @@
 class AggregateResult(dict):
     """Aggregation group
 
     Args:
         count (int): Size of the aggregation group
     """
 
-    def __init__(self, count: int = None, **kwargs: Any):
+    def __init__(self, count: Optional[int] = None, **kwargs: Any):
         super().__init__(count=count, **kwargs)
         self.count = count
 
 
 class AggregateUniqueValuesResult(AggregateResult):
     """Aggregation group
 
     Args:
         count (int): Size of the aggregation group
         value (Union(int, str)): A unique value from the requested field
     """
 
-    def __init__(self, count: int = None, value: Union[int, str] = None, **kwargs: Any):
+    def __init__(self, count: Optional[int] = None, value: Optional[Union[int, str]] = None, **kwargs: Any):
         super().__init__(count=count, value=value, **kwargs)
         self.value = value
 
 
 class AggregateBucketResult(AggregateResult):
     """Aggregation group
 
     Args:
         count (int): Size of the bucket
         value (Union(int, str)): A unique value for the bucket
     """
 
-    def __init__(self, count: int = None, value: Union[int, str] = None, **kwargs: Any):
+    def __init__(self, count: Optional[int] = None, value: Optional[Union[int, str]] = None, **kwargs: Any):
         super().__init__(count=count, value=value, **kwargs)
         self.value = value
 
 
 class Geometry(dict):
     """Represents the points, curves and surfaces in the coordinate space.
 
@@ -164,15 +164,15 @@
     Args: type (str): The GeoJSON type. Currently only 'Feature' is supported.
           geometry (object): The geometry type. One of 'Point', 'MultiPoint, 'LineString', 'MultiLineString', 'Polygon', or 'MultiPolygon'.
           properties (object): Optional additional properties in a String key -> Object value format.
     """
 
     _VALID_TYPES = frozenset({"Feature"})
 
-    def __init__(self, type: Literal["Feature"], geometry: Geometry, properties: dict = None):
+    def __init__(self, type: Literal["Feature"], geometry: Geometry, properties: Optional[dict] = None):
         if type not in self._VALID_TYPES:
             raise ValueError("Only the 'Feature' type is supported.")
         self.type = type
         self.geometry = geometry
         self.properties = properties
 
     type = CognitePropertyClassUtil.declare_property("type")
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/templates.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,21 @@
         description (str): The description of the template groups.
         owners (List[str]): The list of owners for the template groups.
         data_set_id (int): The dataSet which this Template Group belongs to
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        description: str = None,
+        external_id: Optional[str] = None,
+        description: Optional[str] = None,
         owners: Optional[List[str]] = None,
-        data_set_id: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        data_set_id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.description = description
         self.owners = owners
         self.data_set_id = data_set_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
@@ -68,20 +68,20 @@
         schema (str): The GraphQL schema.
         version (int): Incremented by the server whenever the schema of a template groups changes.
         conflict_mode (str): Can be set to 'Patch', 'Update' or 'Force'.
     """
 
     def __init__(
         self,
-        schema: str = None,
-        version: int = None,
-        conflict_mode: str = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        schema: Optional[str] = None,
+        version: Optional[int] = None,
+        conflict_mode: Optional[str] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.schema = schema
         self.version = version
         self.conflict_mode = conflict_mode
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -94,15 +94,15 @@
 class ConstantResolver(CogniteResource):
     """Resolves a field to a constant value. The value can be of any supported JSON type.
 
     Args:
         value (any): The value of the field.
     """
 
-    def __init__(self, value: Any = None, cognite_client: CogniteClient = None):
+    def __init__(self, value: Optional[Any] = None, cognite_client: Optional[CogniteClient] = None):
         self.type = "constant"
         self.value = value
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class RawResolver(CogniteResource):
     """Resolves a field to a RAW column.
@@ -112,19 +112,19 @@
         table_name (str): The table name.
         row_key (str): The row key.
         column_name (str): The column to fetch the value from.
     """
 
     def __init__(
         self,
-        db_name: str = None,
-        table_name: str = None,
-        row_key: str = None,
-        column_name: str = None,
-        cognite_client: CogniteClient = None,
+        db_name: Optional[str] = None,
+        table_name: Optional[str] = None,
+        row_key: Optional[str] = None,
+        column_name: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.type = "raw"
         self.db_name = db_name
         self.table_name = table_name
         self.row_key = row_key
         self.column_name = column_name
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -141,22 +141,22 @@
         is_step (Optional[bool]): Specifies if the synthetic time series is step based.
         is_string (Optional[bool]): Specifies if the synthetic time series returned contains string values.
         unit (Optional[str]): The unit of the time series.
     """
 
     def __init__(
         self,
-        expression: str = None,
+        expression: Optional[str] = None,
         name: Optional[str] = None,
         description: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
         is_step: Optional[bool] = None,
         is_string: Optional[bool] = None,
         unit: Optional[str] = None,
-        cognite_client: CogniteClient = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.type = "syntheticTimeSeries"
         self.expression = expression
         self.name = name
         self.description = description
         self.metadata = metadata
         self.is_step = is_step
@@ -170,15 +170,18 @@
 
     Args:
         external_id (str): The external id of the view.
         input (Optional[Dict[str, any]]): The input used to resolve the view.
     """
 
     def __init__(
-        self, external_id: str = None, input: Optional[Dict[str, Any]] = None, cognite_client: CogniteClient = None
+        self,
+        external_id: Optional[str] = None,
+        input: Optional[Dict[str, Any]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.type = "view"
         self.external_id = external_id
         self.input = input
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
@@ -195,21 +198,21 @@
         data_set_id (int): The id of the dataset this instance belongs to.
         created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        template_name: str = None,
-        field_resolvers: Dict[str, FieldResolvers] = None,
+        external_id: Optional[str] = None,
+        template_name: Optional[str] = None,
+        field_resolvers: Optional[Dict[str, FieldResolvers]] = None,
         data_set_id: Optional[int] = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.template_name = template_name
         self.field_resolvers = field_resolvers
         self.data_set_id = data_set_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
@@ -251,15 +254,15 @@
     def _encode_field_resolvers(field_resolvers: Dict[str, FieldResolvers], camel_case: bool) -> Dict[str, Any]:
         return {
             key: value.dump(camel_case=camel_case) if not isinstance(value, str) else value
             for key, value in field_resolvers.items()
         }
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> TemplateInstance:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> TemplateInstance:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         elif isinstance(resource, Dict):
             instance = cls(cognite_client=cognite_client)
             for key, value in resource.items():
                 snake_case_key = to_snake_case(key)
                 if hasattr(instance, snake_case_key):
@@ -274,15 +277,15 @@
                         )
                     else:
                         setattr(instance, snake_case_key, value)
             return instance
         raise TypeError(f"Resource must be json str or dict, not {type(resource)}")
 
     @staticmethod
-    def _field_resolver_load(resource: Dict, cognite_client: CogniteClient = None) -> CogniteResource:
+    def _field_resolver_load(resource: Dict, cognite_client: Optional[CogniteClient] = None) -> CogniteResource:
         return TemplateInstance.field_resolver_mapper[resource["type"]]._load(resource, cognite_client)
 
 
 class TemplateInstanceUpdate(CogniteUpdate):
     """Changes applied to template instance
 
     Args:
@@ -312,18 +315,18 @@
         type (str): The type of source. Possible values are: "events", "assets", "sequences", "timeSeries", "files".
         filter (Dict[str, any]): The filter to apply to the source when resolving the source. A filter also supports binding view input to the filter, by prefixing the input name with '$'.
         mappings (Dict[str, str]): The mapping between source result and expected schema.
     """
 
     def __init__(
         self,
-        type: str = None,
-        filter: Dict[str, Any] = None,
-        mappings: Dict[str, str] = None,
-        cognite_client: CogniteClient = None,
+        type: Optional[str] = None,
+        filter: Optional[Dict[str, Any]] = None,
+        mappings: Optional[Dict[str, str]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.type = type
         self.filter = filter
         self.mappings = mappings
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
@@ -335,20 +338,20 @@
         external_id (str): The external ID provided by the client. Must be unique for the resource type.
         source (Source): Defines the data source for the view.
         data_set_id (Optional[int]): The dataSetId of the view
     """
 
     def __init__(
         self,
-        external_id: str = None,
-        source: Source = None,
+        external_id: Optional[str] = None,
+        source: Optional[Source] = None,
         data_set_id: Optional[int] = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.external_id = external_id
         self.source = source
         self.data_set_id = data_set_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
@@ -378,60 +381,65 @@
     def resolve_nested_classes(value: Union[CogniteResource, Dict], camel_case: bool) -> Dict:
         if isinstance(value, CogniteResource):
             return value.dump(camel_case)
         else:
             return value
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> View:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> View:
         if isinstance(resource, str):
             return cls._load(json.loads(resource), cognite_client=cognite_client)
         elif isinstance(resource, Dict):
             instance = cls(cognite_client=cognite_client)
             for key, value in resource.items():
                 snake_case_key = to_snake_case(key)
                 if hasattr(instance, snake_case_key):
                     value = value if key != "source" else Source._load(value, cognite_client)
                     setattr(instance, snake_case_key, value)
             return instance
         raise TypeError(f"Resource must be json str or dict, not {type(resource)}")
 
 
 class ViewResolveItem(UserDict, CogniteResource):
-    def __init__(self, data: Dict[str, Any], cognite_client: CogniteClient = None) -> None:
+    def __init__(self, data: Dict[str, Any], cognite_client: Optional[CogniteClient] = None) -> None:
         super().__init__(data)
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     def dump(self, camel_case: bool = False) -> Dict[str, Any]:
         return self.data
 
     @classmethod
-    def _load(cls, data: Union[Dict, str], cognite_client: CogniteClient = None) -> ViewResolveItem:
+    def _load(cls, data: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> ViewResolveItem:
         if isinstance(data, str):
             return cls._load(json.loads(data), cognite_client=cognite_client)
         elif isinstance(data, Dict):
             return cls(data, cognite_client=cognite_client)
 
 
 class GraphQlError(CogniteResource):
     def __init__(
         self,
-        message: str = None,
-        path: List[str] = None,
-        locations: List[Dict[str, Any]] = None,
-        cognite_client: CogniteClient = None,
+        message: Optional[str] = None,
+        path: Optional[List[str]] = None,
+        locations: Optional[List[Dict[str, Any]]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.message = message
         self.path = path
         self.locations = locations
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class GraphQlResponse(CogniteResource):
-    def __init__(self, data: Any = None, errors: List[GraphQlError] = None, cognite_client: CogniteClient = None):
+    def __init__(
+        self,
+        data: Optional[Any] = None,
+        errors: Optional[List[GraphQlError]] = None,
+        cognite_client: Optional[CogniteClient] = None,
+    ):
         self.data = data
         self.errors = errors
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
 class TemplateInstanceList(CogniteResourceList[TemplateInstance]):
     _RESOURCE = TemplateInstance
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/three_d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteLabelUpdate,
     CogniteListUpdate,
     CogniteObjectUpdate,
     CognitePrimitiveUpdate,
     CognitePropertyClassUtil,
@@ -21,15 +21,15 @@
     """Initial camera position and target.
 
     Args:
         target (List[float]): Initial camera target.
         position (List[float]): Initial camera position.
     """
 
-    def __init__(self, target: List[float] = None, position: List[float] = None, **kwargs: Any):
+    def __init__(self, target: Optional[List[float]] = None, position: Optional[List[float]] = None, **kwargs: Any):
         self.target = target
         self.position = position
         self.update(kwargs)
 
     target = CognitePropertyClassUtil.declare_property("target")
     position = CognitePropertyClassUtil.declare_property("position")
 
@@ -38,15 +38,15 @@
     """The bounding box of the subtree with this sector as the root sector. Is null if there are no geometries in the subtree.
 
     Args:
         max (List[float]): No description.
         min (List[float]): No description.
     """
 
-    def __init__(self, max: List[float] = None, min: List[float] = None, **kwargs: Any):
+    def __init__(self, max: Optional[List[float]] = None, min: Optional[List[float]] = None, **kwargs: Any):
         self.max = max
         self.min = min
         self.update(kwargs)
 
     max = CognitePropertyClassUtil.declare_property("max")
     min = CognitePropertyClassUtil.declare_property("min")
 
@@ -60,19 +60,19 @@
         created_time (int): The creation time of the resource, in milliseconds since January 1, 1970 at 00:00 UTC.
         metadata (Dict[str, str]): Custom, application specific metadata. String key -> String value. Limits: Maximum length of key is 32 bytes, value 512 bytes, up to 16 key-value pairs.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        id: int = None,
-        created_time: int = None,
-        metadata: Dict[str, str] = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.id = id
         self.created_time = created_time
         self.metadata = metadata
         self._cognite_client = cast("CogniteClient", cognite_client)
 
@@ -144,26 +144,26 @@
         asset_mapping_count (int): The number of asset mappings for this revision.
         created_time (int): The creation time of the resource, in milliseconds since January 1, 1970 at 00:00 UTC.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        file_id: int = None,
-        published: bool = None,
-        rotation: List[float] = None,
-        camera: Union[Dict[str, Any], RevisionCameraProperties] = None,
-        status: str = None,
-        metadata: Dict[str, str] = None,
-        thumbnail_threed_file_id: int = None,
-        thumbnail_url: str = None,
-        asset_mapping_count: int = None,
-        created_time: int = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        file_id: Optional[int] = None,
+        published: Optional[bool] = None,
+        rotation: Optional[List[float]] = None,
+        camera: Optional[Union[Dict[str, Any], RevisionCameraProperties]] = None,
+        status: Optional[str] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        thumbnail_threed_file_id: Optional[int] = None,
+        thumbnail_url: Optional[str] = None,
+        asset_mapping_count: Optional[int] = None,
+        created_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.file_id = file_id
         self.published = published
         self.rotation = rotation
         self.camera = camera
         self.status = status
@@ -171,15 +171,15 @@
         self.thumbnail_threed_file_id = thumbnail_threed_file_id
         self.thumbnail_url = thumbnail_url
         self.asset_mapping_count = asset_mapping_count
         self.created_time = created_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> ThreeDModelRevision:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> ThreeDModelRevision:
         instance = super()._load(resource, cognite_client)
         if isinstance(resource, Dict):
             if instance.camera is not None:
                 instance.camera = RevisionCameraProperties(**instance.camera)
         return instance
 
 
@@ -255,36 +255,36 @@
         properties (Dict[str, Dict[str, str]]): Properties extracted from 3D model, with property categories containing key/value string pairs.
         bounding_box (Union[Dict[str, Any], BoundingBox3D]): The bounding box of the subtree with this sector as the root sector. Is null if there are no geometries in the subtree.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        tree_index: int = None,
-        parent_id: int = None,
-        depth: int = None,
-        name: str = None,
-        subtree_size: int = None,
-        properties: Dict[str, Dict[str, str]] = None,
-        bounding_box: Union[Dict[str, Any], BoundingBox3D] = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        tree_index: Optional[int] = None,
+        parent_id: Optional[int] = None,
+        depth: Optional[int] = None,
+        name: Optional[str] = None,
+        subtree_size: Optional[int] = None,
+        properties: Optional[Dict[str, Dict[str, str]]] = None,
+        bounding_box: Optional[Union[Dict[str, Any], BoundingBox3D]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.tree_index = tree_index
         self.parent_id = parent_id
         self.depth = depth
         self.name = name
         self.subtree_size = subtree_size
         self.properties = properties
         self.bounding_box = bounding_box
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> ThreeDNode:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> ThreeDNode:
         instance = super()._load(resource, cognite_client)
         if isinstance(resource, Dict):
             if instance.bounding_box is not None:
                 instance.bounding_box = BoundingBox3D(**instance.bounding_box)
         return instance
 
 
@@ -301,19 +301,19 @@
         tree_index (int): A number describing the position of this node in the 3D hierarchy, starting from 0. The tree is traversed in a depth-first order.
         subtree_size (int): The number of nodes in the subtree of this node (this number included the node itself).
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        node_id: int = None,
-        asset_id: int = None,
-        tree_index: int = None,
-        subtree_size: int = None,
-        cognite_client: CogniteClient = None,
+        node_id: Optional[int] = None,
+        asset_id: Optional[int] = None,
+        tree_index: Optional[int] = None,
+        subtree_size: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.node_id = node_id
         self.asset_id = asset_id
         self.tree_index = tree_index
         self.subtree_size = subtree_size
         self._cognite_client = cast("CogniteClient", cognite_client)
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/time_series.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,29 +42,29 @@
         last_updated_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
         legacy_name (str): Set a value for legacyName to allow applications using API v0.3, v04, v05, and v0.6 to access this time series. The legacy name is the human-readable name for the time series and is mapped to the name field used in API versions 0.3-0.6. The legacyName field value must be unique, and setting this value to an already existing value will return an error. We recommend that you set this field to the same value as externalId.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        name: str = None,
-        is_string: bool = None,
-        metadata: Dict[str, str] = None,
-        unit: str = None,
-        asset_id: int = None,
-        is_step: bool = None,
-        description: str = None,
-        security_categories: Sequence[int] = None,
-        data_set_id: int = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        legacy_name: str = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        unit: Optional[str] = None,
+        asset_id: Optional[int] = None,
+        is_step: Optional[bool] = None,
+        description: Optional[str] = None,
+        security_categories: Optional[Sequence[int]] = None,
+        data_set_id: Optional[int] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        legacy_name: Optional[str] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.external_id = external_id
         self.name = name
         self.is_string = is_string
         self.metadata = metadata
         self.unit = unit
@@ -97,15 +97,15 @@
 
         identifier = Identifier.load(self.id, self.external_id).as_dict()
         dps = self._cognite_client.time_series.data.retrieve(
             **identifier, start=MIN_TIMESTAMP_MS, end=MAX_TIMESTAMP_MS + 1, aggregates="count", granularity="100d"
         )
         return sum(dps.count)
 
-    def latest(self, before: Union[int, str, datetime] = None) -> Optional[Datapoint]:
+    def latest(self, before: Optional[Union[int, str, datetime]] = None) -> Optional[Datapoint]:
         """Returns the latest datapoint in this time series. If empty, returns None.
 
         Returns:
             Datapoint: A datapoint object containing the value and timestamp of the latest datapoint.
         """
         identifier = Identifier.load(self.id, self.external_id).as_dict()
         if dps := self._cognite_client.time_series.data.retrieve_latest(**identifier, before=before):
@@ -154,27 +154,27 @@
         created_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
         last_updated_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        name: str = None,
-        unit: str = None,
-        is_string: bool = None,
-        is_step: bool = None,
-        metadata: Dict[str, str] = None,
-        asset_ids: Sequence[int] = None,
-        asset_external_ids: Sequence[str] = None,
-        asset_subtree_ids: Sequence[Dict[str, Any]] = None,
-        data_set_ids: Sequence[Dict[str, Any]] = None,
-        external_id_prefix: str = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        cognite_client: CogniteClient = None,
+        name: Optional[str] = None,
+        unit: Optional[str] = None,
+        is_string: Optional[bool] = None,
+        is_step: Optional[bool] = None,
+        metadata: Optional[Dict[str, str]] = None,
+        asset_ids: Optional[Sequence[int]] = None,
+        asset_external_ids: Optional[Sequence[str]] = None,
+        asset_subtree_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        data_set_ids: Optional[Sequence[Dict[str, Any]]] = None,
+        external_id_prefix: Optional[str] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.name = name
         self.unit = unit
         self.is_string = is_string
         self.is_step = is_step
         self.metadata = metadata
         self.asset_ids = asset_ids
@@ -276,15 +276,15 @@
 class TimeSeriesAggregate(dict):
     """No description.
 
     Args:
         count (int): No description.
     """
 
-    def __init__(self, count: int = None, **kwargs: Any) -> None:
+    def __init__(self, count: Optional[int] = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
 class TimeSeriesList(CogniteResourceList[TimeSeries]):
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/transformations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,17 @@
         session_id (int): CDF source session ID
         client_id (str): Idp source client ID
         project_name (str): CDF source project name
     """
 
     def __init__(
         self,
-        session_id: int = None,
-        client_id: str = None,
-        project_name: str = None,
+        session_id: Optional[int] = None,
+        client_id: Optional[str] = None,
+        project_name: Optional[str] = None,
     ):
         self.session_id = session_id
         self.client_id = client_id
         self.project_name = project_name
 
     def dump(self, camel_case: bool = False) -> Dict[str, Any]:
         """Dump the instance into a json serializable Python data type.
@@ -93,36 +93,36 @@
         destination_nonce (NonceCredentials): Single use credentials to bind to a CDF session for writing.
         source_session (SessionDetails): Details for the session used to read from the source project.
         destination_session (SessionDetails): Details for the session used to write to the destination project.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        name: str = None,
-        query: str = None,
-        destination: TransformationDestination = None,
-        conflict_mode: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        name: Optional[str] = None,
+        query: Optional[str] = None,
+        destination: Optional[TransformationDestination] = None,
+        conflict_mode: Optional[str] = None,
         is_public: bool = True,
         ignore_null_fields: bool = False,
         source_oidc_credentials: Optional[OidcCredentials] = None,
         destination_oidc_credentials: Optional[OidcCredentials] = None,
         created_time: Optional[int] = None,
         last_updated_time: Optional[int] = None,
-        owner: str = None,
+        owner: Optional[str] = None,
         owner_is_current_user: bool = True,
         has_source_oidc_credentials: Optional[bool] = None,
         has_destination_oidc_credentials: Optional[bool] = None,
-        running_job: TransformationJob = None,
-        last_finished_job: TransformationJob = None,
-        blocked: TransformationBlockedInfo = None,
-        schedule: TransformationSchedule = None,
-        data_set_id: int = None,
-        cognite_client: CogniteClient = None,
+        running_job: Optional[TransformationJob] = None,
+        last_finished_job: Optional[TransformationJob] = None,
+        blocked: Optional[TransformationBlockedInfo] = None,
+        schedule: Optional[TransformationSchedule] = None,
+        data_set_id: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
         source_nonce: Optional[NonceCredentials] = None,
         destination_nonce: Optional[NonceCredentials] = None,
         source_session: Optional[SessionDetails] = None,
         destination_session: Optional[SessionDetails] = None,
         tags: Optional[List[str]] = None,
     ):
         self.id = id
@@ -182,15 +182,17 @@
             self.source_nonce,
             self.destination_nonce,
             self.source_session,
             self.destination_session,
             self.tags,
         )
 
-    def _process_credentials(self, sessions_cache: Dict[str, NonceCredentials] = None, keep_none: bool = False) -> None:
+    def _process_credentials(
+        self, sessions_cache: Optional[Dict[str, NonceCredentials]] = None, keep_none: bool = False
+    ) -> None:
         if sessions_cache is None:
             sessions_cache = {}
 
         def try_get_or_create_nonce(
             oidc_credentials: Optional[OidcCredentials], project: str
         ) -> Optional[NonceCredentials]:
             if keep_none and oidc_credentials is None:
@@ -243,15 +245,15 @@
     def run_async(self, timeout: Optional[float] = None) -> Awaitable[TransformationJob]:
         return self._cognite_client.transformations.run_async(transformation_id=self.id, timeout=timeout)
 
     def jobs(self) -> TransformationJobList:
         return self._cognite_client.transformations.jobs.list(transformation_id=self.id)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> Transformation:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> Transformation:
         instance = super()._load(resource, cognite_client)
         if isinstance(instance.destination, dict):
             instance.destination = _load_destination_dct(instance.destination)
 
         if isinstance(instance.running_job, dict):
             snake_dict = convert_all_keys_to_snake_case(instance.running_job)
             instance.running_job = TransformationJob._load(snake_dict, cognite_client=cognite_client)
@@ -412,15 +414,15 @@
 
             List only resources marked as a PUMP or as a VALVE::
 
                 >>> from cognite.client.data_classes import ContainsAny
                 >>> my_tag_filter = ContainsAny(tags=["PUMP", "VALVE"])
     """
 
-    def __init__(self, tags: List[str] = None):
+    def __init__(self, tags: Optional[List[str]] = None):
         self.tags = tags
 
     def dump(self, camel_case: bool = True) -> Dict[str, Any]:
         contains_any_key = "containsAny" if camel_case else "contains_any"
         return {contains_any_key: self.tags}
 
 
@@ -440,24 +442,24 @@
         data_set_ids (List[Dict[str, Any]]): Return only transformations in the specified data sets with these ids.
         tags (TagsFilter): Return only the resource matching the specified tags constraints. It only supports ContainsAny as of now.
     """
 
     def __init__(
         self,
         include_public: bool = True,
-        name_regex: str = None,
-        query_regex: str = None,
-        destination_type: str = None,
-        conflict_mode: str = None,
-        cdf_project_name: str = None,
-        has_blocked_error: bool = None,
-        created_time: Union[Dict[str, Any], TimestampRange] = None,
-        last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
-        data_set_ids: List[Dict[str, Any]] = None,
-        tags: TagsFilter = None,
+        name_regex: Optional[str] = None,
+        query_regex: Optional[str] = None,
+        destination_type: Optional[str] = None,
+        conflict_mode: Optional[str] = None,
+        cdf_project_name: Optional[str] = None,
+        has_blocked_error: Optional[bool] = None,
+        created_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        last_updated_time: Optional[Union[Dict[str, Any], TimestampRange]] = None,
+        data_set_ids: Optional[List[Dict[str, Any]]] = None,
+        tags: Optional[TagsFilter] = None,
     ):
         self.include_public = include_public
         self.name_regex = name_regex
         self.query_regex = query_regex
         self.destination_type = destination_type
         self.conflict_mode = conflict_mode
         self.has_blocked_error = has_blocked_error
@@ -494,24 +496,26 @@
     Args:
         schema (TransformationSchemaColumnList): List of column descriptions.
         results (List[Dict]): List of resulting rows. Each row is a dictionary where the key is the column name and the value is the entrie.
     """
 
     def __init__(
         self,
-        schema: TransformationSchemaColumnList = None,
-        results: List[Dict] = None,
-        cognite_client: CogniteClient = None,
+        schema: Optional[TransformationSchemaColumnList] = None,
+        results: Optional[List[Dict]] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ) -> None:
         self.schema = schema
         self.results = results
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> TransformationPreviewResult:
+    def _load(
+        cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None
+    ) -> TransformationPreviewResult:
         instance = super()._load(resource, cognite_client)
         if isinstance(instance.schema, Dict):
             items = instance.schema.get("items")
             if items is not None:
                 instance.schema = TransformationSchemaColumnList._load(items, cognite_client=cognite_client)
         if isinstance(instance.results, Dict):
             items = instance.results.get("items")
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/transformations/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TransformationDestination:
     """TransformationDestination has static methods to define the target resource type of a transformation
 
     Args:
         type (str): Used as data type identifier on transformation creation/retrieval.
     """
 
-    def __init__(self, type: str = None):
+    def __init__(self, type: Optional[str] = None):
         self.type = type
 
     def __hash__(self) -> int:
         return hash(self.type)
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, type(self)) and hash(other) == hash(self)
@@ -149,25 +149,25 @@
         Returns:
             Instances: pointing to the target centric data model.
         """
         return Instances(data_model=data_model, instance_space=instance_space)
 
 
 class RawTable(TransformationDestination):
-    def __init__(self, database: str = None, table: str = None):
+    def __init__(self, database: Optional[str] = None, table: Optional[str] = None):
         super().__init__(type="raw")
         self.database = database
         self.table = table
 
     def __hash__(self) -> int:
         return hash((self.type, self.database, self.table))
 
 
 class SequenceRows(TransformationDestination):
-    def __init__(self, external_id: str = None):
+    def __init__(self, external_id: Optional[str] = None):
         super().__init__(type="sequence_rows")
         self.external_id = external_id
 
     def __hash__(self) -> int:
         return hash((self.type, self.external_id))
 
 
@@ -275,20 +275,20 @@
             inst.data_model = DataModelInfo(**convert_all_keys_to_snake_case(inst.data_model))
         return inst
 
 
 class OidcCredentials:
     def __init__(
         self,
-        client_id: str = None,
-        client_secret: str = None,
-        scopes: str = None,
-        token_uri: str = None,
-        audience: str = None,
-        cdf_project_name: str = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        scopes: Optional[str] = None,
+        token_uri: Optional[str] = None,
+        audience: Optional[str] = None,
+        cdf_project_name: Optional[str] = None,
     ):
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.scopes = scopes
         self.token_uri = token_uri
         self.audience = audience
@@ -333,15 +333,15 @@
     """Information about the reason why and when a transformation is blocked.
 
     Args:
         reason (str): Reason why the transformation is blocked.
         created_time (Optional[int]): Timestamp when the transformation was blocked.
     """
 
-    def __init__(self, reason: str = None, created_time: Optional[int] = None):
+    def __init__(self, reason: Optional[str] = None, created_time: Optional[int] = None):
         self.reason = reason
         self.created_time = created_time
 
 
 def _load_destination_dct(
     dct: Dict[str, Any]
 ) -> Union[RawTable, Nodes, Edges, SequenceRows, TransformationDestination]:
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/transformations/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,27 +27,29 @@
         name (str): Name of the metric.
         count (int): Value of the metric.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        timestamp: int = None,
-        name: str = None,
-        count: int = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        timestamp: Optional[int] = None,
+        name: Optional[str] = None,
+        count: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.timestamp = timestamp
         self.name = name
         self.count = count
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> TransformationJobMetric:
+    def _load(
+        cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None
+    ) -> TransformationJobMetric:
         instance = super()._load(resource, cognite_client)
         return instance
 
 
 class TransformationJobMetricList(CogniteResourceList[TransformationJobMetric]):
     _RESOURCE = TransformationJobMetric
 
@@ -74,30 +76,30 @@
         finished_time (int): Time when the job finished running.
         last_seen_time (int): Time of the last status update from the job.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        status: TransformationJobStatus = None,
-        transformation_id: int = None,
-        transformation_external_id: str = None,
-        source_project: str = None,
-        destination_project: str = None,
-        destination: TransformationDestination = None,
-        conflict_mode: str = None,
-        query: str = None,
-        error: str = None,
+        id: Optional[int] = None,
+        status: Optional[TransformationJobStatus] = None,
+        transformation_id: Optional[int] = None,
+        transformation_external_id: Optional[str] = None,
+        source_project: Optional[str] = None,
+        destination_project: Optional[str] = None,
+        destination: Optional[TransformationDestination] = None,
+        conflict_mode: Optional[str] = None,
+        query: Optional[str] = None,
+        error: Optional[str] = None,
         ignore_null_fields: bool = False,
-        created_time: int = None,
-        started_time: int = None,
-        finished_time: int = None,
-        last_seen_time: int = None,
-        cognite_client: CogniteClient = None,
+        created_time: Optional[int] = None,
+        started_time: Optional[int] = None,
+        finished_time: Optional[int] = None,
+        last_seen_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.status = status
         self.transformation_id = transformation_id
         self.transformation_external_id = transformation_external_id
         self.source_project = source_project
         self.destination_project = destination_project
@@ -242,15 +244,15 @@
             await asyncio.sleep(to_wait)
             self.update()
             waited += polling_interval
 
         return self
 
     @classmethod
-    def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> TransformationJob:
+    def _load(cls, resource: Union[Dict, str], cognite_client: Optional[CogniteClient] = None) -> TransformationJob:
         instance = super()._load(resource, cognite_client)
         if isinstance(instance.destination, Dict):
             instance.destination = _load_destination_dct(instance.destination)
         return instance
 
     def __hash__(self) -> int:
         return hash(self.id)
@@ -264,10 +266,10 @@
     """
 
     Args:
         transformation_id (Optional[int]):  Filter jobs by transformation internal numeric ID.
         transformation_external_id (str): Filter jobs by transformation external ID.
     """
 
-    def __init__(self, transformation_id: Optional[int] = None, transformation_external_id: str = None):
+    def __init__(self, transformation_id: Optional[int] = None, transformation_external_id: Optional[str] = None):
         self.transformation_id = transformation_id
         self.transformation_external_id = transformation_external_id
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/transformations/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,21 +19,21 @@
         created_time (int): Time when the notification was created.
         last_updated_time (int): Time when the notification was last updated.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        transformation_id: int = None,
-        transformation_external_id: str = None,
-        destination: str = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        cognite_client: CogniteClient = None,
+        id: Optional[int] = None,
+        transformation_id: Optional[int] = None,
+        transformation_external_id: Optional[str] = None,
+        destination: Optional[str] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.transformation_id = transformation_id
         self.transformation_external_id = transformation_external_id
         self.destination = destination
         self.created_time = created_time
         self.last_updated_time = last_updated_time
@@ -53,12 +53,15 @@
     Args:
         transformation_id (Optional[int]): Filter by transformation internal numeric ID.
         transformation_external_id (str): Filter by transformation externalId.
         destination (str): Filter by notification destination.
     """
 
     def __init__(
-        self, transformation_id: Optional[int] = None, transformation_external_id: str = None, destination: str = None
+        self,
+        transformation_id: Optional[int] = None,
+        transformation_external_id: Optional[str] = None,
+        destination: Optional[str] = None,
     ):
         self.transformation_id = transformation_id
         self.transformation_external_id = transformation_external_id
         self.destination = destination
```

### Comparing `cognite_sdk-6.8.4/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.8.5/cognite/client/data_classes/transformations/schedules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, cast
+from typing import TYPE_CHECKING, Any, Optional, cast
 
 from cognite.client.data_classes._base import (
     CognitePrimitiveUpdate,
     CogniteResource,
     CogniteResourceList,
     CogniteUpdate,
 )
@@ -24,21 +24,21 @@
         interval (str): Cron expression describes when the function should be called. Use http://www.cronmaker.com to create a cron expression.
         is_paused (bool): If true, the transformation is not scheduled.
         cognite_client (CogniteClient): The client to associate with this object.
     """
 
     def __init__(
         self,
-        id: int = None,
-        external_id: str = None,
-        created_time: int = None,
-        last_updated_time: int = None,
-        interval: str = None,
+        id: Optional[int] = None,
+        external_id: Optional[str] = None,
+        created_time: Optional[int] = None,
+        last_updated_time: Optional[int] = None,
+        interval: Optional[str] = None,
         is_paused: bool = False,
-        cognite_client: CogniteClient = None,
+        cognite_client: Optional[CogniteClient] = None,
     ):
         self.id = id
         self.external_id = external_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self.interval = interval
         self.is_paused = is_paused
```

### Comparing `cognite_sdk-6.8.4/cognite/client/exceptions.py` & `cognite_sdk-6.8.5/cognite/client/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,19 @@
 
 class CogniteReadTimeout(CogniteException):
     pass
 
 
 class CogniteMultiException(CogniteException):
     def __init__(
-        self, successful: Sequence = None, failed: Sequence = None, unknown: Sequence = None, unwrap_fn: Callable = None
+        self,
+        successful: Optional[Sequence] = None,
+        failed: Optional[Sequence] = None,
+        unknown: Optional[Sequence] = None,
+        unwrap_fn: Optional[Callable] = None,
     ):
         self.successful = successful or []
         self.failed = failed or []
         self.unknown = unknown or []
         self._unwrap_fn = unwrap_fn or (lambda x: x)
 
     def _get_multi_exception_summary(self) -> str:
@@ -109,22 +113,22 @@
                 print(f"The message returned from the API: {e.message}")
     """
 
     def __init__(
         self,
         message: str,
         code: int,
-        x_request_id: str = None,
-        missing: Sequence = None,
-        duplicated: Sequence = None,
-        successful: Sequence = None,
-        failed: Sequence = None,
-        unknown: Sequence = None,
-        unwrap_fn: Callable = None,
-        extra: Dict = None,
+        x_request_id: Optional[str] = None,
+        missing: Optional[Sequence] = None,
+        duplicated: Optional[Sequence] = None,
+        successful: Optional[Sequence] = None,
+        failed: Optional[Sequence] = None,
+        unknown: Optional[Sequence] = None,
+        unwrap_fn: Optional[Callable] = None,
+        extra: Optional[Dict] = None,
     ) -> None:
         self.message = message
         self.code = code
         self.x_request_id = x_request_id
         self.missing = missing
         self.duplicated = duplicated
         self.extra = extra
@@ -154,18 +158,18 @@
         failed (List): List of items which failed.
         unknown (List): List of items which may or may not have been successfully processed.
     """
 
     def __init__(
         self,
         not_found: List,
-        successful: List = None,
-        failed: List = None,
-        unknown: List = None,
-        unwrap_fn: Callable = None,
+        successful: Optional[List] = None,
+        failed: Optional[List] = None,
+        unknown: Optional[List] = None,
+        unwrap_fn: Optional[Callable] = None,
     ):
         self.not_found = not_found
         super().__init__(successful, failed, unknown, unwrap_fn)
 
     def __str__(self) -> str:
         if len(not_found := self.not_found) > 200:
             not_found = reprlib.repr(self.not_found)  # type: ignore [assignment]
@@ -184,18 +188,18 @@
         unknown (List): List of items which may or may not have been successfully processed.
         unwrap_fn: (Callable): Function to extract identifier from the Cognite resource.
     """
 
     def __init__(
         self,
         duplicated: List,
-        successful: List = None,
-        failed: List = None,
-        unknown: List = None,
-        unwrap_fn: Callable = None,
+        successful: Optional[List] = None,
+        failed: Optional[List] = None,
+        unknown: Optional[List] = None,
+        unwrap_fn: Optional[Callable] = None,
     ):
         self.duplicated = duplicated
         super().__init__(successful, failed, unknown, unwrap_fn)
 
     def __str__(self) -> str:
         msg = f"Duplicated: {self.duplicated}"
         msg += self._get_multi_exception_summary()
@@ -208,15 +212,15 @@
     Raised if the user attempts to use functionality which requires an uninstalled package.
 
     Args:
         module (str): Name of the module which could not be imported
         message (str): The error message to output.
     """
 
-    def __init__(self, module: str, message: str = None):
+    def __init__(self, module: str, message: Optional[str] = None):
         self.module = module
         self.message = message or f"The functionality you are trying to use requires '{self.module}' to be installed."
 
     def __str__(self) -> str:
         return self.message
```

### Comparing `cognite_sdk-6.8.4/cognite/client/testing.py` & `cognite_sdk-6.8.5/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/__init__.py` & `cognite_sdk-6.8.5/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.8.5/cognite/client/utils/_auxiliary.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,12 +219,12 @@
 
 
 def exactly_one_is_not_none(*args: Any) -> bool:
     return sum(1 if a is not None else 0 for a in args) == 1
 
 
 def rename_and_exclude_keys(
-    dct: dict[str, Any], aliases: dict[str, str] = None, exclude: set[str] = None
+    dct: dict[str, Any], aliases: Optional[dict[str, str]] = None, exclude: Optional[set[str]] = None
 ) -> dict[str, Any]:
     aliases = aliases or {}
     exclude = exclude or set()
     return {aliases.get(k, k): v for k, v in dct.items() if k not in exclude}
```

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.8.5/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_graph.py` & `cognite_sdk-6.8.5/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_identifier.py` & `cognite_sdk-6.8.5/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_logging.py` & `cognite_sdk-6.8.5/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.8.5/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.8.5/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.8.5/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_text.py` & `cognite_sdk-6.8.5/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_time.py` & `cognite_sdk-6.8.5/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_validation.py` & `cognite_sdk-6.8.5/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.8.5/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.8.4/pyproject.toml` & `cognite_sdk-6.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.8.4"
+version = "6.8.5"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.8.4/PKG-INFO` & `cognite_sdk-6.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.8.4
+Version: 6.8.5
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.8.4 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.8.5 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

