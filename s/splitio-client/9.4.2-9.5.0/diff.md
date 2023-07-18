# Comparing `tmp/splitio_client-9.4.2.tar.gz` & `tmp/splitio_client-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splitio_client-9.4.2.tar", last modified: Tue May 16 17:12:46 2023, max compression
+gzip compressed data, was "dist/splitio_client-9.5.0.tar", last modified: Tue Jul 18 20:14:05 2023, max compression
```

## Comparing `splitio_client-9.4.2.tar` & `splitio_client-9.5.0.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-05-16 17:12:46.000000 splitio_client-9.4.2/PKG-INFO
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/splitio_client.egg-info/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4174 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/SOURCES.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/requires.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/top_level.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/dependency_links.txt
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/integration/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    89669 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_client_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_redis_integration.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11819 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_pluggable_integration.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    60236 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_streaming_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3469 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_segment_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1535 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_split_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11528 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2437 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_processor.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/recorder/test_recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_impressions_count_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_segments_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_impressions_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21478 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_splits_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7167 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_events_synchronizer.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/helpers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/helpers/mockserver.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/helpers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2023-05-16 17:09:46.000000 splitio_client-9.4.2/README.md
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1672 2023-05-16 17:09:46.000000 splitio_client-9.4.2/setup.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/tasks/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/split_sync.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/tasks/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/workerpool.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/asynctask.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/telemetry_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/events_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/segment_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/impressions_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       21 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/version.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/splitio/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/time.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/backoff.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/threadutil.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/decorators.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/factories.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/grammar/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/partitions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/condition.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/misc.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/numeric.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/string.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/sets.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/base.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/token.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/notification.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    32610 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/datatypes.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/splits.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/storage/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    30128 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/pluggable.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/storage/adapters/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/cache_trait.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26328 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20617 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/inmemmory.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/segmentworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2950 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/processor.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14206 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2187 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/splitworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9064 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/manager.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/recorder/recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/api/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/auth.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4145 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/commons.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2642 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/exceptions.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/impression.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/event.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3203 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20354 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/split.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    22571 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/segment.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/unique_keys.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/cache/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/cache/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/cache/lru.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12184 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/splitters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/hashfns/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/legacy.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/murmur3py.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/impressions/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/strategies.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/unique_keys_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7105 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/adapters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/evaluator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/filters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/client/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4821 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/config.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18084 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29024 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/factory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/localhost.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19181 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/input_validator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/listener.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-05-16 17:12:46.000000 splitio_client-9.4.2/setup.cfg
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-07-18 20:14:05.000000 splitio_client-9.5.0/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2023-07-18 20:12:25.000000 splitio_client-9.5.0/README.md
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-07-18 20:14:05.000000 splitio_client-9.5.0/setup.cfg
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1709 2023-07-18 20:12:25.000000 splitio_client-9.5.0/setup.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/api/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/auth.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/commons.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2642 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4145 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/api/telemetry.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/client/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18084 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4821 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/config.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29024 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/factory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19181 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/input_validator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/listener.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/localhost.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/client/util.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/engine/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/engine/cache/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/cache/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/cache/lru.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/evaluator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/filters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/engine/hashfns/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/hashfns/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/hashfns/legacy.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/hashfns/murmur3py.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/engine/impressions/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7105 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/adapters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/strategies.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/impressions/unique_keys_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/splitters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12593 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/engine/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/exceptions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/factories.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/key.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/models/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/datatypes.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/events.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/models/grammar/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/condition.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/base.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/misc.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/numeric.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/sets.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/matchers/string.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/grammar/partitions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/notification.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    33381 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/models/token.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9092 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    15365 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3241 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/processor.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/segmentworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5842 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/splitworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/push/status_tracker.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/recorder/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/recorder/recorder.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/storage/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/storage/adapters/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/adapters/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/adapters/cache_trait.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/adapters/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/adapters/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20899 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/inmemmory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    30128 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/pluggable.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26328 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/storage/redis.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/event.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/impression.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/segment.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21175 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/split.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    23222 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3254 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/unique_keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/sync/util.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/tasks/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/events_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/impressions_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/segment_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/split_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/telemetry_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/unique_keys_sync.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/tasks/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/util/asynctask.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/tasks/util/workerpool.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/util/backoff.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/util/decorators.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/util/threadutil.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/util/time.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       22 2023-07-18 20:12:25.000000 splitio_client-9.5.0/splitio/version.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4174 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/dependency_links.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/requires.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-07-18 20:14:05.000000 splitio_client-9.5.0/splitio_client.egg-info/top_level.txt
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:25.000000 splitio_client-9.5.0/tests/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/helpers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/helpers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/helpers/mockserver.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/integration/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/integration/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    89753 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/integration/test_client_e2e.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11819 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/integration/test_pluggable_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/integration/test_redis_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    64020 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/integration/test_streaming_e2e.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11721 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4181 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2500 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_processor.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_segment_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14070 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_split_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/push/test_status_tracker.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/recorder/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/recorder/test_recorder.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:14:05.000000 splitio_client-9.5.0/tests/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_events_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_impressions_count_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_impressions_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_segments_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21653 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_splits_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7260 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-07-18 20:12:26.000000 splitio_client-9.5.0/tests/sync/test_unique_keys_sync.py
```

### Comparing `splitio_client-9.4.2/PKG-INFO` & `splitio_client-9.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio_client
-Version: 9.4.2
+Version: 9.5.0
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.2
+Download-URL: https://github.com/splitio/python-client/tarball/9.5.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: redis
-Provides-Extra: cpphash
 Provides-Extra: test
+Provides-Extra: redis
 Provides-Extra: uwsgi
+Provides-Extra: cpphash
```

### Comparing `splitio_client-9.4.2/splitio_client.egg-info/PKG-INFO` & `splitio_client-9.5.0/splitio_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio-client
-Version: 9.4.2
+Version: 9.5.0
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.2
+Download-URL: https://github.com/splitio/python-client/tarball/9.5.0
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: redis
-Provides-Extra: cpphash
 Provides-Extra: test
+Provides-Extra: redis
 Provides-Extra: uwsgi
