# Comparing `tmp/useis-1.1.7.tar.gz` & `tmp/useis-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useis-1.1.7.tar", max compression
+gzip compressed data, was "useis-1.1.8.tar", max compression
```

## Comparing `useis-1.1.7.tar` & `useis-1.1.8.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1076 2023-01-15 00:22:18.530236 useis-1.1.7/LICENSE
--rw-r--r--   0        0        0     1584 2023-07-18 13:04:21.084038 useis-1.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.7/useis/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.7/useis/ai/__init__.py
--rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.1.7/useis/ai/create-picking_dataset.py
--rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.1.7/useis/ai/create_classification_dataset.py
--rw-r--r--   0        0        0     5121 2023-04-30 10:55:33.035132 useis-1.1.7/useis/ai/database.py
--rw-r--r--   0        0        0    16324 2023-04-25 01:04:54.358379 useis-1.1.7/useis/ai/dataset.py
--rw-r--r--   0        0        0      686 2023-04-21 11:24:49.731581 useis-1.1.7/useis/ai/event_type_lookup.py
--rw-r--r--   0        0        0    25078 2023-04-30 15:50:36.463629 useis-1.1.7/useis/ai/model.py
--rw-r--r--   0        0        0      248 2023-04-21 13:03:02.416625 useis-1.1.7/useis/ai/params.py
--rw-r--r--   0        0        0    10310 2023-01-15 00:22:18.530236 useis-1.1.7/useis/ai/resnet1d.py
--rw-r--r--   0        0        0     2109 2023-01-15 00:22:18.530236 useis-1.1.7/useis/ai/spectrogram.py
--rw-r--r--   0        0        0        0 2023-01-15 15:22:58.057061 useis-1.1.7/useis/clients/__init__.py
--rw-r--r--   0        0        0     2474 2023-01-15 23:09:56.931370 useis-1.1.7/useis/clients/test_data.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.7/useis/core/__init__.py
--rw-r--r--   0        0        0    26080 2023-04-25 18:54:53.877703 useis-1.1.7/useis/core/project_manager.py
--rw-r--r--   0        0        0     2241 2023-01-15 00:22:18.530236 useis-1.1.7/useis/core/projection.py
--rw-r--r--   0        0        0       37 2023-04-23 11:28:19.261133 useis-1.1.7/useis/examples/classifier/.gitignore
--rw-r--r--   0        0        0        0 2023-04-15 21:09:31.238146 useis-1.1.7/useis/examples/classifier/__init__.py
--rw-r--r--   0        0        0      972 2023-04-25 18:54:53.877703 useis-1.1.7/useis/examples/classifier/classifier.py
--rw-r--r--   0        0        0     6087 2023-05-02 15:29:21.101970 useis-1.1.7/useis/examples/classifier/example.ipynb
--rw-r--r--   0        0        0        4 2023-01-15 23:17:05.571515 useis-1.1.7/useis/examples/picker/.gitignore
--rw-r--r--   0        0        0      111 2023-01-15 15:24:07.968314 useis-1.1.7/useis/examples/picker/ai_picker.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/__init__.py
--rw-r--r--   0        0        0    13705 2023-03-01 13:50:47.712880 useis-1.1.7/useis/processors/beamforming.py
--rw-r--r--   0        0        0     5627 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/data_extractor.py
--rw-r--r--   0        0        0      534 2023-03-01 13:36:57.561961 useis-1.1.7/useis/processors/file_manager.py
--rw-r--r--   0        0        0     6645 2023-04-04 16:58:44.812525 useis-1.1.7/useis/processors/magnitude.py
--rw-r--r--   0        0        0    27203 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/nlloc.py
--rw-r--r--   0        0        0    16230 2023-04-27 19:46:27.993238 useis-1.1.7/useis/processors/picker.py
--rw-r--r--   0        0        0      349 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/ray_tracer.py
--rw-r--r--   0        0        0     2272 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/simple_magnitude.py
--rw-r--r--   0        0        0    20652 2023-01-15 00:22:18.534236 useis-1.1.7/useis/processors/tomography.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/__init__.py
--rw-r--r--   0        0        0     1167 2023-04-14 00:53:50.522884 useis-1.1.7/useis/sandbox/ai_picker/train_picker.py
--rw-r--r--   0        0        0      721 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/Dockerfile
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/__init__.py
--rw-r--r--   0        0        0     1086 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/consumer.py
--rw-r--r--   0        0        0        2 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/demo_kafka.py
--rw-r--r--   0        0        0     6660 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/docker-compose.yml
--rw-r--r--   0        0        0      456 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/demo_kafka/producer.py
--rw-r--r--   0        0        0    13474 2023-03-19 10:30:35.680696 useis-1.1.7/useis/sandbox/event_classification/00_create_training_dataset.py
--rw-r--r--   0        0        0     1731 2023-04-15 10:41:35.083898 useis-1.1.7/useis/sandbox/event_classification/01_train.py
--rw-r--r--   0        0        0     6112 2023-04-23 20:46:56.290082 useis-1.1.7/useis/sandbox/event_classification/02_test.py
--rw-r--r--   0        0        0        0 2023-03-01 01:20:41.974427 useis-1.1.7/useis/sandbox/event_classification/__init__.py
--rw-r--r--   0        0        0      686 2023-03-10 11:19:47.286141 useis-1.1.7/useis/sandbox/event_classification/event_type_lookup.py
--rw-r--r--   0        0        0  1484029 2023-04-16 21:56:26.987377 useis-1.1.7/useis/sandbox/event_classification/inventory/OT.xml
--rw-r--r--   0        0        0  1421855 2023-03-01 00:12:03.885977 useis-1.1.7/useis/sandbox/event_classification/inventory/OT_old.xml
--rw-r--r--   0        0        0        0 2023-03-01 01:20:41.970427 useis-1.1.7/useis/sandbox/event_classification/inventory/__init__.py
--rw-r--r--   0        0        0     1726 2023-04-16 21:56:21.783139 useis-1.1.7/useis/sandbox/event_classification/inventory/update_inventory.py
--rw-r--r--   0        0        0     1040 2023-03-01 13:26:33.688702 useis-1.1.7/useis/sandbox/event_classification/velocity.py
--rw-r--r--   0        0        0     1587 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/tomography/Tomography.ipynb
--rw-r--r--   0        0        0     1470 2023-01-15 00:22:18.534236 useis-1.1.7/useis/sandbox/tomography/test_tomography.py
--rw-r--r--   0        0        0        0 2023-01-15 13:48:12.828128 useis-1.1.7/useis/scripts/__init__.py
--rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.1.7/useis/scripts/ai/create-picking_dataset.py
--rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.1.7/useis/scripts/ai/create_classification_dataset.py
--rw-r--r--   0        0        0     6553 2023-01-15 00:27:33.009528 useis-1.1.7/useis/scripts/ai/create_classification_dataset_1D.py
--rw-r--r--   0        0        0     9765 2023-01-15 00:27:33.009528 useis-1.1.7/useis/scripts/ai/train_classifier.py
--rw-r--r--   0        0        0     9799 2023-01-15 00:27:33.009528 useis-1.1.7/useis/scripts/ai/train_classifier_1d.py
--rw-r--r--   0        0        0     1028 2023-01-15 02:24:36.810810 useis-1.1.7/useis/scripts/ai/train_picker.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/file_server/__init__.py
--rw-r--r--   0        0        0       64 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/file_server/database.env
--rw-r--r--   0        0        0     1616 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/file_server/database.py
--rw-r--r--   0        0        0      236 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/file_server/docker-compose.yml
--rw-r--r--   0        0        0      655 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/file_server/indexer.py
--rw-r--r--   0        0        0       18 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/grid/.gitignore
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/grid/__init__.py
--rw-r--r--   0        0        0     4139 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/grid/client.py
--rw-r--r--   0        0        0     6330 2023-05-04 17:28:01.664387 useis-1.1.7/useis/services/grid/server.py
--rw-r--r--   0        0        0       27 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/grid/start_service.sh
--rw-r--r--   0        0        0     1777 2023-05-04 17:16:40.617228 useis-1.1.7/useis/services/grid/test.py
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/models/__init__.py
--rw-r--r--   0        0        0      492 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/models/base.py
--rw-r--r--   0        0        0      756 2023-04-04 00:35:32.026107 useis-1.1.7/useis/services/models/classifier.py
--rw-r--r--   0        0        0     3982 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/models/event.py
--rw-r--r--   0        0        0     1700 2023-01-15 00:22:18.534236 useis-1.1.7/useis/services/models/grid.py
--rw-r--r--   0        0        0     2674 2023-05-04 17:25:32.301550 useis-1.1.7/useis/services/models/nlloc.py
--rw-r--r--   0        0        0       30 2023-01-23 17:06:39.892533 useis-1.1.7/useis/settings/__init__.py
--rw-r--r--   0        0        0      225 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/beamforming_settings_template.toml
--rw-r--r--   0        0        0      237 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/interloc_settings_template.toml
--rw-r--r--   0        0        0      182 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/magnitude_settings_template.toml
--rw-r--r--   0        0        0      853 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/nlloc_settings_template.py
--rw-r--r--   0        0        0      970 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/picker_settings_template.toml
--rw-r--r--   0        0        0       75 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/projection_settings_template.toml
--rw-r--r--   0        0        0       46 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/services_settings_template.toml
--rw-r--r--   0        0        0      893 2023-01-23 16:59:37.680786 useis-1.1.7/useis/settings/settings.py
--rw-r--r--   0        0        0    12030 2023-03-01 00:12:58.744538 useis-1.1.7/useis/settings/settings_template.toml
--rw-r--r--   0        0        0       12 2023-01-15 00:22:18.534236 useis-1.1.7/useis/settings/tomography_settings_template.toml
--rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.7/useis/tomography/__init__.py
--rwxr-xr-x   0        0        0     5197 2023-01-15 00:22:18.534236 useis-1.1.7/useis/tomography/data.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 useis-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-01-15 00:22:18.530236 useis-1.1.8/LICENSE
+-rw-r--r--   0        0        0     1584 2023-07-18 13:48:58.849093 useis-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.8/useis/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.8/useis/ai/__init__.py
+-rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.1.8/useis/ai/create-picking_dataset.py
+-rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.1.8/useis/ai/create_classification_dataset.py
+-rw-r--r--   0        0        0     5121 2023-04-30 10:55:33.035132 useis-1.1.8/useis/ai/database.py
+-rw-r--r--   0        0        0    16324 2023-04-25 01:04:54.358379 useis-1.1.8/useis/ai/dataset.py
+-rw-r--r--   0        0        0      686 2023-04-21 11:24:49.731581 useis-1.1.8/useis/ai/event_type_lookup.py
+-rw-r--r--   0        0        0    25078 2023-04-30 15:50:36.463629 useis-1.1.8/useis/ai/model.py
+-rw-r--r--   0        0        0      248 2023-04-21 13:03:02.416625 useis-1.1.8/useis/ai/params.py
+-rw-r--r--   0        0        0    10310 2023-01-15 00:22:18.530236 useis-1.1.8/useis/ai/resnet1d.py
+-rw-r--r--   0        0        0     2109 2023-01-15 00:22:18.530236 useis-1.1.8/useis/ai/spectrogram.py
+-rw-r--r--   0        0        0        0 2023-01-15 15:22:58.057061 useis-1.1.8/useis/clients/__init__.py
+-rw-r--r--   0        0        0     2474 2023-01-15 23:09:56.931370 useis-1.1.8/useis/clients/test_data.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.530236 useis-1.1.8/useis/core/__init__.py
+-rw-r--r--   0        0        0    26080 2023-04-25 18:54:53.877703 useis-1.1.8/useis/core/project_manager.py
+-rw-r--r--   0        0        0     2241 2023-01-15 00:22:18.530236 useis-1.1.8/useis/core/projection.py
+-rw-r--r--   0        0        0       37 2023-04-23 11:28:19.261133 useis-1.1.8/useis/examples/classifier/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-15 21:09:31.238146 useis-1.1.8/useis/examples/classifier/__init__.py
+-rw-r--r--   0        0        0      972 2023-04-25 18:54:53.877703 useis-1.1.8/useis/examples/classifier/classifier.py
+-rw-r--r--   0        0        0     6087 2023-05-02 15:29:21.101970 useis-1.1.8/useis/examples/classifier/example.ipynb
+-rw-r--r--   0        0        0        4 2023-01-15 23:17:05.571515 useis-1.1.8/useis/examples/picker/.gitignore
+-rw-r--r--   0        0        0      111 2023-01-15 15:24:07.968314 useis-1.1.8/useis/examples/picker/ai_picker.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/__init__.py
+-rw-r--r--   0        0        0    13705 2023-03-01 13:50:47.712880 useis-1.1.8/useis/processors/beamforming.py
+-rw-r--r--   0        0        0     5627 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/data_extractor.py
+-rw-r--r--   0        0        0      534 2023-03-01 13:36:57.561961 useis-1.1.8/useis/processors/file_manager.py
+-rw-r--r--   0        0        0     6645 2023-04-04 16:58:44.812525 useis-1.1.8/useis/processors/magnitude.py
+-rw-r--r--   0        0        0    27203 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/nlloc.py
+-rw-r--r--   0        0        0    16230 2023-04-27 19:46:27.993238 useis-1.1.8/useis/processors/picker.py
+-rw-r--r--   0        0        0      349 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/ray_tracer.py
+-rw-r--r--   0        0        0     2272 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/simple_magnitude.py
+-rw-r--r--   0        0        0    20652 2023-01-15 00:22:18.534236 useis-1.1.8/useis/processors/tomography.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/__init__.py
+-rw-r--r--   0        0        0     1167 2023-04-14 00:53:50.522884 useis-1.1.8/useis/sandbox/ai_picker/train_picker.py
+-rw-r--r--   0        0        0      721 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/Dockerfile
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/__init__.py
+-rw-r--r--   0        0        0     1086 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/consumer.py
+-rw-r--r--   0        0        0        2 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/demo_kafka.py
+-rw-r--r--   0        0        0     6660 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/docker-compose.yml
+-rw-r--r--   0        0        0      456 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/demo_kafka/producer.py
+-rw-r--r--   0        0        0    13474 2023-03-19 10:30:35.680696 useis-1.1.8/useis/sandbox/event_classification/00_create_training_dataset.py
+-rw-r--r--   0        0        0     1731 2023-04-15 10:41:35.083898 useis-1.1.8/useis/sandbox/event_classification/01_train.py
+-rw-r--r--   0        0        0     6112 2023-04-23 20:46:56.290082 useis-1.1.8/useis/sandbox/event_classification/02_test.py
+-rw-r--r--   0        0        0        0 2023-03-01 01:20:41.974427 useis-1.1.8/useis/sandbox/event_classification/__init__.py
+-rw-r--r--   0        0        0      686 2023-03-10 11:19:47.286141 useis-1.1.8/useis/sandbox/event_classification/event_type_lookup.py
+-rw-r--r--   0        0        0  1484029 2023-04-16 21:56:26.987377 useis-1.1.8/useis/sandbox/event_classification/inventory/OT.xml
+-rw-r--r--   0        0        0  1421855 2023-03-01 00:12:03.885977 useis-1.1.8/useis/sandbox/event_classification/inventory/OT_old.xml
+-rw-r--r--   0        0        0        0 2023-03-01 01:20:41.970427 useis-1.1.8/useis/sandbox/event_classification/inventory/__init__.py
+-rw-r--r--   0        0        0     1726 2023-04-16 21:56:21.783139 useis-1.1.8/useis/sandbox/event_classification/inventory/update_inventory.py
+-rw-r--r--   0        0        0     1040 2023-03-01 13:26:33.688702 useis-1.1.8/useis/sandbox/event_classification/velocity.py
+-rw-r--r--   0        0        0     1587 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/tomography/Tomography.ipynb
+-rw-r--r--   0        0        0     1470 2023-01-15 00:22:18.534236 useis-1.1.8/useis/sandbox/tomography/test_tomography.py
+-rw-r--r--   0        0        0        0 2023-01-15 13:48:12.828128 useis-1.1.8/useis/scripts/__init__.py
+-rw-r--r--   0        0        0     5808 2023-01-15 00:27:33.009528 useis-1.1.8/useis/scripts/ai/create-picking_dataset.py
+-rw-r--r--   0        0        0     7725 2023-01-15 00:27:33.009528 useis-1.1.8/useis/scripts/ai/create_classification_dataset.py
+-rw-r--r--   0        0        0     6553 2023-01-15 00:27:33.009528 useis-1.1.8/useis/scripts/ai/create_classification_dataset_1D.py
+-rw-r--r--   0        0        0     9765 2023-01-15 00:27:33.009528 useis-1.1.8/useis/scripts/ai/train_classifier.py
+-rw-r--r--   0        0        0     9799 2023-01-15 00:27:33.009528 useis-1.1.8/useis/scripts/ai/train_classifier_1d.py
+-rw-r--r--   0        0        0     1028 2023-01-15 02:24:36.810810 useis-1.1.8/useis/scripts/ai/train_picker.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/file_server/__init__.py
+-rw-r--r--   0        0        0       64 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/file_server/database.env
+-rw-r--r--   0        0        0     1616 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/file_server/database.py
+-rw-r--r--   0        0        0      236 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/file_server/docker-compose.yml
+-rw-r--r--   0        0        0      655 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/file_server/indexer.py
+-rw-r--r--   0        0        0       18 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/grid/.gitignore
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/grid/__init__.py
+-rw-r--r--   0        0        0     4139 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/grid/client.py
+-rw-r--r--   0        0        0     6330 2023-05-04 17:28:01.664387 useis-1.1.8/useis/services/grid/server.py
+-rw-r--r--   0        0        0       27 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/grid/start_service.sh
+-rw-r--r--   0        0        0     1777 2023-05-04 17:16:40.617228 useis-1.1.8/useis/services/grid/test.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/models/__init__.py
+-rw-r--r--   0        0        0      492 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/models/base.py
+-rw-r--r--   0        0        0      756 2023-04-04 00:35:32.026107 useis-1.1.8/useis/services/models/classifier.py
+-rw-r--r--   0        0        0     3982 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/models/event.py
+-rw-r--r--   0        0        0     1700 2023-01-15 00:22:18.534236 useis-1.1.8/useis/services/models/grid.py
+-rw-r--r--   0        0        0     2674 2023-05-04 17:25:32.301550 useis-1.1.8/useis/services/models/nlloc.py
+-rw-r--r--   0        0        0       30 2023-01-23 17:06:39.892533 useis-1.1.8/useis/settings/__init__.py
+-rw-r--r--   0        0        0      225 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/beamforming_settings_template.toml
+-rw-r--r--   0        0        0      237 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/interloc_settings_template.toml
+-rw-r--r--   0        0        0      182 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/magnitude_settings_template.toml
+-rw-r--r--   0        0        0      853 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/nlloc_settings_template.py
+-rw-r--r--   0        0        0      970 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/picker_settings_template.toml
+-rw-r--r--   0        0        0       75 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/projection_settings_template.toml
+-rw-r--r--   0        0        0       46 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/services_settings_template.toml
+-rw-r--r--   0        0        0      893 2023-01-23 16:59:37.680786 useis-1.1.8/useis/settings/settings.py
+-rw-r--r--   0        0        0    12030 2023-03-01 00:12:58.744538 useis-1.1.8/useis/settings/settings_template.toml
+-rw-r--r--   0        0        0       12 2023-01-15 00:22:18.534236 useis-1.1.8/useis/settings/tomography_settings_template.toml
+-rw-r--r--   0        0        0        0 2023-01-15 00:22:18.534236 useis-1.1.8/useis/tomography/__init__.py
+-rwxr-xr-x   0        0        0     5197 2023-01-15 00:22:18.534236 useis-1.1.8/useis/tomography/data.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 useis-1.1.8/PKG-INFO
```

### Comparing `useis-1.1.7/LICENSE` & `useis-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/pyproject.toml` & `useis-1.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "useis"
-version = "1.1.7"
+version = "1.1.8"
 description = ""
 authors = ["jpmercier <jpmercier01@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dynaconf = "^3.1.4"
@@ -27,15 +27,15 @@
 #uquake = {path = "libraries/uquake", develop = true}
 numpy = "^1.3.0"
 pyproj = "3.4.1"
 pillow = "^9.4.0"
 #torch = {path = "/data_1/libraries/torch-1.11.0+cu115-cp39-cp39-linux_x86_64.whl"}
 #torchaudio = {url = "https://download.pytorch.org/whl/cu115/torchaudio-0.11.0%2Bcu115-cp39-cp39-linux_x86_64.whl"}
 #torchvision = {url = "https://download.pytorch.org/whl/cu115/torchvision-0.12.0%2Bcu115-cp39-cp39-linux_x86_64.whl"}
-uquake = "^1.4.7"
+uquake = "^1.4.8"
 
 [tool.poetry.dev-dependencies]
 ipdb = "^0.13.9"
 notebook = "^6.4.4"
 jupyterlab = "^3.1.13"
 jupyter-http-over-ws = "^0.0.8"
 jupyter = "^1.0.0"
```

### Comparing `useis-1.1.7/useis/ai/create-picking_dataset.py` & `useis-1.1.8/useis/ai/create-picking_dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/create_classification_dataset.py` & `useis-1.1.8/useis/ai/create_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/database.py` & `useis-1.1.8/useis/ai/database.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/dataset.py` & `useis-1.1.8/useis/ai/dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/event_type_lookup.py` & `useis-1.1.8/useis/ai/event_type_lookup.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/model.py` & `useis-1.1.8/useis/ai/model.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/resnet1d.py` & `useis-1.1.8/useis/ai/resnet1d.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/ai/spectrogram.py` & `useis-1.1.8/useis/ai/spectrogram.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/clients/test_data.py` & `useis-1.1.8/useis/clients/test_data.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/core/project_manager.py` & `useis-1.1.8/useis/core/project_manager.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/core/projection.py` & `useis-1.1.8/useis/core/projection.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/examples/classifier/classifier.py` & `useis-1.1.8/useis/examples/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/examples/classifier/example.ipynb` & `useis-1.1.8/useis/examples/classifier/example.ipynb`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/beamforming.py` & `useis-1.1.8/useis/processors/beamforming.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/data_extractor.py` & `useis-1.1.8/useis/processors/data_extractor.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/file_manager.py` & `useis-1.1.8/useis/processors/file_manager.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/magnitude.py` & `useis-1.1.8/useis/processors/magnitude.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/nlloc.py` & `useis-1.1.8/useis/processors/nlloc.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/picker.py` & `useis-1.1.8/useis/processors/picker.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/simple_magnitude.py` & `useis-1.1.8/useis/processors/simple_magnitude.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/processors/tomography.py` & `useis-1.1.8/useis/processors/tomography.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/ai_picker/train_picker.py` & `useis-1.1.8/useis/sandbox/ai_picker/train_picker.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/demo_kafka/Dockerfile` & `useis-1.1.8/useis/sandbox/demo_kafka/Dockerfile`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/demo_kafka/consumer.py` & `useis-1.1.8/useis/sandbox/demo_kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/demo_kafka/docker-compose.yml` & `useis-1.1.8/useis/sandbox/demo_kafka/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/00_create_training_dataset.py` & `useis-1.1.8/useis/sandbox/event_classification/00_create_training_dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/01_train.py` & `useis-1.1.8/useis/sandbox/event_classification/01_train.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/02_test.py` & `useis-1.1.8/useis/sandbox/event_classification/02_test.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/event_type_lookup.py` & `useis-1.1.8/useis/sandbox/event_classification/event_type_lookup.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/inventory/OT.xml` & `useis-1.1.8/useis/sandbox/event_classification/inventory/OT.xml`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/inventory/OT_old.xml` & `useis-1.1.8/useis/sandbox/event_classification/inventory/OT_old.xml`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/inventory/update_inventory.py` & `useis-1.1.8/useis/sandbox/event_classification/inventory/update_inventory.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/event_classification/velocity.py` & `useis-1.1.8/useis/sandbox/event_classification/velocity.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/tomography/Tomography.ipynb` & `useis-1.1.8/useis/sandbox/tomography/Tomography.ipynb`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/sandbox/tomography/test_tomography.py` & `useis-1.1.8/useis/sandbox/tomography/test_tomography.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/create-picking_dataset.py` & `useis-1.1.8/useis/scripts/ai/create-picking_dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/create_classification_dataset.py` & `useis-1.1.8/useis/scripts/ai/create_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/create_classification_dataset_1D.py` & `useis-1.1.8/useis/scripts/ai/create_classification_dataset_1D.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/train_classifier.py` & `useis-1.1.8/useis/scripts/ai/train_classifier.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/train_classifier_1d.py` & `useis-1.1.8/useis/scripts/ai/train_classifier_1d.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/scripts/ai/train_picker.py` & `useis-1.1.8/useis/scripts/ai/train_picker.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/file_server/database.py` & `useis-1.1.8/useis/services/file_server/database.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/file_server/indexer.py` & `useis-1.1.8/useis/services/file_server/indexer.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/grid/client.py` & `useis-1.1.8/useis/services/grid/client.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/grid/server.py` & `useis-1.1.8/useis/services/grid/server.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/grid/test.py` & `useis-1.1.8/useis/services/grid/test.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/models/classifier.py` & `useis-1.1.8/useis/services/models/classifier.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/models/event.py` & `useis-1.1.8/useis/services/models/event.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/models/grid.py` & `useis-1.1.8/useis/services/models/grid.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/services/models/nlloc.py` & `useis-1.1.8/useis/services/models/nlloc.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/settings/nlloc_settings_template.py` & `useis-1.1.8/useis/settings/nlloc_settings_template.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/settings/picker_settings_template.toml` & `useis-1.1.8/useis/settings/picker_settings_template.toml`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/settings/settings.py` & `useis-1.1.8/useis/settings/settings.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/settings/settings_template.toml` & `useis-1.1.8/useis/settings/settings_template.toml`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/useis/tomography/data.py` & `useis-1.1.8/useis/tomography/data.py`

 * *Files identical despite different names*

### Comparing `useis-1.1.7/PKG-INFO` & `useis-1.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useis
-Version: 1.1.7
+Version: 1.1.8
 Summary: 
 License: MIT
 Author: jpmercier
 Author-email: jpmercier01@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,9 +21,9 @@
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyproj (==3.4.1)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: rinohtype (>=0.5.3,<0.6.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
-Requires-Dist: uquake (>=1.4.7,<2.0.0)
+Requires-Dist: uquake (>=1.4.8,<2.0.0)
 Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
```