+Provides-Extra: cpphash
```

### Comparing `splitio_client-9.4.2/splitio_client.egg-info/SOURCES.txt` & `splitio_client-9.5.0/splitio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/integration/test_client_e2e.py` & `splitio_client-9.5.0/tests/integration/test_client_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -961,15 +961,15 @@
 
         # Tests 2
         assert self.factory.manager().split_names() == ["SPLIT_1"]
         assert client.get_treatment("key", "SPLIT_1") == 'off'
 
         # Tests 1
         self.factory._storages['splits'].remove('SPLIT_1')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._split_storage.set_change_number(-1)
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._feature_flag_storage.set_change_number(-1)
         self._update_temp_file(splits_json['splitChange1_1'])
         self._synchronize_now()
 
         assert sorted(self.factory.manager().split_names()) == ["SPLIT_1", "SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_1", None) == 'off'
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
@@ -985,30 +985,30 @@
 
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_1", None) == 'control'
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
         # Tests 3
         self.factory._storages['splits'].remove('SPLIT_1')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._split_storage.set_change_number(-1)
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._feature_flag_storage.set_change_number(-1)
         self._update_temp_file(splits_json['splitChange3_1'])
         self._synchronize_now()
 
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
         self._update_temp_file(splits_json['splitChange3_2'])
         self._synchronize_now()
 
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_2", None) == 'off'
 
         # Tests 4
         self.factory._storages['splits'].remove('SPLIT_2')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._split_storage.set_change_number(-1)
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._feature_flag_storage.set_change_number(-1)
         self._update_temp_file(splits_json['splitChange4_1'])
         self._synchronize_now()
 
         assert sorted(self.factory.manager().split_names()) == ["SPLIT_1", "SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_1", None) == 'off'
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
@@ -1025,30 +1025,30 @@
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_1", None) == 'control'
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
         # Tests 5
         self.factory._storages['splits'].remove('SPLIT_1')
         self.factory._storages['splits'].remove('SPLIT_2')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._split_storage.set_change_number(-1)
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._feature_flag_storage.set_change_number(-1)
         self._update_temp_file(splits_json['splitChange5_1'])
         self._synchronize_now()
 
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
         self._update_temp_file(splits_json['splitChange5_2'])
         self._synchronize_now()
 
         assert self.factory.manager().split_names() == ["SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
         # Tests 6
         self.factory._storages['splits'].remove('SPLIT_2')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._split_storage.set_change_number(-1)
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._feature_flag_storage.set_change_number(-1)
         self._update_temp_file(splits_json['splitChange6_1'])
         self._synchronize_now()
 
         assert sorted(self.factory.manager().split_names()) == ["SPLIT_1", "SPLIT_2"]
         assert client.get_treatment("key", "SPLIT_1", None) == 'off'
         assert client.get_treatment("key", "SPLIT_2", None) == 'on'
 
@@ -1069,16 +1069,16 @@
     def _update_temp_file(self, json_body):
         f = open(os.path.join(os.path.dirname(__file__), 'files','split_changes_temp.json'), 'w')
         f.write(json.dumps(json_body))
         f.close()
 
     def _synchronize_now(self):
         filename = os.path.join(os.path.dirname(__file__), 'files', 'split_changes_temp.json')
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync._filename = filename
-        self.factory._sync_manager._synchronizer._split_synchronizers._split_sync.synchronize_splits()
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync._filename = filename
+        self.factory._sync_manager._synchronizer._split_synchronizers._feature_flag_sync.synchronize_splits()
 
     def test_incorrect_file_e2e(self):
         """Test initialize factory with a incorrect file name."""
         # TODO: secontion below is removed when legacu use BUR
         # legacy and yaml
         exception_raised = False
         factory = None
```

### Comparing `splitio_client-9.4.2/tests/integration/test_redis_integration.py` & `splitio_client-9.5.0/tests/integration/test_redis_integration.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/integration/__init__.py` & `splitio_client-9.5.0/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/integration/test_pluggable_integration.py` & `splitio_client-9.5.0/tests/integration/test_pluggable_integration.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/integration/test_streaming_e2e.py` & `splitio_client-9.5.0/tests/integration/test_streaming_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Streaming integration tests."""
 # pylint:disable=no-self-use,invalid-name,too-many-arguments,too-few-public-methods,line-too-long
 # pylint:disable=too-many-statements,too-many-locals,too-many-lines
 import threading
 import time
 import json
+import base64
+import pytest
+
 from queue import Queue
 from splitio.client.factory import get_factory
 from tests.helpers.mockserver import SSEMockServer, SplitMockServer
 from urllib.parse import parse_qs
 from splitio.models.telemetry import StreamingEventTypes, SSESyncMode
 
 
@@ -102,14 +105,19 @@
         time.sleep(1)
         sse_server.publish(make_segment_change_event('segment1', 1))
         time.sleep(1)
 
         assert factory.client().get_treatment('pindon', 'split2') == 'off'
         assert factory.client().get_treatment('maldo', 'split2') == 'on'
 
+        sse_server.publish(make_split_fast_change_event(4))
+        time.sleep(1)
+        assert factory.client().get_treatment('maldo', 'split5') == 'on'
+
+
         # Validate the SSE request
         sse_request = sse_requests.get()
         assert sse_request.method == 'GET'
         path, qs = sse_request.path.split('?', 1)
         assert path == '/event-stream'
         qs = parse_qs(qs)
         assert qs['accessToken'][0] == (
@@ -1211,14 +1219,74 @@
         destroy_event = threading.Event()
         factory.destroy(destroy_event)
         destroy_event.wait()
         sse_server.publish(sse_server.GRACEFUL_REQUEST_END)
         sse_server.stop()
         split_backend.stop()
 
+    def test_change_number(mocker):
+        # test if changeNumber is missing
+        auth_server_response = {
+            'pushEnabled': True,
+            'token': ('eyJhbGciOiJIUzI1NiIsImtpZCI6IjVZOU05US45QnJtR0EiLCJ0eXAiOiJKV1QifQ.'
+                      'eyJ4LWFibHktY2FwYWJpbGl0eSI6IntcIk1UWXlNVGN4T1RRNE13PT1fTWpBNE16Y3pO'
+                      'RFUxTWc9PV9zZWdtZW50c1wiOltcInN1YnNjcmliZVwiXSxcIk1UWXlNVGN4T1RRNE13P'
+                      'T1fTWpBNE16Y3pORFUxTWc9PV9zcGxpdHNcIjpbXCJzdWJzY3JpYmVcIl0sXCJjb250cm'
+                      '9sX3ByaVwiOltcInN1YnNjcmliZVwiLFwiY2hhbm5lbC1tZXRhZGF0YTpwdWJsaXNoZXJ'
+                      'zXCJdLFwiY29udHJvbF9zZWNcIjpbXCJzdWJzY3JpYmVcIixcImNoYW5uZWwtbWV0YWRh'
+                      'dGE6cHVibGlzaGVyc1wiXX0iLCJ4LWFibHktY2xpZW50SWQiOiJjbGllbnRJZCIsImV4c'
+                      'CI6MTYwNDEwMDU5MSwiaWF0IjoxNjA0MDk2OTkxfQ.aP9BfR534K6J9h8gfDWg_CQgpz5E'
+                      'vJh17WlOlAKhcD0')
+        }
+
+        split_changes = {
+            -1: {
+                'since': -1,
+                'till': 1,
+                'splits': [make_simple_split('split1', 1, True, False, 'off', 'user', True)]
+            },
+            1: {'since': 1, 'till': 1, 'splits': []}
+        }
+
+        segment_changes = {}
+        split_backend_requests = Queue()
+        split_backend = SplitMockServer(split_changes, segment_changes, split_backend_requests,
+                                        auth_server_response)
+        sse_requests = Queue()
+        sse_server = SSEMockServer(sse_requests)
+
+        split_backend.start()
+        sse_server.start()
+        sse_server.publish(make_initial_event())
+        sse_server.publish(make_occupancy('control_pri', 2))
+        sse_server.publish(make_occupancy('control_sec', 2))
+
+        kwargs = {
+            'sdk_api_base_url': 'http://localhost:%d/api' % split_backend.port(),
+            'events_api_base_url': 'http://localhost:%d/api' % split_backend.port(),
+            'auth_api_base_url': 'http://localhost:%d/api' % split_backend.port(),
+            'streaming_api_base_url': 'http://localhost:%d' % sse_server.port(),
+            'config': {'connectTimeout': 10000, 'featuresRefreshRate': 10}
+        }
+
+        factory = get_factory('some_apikey', **kwargs)
+        factory.block_until_ready(1)
+        assert factory.ready
+        time.sleep(2)
+
+        split_changes = make_split_fast_change_event(5).copy()
+        data = json.loads(split_changes['data'])
+        inner_data = json.loads(data['data'])
+        inner_data['changeNumber'] = None
+        data['data'] = json.dumps(inner_data)
+        split_changes['data'] = json.dumps(data)
+        sse_server.publish(split_changes)
+        time.sleep(1)
+        assert factory._storages['splits'].get_change_number() == 1
+
 
 def make_split_change_event(change_number):
     """Make a split change event."""
     return {
         'event': 'message',
         'data': json.dumps({
             'id':'TVUsxaabHs:0:0',
@@ -1229,14 +1297,40 @@
             'data': json.dumps({
                 'type': 'SPLIT_UPDATE',
                 'changeNumber': change_number
             })
         })
     }
 
+def make_split_fast_change_event(change_number):
+    """Make a split change event."""
+    json1 = make_simple_split('split5', 1, True, False, 'off', 'user', True)
+    str1 = json.dumps(json1)
+    byt1 = bytes(str1, encoding='utf-8')
+    compressed = base64.b64encode(byt1)
+    final = compressed.decode('utf-8')
+
+    return {
+        'event': 'message',
+        'data': json.dumps({
+            'id':'TVUsxaabHs:0:0',
+            'clientId':'pri:MzM0ODI1MTkxMw==',
+            'timestamp': change_number-1,
+            'encoding':'json',
+            'channel':'MTYyMTcxOTQ4Mw==_MjA4MzczNDU1Mg==_splits',
+            'data': json.dumps({
+                'type': 'SPLIT_UPDATE',
+                'changeNumber': change_number,
+                'pcn': 3,
+                'c': 0,
+                'd': final
+            })
+        })
+    }
+
 def make_split_kill_event(name, default_treatment, change_number):
     """Make a split change event."""
     return {
         'event': 'message',
         'data': json.dumps({
             'id':'TVUsxaabHs:0:0',
             'clientId':'pri:MzM0ODI1MTkxMw==',
```

### Comparing `splitio_client-9.4.2/tests/push/test_parser.py` & `splitio_client-9.5.0/tests/push/test_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -51,23 +51,38 @@
             'NDA5ODc2MTAyNg==_MzAyODY0NDkyOA==_splits',
             {'type':'SPLIT_KILL','changeNumber':1591996754396,'defaultTreatment':'some','splitName':'test'},
         )
         parsed0 = parse_incoming_event(e0)
         assert isinstance(parsed0, SplitKillUpdate)
         assert parsed0.default_treatment == 'some'
         assert parsed0.change_number == 1591996754396
-        assert parsed0.split_name == 'test'
+        assert parsed0.feature_flag_name == 'test'
+
+        e1 = make_message(
+            'NDA5ODc2MTAyNg==_MzAyODY0NDkyOA==_splits',
+            {'type':'SPLIT_UPDATE','changeNumber':1591996685190, 'pcn': 12, 'c': 2, 'd': 'eJzEUtFu2kAQ/BU0z4d0hw2Be0MFRVGJIx'},
+        )
+        parsed1 = parse_incoming_event(e1)
+        assert isinstance(parsed1, SplitChangeUpdate)
+        assert parsed1.change_number == 1591996685190
+        assert parsed1.previous_change_number == 12
+        assert parsed1.compression == 2
+        assert parsed1.feature_flag_definition == 'eJzEUtFu2kAQ/BU0z4d0hw2Be0MFRVGJIx'
 
         e1 = make_message(
             'NDA5ODc2MTAyNg==_MzAyODY0NDkyOA==_splits',
             {'type':'SPLIT_UPDATE','changeNumber':1591996685190},
         )
         parsed1 = parse_incoming_event(e1)
         assert isinstance(parsed1, SplitChangeUpdate)
         assert parsed1.change_number == 1591996685190
+        assert parsed1.previous_change_number == None
+        assert parsed1.compression == None
+        assert parsed1.feature_flag_definition == None
+
 
         e2 = make_message(
             'NDA5ODc2MTAyNg==_MzAyODY0NDkyOA==_segments',
             {'type':'SEGMENT_UPDATE','changeNumber':1591988398533,'segmentName':'some'},
         )
         parsed2 = parse_incoming_event(e2)
         assert isinstance(parsed2, SegmentChangeUpdate)
```

### Comparing `splitio_client-9.4.2/tests/push/test_splitsse.py` & `splitio_client-9.5.0/tests/push/test_splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/push/test_sse.py` & `splitio_client-9.5.0/tests/push/test_sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/push/test_segment_worker.py` & `splitio_client-9.5.0/tests/push/test_segment_worker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/push/test_status_tracker.py` & `splitio_client-9.5.0/tests/push/test_status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/push/test_manager.py` & `splitio_client-9.5.0/tests/push/test_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,68 +133,71 @@
         assert feedback_loop.get() == Status.PUSH_RETRYABLE_ERROR
         assert timer_mock.mock_calls == [mocker.call(0, Any())]
         assert sse_mock.mock_calls == []
 
     def test_split_change(self, mocker):
         """Test update-type messages are properly forwarded to the processor."""
         sse_event = SSEEvent('1', EventType.MESSAGE, '', '{}')
-        update_message = SplitChangeUpdate('chan', 123, 456)
+        update_message = SplitChangeUpdate('chan', 123, 456, None, None, None)
         parse_event_mock = mocker.Mock(spec=parse_incoming_event)
         parse_event_mock.return_value = update_message
         mocker.patch('splitio.push.manager.parse_incoming_event', new=parse_event_mock)
 
         processor_mock = mocker.Mock(spec=MessageProcessor)
         mocker.patch('splitio.push.manager.MessageProcessor', new=processor_mock)
 
-        telemetry_storage = InMemoryTelemetryStorage()
-        telemetry_producer = TelemetryStorageProducer(telemetry_storage)
-        telemetry_runtime_producer = telemetry_producer.get_telemetry_runtime_producer()
-        manager = PushManager(mocker.Mock(), mocker.Mock(), mocker.Mock(), mocker.Mock(), telemetry_runtime_producer)
+        telemetry_runtime_producer = mocker.Mock()
+        synchronizer = mocker.Mock()
+        manager = PushManager(mocker.Mock(), synchronizer, mocker.Mock(), mocker.Mock(), telemetry_runtime_producer)
         manager._event_handler(sse_event)
         assert parse_event_mock.mock_calls == [mocker.call(sse_event)]
         assert processor_mock.mock_calls == [
-            mocker.call(Any()),
+            mocker.call(synchronizer, telemetry_runtime_producer),
             mocker.call().handle(update_message)
         ]
 
     def test_split_kill(self, mocker):
         """Test update-type messages are properly forwarded to the processor."""
         sse_event = SSEEvent('1', EventType.MESSAGE, '', '{}')
         update_message = SplitKillUpdate('chan', 123, 456, 'some_split', 'off')
         parse_event_mock = mocker.Mock(spec=parse_incoming_event)
         parse_event_mock.return_value = update_message
         mocker.patch('splitio.push.manager.parse_incoming_event', new=parse_event_mock)
 
         processor_mock = mocker.Mock(spec=MessageProcessor)
         mocker.patch('splitio.push.manager.MessageProcessor', new=processor_mock)
 
-        manager = PushManager(mocker.Mock(), mocker.Mock(), mocker.Mock(), mocker.Mock(), mocker.Mock())
+        telemetry_runtime_producer = mocker.Mock()
+        synchronizer = mocker.Mock()
+        manager = PushManager(mocker.Mock(), synchronizer, mocker.Mock(), mocker.Mock(), telemetry_runtime_producer)
         manager._event_handler(sse_event)
         assert parse_event_mock.mock_calls == [mocker.call(sse_event)]
         assert processor_mock.mock_calls == [
-            mocker.call(Any()),
+            mocker.call(synchronizer, telemetry_runtime_producer),
             mocker.call().handle(update_message)
         ]
 
     def test_segment_change(self, mocker):
         """Test update-type messages are properly forwarded to the processor."""
         sse_event = SSEEvent('1', EventType.MESSAGE, '', '{}')
         update_message = SegmentChangeUpdate('chan', 123, 456, 'some_segment')
         parse_event_mock = mocker.Mock(spec=parse_incoming_event)
         parse_event_mock.return_value = update_message
         mocker.patch('splitio.push.manager.parse_incoming_event', new=parse_event_mock)
 
         processor_mock = mocker.Mock(spec=MessageProcessor)
         mocker.patch('splitio.push.manager.MessageProcessor', new=processor_mock)
 
-        manager = PushManager(mocker.Mock(), mocker.Mock(), mocker.Mock(), mocker.Mock(), mocker.Mock())
+        telemetry_runtime_producer = mocker.Mock()
+        synchronizer = mocker.Mock()
+        manager = PushManager(mocker.Mock(), synchronizer, mocker.Mock(), mocker.Mock(), telemetry_runtime_producer)
         manager._event_handler(sse_event)
         assert parse_event_mock.mock_calls == [mocker.call(sse_event)]
         assert processor_mock.mock_calls == [
-            mocker.call(Any()),
+            mocker.call(synchronizer, telemetry_runtime_producer),
             mocker.call().handle(update_message)
         ]
 
     def test_control_message(self, mocker):
         """Test control mesage is forwarded to status tracker."""
         sse_event = SSEEvent('1', EventType.MESSAGE, '', '{}')
         control_message = ControlMessage('chan', 123, ControlType.STREAMING_ENABLED)
```

### Comparing `splitio_client-9.4.2/tests/push/test_processor.py` & `splitio_client-9.5.0/tests/push/test_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     """Message processor test cases."""
 
     def test_split_change(self, mocker):
         """Test split change is properly handled."""
         sync_mock = mocker.Mock(spec=Synchronizer)
         queue_mock = mocker.Mock(spec=Queue)
         mocker.patch('splitio.push.processor.Queue', new=queue_mock)
-        processor = MessageProcessor(sync_mock)
-        update = SplitChangeUpdate('sarasa', 123, 123)
+        processor = MessageProcessor(sync_mock, mocker.Mock())
+        update = SplitChangeUpdate('sarasa', 123, 123, None, None, None)
         processor.handle(update)
         assert queue_mock.mock_calls == [
             mocker.call(),  # construction of split queue
             mocker.call(),  # construction of split queue
             mocker.call().put(update)
         ]
 
     def test_split_kill(self, mocker):
         """Test split kill is properly handled."""
         sync_mock = mocker.Mock(spec=Synchronizer)
         queue_mock = mocker.Mock(spec=Queue)
         mocker.patch('splitio.push.processor.Queue', new=queue_mock)
-        processor = MessageProcessor(sync_mock)
+        processor = MessageProcessor(sync_mock, mocker.Mock())
         update = SplitKillUpdate('sarasa', 123, 456, 'some_split', 'off')
         processor.handle(update)
         assert queue_mock.mock_calls == [
             mocker.call(),  # construction of split queue
             mocker.call(),  # construction of split queue
             mocker.call().put(update)
         ]
@@ -40,15 +40,15 @@
         ]
 
     def test_segment_change(self, mocker):
         """Test segment change is properly handled."""
         sync_mock = mocker.Mock(spec=Synchronizer)
         queue_mock = mocker.Mock(spec=Queue)
         mocker.patch('splitio.push.processor.Queue', new=queue_mock)
-        processor = MessageProcessor(sync_mock)
+        processor = MessageProcessor(sync_mock, mocker.Mock())
         update = SegmentChangeUpdate('sarasa', 123, 123, 'some_segment')
         processor.handle(update)
         assert queue_mock.mock_calls == [
             mocker.call(),  # construction of split queue
             mocker.call(),  # construction of split queue
             mocker.call().put(update)
         ]
```

### Comparing `splitio_client-9.4.2/tests/recorder/test_recorder.py` & `splitio_client-9.5.0/tests/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_impressions_count_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_impressions_count_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_unique_keys_sync.py` & `splitio_client-9.5.0/tests/sync/test_unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_segments_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_segments_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_impressions_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_impressions_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_splits_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_splits_synchronizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -263,19 +263,19 @@
                        ],
                        'combiner': 'AND'
                    }
                }
             ]
         }]
 
-        def read_splits_from_json_file(*args, **kwargs):
+        def read_feature_flags_from_json_file(*args, **kwargs):
                 return splits, till
 
         split_synchronizer = LocalSplitSynchronizer("split.json", storage, LocalhostMode.JSON)
-        split_synchronizer._read_splits_from_json_file = read_splits_from_json_file
+        split_synchronizer._read_feature_flags_from_json_file = read_feature_flags_from_json_file
 
         split_synchronizer.synchronize_splits()
         inserted_split = storage.get(splits[0]['name'])
         assert isinstance(inserted_split, Split)
         assert inserted_split.name == 'some_name'
 
         # Should sync when changenumber is not changed
@@ -395,130 +395,130 @@
         assert (split_synchronizer._sanitize_json_elements(parsed2) == parsed)
 
     def test_split_elements_sanitization(self, mocker):
         """Test sanitization."""
         split_synchronizer = LocalSplitSynchronizer(mocker.Mock(), mocker.Mock(), mocker.Mock())
 
         # No changes when split structure is good
-        assert (split_synchronizer._sanitize_split_elements(splits_json["splitChange1_1"]["splits"]) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(splits_json["splitChange1_1"]["splits"]) == splits_json["splitChange1_1"]["splits"])
 
         # test 'trafficTypeName' value None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficTypeName'] = None
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'trafficAllocation' value None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficAllocation'] = None
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'trafficAllocation' valid value should not change
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficAllocation'] = 50
-        assert (split_synchronizer._sanitize_split_elements(split) == split)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == split)
 
         # test 'trafficAllocation' invalid value should change
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficAllocation'] = 110
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'trafficAllocationSeed' is set to millisec epoch when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficAllocationSeed'] = None
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['trafficAllocationSeed'] > 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['trafficAllocationSeed'] > 0)
 
         # test 'trafficAllocationSeed' is set to millisec epoch when 0
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['trafficAllocationSeed'] = 0
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['trafficAllocationSeed'] > 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['trafficAllocationSeed'] > 0)
 
         # test 'seed' is set to millisec epoch when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['seed'] = None
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['seed'] > 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['seed'] > 0)
 
         # test 'seed' is set to millisec epoch when its 0
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['seed'] = 0
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['seed'] > 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['seed'] > 0)
 
         # test 'status' is set to ACTIVE when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['status'] = None
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'status' is set to ACTIVE when incorrect
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['status'] = 'ww'
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test ''killed' is set to False when incorrect
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['killed'] = None
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'defaultTreatment' is set to on when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['defaultTreatment'] = None
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['defaultTreatment'] == 'control')
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['defaultTreatment'] == 'control')
 
         # test 'defaultTreatment' is set to on when its empty
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['defaultTreatment'] = ' '
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['defaultTreatment'] == 'control')
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['defaultTreatment'] == 'control')
 
         # test 'changeNumber' is set to 0 when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['changeNumber'] = None
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['changeNumber'] == 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['changeNumber'] == 0)
 
         # test 'changeNumber' is set to 0 when invalid
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['changeNumber'] = -33
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['changeNumber'] == 0)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['changeNumber'] == 0)
 
         # test 'algo' is set to 2 when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['algo'] = None
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['algo'] == 2)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['algo'] == 2)
 
         # test 'algo' is set to 2 when higher than 2
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['algo'] = 3
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['algo'] == 2)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['algo'] == 2)
 
         # test 'algo' is set to 2 when lower than 2
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['algo'] = 1
-        assert (split_synchronizer._sanitize_split_elements(split)[0]['algo'] == 2)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split)[0]['algo'] == 2)
 
     def test_split_condition_sanitization(self, mocker):
         """Test sanitization."""
         split_synchronizer = LocalSplitSynchronizer(mocker.Mock(), mocker.Mock(), mocker.Mock())
 
         # test missing all conditions with default rule set to 100% off
         split = splits_json["splitChange1_1"]["splits"].copy()
         target_split = splits_json["splitChange1_1"]["splits"].copy()
         target_split[0]["conditions"][0]['partitions'][0]['size'] = 0
         target_split[0]["conditions"][0]['partitions'][1]['size'] = 100
         del split[0]["conditions"]
-        assert (split_synchronizer._sanitize_split_elements(split) == target_split)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == target_split)
 
         # test missing ALL_KEYS condition matcher with default rule set to 100% off
         split = splits_json["splitChange1_1"]["splits"].copy()
         target_split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]["conditions"][0]["matcherGroup"]["matchers"][0]["matcherType"] = "IN_STR"
         target_split = split.copy()
         target_split[0]["conditions"].append(splits_json["splitChange1_1"]["splits"][0]["conditions"][0])
         target_split[0]["conditions"][1]['partitions'][0]['size'] = 0
         target_split[0]["conditions"][1]['partitions'][1]['size'] = 100
-        assert (split_synchronizer._sanitize_split_elements(split) == target_split)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == target_split)
 
         # test missing ROLLOUT condition type with default rule set to 100% off
         split = splits_json["splitChange1_1"]["splits"].copy()
         target_split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]["conditions"][0]["conditionType"] = "NOT"
         target_split = split.copy()
         target_split[0]["conditions"].append(splits_json["splitChange1_1"]["splits"][0]["conditions"][0])
         target_split[0]["conditions"][1]['partitions'][0]['size'] = 0
         target_split[0]["conditions"][1]['partitions'][1]['size'] = 100
-        assert (split_synchronizer._sanitize_split_elements(split) == target_split)
+        assert (split_synchronizer._sanitize_feature_flag_elements(split) == target_split)
```

### Comparing `splitio_client-9.4.2/tests/sync/test_manager.py` & `splitio_client-9.5.0/tests/sync/test_manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/sync/test_telemetry.py` & `splitio_client-9.5.0/tests/sync/test_telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         telemetry_storage._counters._impressions_deduped = 30
         telemetry_storage._counters._impressions_dropped = 0
         telemetry_storage._counters._events_queued = 20
         telemetry_storage._counters._events_dropped = 10
         telemetry_storage._counters._auth_rejections = 1
         telemetry_storage._counters._token_refreshes = 3
         telemetry_storage._counters._session_length = 3
+        telemetry_storage._counters._update_from_sse['sp'] = 3
 
         telemetry_storage._method_exceptions._treatment =  10
         telemetry_storage._method_exceptions._treatments = 1
         telemetry_storage._method_exceptions._treatment_with_config = 5
         telemetry_storage._method_exceptions._treatments_with_config = 1
         telemetry_storage._method_exceptions._track = 3
 
@@ -130,9 +131,10 @@
             "sE": [],
             "sL": 3,
             "mE": {"t": 10, "ts": 1, "tc": 5, "tcs": 1, "tr": 3},
             "mL": {"t": [1] + [0] * 22, "ts": [0] * 23, "tc": [0] * 23, "tcs": [0] * 23, "tr": [0] * 23},
             "spC": 1,
             "seC": 1,
             "skC": 0,
+            "ufs": {"sp": 3},
             "t": ['tag1']
         })
```

### Comparing `splitio_client-9.4.2/tests/sync/test_events_synchronizer.py` & `splitio_client-9.5.0/tests/sync/test_events_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/tests/helpers/mockserver.py` & `splitio_client-9.5.0/tests/helpers/mockserver.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/README.md` & `splitio_client-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/setup.py` & `splitio_client-9.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 INSTALL_REQUIRES = [
     'requests>=2.9.1',
     'pyyaml>=5.4',
     'docopt>=0.6.2',
     'enum34;python_version<"3.4"',
-    'bloom-filter2>=2.0.0',
+    'bloom-filter2>=2.0.0'
 ]
 
 with open(path.join(path.abspath(path.dirname(__file__)), 'splitio', 'version.py')) as f:
     exec(f.read())  # pylint: disable=exec-used
 
 setup(
     name='splitio_client',
@@ -40,15 +40,15 @@
     tests_require=TESTS_REQUIRES,
     extras_require={
         'test': TESTS_REQUIRES,
         'redis': ['redis>=2.10.5'],
         'uwsgi': ['uwsgi>=2.0.0'],
         'cpphash': ['mmh3cffi==0.2.1'],
     },
-    setup_requires=['pytest-runner'],
+    setup_requires=['pytest-runner', 'pluggy==1.0.0;python_version<"3.7"'],
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries'
```

### Comparing `splitio_client-9.4.2/splitio/tasks/split_sync.py` & `splitio_client-9.5.0/splitio/tasks/split_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/util/workerpool.py` & `splitio_client-9.5.0/splitio/tasks/util/workerpool.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/util/asynctask.py` & `splitio_client-9.5.0/splitio/tasks/util/asynctask.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/telemetry_sync.py` & `splitio_client-9.5.0/splitio/tasks/telemetry_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/__init__.py` & `splitio_client-9.5.0/splitio/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/events_sync.py` & `splitio_client-9.5.0/splitio/tasks/events_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/segment_sync.py` & `splitio_client-9.5.0/splitio/tasks/segment_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/impressions_sync.py` & `splitio_client-9.5.0/splitio/tasks/impressions_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/tasks/unique_keys_sync.py` & `splitio_client-9.5.0/splitio/tasks/unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/util/time.py` & `splitio_client-9.5.0/splitio/util/time.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/util/backoff.py` & `splitio_client-9.5.0/splitio/util/backoff.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/util/threadutil.py` & `splitio_client-9.5.0/splitio/util/threadutil.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/partitions.py` & `splitio_client-9.5.0/splitio/models/grammar/partitions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/condition.py` & `splitio_client-9.5.0/splitio/models/grammar/condition.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/misc.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/misc.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/__init__.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/keys.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/numeric.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/numeric.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/string.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/string.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/sets.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/sets.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/grammar/matchers/base.py` & `splitio_client-9.5.0/splitio/models/grammar/matchers/base.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/token.py` & `splitio_client-9.5.0/splitio/models/token.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/segments.py` & `splitio_client-9.5.0/splitio/models/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/notification.py` & `splitio_client-9.5.0/splitio/models/notification.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/telemetry.py` & `splitio_client-9.5.0/splitio/models/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,18 @@
 
 class OperationMode(Enum):
     """Storage modes constants"""
     STANDALONE = 'standalone'
     CONSUMER = 'consumer'
     PARTIAL_CONSUMER = 'partial_consumer'
 
+class UpdateFromSSE(Enum):
+    """Update from sse constants"""
+    SPLIT_UPDATE = 'sp'
+
 def get_latency_bucket_index(micros):
     """
     Find the bucket index for a measured latency.
 
     :param micros: Measured latency in microseconds
     :type micros: int
     :return: Bucket index for the given latency
@@ -478,14 +482,15 @@
             self._impressions_deduped = 0
             self._impressions_dropped = 0
             self._events_queued = 0
             self._events_dropped = 0
             self._auth_rejections = 0
             self._token_refreshes = 0
             self._session_length = 0
+            self._update_from_sse = {}
 
     def record_impressions_value(self, resource, value):
         """
         Append to the resource value
 
         :param resource: passed resource name
         :type resource: str
@@ -515,25 +520,35 @@
             if resource == CounterConstants.EVENTS_QUEUED:
                 self._events_queued += value
             elif resource == CounterConstants.EVENTS_DROPPED:
                 self._events_dropped += value
             else:
                 return
 
+    def record_update_from_sse(self, event):
+        """
+        Increment the update from sse resource by one.
+
+        """
+        with self._lock:
+            if event.value not in self._update_from_sse:
+                self._update_from_sse[event.value] = 0
+            self._update_from_sse[event.value] += 1
+
     def record_auth_rejections(self):
         """
-        Increament the auth rejection resource by one.
+        Increment the auth rejection resource by one.
 
         """
         with self._lock:
             self._auth_rejections += 1
 
     def record_token_refreshes(self):
         """
-        Increament the token refreshes resource by one.
+        Increment the token refreshes resource by one.
 
         """
         with self._lock:
             self._token_refreshes += 1
 
     def record_session_length(self, session):
         """
@@ -600,14 +615,26 @@
         :rtype: int
         """
         with self._lock:
             token_refreshes = self._token_refreshes
             self._token_refreshes = 0
             return token_refreshes
 
+    def pop_update_from_sse(self, event):
+        """
+        Pop update from sse
+
+        :return: update from sse value
+        :rtype: int
+        """
+        with self._lock:
+            update_from_sse = self._update_from_sse[event.value]
+            self._update_from_sse[event.value] = 0
+            return update_from_sse
+
 class StreamingEvent(object):
     """
     Streaming event class
 
     """
     def __init__(self, streaming_event):
         """
```

### Comparing `splitio_client-9.4.2/splitio/models/impressions.py` & `splitio_client-9.5.0/splitio/models/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/datatypes.py` & `splitio_client-9.5.0/splitio/models/datatypes.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/models/splits.py` & `splitio_client-9.5.0/splitio/models/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/pluggable.py` & `splitio_client-9.5.0/splitio/storage/pluggable.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/__init__.py` & `splitio_client-9.5.0/splitio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/adapters/util.py` & `splitio_client-9.5.0/splitio/storage/adapters/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/adapters/cache_trait.py` & `splitio_client-9.5.0/splitio/storage/adapters/cache_trait.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/adapters/redis.py` & `splitio_client-9.5.0/splitio/storage/adapters/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/redis.py` & `splitio_client-9.5.0/splitio/storage/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/storage/inmemmory.py` & `splitio_client-9.5.0/splitio/storage/inmemmory.py`

 * *Files 4% similar despite different names*

```diff
@@ -559,14 +559,18 @@
         """Record incoming streaming event."""
         self._streaming_events.record_streaming_event(streaming_event)
 
     def record_session_length(self, session):
         """Record session length."""
         self._counters.record_session_length(session)
 
+    def record_update_from_sse(self, event):
+        """Record update from sse."""
+        self._counters.record_update_from_sse(event)
+
     def get_bur_time_outs(self):
         """Get block until ready timeout."""
         return self._tel_config.get_bur_time_outs()
 
     def get_non_ready_usage(self):
         """Get non-ready usage."""
         return self._tel_config.get_non_ready_usage()
@@ -628,14 +632,18 @@
     def pop_streaming_events(self):
         return self._streaming_events.pop_streaming_events()
 
     def get_session_length(self):
         """Get session length"""
         return self._counters.get_session_length()
 
+    def pop_update_from_sse(self, event):
+        """Get and reset update from sse."""
+        return self._counters.pop_update_from_sse(event)
+
 class LocalhostTelemetryStorage():
     """Localhost telemetry storage."""
     def do_nothing(*_, **__):
         return {}
 
     def __getattr__(self, _):
         return self.do_nothing
```

### Comparing `splitio_client-9.4.2/splitio/push/splitsse.py` & `splitio_client-9.5.0/splitio/push/splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/push/segmentworker.py` & `splitio_client-9.5.0/splitio/push/segmentworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/push/processor.py` & `splitio_client-9.5.0/splitio/push/processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,55 +2,54 @@
 
 from queue import Queue
 
 from splitio.push.parser import UpdateType
 from splitio.push.splitworker import SplitWorker
 from splitio.push.segmentworker import SegmentWorker
 
-
 class MessageProcessor(object):
     """Message processor class."""
 
-    def __init__(self, synchronizer):
+    def __init__(self, synchronizer, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param synchronizer: synchronizer component
         :type synchronizer: splitio.sync.synchronizer.Synchronizer
         """
-        self._split_queue = Queue()
+        self._feature_flag_queue = Queue()
         self._segments_queue = Queue()
         self._synchronizer = synchronizer
-        self._split_worker = SplitWorker(synchronizer.synchronize_splits, self._split_queue)
+        self._feature_flag_worker = SplitWorker(synchronizer.synchronize_splits, synchronizer.synchronize_segment, self._feature_flag_queue, synchronizer.split_sync.feature_flag_storage, synchronizer.segment_storage, telemetry_runtime_producer)
         self._segments_worker = SegmentWorker(synchronizer.synchronize_segment, self._segments_queue)
         self._handlers = {
-            UpdateType.SPLIT_UPDATE: self._handle_split_update,
-            UpdateType.SPLIT_KILL: self._handle_split_kill,
+            UpdateType.SPLIT_UPDATE: self._handle_feature_flag_update,
+            UpdateType.SPLIT_KILL: self._handle_feature_flag_kill,
             UpdateType.SEGMENT_UPDATE: self._handle_segment_change
         }
 
-    def _handle_split_update(self, event):
+    def _handle_feature_flag_update(self, event):
         """
-        Handle incoming split update notification.
+        Handle incoming feature flag update notification.
 
-        :param event: Incoming split change event
+        :param event: Incoming feature flag change event
         :type event: splitio.push.parser.SplitChangeUpdate
         """
-        self._split_queue.put(event)
+        self._feature_flag_queue.put(event)
 
-    def _handle_split_kill(self, event):
+    def _handle_feature_flag_kill(self, event):
         """
-        Handle incoming split kill notification.
+        Handle incoming feature flag kill notification.
 
-        :param event: Incoming split kill event
+        :param event: Incoming feature flag kill event
         :type event: splitio.push.parser.SplitKillUpdate
         """
-        self._synchronizer.kill_split(event.split_name, event.default_treatment,
+        self._synchronizer.kill_split(event.feature_flag_name, event.default_treatment,
                                       event.change_number)
-        self._split_queue.put(event)
+        self._feature_flag_queue.put(event)
 
     def _handle_segment_change(self, event):
         """
         Handle incoming segment update notification.
 
         :param event: Incoming segment change event
         :type event: splitio.push.parser.Update
@@ -61,18 +60,18 @@
         """
         Enable/Disable push update workers.
 
         :param enabled: if True, enable workers. If False, disable them.
         :type enabled: bool
         """
         if enabled:
-            self._split_worker.start()
+            self._feature_flag_worker.start()
             self._segments_worker.start()
         else:
-            self._split_worker.stop()
+            self._feature_flag_worker.stop()
             self._segments_worker.stop()
 
     def handle(self, event):
         """
         Handle incoming update event.
 
         :param event: incoming data update event.
@@ -82,10 +81,10 @@
             handle = self._handlers[event.update_type]
         except KeyError as exc:
             raise Exception('no handler for notification type: %s' % event.update_type) from exc
 
         handle(event)
 
     def shutdown(self):
-        """Stop splits & segments workers."""
-        self._split_worker.stop()
+        """Stop feature flags & segments workers."""
+        self._feature_flag_worker.stop()
         self._segments_worker.stop()
```

### Comparing `splitio_client-9.4.2/splitio/push/sse.py` & `splitio_client-9.5.0/splitio/push/sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/push/parser.py` & `splitio_client-9.5.0/splitio/push/parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 from enum import Enum
 
 from splitio.util.decorators import abstract_property
 from splitio.util.time import utctime_ms
 from splitio.push.sse import SSE_EVENT_ERROR, SSE_EVENT_MESSAGE
 
-
 class EventType(Enum):
     """Event type enumeration."""
 
     MESSAGE = SSE_EVENT_MESSAGE
     ERROR = SSE_EVENT_ERROR
 
 
@@ -273,15 +272,15 @@
 
     def __str__(self):
         """Return string representation."""
         return "Occupancy - channel=%s, publishers=%d" % (self.channel, self.publishers)
 
 
 class BaseUpdate(BaseMessage, metaclass=abc.ABCMeta):
-    """Split data update notification."""
+    """Feature flag data update notification."""
 
     def __init__(self, channel, timestamp, change_number):
         """
         Construct an update event.
 
         :param data: raw message data.
         :type data: dict
@@ -320,78 +319,111 @@
         :returns: change number
         :rtype: int
         """
         return self._change_number
 
 
 class SplitChangeUpdate(BaseUpdate):
-    """Split Change notification."""
+    """Feature flag Change notification."""
 
-    def __init__(self, channel, timestamp, change_number):
+    def __init__(self, channel, timestamp, change_number, previous_change_number, feature_flag_definition, compression):
         """Class constructor."""
         BaseUpdate.__init__(self, channel, timestamp, change_number)
+        self._previous_change_number = previous_change_number
+        self._feature_flag_definition = feature_flag_definition
+        self._compression = compression
 
     @property
     def update_type(self):  # pylint:disable=no-self-use
         """
         Return the message type.
 
         :returns: The type of this parsed Update.
         :rtype: UpdateType
         """
         return UpdateType.SPLIT_UPDATE
 
+    @property
+    def previous_change_number(self):  # pylint:disable=no-self-use
+        """
+        Return previous change number
+
+        :returns: The previous change number
+        :rtype: int
+        """
+        return self._previous_change_number
+
+    @property
+    def feature_flag_definition(self):  # pylint:disable=no-self-use
+        """
+        Return feature flag definition
+
+        :returns: The new feature flag definition
+        :rtype: str
+        """
+        return self._feature_flag_definition
+
+    @property
+    def compression(self):  # pylint:disable=no-self-use
+        """
+        Return previous compression type
+
+        :returns: The compression type
+        :rtype: int
+        """
+        return self._compression
+
     def __str__(self):
         """Return string representation."""
         return "SplitChange - changeNumber=%d" % (self.change_number)
 
 
 class SplitKillUpdate(BaseUpdate):
-    """Split Kill notification."""
+    """Feature flag Kill notification."""
 
-    def __init__(self, channel, timestamp, change_number, split_name, default_treatment):  # pylint:disable=too-many-arguments
+    def __init__(self, channel, timestamp, change_number, feature_flag_name, default_treatment):  # pylint:disable=too-many-arguments
         """Class constructor."""
         BaseUpdate.__init__(self, channel, timestamp, change_number)
-        self._split_name = split_name
+        self._feature_flag_name = feature_flag_name
         self._default_treatment = default_treatment
 
     @property
     def update_type(self):  # pylint:disable=no-self-use
         """
         Return the message type.
 
         :returns: The type of this parsed Update.
         :rtype: UpdateType
         """
         return UpdateType.SPLIT_KILL
 
     @property
-    def split_name(self):
+    def feature_flag_name(self):
         """
-        Return the name of the killed split.
+        Return the name of the killed feature flag.
 
-        :returns: name of the killed split
+        :returns: name of the killed feature flag
         :rtype: str
         """
-        return self._split_name
+        return self._feature_flag_name
 
     @property
     def default_treatment(self):
         """
         Return the default treatment.
 
         :returns: default treatment
         :rtype: str
         """
         return self._default_treatment
 
     def __str__(self):
         """Return string representation."""
         return "SplitKill - changeNumber=%d, name=%s, defaultTreatment=%s" % \
-            (self.change_number, self.split_name, self.default_treatment)
+            (self.change_number, self.feature_flag_name, self.default_treatment)
 
 
 class SegmentChangeUpdate(BaseUpdate):
     """Segment Change notification."""
 
     def __init__(self, channel, timestamp, change_number, segment_name):
         """Class constructor."""
@@ -467,17 +499,17 @@
     :type data: dict
 
     :returns: Parsed ably error notification.
     :rtype: BaseUpdate
     """
     update_type = UpdateType(data['type'])
     change_number = data['changeNumber']
-    if update_type == UpdateType.SPLIT_UPDATE:
-        return SplitChangeUpdate(channel, timestamp, change_number)
-    elif update_type == UpdateType.SPLIT_KILL:
+    if update_type == UpdateType.SPLIT_UPDATE and change_number is not None:
+        return SplitChangeUpdate(channel, timestamp, change_number, data.get('pcn'), data.get('d'), data.get('c'))
+    elif update_type == UpdateType.SPLIT_KILL and change_number is not None:
         return SplitKillUpdate(channel, timestamp, change_number,
                                data['splitName'], data['defaultTreatment'])
     elif update_type == UpdateType.SEGMENT_UPDATE:
         return SegmentChangeUpdate(channel, timestamp, change_number, data['segmentName'])
     raise EventParsingException('unrecognized event type %s' % update_type)
```

### Comparing `splitio_client-9.4.2/splitio/push/status_tracker.py` & `splitio_client-9.5.0/splitio/push/status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/push/manager.py` & `splitio_client-9.5.0/splitio/push/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         :type sse_url: str
 
         :param client_key: client key.
         :type client_key: str
         """
         self._auth_api = auth_api
         self._feedback_loop = feedback_loop
-        self._processor = MessageProcessor(synchronizer)
+        self._processor = MessageProcessor(synchronizer, telemetry_runtime_producer)
         self._status_tracker = PushStatusTracker(telemetry_runtime_producer)
         self._event_handlers = {
             EventType.MESSAGE: self._handle_message,
             EventType.ERROR: self._handle_error
         }
 
         self._message_handlers = {
```

### Comparing `splitio_client-9.4.2/splitio/recorder/recorder.py` & `splitio_client-9.5.0/splitio/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/auth.py` & `splitio_client-9.5.0/splitio/api/auth.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/events.py` & `splitio_client-9.5.0/splitio/api/events.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/segments.py` & `splitio_client-9.5.0/splitio/api/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/client.py` & `splitio_client-9.5.0/splitio/api/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/telemetry.py` & `splitio_client-9.5.0/splitio/api/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/impressions.py` & `splitio_client-9.5.0/splitio/api/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/commons.py` & `splitio_client-9.5.0/splitio/api/commons.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/api/splits.py` & `splitio_client-9.5.0/splitio/api/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/impression.py` & `splitio_client-9.5.0/splitio/sync/impression.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/event.py` & `splitio_client-9.5.0/splitio/sync/event.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/util.py` & `splitio_client-9.5.0/splitio/sync/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/telemetry.py` & `splitio_client-9.5.0/splitio/sync/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Telemetry Sync Class."""
 import abc
 
 from splitio.api.telemetry import TelemetryAPI
 from splitio.engine.telemetry import TelemetryStorageConsumer
+from splitio.models.telemetry import UpdateFromSSE
 
 class TelemetrySynchronizer(object):
     """Telemetry synchronizer class."""
 
     def __init__(self, telemetry_submitter):
         """Initialize Telemetry sync class."""
         self._telemetry_submitter = telemetry_submitter
```

### Comparing `splitio_client-9.4.2/splitio/sync/split.py` & `splitio_client-9.5.0/splitio/sync/split.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,30 +26,35 @@
 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT = 30  # don't sleep for more than 30 seconds
 _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES = 10
 
 
 class SplitSynchronizer(object):
     """Feature Flag changes synchronizer."""
 
-    def __init__(self, split_api, split_storage):
+    def __init__(self, feature_flag_api, feature_flag_storage):
         """
         Class constructor.
 
         :param split_api: Feature Flag API Client.
         :type split_api: splitio.api.splits.SplitsAPI
 
-        :param split_storage: Feature Flag Storage.
-        :type split_storage: splitio.storage.InMemorySplitStorage
+        :param feature_flag_storage: Feature Flag Storage.
+        :type feature_flag_storage: splitio.storage.InMemorySplitStorage
         """
-        self._api = split_api
-        self._split_storage = split_storage
+        self._api = feature_flag_api
+        self._feature_flag_storage = feature_flag_storage
         self._backoff = Backoff(
                                 _ON_DEMAND_FETCH_BACKOFF_BASE,
                                 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT)
 
+    @property
+    def feature_flag_storage(self):
+        """Return Feature_flag storage object"""
+        return self._feature_flag_storage
+
     def _fetch_until(self, fetch_options, till=None):
         """
         Hit endpoint, update storage and return when since==till.
 
         :param fetch_options Fetch options for getting feature flag definitions.
         :type fetch_options splitio.api.FetchOptions
 
@@ -57,40 +62,40 @@
         :type till: int
 
         :return: last change number
         :rtype: int
         """
         segment_list = set()
         while True:  # Fetch until since==till
-            change_number = self._split_storage.get_change_number()
+            change_number = self._feature_flag_storage.get_change_number()
             if change_number is None:
                 change_number = -1
             if till is not None and till < change_number:
                 # the passed till is less than change_number, no need to perform updates
                 return change_number, segment_list
 
             try:
-                split_changes = self._api.fetch_splits(change_number, fetch_options)
+                feature_flag_changes = self._api.fetch_splits(change_number, fetch_options)
             except APIException as exc:
                 _LOGGER.error('Exception raised while fetching feature flags')
                 _LOGGER.debug('Exception information: ', exc_info=True)
                 raise exc
 
-            for split in split_changes.get('splits', []):
-                if split['status'] == splits.Status.ACTIVE.value:
-                    parsed = splits.from_raw(split)
-                    self._split_storage.put(parsed)
+            for feature_flag in feature_flag_changes.get('splits', []):
+                if feature_flag['status'] == splits.Status.ACTIVE.value:
+                    parsed = splits.from_raw(feature_flag)
+                    self._feature_flag_storage.put(parsed)
                     segment_list.update(set(parsed.get_segment_names()))
                 else:
-                    self._split_storage.remove(split['name'])
-            self._split_storage.set_change_number(split_changes['till'])
-            if split_changes['till'] == split_changes['since']:
-                return split_changes['till'], segment_list
+                    self._feature_flag_storage.remove(feature_flag['name'])
+            self._feature_flag_storage.set_change_number(feature_flag_changes['till'])
+            if feature_flag_changes['till'] == feature_flag_changes['since']:
+                return feature_flag_changes['till'], segment_list
 
-    def _attempt_split_sync(self, fetch_options, till=None):
+    def _attempt_feature_flag_sync(self, fetch_options, till=None):
         """
         Hit endpoint, update storage and return True if sync is complete.
 
         :param fetch_options Fetch options for getting feature flag definitions.
         :type fetch_options splitio.api.FetchOptions
 
         :param till: Passed till from Streaming.
@@ -118,85 +123,85 @@
         Hit endpoint, update storage and return True if sync is complete.
 
         :param till: Passed till from Streaming.
         :type till: int
         """
         final_segment_list = set()
         fetch_options = FetchOptions(True)  # Set Cache-Control to no-cache
-        successful_sync, remaining_attempts, change_number, segment_list = self._attempt_split_sync(fetch_options,
+        successful_sync, remaining_attempts, change_number, segment_list = self._attempt_feature_flag_sync(fetch_options,
                                                                                       till)
         final_segment_list.update(segment_list)
         attempts = _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES - remaining_attempts
         if successful_sync:  # succedeed sync
             _LOGGER.debug('Refresh completed in %d attempts.', attempts)
             return final_segment_list
         with_cdn_bypass = FetchOptions(True, change_number)  # Set flag for bypassing CDN
-        without_cdn_successful_sync, remaining_attempts, change_number, segment_list = self._attempt_split_sync(with_cdn_bypass, till)
+        without_cdn_successful_sync, remaining_attempts, change_number, segment_list = self._attempt_feature_flag_sync(with_cdn_bypass, till)
         final_segment_list.update(segment_list)
         without_cdn_attempts = _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES - remaining_attempts
         if without_cdn_successful_sync:
             _LOGGER.debug('Refresh completed bypassing the CDN in %d attempts.',
                           without_cdn_attempts)
             return final_segment_list
         else:
             _LOGGER.debug('No changes fetched after %d attempts with CDN bypassed.',
                           without_cdn_attempts)
 
-    def kill_split(self, split_name, default_treatment, change_number):
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
         """
         Local kill for feature flag.
 
-        :param split_name: name of the feature flag to perform kill
-        :type split_name: str
+        :param feature_flag_name: name of the feature flag to perform kill
+        :type feature_flag_name: str
         :param default_treatment: name of the default treatment to return
         :type default_treatment: str
         :param change_number: change_number
         :type change_number: int
         """
-        self._split_storage.kill_locally(split_name, default_treatment, change_number)
+        self._feature_flag_storage.kill_locally(feature_flag_name, default_treatment, change_number)
 
 class LocalhostMode(Enum):
     """types for localhost modes"""
     LEGACY = 0
     YAML = 1
     JSON = 2
 
 class LocalSplitSynchronizer(object):
-    """Localhost mode split synchronizer."""
+    """Localhost mode feature_flag synchronizer."""
 
-    _DEFAULT_SPLIT_TILL = -1
+    _DEFAULT_FEATURE_FLAG_TILL = -1
 
-    def __init__(self, filename, split_storage, localhost_mode=LocalhostMode.LEGACY):
+    def __init__(self, filename, feature_flag_storage, localhost_mode=LocalhostMode.LEGACY):
         """
         Class constructor.
 
         :param filename: File to parse feature flags from.
         :type filename: str
-        :param split_storage: Feature flag Storage.
-        :type split_storage: splitio.storage.InMemorySplitStorage
+        :param feature_flag_storage: Feature flag Storage.
+        :type feature_flag_storage: splitio.storage.InMemorySplitStorage
         :param localhost_mode: mode for localhost either JSON, YAML or LEGACY.
         :type localhost_mode: splitio.sync.split.LocalhostMode
         """
         self._filename = filename
-        self._split_storage = split_storage
+        self._feature_flag_storage = feature_flag_storage
         self._localhost_mode = localhost_mode
         self._current_json_sha = "-1"
 
     @staticmethod
-    def _make_split(split_name, conditions, configs=None):
+    def _make_feature_flag(feature_flag_name, conditions, configs=None):
         """
         Make a Feature flag with a single all_keys matcher.
 
-        :param split_name: Name of the feature flag.
-        :type split_name: str.
+        :param feature_flag_name: Name of the feature flag.
+        :type feature_flag_name: str.
         """
         return splits.from_raw({
             'changeNumber': 123,
             'trafficTypeName': 'user',
-            'name': split_name,
+            'name': feature_flag_name,
             'trafficAllocation': 100,
             'trafficAllocationSeed': 123456,
             'seed': 321654,
             'status': 'ACTIVE',
             'killed': False,
             'defaultTreatment': 'control',
             'algo': 2,
@@ -242,15 +247,15 @@
                     }
                 ],
                 'combiner': 'AND'
             }
         }
 
     @classmethod
-    def _read_splits_from_legacy_file(cls, filename):
+    def _read_feature_flags_from_legacy_file(cls, filename):
         """
         Parse a feature flags file and return a populated storage.
 
         :param filename: Path of the file containing mocked feature flags & treatments.
         :type filename: str.
 
         :return: Storage populataed with feature flags ready to be evaluated.
@@ -269,23 +274,23 @@
                             'Invalid line on localhost environment feature flag '
                             'definition. Line = %s',
                             line
                         )
                         continue
 
                     cond = cls._make_all_keys_condition(definition_match.group('treatment'))
-                    splt = cls._make_split(definition_match.group('feature'), [cond])
+                    splt = cls._make_feature_flag(definition_match.group('feature'), [cond])
                     to_return[splt.name] = splt
             return to_return
 
         except IOError as exc:
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
     @classmethod
-    def _read_splits_from_yaml_file(cls, filename):
+    def _read_feature_flags_from_yaml_file(cls, filename):
         """
         Parse a feature flags file and return a populated storage.
 
         :param filename: Path of the file containing mocked feature flags & treatments.
         :type filename: str.
 
         :return: Storage populated with feature flags ready to be evaluated.
@@ -296,28 +301,28 @@
                 parsed = yaml.load(flo.read(), Loader=yaml.FullLoader)
 
             grouped_by_feature_name = itertools.groupby(
                 sorted(parsed, key=lambda i: next(iter(i.keys()))),
                 lambda i: next(iter(i.keys())))
 
             to_return = {}
-            for (split_name, statements) in grouped_by_feature_name:
+            for (feature_flag_name, statements) in grouped_by_feature_name:
                 configs = {}
                 whitelist = []
                 all_keys = []
                 for statement in statements:
                     data = next(iter(statement.values()))  # grab the first (and only) value.
                     if 'keys' in data:
                         keys = data['keys'] if isinstance(data['keys'], list) else [data['keys']]
                         whitelist.append(cls._make_whitelist_condition(keys, data['treatment']))
                     else:
                         all_keys.append(cls._make_all_keys_condition(data['treatment']))
                     if 'config' in data:
                         configs[data['treatment']] = data['config']
-                to_return[split_name] = cls._make_split(split_name, whitelist + all_keys, configs)
+                to_return[feature_flag_name] = cls._make_feature_flag(feature_flag_name, whitelist + all_keys, configs)
             return to_return
 
         except IOError as exc:
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
     def synchronize_splits(self, till=None):  # pylint:disable=unused-argument
         """Update feature flags in storage."""
@@ -333,88 +338,88 @@
         Update feature flags in storage for legacy mode.
 
         :return: empty array for compatibility with json mode
         :rtype: []
         """
 
         if self._filename.lower().endswith(('.yaml', '.yml')):
-            fetched = self._read_splits_from_yaml_file(self._filename)
+            fetched = self._read_feature_flags_from_yaml_file(self._filename)
         else:
-            fetched = self._read_splits_from_legacy_file(self._filename)
-        to_delete = [name for name in self._split_storage.get_split_names()
+            fetched = self._read_feature_flags_from_legacy_file(self._filename)
+        to_delete = [name for name in self._feature_flag_storage.get_split_names()
                      if name not in fetched.keys()]
-        for split in fetched.values():
-            self._split_storage.put(split)
+        for feature_flag in fetched.values():
+            self._feature_flag_storage.put(feature_flag)
 
-        for split in to_delete:
-            self._split_storage.remove(split)
+        for feature_flag in to_delete:
+            self._feature_flag_storage.remove(feature_flag)
 
         return []
 
     def _synchronize_json(self):
         """
         Update feature flags in storage for json mode.
 
         :return: segment names string array
         :rtype: [str]
         """
         try:
-            fetched, till = self._read_splits_from_json_file(self._filename)
+            fetched, till = self._read_feature_flags_from_json_file(self._filename)
             segment_list = set()
             fecthed_sha = util._get_sha(json.dumps(fetched))
             if fecthed_sha == self._current_json_sha:
                 return []
             self._current_json_sha = fecthed_sha
-            if self._split_storage.get_change_number() > till and till != self._DEFAULT_SPLIT_TILL:
+            if self._feature_flag_storage.get_change_number() > till and till != self._DEFAULT_FEATURE_FLAG_TILL:
                 return []
-            for split in fetched:
-                if split['status'] == splits.Status.ACTIVE.value:
-                    parsed = splits.from_raw(split)
-                    self._split_storage.put(parsed)
+            for feature_flag in fetched:
+                if feature_flag['status'] == splits.Status.ACTIVE.value:
+                    parsed = splits.from_raw(feature_flag)
+                    self._feature_flag_storage.put(parsed)
                     _LOGGER.debug("feature flag %s is updated", parsed.name)
                     segment_list.update(set(parsed.get_segment_names()))
                 else:
-                    self._split_storage.remove(split['name'])
+                    self._feature_flag_storage.remove(feature_flag['name'])
 
-                self._split_storage.set_change_number(till)
+                self._feature_flag_storage.set_change_number(till)
             return segment_list
         except Exception as exc:
             raise ValueError("Error reading feature flags from json.") from exc
 
-    def _read_splits_from_json_file(self, filename):
+    def _read_feature_flags_from_json_file(self, filename):
         """
         Parse a feature flags file and return a populated storage.
 
         :param filename: Path of the file containing feature flags
         :type filename: str.
 
         :return: Tuple: sanitized feature flag structure dict and till
         :rtype: Tuple(Dict, int)
         """
         try:
             with open(filename, 'r') as flo:
                 parsed = json.load(flo)
-            santitized = self._sanitize_split(parsed)
+            santitized = self._sanitize_feature_flag(parsed)
             return santitized['splits'], santitized['till']
         except Exception as exc:
             _LOGGER.error(str(exc))
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
-    def _sanitize_split(self, parsed):
+    def _sanitize_feature_flag(self, parsed):
         """
         implement Sanitization if neded.
 
         :param parsed: feature flags, till and since elements dict
         :type parsed: Dict
 
         :return: sanitized structure dict
         :rtype: Dict
         """
         parsed = self._sanitize_json_elements(parsed)
-        parsed['splits'] = self._sanitize_split_elements(parsed['splits'])
+        parsed['splits'] = self._sanitize_feature_flag_elements(parsed['splits'])
 
         return parsed
 
     def _sanitize_json_elements(self, parsed):
         """
         Sanitize all json elements.
 
@@ -429,69 +434,69 @@
         if 'till' not in parsed or parsed['till'] is None or parsed['till'] < -1:
             parsed['till'] = -1
         if 'since' not in parsed or parsed['since'] is None or parsed['since'] < -1 or parsed['since'] > parsed['till']:
             parsed['since'] = parsed['till']
 
         return parsed
 
-    def _sanitize_split_elements(self, parsed_splits):
+    def _sanitize_feature_flag_elements(self, parsed_feature_flags):
         """
         Sanitize all feature flags elements.
 
-        :param parsed_splits: feature flags array
-        :type parsed_splits: [Dict]
+        :param parsed_feature_flags: feature flags array
+        :type parsed_feature_flags: [Dict]
 
         :return: sanitized structure dict
         :rtype: [Dict]
         """
-        sanitized_splits = []
-        for split in parsed_splits:
-            if 'name' not in split or split['name'].strip() == '':
+        sanitized_feature_flags = []
+        for feature_flag in parsed_feature_flags:
+            if 'name' not in feature_flag or feature_flag['name'].strip() == '':
                 _LOGGER.warning("A feature flag in json file does not have (Name) or property is empty, skipping.")
                 continue
             for element in [('trafficTypeName', 'user', None, None, None, None),
                             ('trafficAllocation', 100, 0, 100,  None, None),
                             ('trafficAllocationSeed', int(get_current_epoch_time_ms() / 1000), None, None, None, [0]),
                             ('seed', int(get_current_epoch_time_ms() / 1000), None, None, None, [0]),
                             ('status', splits.Status.ACTIVE.value, None, None, [e.value for e in splits.Status], None),
                             ('killed', False, None, None, None, None),
                             ('defaultTreatment', 'control', None, None, None, ['', ' ']),
                             ('changeNumber', 0, 0, None, None, None),
                             ('algo', 2, 2, 2, None, None)]:
-                split = util._sanitize_object_element(split, 'split', element[0], element[1], lower_value=element[2], upper_value=element[3], in_list=element[4], not_in_list=element[5])
-            split = self._sanitize_condition(split)
-            sanitized_splits.append(split)
-        return sanitized_splits
+                feature_flag = util._sanitize_object_element(feature_flag, 'split', element[0], element[1], lower_value=element[2], upper_value=element[3], in_list=element[4], not_in_list=element[5])
+            feature_flag = self._sanitize_condition(feature_flag)
+            sanitized_feature_flags.append(feature_flag)
+        return sanitized_feature_flags
 
-    def _sanitize_condition(self, split):
+    def _sanitize_condition(self, feature_flag):
         """
         Sanitize feature flag and ensure a condition type ROLLOUT and matcher exist with ALL_KEYS elements.
 
-        :param split: feature flag dict object
-        :type split: Dict
+        :param feature_flag: feature flag dict object
+        :type feature_flag: Dict
 
         :return: sanitized feature flag
         :rtype: Dict
         """
         found_all_keys_matcher = False
-        split['conditions'] = split.get('conditions', [])
-        if len(split['conditions']) > 0:
-            last_condition = split['conditions'][-1]
+        feature_flag['conditions'] = feature_flag.get('conditions', [])
+        if len(feature_flag['conditions']) > 0:
+            last_condition = feature_flag['conditions'][-1]
             if 'conditionType' in last_condition:
                 if last_condition['conditionType'] == 'ROLLOUT':
                     if 'matcherGroup' in last_condition:
                         if 'matchers' in last_condition['matcherGroup']:
                             for matcher in last_condition['matcherGroup']['matchers']:
                                 if matcher['matcherType'] == 'ALL_KEYS':
                                     found_all_keys_matcher = True
                                     break
 
         if not found_all_keys_matcher:
-            _LOGGER.debug("Missing default rule condition for feature flag: %s, adding default rule with 100%% off treatment", split['name'])
-            split['conditions'].append(
+            _LOGGER.debug("Missing default rule condition for feature flag: %s, adding default rule with 100%% off treatment", feature_flag['name'])
+            feature_flag['conditions'].append(
             {
                 "conditionType": "ROLLOUT",
                 "matcherGroup": {
                 "combiner": "AND",
                 "matchers": [{
                     "keySelector": { "trafficType": "user", "attribute": None },
                     "matcherType": "ALL_KEYS",
@@ -508,8 +513,8 @@
                 "partitions": [
                     { "treatment": "on", "size": 0 },
                     { "treatment": "off", "size": 100 }
                 ],
             "label": "default rule"
         })
 
-        return split
+        return feature_flag
```

### Comparing `splitio_client-9.4.2/splitio/sync/synchronizer.py` & `splitio_client-9.5.0/splitio/sync/synchronizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 
 _LOGGER = logging.getLogger(__name__)
 _SYNC_ALL_NO_RETRIES = -1
 
 class SplitSynchronizers(object):
     """SplitSynchronizers."""
 
-    def __init__(self, split_sync, segment_sync, impressions_sync, events_sync,  # pylint:disable=too-many-arguments
+    def __init__(self, feature_flag_sync, segment_sync, impressions_sync, events_sync,  # pylint:disable=too-many-arguments
                  impressions_count_sync, telemetry_sync=None, unique_keys_sync = None, clear_filter_sync = None):
         """
         Class constructor.
 
-        :param split_sync: sync for splits
-        :type split_sync: splitio.sync.split.SplitSynchronizer
+        :param feature_flag_sync: sync for feature_flags
+        :type feature_flag_sync: splitio.sync.split.SplitSynchronizer
         :param segment_sync: sync for segments
         :type segment_sync: splitio.sync.segment.SegmentSynchronizer
         :param impressions_sync: sync for impressions
         :type impressions_sync: splitio.sync.impression.ImpressionSynchronizer
         :param events_sync: sync for events
         :type events_sync: splitio.sync.event.EventSynchronizer
         :param impressions_count_sync: sync for impression_counts
         :type impressions_count_sync: splitio.sync.impression.ImpressionsCountSynchronizer
         """
-        self._split_sync = split_sync
+        self._feature_flag_sync = feature_flag_sync
         self._segment_sync = segment_sync
         self._impressions_sync = impressions_sync
         self._events_sync = events_sync
         self._impressions_count_sync = impressions_count_sync
         self._unique_keys_sync = unique_keys_sync
         self._clear_filter_sync = clear_filter_sync
         self._telemetry_sync = telemetry_sync
 
     @property
     def split_sync(self):
         """Return split synchonizer."""
-        return self._split_sync
+        return self._feature_flag_sync
 
     @property
     def segment_sync(self):
         """Return segment synchonizer."""
         return self._segment_sync
 
     @property
@@ -79,43 +79,43 @@
     def telemetry_sync(self):
         """Return clear filter synchonizer."""
         return self._telemetry_sync
 
 class SplitTasks(object):
     """SplitTasks."""
 
-    def __init__(self, split_task, segment_task, impressions_task, events_task,  # pylint:disable=too-many-arguments
+    def __init__(self, feature_flag_task, segment_task, impressions_task, events_task,  # pylint:disable=too-many-arguments
                  impressions_count_task, telemetry_task=None, unique_keys_task = None, clear_filter_task = None):
         """
         Class constructor.
 
-        :param split_task: sync for splits
-        :type split_task: splitio.tasks.split_sync.SplitSynchronizationTask
+        :param feature_flag_task: sync for feature flags
+        :type feature_flag_task: splitio.tasks.split_sync.SplitSynchronizationTask
         :param segment_task: sync for segments
         :type segment_task: splitio.tasks.segment_sync.SegmentSynchronizationTask
         :param impressions_task: sync for impressions
         :type impressions_task: splitio.tasks.impressions_sync.ImpressionsSyncTask
         :param events_task: sync for events
         :type events_task: splitio.tasks.events_sync.EventsSyncTask
         :param impressions_count_task: sync for impression_counts
         :type impressions_count_task: splitio.tasks.impressions_sync.ImpressionsCountSyncTask
         """
-        self._split_task = split_task
+        self._feature_flag_task = feature_flag_task
         self._segment_task = segment_task
         self._impressions_task = impressions_task
         self._events_task = events_task
         self._impressions_count_task = impressions_count_task
         self._unique_keys_task = unique_keys_task
         self._clear_filter_task = clear_filter_task
         self._telemetry_task = telemetry_task
 
     @property
     def split_task(self):
-        """Return split sync task."""
-        return self._split_task
+        """Return feature flag sync task."""
+        return self._feature_flag_task
 
     @property
     def segment_task(self):
         """Return segment sync task."""
         return self._segment_task
 
     @property
@@ -162,53 +162,53 @@
         :type till: int
         """
         pass
 
     @abc.abstractmethod
     def synchronize_splits(self, till):
         """
-        Synchronize all splits.
+        Synchronize all feature flags.
 
         :param till: to fetch
         :type till: int
         """
         pass
 
     @abc.abstractmethod
     def sync_all(self):
-        """Synchronize all split data."""
+        """Synchronize all feature flag data."""
         pass
 
     @abc.abstractmethod
     def start_periodic_fetching(self):
-        """Start fetchers for splits and segments."""
+        """Start fetchers for feature flags and segments."""
         pass
 
     @abc.abstractmethod
     def stop_periodic_fetching(self):
-        """Stop fetchers for splits and segments."""
+        """Stop fetchers for feature flags and segments."""
         pass
 
     @abc.abstractmethod
     def start_periodic_data_recording(self):
         """Start recorders."""
         pass
 
     @abc.abstractmethod
     def stop_periodic_data_recording(self, blocking):
         """Stop recorders."""
         pass
 
     @abc.abstractmethod
-    def kill_split(self, split_name, default_treatment, change_number):
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
         """
-        Kill a split locally.
+        Kill a feature flag locally.
 
-        :param split_name: name of the split to perform kill
-        :type split_name: str
+        :param feature_flag_name: name of the feature flag to perform kill
+        :type feature_flag_name: str
         :param default_treatment: name of the default treatment to return
         :type default_treatment: str
         :param change_number: change_number
         :type change_number: int
         """
         pass
 
@@ -226,15 +226,15 @@
 class Synchronizer(BaseSynchronizer):
     """Synchronizer."""
 
     def __init__(self, split_synchronizers, split_tasks):
         """
         Class constructor.
 
-        :param split_synchronizers: syncs for performing synchronization of segments and splits
+        :param split_synchronizers: syncs for performing synchronization of segments and feature flags
         :type split_synchronizers: splitio.sync.synchronizer.SplitSynchronizers
         :param split_tasks: tasks for starting/stopping tasks
         :type split_tasks: splitio.sync.synchronizer.SplitTasks
         """
         self._backoff = Backoff(
                                 _ON_DEMAND_FETCH_BACKOFF_BASE,
                                 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT)
@@ -248,14 +248,22 @@
         if self._split_tasks.impressions_count_task:
             self._periodic_data_recording_tasks.append(self._split_tasks.impressions_count_task)
         if self._split_tasks.unique_keys_task:
             self._periodic_data_recording_tasks.append(self._split_tasks.unique_keys_task)
         if self._split_tasks.clear_filter_task:
             self._periodic_data_recording_tasks.append(self._split_tasks.clear_filter_task)
 
+    @property
+    def split_sync(self):
+        return self._split_synchronizers.split_sync
+
+    @property
+    def segment_storage(self):
+        return self._split_synchronizers.segment_sync._segment_storage
+
     def _synchronize_segments(self):
         _LOGGER.debug('Starting segments synchronization')
         return self._split_synchronizers.segment_sync.synchronize_segments()
 
     def synchronize_segment(self, segment_name, till):
         """
         Synchronize particular segment.
@@ -269,23 +277,23 @@
         success = self._split_synchronizers.segment_sync.synchronize_segment(segment_name, till)
         if not success:
             _LOGGER.error('Failed to sync some segments.')
         return success
 
     def synchronize_splits(self, till, sync_segments=True):
         """
-        Synchronize all splits.
+        Synchronize all feature flags.
 
         :param till: to fetch
         :type till: int
 
         :returns: whether the synchronization was successful or not.
         :rtype: bool
         """
-        _LOGGER.debug('Starting splits synchronization')
+        _LOGGER.debug('Starting feature flags synchronization')
         try:
             new_segments = []
             for segment in self._split_synchronizers.split_sync.synchronize_splits(till):
                     if not self._split_synchronizers.segment_sync.segment_exist_in_storage(segment):
                         new_segments.append(segment)
             if sync_segments and len(new_segments) != 0:
                 _LOGGER.debug('Synching Segments: %s', ','.join(new_segments))
@@ -293,32 +301,32 @@
                 if not success:
                     _LOGGER.error('Failed to schedule sync one or all segment(s) below.')
                     _LOGGER.error(','.join(new_segments))
                 else:
                     _LOGGER.debug('Segment sync scheduled.')
             return True
         except APIException:
-            _LOGGER.error('Failed syncing splits')
+            _LOGGER.error('Failed syncing feature flags')
             _LOGGER.debug('Error: ', exc_info=True)
             return False
 
     def sync_all(self, max_retry_attempts=_SYNC_ALL_NO_RETRIES):
         """
-        Synchronize all splits.
+        Synchronize all feature flags.
 
         :param max_retry_attempts: apply max attempts if it set to absilute integer.
         :type max_retry_attempts: int
         """
         retry_attempts = 0
         while True:
             try:
                 if not self.synchronize_splits(None, False):
                     raise Exception("split sync failed")
 
-                # Only retrying splits, since segments may trigger too many calls.
+                # Only retrying feature flags, since segments may trigger too many calls.
 
                 if not self._synchronize_segments():
                     _LOGGER.warning('Segments failed to synchronize.')
 
                 # All is good
                 return
             except Exception as exc:  # pylint:disable=broad-except
@@ -327,15 +335,15 @@
                 if max_retry_attempts != _SYNC_ALL_NO_RETRIES:
                     retry_attempts += 1
                     if retry_attempts > max_retry_attempts:
                         break
                 how_long = self._backoff.get()
                 time.sleep(how_long)
 
-        _LOGGER.error("Could not correctly synchronize splits and segments after %d attempts.", retry_attempts)
+        _LOGGER.error("Could not correctly synchronize feature flags and segments after %d attempts.", retry_attempts)
 
     def _retry_block(self, max_retry_attempts, retry_attempts):
         return retry_attempts
 
     def shutdown(self, blocking):
         """
         Stop tasks.
@@ -345,21 +353,21 @@
         """
         _LOGGER.debug('Shutting down tasks.')
         self._split_synchronizers.segment_sync.shutdown()
         self.stop_periodic_fetching()
         self.stop_periodic_data_recording(blocking)
 
     def start_periodic_fetching(self):
-        """Start fetchers for splits and segments."""
+        """Start fetchers for feature flags and segments."""
         _LOGGER.debug('Starting periodic data fetching')
         self._split_tasks.split_task.start()
         self._split_tasks.segment_task.start()
 
     def stop_periodic_fetching(self):
-        """Stop fetchers for splits and segments."""
+        """Stop fetchers for feature flags and segments."""
         _LOGGER.debug('Stopping periodic fetching')
         self._split_tasks.split_task.stop()
         self._split_tasks.segment_task.stop()
 
     def start_periodic_data_recording(self):
         """Start recorders."""
         _LOGGER.debug('Starting periodic data recording')
@@ -386,36 +394,36 @@
             self._split_tasks.telemetry_task.stop(telemetry_event)
             if telemetry_event.wait():
                 _LOGGER.debug('all tasks finished successfully.')
         else:
             for task in self._periodic_data_recording_tasks:
                 task.stop()
 
-    def kill_split(self, split_name, default_treatment, change_number):
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
         """
-        Kill a split locally.
+        Kill a feature flag locally.
 
-        :param split_name: name of the split to perform kill
-        :type split_name: str
+        :param feature_flag_name: name of the feature flag to perform kill
+        :type feature_flag_name: str
         :param default_treatment: name of the default treatment to return
         :type default_treatment: str
         :param change_number: change_number
         :type change_number: int
         """
-        self._split_synchronizers.split_sync.kill_split(split_name, default_treatment,
+        self._split_synchronizers.split_sync.kill_split(feature_flag_name, default_treatment,
                                                         change_number)
 
 class RedisSynchronizer(BaseSynchronizer):
     """Redis Synchronizer."""
 
     def __init__(self, split_synchronizers, split_tasks):
         """
         Class constructor.
 
-        :param split_synchronizers: syncs for performing synchronization of segments and splits
+        :param split_synchronizers: syncs for performing synchronization of segments and feature flags
         :type split_synchronizers: splitio.sync.synchronizer.SplitSynchronizers
         :param split_tasks: tasks for starting/stopping tasks
         :type split_tasks: splitio.sync.synchronizer.SplitTasks
         """
         self._split_synchronizers = split_synchronizers
         self._tasks = []
         if split_tasks.impressions_count_task is not None:
@@ -464,56 +472,56 @@
                 events.append(stop_event)
             if all(event.wait() for event in events):
                 _LOGGER.debug('all tasks finished successfully.')
         else:
             for task in self._tasks:
                 task.stop()
 
-    def kill_split(self, split_name, default_treatment, change_number):
-        """Kill a split locally."""
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
+        """Kill a feature flag locally."""
         raise NotImplementedError()
 
     def synchronize_splits(self, till):
-        """Synchronize all splits."""
+        """Synchronize all feature flags."""
         raise NotImplementedError()
 
     def synchronize_segment(self, segment_name, till):
         """Synchronize particular segment."""
         raise NotImplementedError()
 
     def start_periodic_fetching(self):
-        """Start fetchers for splits and segments."""
+        """Start fetchers for feature flags and segments."""
         raise NotImplementedError()
 
     def stop_periodic_fetching(self):
-        """Stop fetchers for splits and segments."""
+        """Stop fetchers for feature flags and segments."""
         raise NotImplementedError()
 
 class LocalhostSynchronizer(BaseSynchronizer):
     """LocalhostSynchronizer."""
 
     def __init__(self, split_synchronizers, split_tasks, localhost_mode):
         """
         Class constructor.
 
-        :param split_synchronizers: syncs for performing synchronization of segments and splits
+        :param split_synchronizers: syncs for performing synchronization of segments and feature flags
         :type split_synchronizers: splitio.sync.synchronizer.SplitSynchronizers
         :param split_tasks: tasks for starting/stopping tasks
         :type split_tasks: splitio.sync.synchronizer.SplitTasks
         """
         self._split_synchronizers = split_synchronizers
         self._split_tasks = split_tasks
         self._localhost_mode = localhost_mode
         self._backoff = Backoff(
                                 _ON_DEMAND_FETCH_BACKOFF_BASE,
                                 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT)
 
     def sync_all(self, till=None):
         """
-        Synchronize all splits.
+        Synchronize all feature flags.
         """
         # TODO: to be removed when legacy and yaml use BUR
         if self._localhost_mode != LocalhostMode.JSON:
             return self.synchronize_splits()
 
         self._backoff.reset()
         remaining_attempts = _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES
@@ -525,35 +533,35 @@
                 _LOGGER.error('Failed syncing all')
                 _LOGGER.error(str(exc))
 
             how_long = self._backoff.get()
             time.sleep(how_long)
 
     def start_periodic_fetching(self):
-        """Start fetchers for splits and segments."""
+        """Start fetchers for feature flags and segments."""
         if self._split_tasks.split_task is not None:
             _LOGGER.debug('Starting periodic data fetching')
             self._split_tasks.split_task.start()
         if self._split_tasks.segment_task is not None:
             self._split_tasks.segment_task.start()
 
     def stop_periodic_fetching(self):
-        """Stop fetchers for splits and segments."""
+        """Stop fetchers for feature flags and segments."""
         if self._split_tasks.split_task is not None:
             _LOGGER.debug('Stopping periodic fetching')
             self._split_tasks.split_task.stop()
         if self._split_tasks.segment_task is not None:
             self._split_tasks.segment_task.stop()
 
-    def kill_split(self, split_name, default_treatment, change_number):
-        """Kill a split locally."""
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
+        """Kill a feature flag locally."""
         raise NotImplementedError()
 
     def synchronize_splits(self):
-        """Synchronize all splits."""
+        """Synchronize all feature flags."""
         try:
             new_segments = []
             for segment in self._split_synchronizers.split_sync.synchronize_splits():
                     if not self._split_synchronizers.segment_sync.segment_exist_in_storage(segment):
                         new_segments.append(segment)
             if len(new_segments) > 0:
                 _LOGGER.debug('Synching Segments: %s', ','.join(new_segments))
@@ -562,16 +570,16 @@
                     _LOGGER.error('Failed to schedule sync one or all segment(s) below.')
                     _LOGGER.error(','.join(new_segments))
                 else:
                     _LOGGER.debug('Segment sync scheduled.')
             return True
 
         except APIException as exc:
-            _LOGGER.error('Failed syncing splits')
-            raise APIException('Failed to sync splits') from exc
+            _LOGGER.error('Failed syncing feature flags')
+            raise APIException('Failed to sync feature flags') from exc
 
     def synchronize_segment(self, segment_name, till):
         """Synchronize particular segment."""
         pass
 
     def start_periodic_data_recording(self):
         """Start recorders."""
@@ -603,47 +611,47 @@
         :param till: to fetch
         :type till: int
         """
         pass
 
     def synchronize_splits(self, till):
         """
-        Synchronize all splits.
+        Synchronize all feature flags.
 
         :param till: to fetch
         :type till: int
         """
         pass
 
     def sync_all(self):
-        """Synchronize all split data."""
+        """Synchronize all feature flag data."""
         pass
 
     def start_periodic_fetching(self):
-        """Start fetchers for splits and segments."""
+        """Start fetchers for feature flags and segments."""
         pass
 
     def stop_periodic_fetching(self):
-        """Stop fetchers for splits and segments."""
+        """Stop fetchers for feature flags and segments."""
         pass
 
     def start_periodic_data_recording(self):
         """Start recorders."""
         pass
 
     def stop_periodic_data_recording(self, blocking):
         """Stop recorders."""
         pass
 
-    def kill_split(self, split_name, default_treatment, change_number):
+    def kill_split(self, feature_flag_name, default_treatment, change_number):
         """
-        Kill a split locally.
+        Kill a feature_flag locally.
 
-        :param split_name: name of the split to perform kill
-        :type split_name: str
+        :param feature_flag_name: name of the feature flag to perform kill
+        :type feature_flag_name: str
         :param default_treatment: name of the default treatment to return
         :type default_treatment: str
         :param change_number: change_number
         :type change_number: int
         """
         pass
```

### Comparing `splitio_client-9.4.2/splitio/sync/segment.py` & `splitio_client-9.5.0/splitio/sync/segment.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/manager.py` & `splitio_client-9.5.0/splitio/sync/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/sync/unique_keys.py` & `splitio_client-9.5.0/splitio/sync/unique_keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/cache/lru.py` & `splitio_client-9.5.0/splitio/engine/cache/lru.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/telemetry.py` & `splitio_client-9.5.0/splitio/engine/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 
 import logging
 _LOGGER = logging.getLogger(__name__)
 
 from  splitio.storage.inmemmory import InMemoryTelemetryStorage
-from splitio.models.telemetry import CounterConstants
+from splitio.models.telemetry import CounterConstants, UpdateFromSSE
 
 class TelemetryStorageProducer(object):
     """Telemetry storage producer class."""
 
     def __init__(self, telemetry_storage):
         """Initialize all producer classes."""
         self._telemetry_init_producer = TelemetryInitProducer(telemetry_storage)
@@ -135,14 +135,18 @@
         """Record incoming streaming event."""
         self._telemetry_storage.record_streaming_event(streaming_event)
 
     def record_session_length(self, session):
         """Record session length."""
         self._telemetry_storage.record_session_length(session)
 
+    def record_update_from_sse(self, event):
+        """Record update from sse."""
+        self._telemetry_storage.record_update_from_sse(event)
+
 class TelemetryStorageConsumer(object):
     """Telemetry storage consumer class."""
 
     def __init__(self, telemetry_storage):
         """Initialize all consumer classes."""
         self._telemetry_init_consumer = TelemetryInitConsumer(telemetry_storage)
         self._telemetry_evaluation_consumer = TelemetryEvaluationConsumer(telemetry_storage)
@@ -267,14 +271,18 @@
         """Get and reset token refreshes."""
         return self._telemetry_storage.pop_token_refreshes()
 
     def pop_streaming_events(self):
         """Get and reset streaming events."""
         return self._telemetry_storage.pop_streaming_events()
 
+    def pop_update_from_sse(self, event):
+        """Get and reset update from sse."""
+        return self._telemetry_storage.pop_update_from_sse(event)
+
     def get_session_length(self):
         """Get session length"""
         return self._telemetry_storage.get_session_length()
 
     def pop_formatted_stats(self):
         """
         Get formatted and reset stats.
@@ -288,14 +296,15 @@
 
         return {
             'iQ': self.get_impressions_stats(CounterConstants.IMPRESSIONS_QUEUED),
             'iDe': self.get_impressions_stats(CounterConstants.IMPRESSIONS_DEDUPED),
             'iDr': self.get_impressions_stats(CounterConstants.IMPRESSIONS_DROPPED),
             'eQ': self.get_events_stats(CounterConstants.EVENTS_QUEUED),
             'eD': self.get_events_stats(CounterConstants.EVENTS_DROPPED),
+            'ufs': {event.value: self.pop_update_from_sse(event) for event in UpdateFromSSE},
             'lS': {'sp': last_synchronization['split'],
                       'se': last_synchronization['segment'],
                       'im': last_synchronization['impression'],
                       'ic': last_synchronization['impressionCount'],
                       'ev': last_synchronization['event'],
                       'te': last_synchronization['telemetry'],
                       'to': last_synchronization['token']
```

### Comparing `splitio_client-9.4.2/splitio/engine/splitters.py` & `splitio_client-9.5.0/splitio/engine/splitters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/hashfns/legacy.py` & `splitio_client-9.5.0/splitio/engine/hashfns/legacy.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/hashfns/__init__.py` & `splitio_client-9.5.0/splitio/engine/hashfns/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/hashfns/murmur3py.py` & `splitio_client-9.5.0/splitio/engine/hashfns/murmur3py.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/strategies.py` & `splitio_client-9.5.0/splitio/engine/impressions/strategies.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/__init__.py` & `splitio_client-9.5.0/splitio/engine/impressions/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/impressions.py` & `splitio_client-9.5.0/splitio/engine/impressions/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/unique_keys_tracker.py` & `splitio_client-9.5.0/splitio/engine/impressions/unique_keys_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/manager.py` & `splitio_client-9.5.0/splitio/engine/impressions/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/impressions/adapters.py` & `splitio_client-9.5.0/splitio/engine/impressions/adapters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/evaluator.py` & `splitio_client-9.5.0/splitio/engine/evaluator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/engine/filters.py` & `splitio_client-9.5.0/splitio/engine/filters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/config.py` & `splitio_client-9.5.0/splitio/client/config.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/util.py` & `splitio_client-9.5.0/splitio/client/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/key.py` & `splitio_client-9.5.0/splitio/client/key.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/client.py` & `splitio_client-9.5.0/splitio/client/client.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/factory.py` & `splitio_client-9.5.0/splitio/client/factory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/localhost.py` & `splitio_client-9.5.0/splitio/client/localhost.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/input_validator.py` & `splitio_client-9.5.0/splitio/client/input_validator.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/manager.py` & `splitio_client-9.5.0/splitio/client/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.2/splitio/client/listener.py` & `splitio_client-9.5.0/splitio/client/listener.py`

 * *Files identical despite different names*

