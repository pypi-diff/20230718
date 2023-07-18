# Comparing `tmp/azure-monitor-opentelemetry-exporter-1.0.0b8.zip` & `tmp/azure-monitor-opentelemetry-exporter-1.0.0b9.zip`

## zipinfo {}

```diff
@@ -1,152 +1,154 @@
-Zip file size: 166032 bytes, number of entries: 150
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/
--rw-rw-r--  2.0 unx       67 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/setup.cfg
--rw-rw-r--  2.0 unx     3363 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/setup.py
--rw-rw-r--  2.0 unx    26085 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/PKG-INFO
--rw-rw-r--  2.0 unx     6454 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/CHANGELOG.md
--rw-rw-r--  2.0 unx    25249 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/README.md
--rw-rw-r--  2.0 unx     1073 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/LICENSE
--rw-rw-r--  2.0 unx      256 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/collector/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/
--rw-rw-r--  2.0 unx     2561 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_chat.py
--rw-rw-r--  2.0 unx     1775 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_storage_blob.py
--rw-rw-r--  2.0 unx     2235 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_cosmos.py
--rw-rw-r--  2.0 unx     1427 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_psycopg2.py
--rw-rw-r--  2.0 unx     1388 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_flask.py
--rw-rw-r--  2.0 unx     1903 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_grid.py
--rw-rw-r--  2.0 unx     2078 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_send.py
--rw-rw-r--  2.0 unx     1955 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_app_config.py
--rw-rw-r--  2.0 unx     2453 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_blob_checkpoint.py
--rw-rw-r--  2.0 unx     2051 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_secret.py
--rw-rw-r--  2.0 unx     1980 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_form_recognizer.py
--rw-rw-r--  2.0 unx    18269 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/README.md
--rw-rw-r--  2.0 unx     1358 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_requests.py
--rw-rw-r--  2.0 unx     2243 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_text_analytics.py
--rw-rw-r--  2.0 unx     1113 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_span_event.py
--rw-rw-r--  2.0 unx     1301 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_jaeger.py
--rw-rw-r--  2.0 unx     2195 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_keys.py
--rw-rw-r--  2.0 unx     1896 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_hub.py
--rw-rw-r--  2.0 unx     2272 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_receive.py
--rw-rw-r--  2.0 unx      919 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_trace.py
--rw-rw-r--  2.0 unx     1923 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_phone.py
--rw-rw-r--  2.0 unx     1882 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_sms.py
--rw-rw-r--  2.0 unx     2174 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_cert.py
--rw-rw-r--  2.0 unx     1312 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/collector/sample_collector.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/
--rw-rw-r--  2.0 unx      917 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/manage.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/migrations/
--rw-rw-r--  2.0 unx      865 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/views.py
--rw-rw-r--  2.0 unx       93 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/__init__.py
--rw-rw-r--  2.0 unx      240 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/apps.py
--rw-rw-r--  2.0 unx      204 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/urls.py
--rw-rw-r--  2.0 unx      154 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/tests.py
--rw-rw-r--  2.0 unx      157 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/admin.py
--rw-rw-r--  2.0 unx      151 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/models.py
--rw-rw-r--  2.0 unx       93 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/migrations/__init__.py
--rw-rw-r--  2.0 unx       93 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/__init__.py
--rw-rw-r--  2.0 unx      820 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/urls.py
--rw-rw-r--  2.0 unx     3367 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/settings.py
--rw-rw-r--  2.0 unx      518 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/asgi.py
--rw-rw-r--  2.0 unx      483 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/wsgi.py
--rw-rw-r--  2.0 unx     1253 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_exception.py
--rw-rw-r--  2.0 unx     1063 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_log.py
--rw-rw-r--  2.0 unx     1571 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/README.md
--rw-rw-r--  2.0 unx      976 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_properties.py
--rw-rw-r--  2.0 unx     1227 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_correlate.py
--rw-rw-r--  2.0 unx      909 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/README.md
--rw-rw-r--  2.0 unx     1401 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_views.py
--rw-rw-r--  2.0 unx     1495 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_attributes.py
--rw-rw-r--  2.0 unx     2065 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_instruments.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/
--rw-rw-r--  2.0 unx       65 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/
--rw-rw-r--  2.0 unx       80 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/
--rw-rw-r--  2.0 unx      347 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_version.py
--rw-rw-r--  2.0 unx     4835 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_utils.py
--rw-rw-r--  2.0 unx     2355 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_constants.py
--rw-rw-r--  2.0 unx     4394 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_connection_string_parser.py
--rw-rw-r--  2.0 unx      917 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/__init__.py
--rw-rw-r--  2.0 unx     7342 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_storage.py
--rw-rw-r--  2.0 unx        1 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/
--rw-rw-r--  2.0 unx      777 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_vendor.py
--rw-rw-r--  2.0 unx     3436 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py
--rw-rw-r--  2.0 unx      785 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/__init__.py
--rw-rw-r--  2.0 unx     1529 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_patch.py
--rw-rw-r--  2.0 unx     2566 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_configuration.py
--rw-rw-r--  2.0 unx    54541 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models.py
--rw-rw-r--  2.0 unx    58422 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py
--rw-rw-r--  2.0 unx     2825 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py
--rw-rw-r--  2.0 unx     2428 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py
--rw-rw-r--  2.0 unx      604 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx     5121 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/
--rw-rw-r--  2.0 unx     3288 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py
--rw-rw-r--  2.0 unx      785 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     1529 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     2400 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      604 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     4235 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/__init__.py
--rw-rw-r--  2.0 unx    16730 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/_base.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/__init__.py
--rw-rw-r--  2.0 unx     6351 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/__init__.py
--rw-rw-r--  2.0 unx     6177 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/__init__.py
--rw-rw-r--  2.0 unx     3238 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py
--rw-rw-r--  2.0 unx    26243 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/__init__.py
--rw-rw-r--  2.0 unx     1245 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_state.py
--rw-rw-r--  2.0 unx     4181 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py
--rw-rw-r--  2.0 unx    15675 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py
--rw-rw-r--  2.0 unx     1092 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/
--rw-rw-r--  2.0 unx     2015 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_utils.py
--rw-rw-r--  2.0 unx     6663 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_storage.py
--rw-rw-r--  2.0 unx    27232 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_base_exporter.py
--rw-rw-r--  2.0 unx     1439 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/conftest.py
--rw-rw-r--  2.0 unx     8601 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_connection_string_parser.py
--rw-rw-r--  2.0 unx     1917 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/trace_exporter.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx       94 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/__init__.py
--rw-rw-r--  2.0 unx    11490 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/test_logs.py
--rw-rw-r--  2.0 unx    11925 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/test_metrics.py
--rw-rw-r--  2.0 unx       94 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/__init__.py
--rw-rw-r--  2.0 unx       94 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/__init__.py
--rw-rw-r--  2.0 unx    47178 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/test_trace.py
--rw-rw-r--  2.0 unx    31786 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_statsbeat.py
--rw-rw-r--  2.0 unx       94 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/__init__.py
--rw-rw-r--  2.0 unx     7184 b- defN 22-Sep-26 23:37 azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_exporter.py
--rw-rw-r--  2.0 unx      402 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/entry_points.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    26085 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx     5242 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx      123 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 22-Sep-26 23:39 azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/top_level.txt
-150 files, 580134 bytes uncompressed, 128880 bytes compressed:  77.8%
+Zip file size: 170792 bytes, number of entries: 152
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/
+-rw-rw-r--  2.0 unx      256 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/MANIFEST.in
+-rw-rw-r--  2.0 unx     7444 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/CHANGELOG.md
+-rw-rw-r--  2.0 unx    29625 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/PKG-INFO
+-rw-rw-r--  2.0 unx     3622 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/setup.py
+-rw-rw-r--  2.0 unx       67 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/setup.cfg
+-rw-rw-r--  2.0 unx    28738 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/README.md
+-rw-rw-r--  2.0 unx     1073 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/
+-rw-rw-r--  2.0 unx     8601 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_connection_string_parser.py
+-rw-rw-r--  2.0 unx     6663 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_storage.py
+-rw-rw-r--  2.0 unx    28816 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_base_exporter.py
+-rw-rw-r--  2.0 unx     2015 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_utils.py
+-rw-rw-r--  2.0 unx     1439 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/conftest.py
+-rw-rw-r--  2.0 unx       94 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/__init__.py
+-rw-rw-r--  2.0 unx    11925 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/test_metrics.py
+-rw-rw-r--  2.0 unx     1917 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/trace_exporter.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx    31786 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_statsbeat.py
+-rw-rw-r--  2.0 unx     7184 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_exporter.py
+-rw-rw-r--  2.0 unx       94 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/__init__.py
+-rw-rw-r--  2.0 unx    11490 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/test_logs.py
+-rw-rw-r--  2.0 unx       94 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/__init__.py
+-rw-rw-r--  2.0 unx     1550 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/test_sampling.py
+-rw-rw-r--  2.0 unx    48215 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/test_trace.py
+-rw-rw-r--  2.0 unx       94 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/
+-rw-rw-r--  2.0 unx     1503 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_attributes.py
+-rw-rw-r--  2.0 unx     2107 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_instruments.py
+-rw-rw-r--  2.0 unx     1409 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_views.py
+-rw-rw-r--  2.0 unx     1622 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/README.md
+-rw-rw-r--  2.0 unx     1253 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_exception.py
+-rw-rw-r--  2.0 unx     1227 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_correlate.py
+-rw-rw-r--  2.0 unx      976 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_properties.py
+-rw-rw-r--  2.0 unx     1063 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_log.py
+-rw-rw-r--  2.0 unx     1571 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/README.md
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/collector/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/
+-rw-rw-r--  2.0 unx     1388 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_flask.py
+-rw-rw-r--  2.0 unx     2174 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_cert.py
+-rw-rw-r--  2.0 unx     1903 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_grid.py
+-rw-rw-r--  2.0 unx     1372 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_sampling.py
+-rw-rw-r--  2.0 unx     2453 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_blob_checkpoint.py
+-rw-rw-r--  2.0 unx     2078 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_send.py
+-rw-rw-r--  2.0 unx      919 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_trace.py
+-rw-rw-r--  2.0 unx     1113 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_span_event.py
+-rw-rw-r--  2.0 unx     2235 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_cosmos.py
+-rw-rw-r--  2.0 unx     1882 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_sms.py
+-rw-rw-r--  2.0 unx     2272 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_receive.py
+-rw-rw-r--  2.0 unx     1955 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_app_config.py
+-rw-rw-r--  2.0 unx     1923 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_phone.py
+-rw-rw-r--  2.0 unx     1469 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_psycopg2.py
+-rw-rw-r--  2.0 unx     1358 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_requests.py
+-rw-rw-r--  2.0 unx     1896 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_hub.py
+-rw-rw-r--  2.0 unx     2561 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_chat.py
+-rw-rw-r--  2.0 unx     2195 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_keys.py
+-rw-rw-r--  2.0 unx    18391 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/README.md
+-rw-rw-r--  2.0 unx     2051 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_secret.py
+-rw-rw-r--  2.0 unx     1980 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_form_recognizer.py
+-rw-rw-r--  2.0 unx     1775 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_storage_blob.py
+-rw-rw-r--  2.0 unx     1301 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_jaeger.py
+-rw-rw-r--  2.0 unx     2243 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_text_analytics.py
+-rw-rw-r--  2.0 unx     1312 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/collector/sample_collector.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/
+-rw-rw-r--  2.0 unx      917 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/manage.py
+-rw-rw-r--  2.0 unx      518 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/asgi.py
+-rw-rw-r--  2.0 unx      483 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/wsgi.py
+-rw-rw-r--  2.0 unx      820 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/urls.py
+-rw-rw-r--  2.0 unx       93 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/__init__.py
+-rw-rw-r--  2.0 unx     3367 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/settings.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/migrations/
+-rw-rw-r--  2.0 unx      154 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/tests.py
+-rw-rw-r--  2.0 unx      157 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/admin.py
+-rw-rw-r--  2.0 unx      151 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/models.py
+-rw-rw-r--  2.0 unx      204 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/urls.py
+-rw-rw-r--  2.0 unx      240 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/apps.py
+-rw-rw-r--  2.0 unx      865 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/views.py
+-rw-rw-r--  2.0 unx       93 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/__init__.py
+-rw-rw-r--  2.0 unx       93 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/migrations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/
+-rw-rw-r--  2.0 unx       65 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/
+-rw-rw-r--  2.0 unx       80 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/
+-rw-rw-r--  2.0 unx     4835 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_utils.py
+-rw-rw-r--  2.0 unx     7340 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_storage.py
+-rw-rw-r--  2.0 unx      347 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_version.py
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/py.typed
+-rw-rw-r--  2.0 unx      917 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/__init__.py
+-rw-rw-r--  2.0 unx     2406 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_constants.py
+-rw-rw-r--  2.0 unx     4394 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_connection_string_parser.py
+-rw-rw-r--  2.0 unx     4181 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py
+-rw-rw-r--  2.0 unx     1245 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_state.py
+-rw-rw-r--  2.0 unx     1092 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py
+-rw-rw-r--  2.0 unx    15675 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/
+-rw-rw-r--  2.0 unx    17493 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/_base.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/__init__.py
+-rw-rw-r--  2.0 unx     6738 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/__init__.py
+-rw-rw-r--  2.0 unx     6351 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/__init__.py
+-rw-rw-r--  2.0 unx     3676 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py
+-rw-rw-r--  2.0 unx    26506 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
+-rw-rw-r--  2.0 unx        0 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/
+-rw-rw-r--  2.0 unx     3436 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py
+-rw-rw-r--  2.0 unx      777 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     1529 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_patch.py
+-rw-rw-r--  2.0 unx      785 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/__init__.py
+-rw-rw-r--  2.0 unx     2566 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      604 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx     5121 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/
+-rw-rw-r--  2.0 unx     3288 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py
+-rw-rw-r--  2.0 unx     1529 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      785 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     2400 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      604 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     4235 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py
+-rw-rw-r--  2.0 unx     2428 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py
+-rw-rw-r--  2.0 unx    54541 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models.py
+-rw-rw-r--  2.0 unx    58422 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx     2825 b- defN 22-Nov-08 23:46 azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx        6 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      123 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/requires.txt
+-rw-rw-r--  2.0 unx    29625 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     5305 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx      576 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/entry_points.txt
+-rw-rw-r--  2.0 unx        1 b- defN 22-Nov-08 23:47 azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/not-zip-safe
+152 files, 600741 bytes uncompressed, 133186 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -1,451 +1,457 @@
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/setup.cfg
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/MANIFEST.in
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/setup.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/CHANGELOG.md
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/PKG-INFO
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/CHANGELOG.md
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/setup.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/README.md
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/setup.cfg
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/LICENSE
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/README.md
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/MANIFEST.in
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/LICENSE
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/collector/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_chat.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_connection_string_parser.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_storage_blob.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_storage.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_cosmos.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_base_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_psycopg2.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_utils.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_flask.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/conftest.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_grid.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_send.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/test_metrics.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_app_config.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/trace_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_blob_checkpoint.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_secret.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_statsbeat.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_form_recognizer.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/README.md
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_requests.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/test_logs.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_text_analytics.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_span_event.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/test_sampling.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_jaeger.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/test_trace.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_keys.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_hub.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_receive.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_trace.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_phone.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_attributes.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_sms.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_instruments.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_cert.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_views.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/collector/sample_collector.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/README.md
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_exception.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_correlate.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_properties.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/manage.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_log.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/migrations/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/README.md
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/views.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/collector/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/apps.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_flask.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/urls.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_cert.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/tests.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_grid.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/admin.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_sampling.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/models.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_blob_checkpoint.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/migrations/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_send.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_trace.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/urls.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_span_event.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/settings.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_cosmos.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/asgi.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_sms.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/wsgi.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_receive.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_exception.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_app_config.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_log.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_phone.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/README.md
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_psycopg2.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_properties.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_requests.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_correlate.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_hub.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/README.md
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_chat.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_views.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_keys.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_attributes.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/README.md
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_instruments.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_secret.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_form_recognizer.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_storage_blob.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_jaeger.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_text_analytics.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/collector/sample_collector.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/manage.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_version.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/asgi.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_utils.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/wsgi.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_constants.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/urls.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_connection_string_parser.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/settings.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_storage.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/migrations/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/py.typed
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/tests.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/admin.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/models.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/urls.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_vendor.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/apps.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/views.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_patch.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/migrations/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_configuration.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_utils.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_storage.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_version.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/py.typed
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_constants.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_connection_string_parser.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_state.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/_base.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/_base.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_state.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_utils.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_storage.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_vendor.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_base_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_patch.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/conftest.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_connection_string_parser.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_configuration.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/trace_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/test_logs.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/test_metrics.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/test_trace.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_statsbeat.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/__init__.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_exporter.py
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/entry_points.txt
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/not-zip-safe
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/dependency_links.txt
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/requires.txt
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/requires.txt
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/top_level.txt
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/entry_points.txt
+Comment: 
+
+Filename: azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/not-zip-safe
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/setup.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         "Development Status :: 4 - Beta",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     zip_safe=False,
     packages=find_packages(exclude=[
         'tests',
         'samples',
         # Exclude packages that will be covered by PEP420 or nspkg
@@ -91,11 +92,14 @@
             "azure_monitor_opentelemetry_exporter = azure.monitor.opentelemetry.exporter:AzureMonitorTraceExporter"
         ],
         "opentelemetry_logs_exporter": [
             "azure_monitor_opentelemetry_exporter = azure.monitor.opentelemetry.exporter:AzureMonitorLogExporter"
         ],
         "opentelemetry_metrics_exporter": [
             "azure_monitor_opentelemetry_exporter = azure.monitor.opentelemetry.exporter:AzureMonitorMetricExporter"
+        ],
+        "opentelemetry_traces_sampler": [
+            "azure_monitor_opentelemetry_sampler = azure.monitor.opentelemetry.exporter.export.trace._sampling:azure_monitor_opentelemetry_sampler_factory"
         ]
     }
 )
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/PKG-INFO` & `azure-monitor-opentelemetry-exporter-1.0.0b9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry-exporter
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Microsoft Azure Monitor Opentelemetry Exporter Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Microsoft OpenTelemetry exporter for Azure Monitor
 
-[![Gitter chat](https://img.shields.io/gitter/room/Microsoft/azure-monitor-python)](https://gitter.im/Azure/azure-sdk-for-python)
-
 The exporter for Azure Monitor allows you to export data utilizing the OpenTelemetry SDK and send telemetry data to Azure Monitor for applications written in Python.
 
 [Source code](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter) | [Package (PyPi)][pypi] | [API reference documentation][api_docs] | [Product documentation][product_docs] | [Samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter/samples) | [Changelog](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/CHANGELOG.md)
 
 ## Getting started
 
 ### Install the package
@@ -39,15 +38,15 @@
 ### Prerequisites
 
 To use this package, you must have:
 
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Monitor - [How to use application insights][application_insights_namespace]
 * OpenTelemetry SDK - [OpenTelemetry SDK for Python][ot_sdk_python]
-* Python 3.6 or later - [Install Python][python]
+* Python 3.7 or later - [Install Python][python]
 
 ### Instantiate the client
 
 Interaction with Azure monitor exporter starts with an instance of the `AzureMonitorTraceExporter` class for distributed tracing, `AzureMonitorLogExporter` for logging and `AzureMonitorMetricExporter` for metrics. You will need a **connection_string** to instantiate the object.
 Please find the samples linked below for demonstration as to how to construct the exporter using a connection string.
 
 #### Logging (experimental)
@@ -146,30 +145,44 @@
 
 * [Sampling][sampler_ref]: Sampling is a mechanism to control the noise and overhead introduced by OpenTelemetry by reducing the number of samples of traces collected and sent to the backend.
 
 * ApplicationInsightsSampler: Application Insights specific sampler used for consistent sampling across Application Insights SDKs and OpenTelemetry-based SDKs sending data to Application Insights. This sampler MUST be used whenever `AzureMonitorTraceExporter` is used.
 
 For more information about these resources, see [What is Azure Monitor?][product_docs].
 
+## Configuration
+
+All configuration options can be passed through the constructors of exporters through `kwargs`. Below is a list of configurable options.
+
+`connection_string`: The connection string used for your Application Insights resource.
+`disable_offline_storage`: Boolean value to determine whether to disable storing failed telemetry records for retry. Defaults to `False`.
+`storage_directory`: Storage directory in which to store retry files. Defaults to `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
+
 ## Examples
 
 ### Logging (experimental)
 
 NOTE: The logging signal for the `AzureMonitorLogExporter` is currently in an EXPERIMENTAL state. Possible breaking changes may ensue in the future.
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a log record](#export-hello-world-log)
 * [Exporting correlated log record](#export-correlated-log)
 * [Exporting log record with custom properties](#export-custom-properties-log)
 * [Exporting an exceptions log record](#export-exceptions-log)
 
+Review the [OpenTelemetry Logging SDK][ot_logging_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Log
 
 ```Python
+"""
+An example to show an application using Opentelemetry logging sdk. Logging calls to the standard Python
+logging library are tracked and telemetry is exported to application insights with the AzureMonitorLogExporter.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -196,14 +209,17 @@
 
 logger.warning("Hello World!")
 ```
 
 #### Export Correlated Log
 
 ```Python
+"""
+An example showing how to include context correlation information in logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry import trace
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
@@ -237,14 +253,17 @@
     logger.warning("WARNING: Inside of span")
 logger.error("ERROR: After span")
 ```
 
 #### Export Custom Properties Log
 
 ```Python
+"""
+An example showing how to add custom properties to logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -272,16 +291,14 @@
 # Custom properties
 logger.debug("DEBUG: Debug with properties", extra={"debug": "true"})
 ```
 
 #### Export Exceptions Log
 
 ```Python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example showing how to export exception telemetry using the AzureMonitorLogExporter.
 """
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
@@ -325,19 +342,19 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Using different metric instruments](#metric-instrument-usage)
 * [Customizing outputted metrics with views](#metric-custom-views)
 * [Recording instruments with attributes](#metric-record-attributes)
 
+Review the [OpenTelemetry Metrics SDK][ot_metrics_sdk] to learn how to use OpenTelemetry components to collect metrics.
+
 #### Metric instrument usage
 
 ```python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example to show an application using all instruments in the OpenTelemetry SDK. Metrics created
 and recorded using the sdk are tracked and telemetry is exported to application insights with the
 AzureMonitorMetricsExporter.
 """
 import os
 from typing import Iterable
@@ -399,14 +416,19 @@
 gauge = meter.create_observable_gauge("gauge", [observable_gauge_func])
 
 ```
 
 #### Metric custom views
 
 ```python
+"""
+This example shows how to customize the metrics that are output by the SDK using Views. Metrics created
+and recorded using the sdk are tracked and telemetry is exported to application insights with the
+AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import Counter, MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.metrics.view import View
 
@@ -436,17 +458,24 @@
 
 meter = metrics.get_meter_provider().get_meter("view-name-change")
 my_counter = meter.create_counter("my.counter")
 my_counter.add(100)
 
 ```
 
+More examples with the metrics `Views` SDK can be found [here](https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views).
+
 #### Metric record attributes
 
 ```python
+"""
+An example to show an application using different attributes with instruments in the OpenTelemetry SDK.
+Metrics created and recorded using the sdk are tracked and telemetry is exported to application insights
+with the AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
@@ -491,17 +520,23 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a custom span](#export-hello-world-trace)
 * [Using an instrumentation to track a library](#instrumentation-with-requests-library)
 * [Enabling sampling to limit the amount of telemetry sent](#enabling-sampling)
 
+Review the [OpenTelemetry Tracing SDK][ot_tracing_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Trace
 
 ```Python
+"""
+An example to show an application using Opentelemetry tracing api and sdk. Custom dependencies are
+tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 
 trace.set_tracer_provider(TracerProvider())
@@ -517,19 +552,28 @@
     print("Hello, World!")
 ```
 
 #### Instrumentation with requests library
 
 OpenTelemetry also supports several instrumentations which allows to instrument with third party libraries.
 
+For a list of instrumentations available in OpenTelemetry, visit the contrib [documentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/).
+
 This example shows how to instrument with the [requests](https://pypi.org/project/requests/) library.
 
-* Install the requests integration package using pip install opentelemetry-instrumentation-requests.
+* Install the requests instrumentation package using pip install opentelemetry-instrumentation-requests.
 
 ```Python
+"""
+An example to show an application instrumented with the OpenTelemetry requests instrumentation.
+Calls made with the requests library will be automatically tracked and telemetry is exported to 
+application insights with the AzureMonitorTraceExporter.
+See more info on the requests instrumentation here:
+https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
+"""
 import os
 import requests
 from opentelemetry import trace
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
@@ -547,15 +591,22 @@
 
 # This request will be traced
 response = requests.get(url="https://azure.microsoft.com/")
 ```
 
 #### Enabling sampling
 
+You can enable sampling to limit the amount of telemetry records you receive. In order to enable correct sampling in Application Insights, use the `ApplicationInsightsSampler` as shown below.
+
 ```Python
+"""
+An example to show an application using the ApplicationInsightsSampler to enable sampling for your telemetry.
+Specify a sampling rate for the sampler to limit the amount of telemetry records you receive. Custom dependencies
+ are tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import (
     ApplicationInsightsSampler,
     AzureMonitorTraceExporter,
@@ -590,14 +641,18 @@
 
 ### Additional documentation
 
 For more extensive documentation on the Azure Monitor service, see the [Azure Monitor documentation][product_docs] on docs.microsoft.com.
 
 For detailed overview of OpenTelemetry, visit their [overview](https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md) page.
 
+For the official OpenTelemetry Python documentation and how to enable other telemetry scenarios, visit the official OpenTelemetry [website](https://opentelemetry.io/docs/instrumentation/python/).
+
+For more information on the Azure Monitor OpenTelemetry Distro, which is a bundle of useful, pre-assembled components (one of them being this current package) that enable telemetry scenarios with Azure Monitor, visit the [README](https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry-distro).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
@@ -605,44 +660,41 @@
 provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 <!-- LINKS -->
-[azure_cli]: https://docs.microsoft.com/cli/azure
 [api_docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-opentelemetry-exporter-azuremonitor/1.0.0b2/index.html
 [product_docs]: https://docs.microsoft.com/azure/azure-monitor/overview
-[azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
-[cloud_shell]: https://docs.microsoft.com/azure/cloud-shell/overview
-[cloud_shell_bash]: https://shell.azure.com/bash
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/project/azure-monitor-opentelemetry-exporter/
 [python]: https://www.python.org/downloads/
-[venv]: https://docs.python.org/3/library/venv.html
-[virtualenv]: https://virtualenv.pypa.io
 [ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
 [application_insights_namespace]: https://docs.microsoft.com/azure/azure-monitor/app/app-insights-overview#how-do-i-use-application-insights
 [opentelemetry_spec]: https://opentelemetry.io/
 [instrumentation_library]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md#instrumentation-libraries
 [log_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#log-signal
 [log_record]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogRecord
 [log_emitter]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitter
 [log_emitter_provider]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitterProvider
 [log_processor]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogProcessor
 [logging_handler]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LoggingHandler
 [log_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
+[ot_logging_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html
 [metric_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#metric-signal
 [measurement]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#measurement
 [instrument]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#instrument
 [meter]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meter
 [meter_provider]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meterprovider
 [metric_reader]:https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
 [metric_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
+[ot_metrics_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.html
 [trace_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#tracing-signal
 [span]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Span
 [tracer]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Tracer
 [tracer_provider]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.TracerProvider
 [span_processor]: https://opentelemetry-python.readthedocs.io/en/stable/_modules/opentelemetry/sdk/trace.html?highlight=SpanProcessor#
 [trace_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
+[ot_tracing_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/trace.html
 [sampler_ref]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/trace/sdk.md#sampling
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/CHANGELOG.md` & `azure-monitor-opentelemetry-exporter-1.0.0b9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,37 @@
 # Release History
 
+## 1.0.0b9 (2022-11-08)
+
+### Features Added
+
+- Add Sampler factory and entry point
+    ([#27236](https://github.com/Azure/azure-sdk-for-python/pull/27236))
+- Add validation logic to ApplicationInsightsSampler
+    ([#26546](https://github.com/Azure/azure-sdk-for-python/pull/26546))
+- Change default temporality of metrics to follow OTLP
+    ([#26924](https://github.com/Azure/azure-sdk-for-python/pull/26924))
+
+### Breaking Changes
+
+- Rename local storage configuration, change default path
+    ([#26891](https://github.com/Azure/azure-sdk-for-python/pull/26891))
+- Change default storage retention period to 48 hours
+    ([#26960](https://github.com/Azure/azure-sdk-for-python/pull/26960))
+
+### Bugs Fixed
+
+- Fixed sampleRate field in ApplicationInsightsSampler, changed attribute to `_MS.sampleRate`
+    ([#26771](https://github.com/Azure/azure-sdk-for-python/pull/26771))
+
+### Other Changes
+
+- Update `README.md`
+    ([#26520](https://github.com/Azure/azure-sdk-for-python/pull/26520))
+
 ## 1.0.0b8 (2022-09-26)
 
 ### Features Added
 
 - Implement success count network statsbeat
     ([#25752](https://github.com/Azure/azure-sdk-for-python/pull/25752))
 - Implement all network statsbeat
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/README.md` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,29 @@
-# Microsoft OpenTelemetry exporter for Azure Monitor
+Metadata-Version: 2.1
+Name: azure-monitor-opentelemetry-exporter
+Version: 1.0.0b9
+Summary: Microsoft Azure Monitor Opentelemetry Exporter Client Library for Python
+Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter
+Author: Microsoft Corporation
+Author-email: ascl@microsoft.com
+License: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-[![Gitter chat](https://img.shields.io/gitter/room/Microsoft/azure-monitor-python)](https://gitter.im/Azure/azure-sdk-for-python)
+# Microsoft OpenTelemetry exporter for Azure Monitor
 
 The exporter for Azure Monitor allows you to export data utilizing the OpenTelemetry SDK and send telemetry data to Azure Monitor for applications written in Python.
 
 [Source code](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter) | [Package (PyPi)][pypi] | [API reference documentation][api_docs] | [Product documentation][product_docs] | [Samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter/samples) | [Changelog](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/CHANGELOG.md)
 
 ## Getting started
 
@@ -19,15 +38,15 @@
 ### Prerequisites
 
 To use this package, you must have:
 
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Monitor - [How to use application insights][application_insights_namespace]
 * OpenTelemetry SDK - [OpenTelemetry SDK for Python][ot_sdk_python]
-* Python 3.6 or later - [Install Python][python]
+* Python 3.7 or later - [Install Python][python]
 
 ### Instantiate the client
 
 Interaction with Azure monitor exporter starts with an instance of the `AzureMonitorTraceExporter` class for distributed tracing, `AzureMonitorLogExporter` for logging and `AzureMonitorMetricExporter` for metrics. You will need a **connection_string** to instantiate the object.
 Please find the samples linked below for demonstration as to how to construct the exporter using a connection string.
 
 #### Logging (experimental)
@@ -126,30 +145,44 @@
 
 * [Sampling][sampler_ref]: Sampling is a mechanism to control the noise and overhead introduced by OpenTelemetry by reducing the number of samples of traces collected and sent to the backend.
 
 * ApplicationInsightsSampler: Application Insights specific sampler used for consistent sampling across Application Insights SDKs and OpenTelemetry-based SDKs sending data to Application Insights. This sampler MUST be used whenever `AzureMonitorTraceExporter` is used.
 
 For more information about these resources, see [What is Azure Monitor?][product_docs].
 
+## Configuration
+
+All configuration options can be passed through the constructors of exporters through `kwargs`. Below is a list of configurable options.
+
+`connection_string`: The connection string used for your Application Insights resource.
+`disable_offline_storage`: Boolean value to determine whether to disable storing failed telemetry records for retry. Defaults to `False`.
+`storage_directory`: Storage directory in which to store retry files. Defaults to `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
+
 ## Examples
 
 ### Logging (experimental)
 
 NOTE: The logging signal for the `AzureMonitorLogExporter` is currently in an EXPERIMENTAL state. Possible breaking changes may ensue in the future.
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a log record](#export-hello-world-log)
 * [Exporting correlated log record](#export-correlated-log)
 * [Exporting log record with custom properties](#export-custom-properties-log)
 * [Exporting an exceptions log record](#export-exceptions-log)
 
+Review the [OpenTelemetry Logging SDK][ot_logging_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Log
 
 ```Python
+"""
+An example to show an application using Opentelemetry logging sdk. Logging calls to the standard Python
+logging library are tracked and telemetry is exported to application insights with the AzureMonitorLogExporter.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -176,14 +209,17 @@
 
 logger.warning("Hello World!")
 ```
 
 #### Export Correlated Log
 
 ```Python
+"""
+An example showing how to include context correlation information in logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry import trace
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
@@ -217,14 +253,17 @@
     logger.warning("WARNING: Inside of span")
 logger.error("ERROR: After span")
 ```
 
 #### Export Custom Properties Log
 
 ```Python
+"""
+An example showing how to add custom properties to logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -252,16 +291,14 @@
 # Custom properties
 logger.debug("DEBUG: Debug with properties", extra={"debug": "true"})
 ```
 
 #### Export Exceptions Log
 
 ```Python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example showing how to export exception telemetry using the AzureMonitorLogExporter.
 """
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
@@ -305,19 +342,19 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Using different metric instruments](#metric-instrument-usage)
 * [Customizing outputted metrics with views](#metric-custom-views)
 * [Recording instruments with attributes](#metric-record-attributes)
 
+Review the [OpenTelemetry Metrics SDK][ot_metrics_sdk] to learn how to use OpenTelemetry components to collect metrics.
+
 #### Metric instrument usage
 
 ```python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example to show an application using all instruments in the OpenTelemetry SDK. Metrics created
 and recorded using the sdk are tracked and telemetry is exported to application insights with the
 AzureMonitorMetricsExporter.
 """
 import os
 from typing import Iterable
@@ -379,14 +416,19 @@
 gauge = meter.create_observable_gauge("gauge", [observable_gauge_func])
 
 ```
 
 #### Metric custom views
 
 ```python
+"""
+This example shows how to customize the metrics that are output by the SDK using Views. Metrics created
+and recorded using the sdk are tracked and telemetry is exported to application insights with the
+AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import Counter, MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.metrics.view import View
 
@@ -416,17 +458,24 @@
 
 meter = metrics.get_meter_provider().get_meter("view-name-change")
 my_counter = meter.create_counter("my.counter")
 my_counter.add(100)
 
 ```
 
+More examples with the metrics `Views` SDK can be found [here](https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views).
+
 #### Metric record attributes
 
 ```python
+"""
+An example to show an application using different attributes with instruments in the OpenTelemetry SDK.
+Metrics created and recorded using the sdk are tracked and telemetry is exported to application insights
+with the AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
@@ -471,17 +520,23 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a custom span](#export-hello-world-trace)
 * [Using an instrumentation to track a library](#instrumentation-with-requests-library)
 * [Enabling sampling to limit the amount of telemetry sent](#enabling-sampling)
 
+Review the [OpenTelemetry Tracing SDK][ot_tracing_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Trace
 
 ```Python
+"""
+An example to show an application using Opentelemetry tracing api and sdk. Custom dependencies are
+tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 
 trace.set_tracer_provider(TracerProvider())
@@ -497,19 +552,28 @@
     print("Hello, World!")
 ```
 
 #### Instrumentation with requests library
 
 OpenTelemetry also supports several instrumentations which allows to instrument with third party libraries.
 
+For a list of instrumentations available in OpenTelemetry, visit the contrib [documentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/).
+
 This example shows how to instrument with the [requests](https://pypi.org/project/requests/) library.
 
-* Install the requests integration package using pip install opentelemetry-instrumentation-requests.
+* Install the requests instrumentation package using pip install opentelemetry-instrumentation-requests.
 
 ```Python
+"""
+An example to show an application instrumented with the OpenTelemetry requests instrumentation.
+Calls made with the requests library will be automatically tracked and telemetry is exported to 
+application insights with the AzureMonitorTraceExporter.
+See more info on the requests instrumentation here:
+https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
+"""
 import os
 import requests
 from opentelemetry import trace
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
@@ -527,15 +591,22 @@
 
 # This request will be traced
 response = requests.get(url="https://azure.microsoft.com/")
 ```
 
 #### Enabling sampling
 
+You can enable sampling to limit the amount of telemetry records you receive. In order to enable correct sampling in Application Insights, use the `ApplicationInsightsSampler` as shown below.
+
 ```Python
+"""
+An example to show an application using the ApplicationInsightsSampler to enable sampling for your telemetry.
+Specify a sampling rate for the sampler to limit the amount of telemetry records you receive. Custom dependencies
+ are tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import (
     ApplicationInsightsSampler,
     AzureMonitorTraceExporter,
@@ -570,14 +641,18 @@
 
 ### Additional documentation
 
 For more extensive documentation on the Azure Monitor service, see the [Azure Monitor documentation][product_docs] on docs.microsoft.com.
 
 For detailed overview of OpenTelemetry, visit their [overview](https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md) page.
 
+For the official OpenTelemetry Python documentation and how to enable other telemetry scenarios, visit the official OpenTelemetry [website](https://opentelemetry.io/docs/instrumentation/python/).
+
+For more information on the Azure Monitor OpenTelemetry Distro, which is a bundle of useful, pre-assembled components (one of them being this current package) that enable telemetry scenarios with Azure Monitor, visit the [README](https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry-distro).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
@@ -585,44 +660,41 @@
 provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 <!-- LINKS -->
-[azure_cli]: https://docs.microsoft.com/cli/azure
 [api_docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-opentelemetry-exporter-azuremonitor/1.0.0b2/index.html
 [product_docs]: https://docs.microsoft.com/azure/azure-monitor/overview
-[azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
-[cloud_shell]: https://docs.microsoft.com/azure/cloud-shell/overview
-[cloud_shell_bash]: https://shell.azure.com/bash
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/project/azure-monitor-opentelemetry-exporter/
 [python]: https://www.python.org/downloads/
-[venv]: https://docs.python.org/3/library/venv.html
-[virtualenv]: https://virtualenv.pypa.io
 [ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
 [application_insights_namespace]: https://docs.microsoft.com/azure/azure-monitor/app/app-insights-overview#how-do-i-use-application-insights
 [opentelemetry_spec]: https://opentelemetry.io/
 [instrumentation_library]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md#instrumentation-libraries
 [log_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#log-signal
 [log_record]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogRecord
 [log_emitter]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitter
 [log_emitter_provider]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitterProvider
 [log_processor]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogProcessor
 [logging_handler]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LoggingHandler
 [log_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
+[ot_logging_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html
 [metric_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#metric-signal
 [measurement]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#measurement
 [instrument]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#instrument
 [meter]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meter
 [meter_provider]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meterprovider
 [metric_reader]:https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
 [metric_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
+[ot_metrics_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.html
 [trace_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#tracing-signal
 [span]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Span
 [tracer]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Tracer
 [tracer_provider]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.TracerProvider
 [span_processor]: https://opentelemetry-python.readthedocs.io/en/stable/_modules/opentelemetry/sdk/trace.html?highlight=SpanProcessor#
 [trace_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
+[ot_tracing_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/trace.html
 [sampler_ref]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/trace/sdk.md#sampling
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/LICENSE` & `azure-monitor-opentelemetry-exporter-1.0.0b9/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_chat.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_chat.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_storage_blob.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_storage_blob.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_cosmos.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_cosmos.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_psycopg2.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_psycopg2.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,14 @@
 span_processor = BatchSpanProcessor(
     AzureMonitorTraceExporter.from_connection_string(
         os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
     )
 )
 trace.get_tracer_provider().add_span_processor(span_processor)
 
-cnx = psycopg2.connect(database='Database')
+cnx = psycopg2.connect(database='test', user="<user>", password="<password>")
 cursor = cnx.cursor()
-cursor.execute("INSERT INTO test (testField) VALUES (123)")
+cursor.execute("INSERT INTO test_tables (test_field) VALUES (123)")
 cursor.close()
 cnx.close()
 
 # cSpell:enable
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_flask.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_flask.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_grid.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_grid.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_send.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_send.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_app_config.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_app_config.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_blob_checkpoint.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_blob_checkpoint.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_secret.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_secret.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_form_recognizer.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_form_recognizer.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/README.md` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 $ python sample_requests.py
 ```
 
 ### Psycopg2 instrumentation
 
 * Update `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable
 
-* Ensure you have a database named `Database` with a table named `test`
+* Ensure you have a database named `test` with a table named `test_table`, make sure `test_table` has a field called `test_field`
+* Supply your `user` and `password` for your database if needed
 * Run the sample
 
 ```sh
 $ pip install opentelemetry-instrumentation-psygopg2
 $ # from this directory
 $ python sample_psycopg2.py
 ```
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_requests.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_requests.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_text_analytics.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_text_analytics.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_span_event.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_span_event.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_jaeger.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_jaeger.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_keys.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_keys.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_event_hub.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_event_hub.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_servicebus_receive.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_servicebus_receive.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_trace.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_trace.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_phone.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_phone.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_comm_sms.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_comm_sms.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/sample_key_cert.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/sample_key_cert.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/collector/sample_collector.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/collector/sample_collector.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/manage.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/manage.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/example/views.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/example/views.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/urls.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/urls.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/settings.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/settings.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/traces/django/sample/sample/asgi.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/traces/django/sample/sample/asgi.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_exception.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_exception.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_log.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_log.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/README.md` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/README.md`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_properties.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_properties.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/logs/sample_correlate.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/logs/sample_correlate.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_views.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 """
 This example shows how to customize the metrics that are output by the SDK using Views. Metrics created
 and recorded using the sdk are tracked and telemetry is exported to application insights with the
-AzureMonitorMetricsExporter.
+AzureMonitorMetricExporter.
 """
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import Counter, MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.metrics.view import View
@@ -21,15 +21,16 @@
 # and configure the new name `my.counter.total` for the result metrics stream
 change_metric_name_view = View(
     instrument_type=Counter,
     instrument_name="my.counter",
     name="my.counter.total",
 )
 
-reader = PeriodicExportingMetricReader(exporter, export_interval_millis=5000)
+# Metrics are reported every 1 minute
+reader = PeriodicExportingMetricReader(exporter)
 provider = MeterProvider(
     metric_readers=[
         reader,
     ],
     views=[
         change_metric_name_view,
     ],
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_attributes.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_attributes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 """
 An example to show an application using different attributes with instruments in the OpenTelemetry SDK.
 Metrics created and recorded using the sdk are tracked and telemetry is exported to application insights
-with the AzureMonitorMetricsExporter.
+with the AzureMonitorMetricExporter.
 """
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
 
 exporter = AzureMonitorMetricExporter.from_connection_string(
     os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
 )
-reader = PeriodicExportingMetricReader(exporter, export_interval_millis=5000)
+# Metrics are reported every 1 minute
+reader = PeriodicExportingMetricReader(exporter)
 metrics.set_meter_provider(MeterProvider(metric_readers=[reader]))
 
 attribute_set1 = {
     "key1": "val1"
 }
 attribute_set2 = {
     "key2": "val2"
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/samples/metrics/sample_instruments.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/samples/metrics/sample_instruments.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
+# cSpell:disable
 """
 An example to show an application using all instruments in the OpenTelemetry SDK. Metrics created
 and recorded using the sdk are tracked and telemetry is exported to application insights with the
-AzureMonitorMetricsExporter.
+AzureMonitorMetricExporter.
 """
 import os
 from typing import Iterable
 
 from opentelemetry import metrics
 from opentelemetry.metrics import CallbackOptions, Observation
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
 
 exporter = AzureMonitorMetricExporter.from_connection_string(
     os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
 )
-reader = PeriodicExportingMetricReader(exporter, export_interval_millis=5000)
+# Metrics are reported every 1 minute
+reader = PeriodicExportingMetricReader(exporter)
 metrics.set_meter_provider(MeterProvider(metric_readers=[reader]))
 
 # Create a namespaced meter
 meter = metrics.get_meter_provider().get_meter("sample")
 
 # Callback functions for observable instruments
 def observable_counter_func(options: CallbackOptions) -> Iterable[Observation]:
@@ -59,7 +61,9 @@
 
 # Histogram
 histogram = meter.create_histogram("histogram")
 histogram.record(99.9)
 
 # Async Gauge
 gauge = meter.create_observable_gauge("gauge", [observable_gauge_func])
+
+# cSpell:disable
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_utils.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_constants.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,7 +94,11 @@
     "system-metrics",
     "tornado",
     "urllib",
     "urllib3",
 ]
 # cSpell:enable
 _INSTRUMENTATIONS_BIT_MAP = {_INSTRUMENTATIONS_LIST[i]: _BASE**i for i in range(len(_INSTRUMENTATIONS_LIST))}
+
+# sampleRate
+
+_SAMPLE_RATE_KEY = "_MS.sampleRate"
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_connection_string_parser.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_storage.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 # pylint: disable=broad-except
 class LocalFileStorage:
     def __init__(
         self,
         path,
         max_size=50 * 1024 * 1024,  # 50MiB
         maintenance_period=60,  # 1 minute
-        retention_period=7 * 24 * 60 * 60,  # 7 days
+        retention_period=48 * 60 * 60,  # 48 hours
         write_timeout=60,  # 1 minute,
         name=None,
         lease_period=60,  # 1 minute
     ):
         self._path = os.path.abspath(path)
         self._max_size = max_size
         self._retention_period = retention_period
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_vendor.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_azure_monitor_client.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_patch.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/_configuration.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/models/_azure_monitor_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/operations/_azure_monitor_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_azure_monitor_client.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/_generated/aio/operations/_azure_monitor_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/_base.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     increment_and_check_statsbeat_failure_count,
     is_statsbeat_enabled,
     set_statsbeat_initial_success,
 )
 
 logger = logging.getLogger(__name__)
 
+_AZURE_TEMPDIR_PREFIX = "Microsoft/AzureMonitor"
 _TEMPDIR_PREFIX = "opentelemetry-python-"
 _SERVICE_API_LATEST = "2020-09-15_Preview"
 
 class ExportResult(Enum):
     SUCCESS = 0
     FAILED_RETRYABLE = 1
     FAILED_NOT_RETRYABLE = 2
@@ -54,32 +55,35 @@
 class BaseExporter:
     """Azure Monitor base exporter for OpenTelemetry."""
 
     def __init__(self, **kwargs: Any) -> None:
         """Azure Monitor base exporter for OpenTelemetry.
 
         :keyword str api_version: The service API version used. Defaults to latest.
+        :keyword str connection_string: The connection string used for your Application Insights resource.
+        :keyword bool disable_offline_storage: Determines whether to disable storing failed telemetry records for retry. Defaults to `False`.
+        :keyword str storage_directory: Storage path in which to store retry files. Defaults to `<tempfile.gettempdir()>/opentelemetry-python-<your-instrumentation-key>`.
         :rtype: None
         """
         parsed_connection_string = ConnectionStringParser(kwargs.get('connection_string'))
 
         self._api_version = kwargs.get('api_version') or _SERVICE_API_LATEST
         self._consecutive_redirects = 0  # To prevent circular redirects
-        self._enable_local_storage = kwargs.get('enable_local_storage', True)
+        self._disable_offline_storage = kwargs.get('disable_offline_storage', False)
         self._endpoint = parsed_connection_string.endpoint
         self._instrumentation_key = parsed_connection_string.instrumentation_key
         self._storage_maintenance_period = kwargs.get('storage_maintenance_period', 60)  # Maintenance interval in seconds.
         self._storage_max_size = kwargs.get('storage_max_size', 50 * 1024 * 1024)  # Maximum size in bytes (default 50MiB)
         self._storage_min_retry_interval = kwargs.get('storage_min_retry_interval', 60)  # minimum retry interval in seconds
         temp_suffix = self._instrumentation_key or ""
-        default_storage_path = os.path.join(
-            tempfile.gettempdir(), _TEMPDIR_PREFIX + temp_suffix
+        default_storage_directory = os.path.join(
+            tempfile.gettempdir(), _AZURE_TEMPDIR_PREFIX, _TEMPDIR_PREFIX + temp_suffix
         )
-        self._storage_path = kwargs.get('storage_path', default_storage_path)  # Maintenance interval in seconds.
-        self._storage_retention_period = kwargs.get('storage_retention_period', 7 * 24 * 60 * 60)  # Retention period in seconds
+        self._storage_directory = kwargs.get('storage_directory', default_storage_directory)  # Storage path in which to store retry files.
+        self._storage_retention_period = kwargs.get('storage_retention_period', 48 * 60 * 60)  # Retention period in seconds (default 48 hrs)
         self._timeout = kwargs.get('timeout', 10.0)  # networking timeout in seconds
 
         config = AzureMonitorClientConfiguration(self._endpoint, **kwargs)
         policies = [
             RequestIdPolicy(**kwargs),
             config.headers_policy,
             config.user_agent_policy,
@@ -94,17 +98,17 @@
             # Explicitly disabling to avoid infinite loop of Span creation when data is exported
             # DistributedTracingPolicy(**kwargs),
             config.http_logging_policy or HttpLoggingPolicy(**kwargs)
         ]
         self.client = AzureMonitorClient(
             host=self._endpoint, connection_timeout=self._timeout, policies=policies, **kwargs)
         self.storage = None
-        if self._enable_local_storage:
+        if not self._disable_offline_storage:
             self.storage = LocalFileStorage(
-                path=self._storage_path,
+                path=self._storage_directory,
                 max_size=self._storage_max_size,
                 maintenance_period=self._storage_maintenance_period,
                 retention_period=self._storage_retention_period,
                 name="{} Storage".format(self.__class__.__name__),
                 lease_period=self._storage_min_retry_interval,
             )
         # statsbeat initialization
@@ -114,15 +118,15 @@
             collect_statsbeat_metrics(self)
 
     def _transmit_from_storage(self) -> None:
         for blob in self.storage.gets():
             # give a few more seconds for blob lease operation
             # to reduce the chance of race (for perf consideration)
             if blob.lease(self._timeout + 5):
-                envelopes = [TelemetryItem(**x) for x in blob.get()]
+                envelopes = [TelemetryItem.from_dict(x) for x in blob.get()]
                 result = self._transmit(list(envelopes))
                 if result == ExportResult.FAILED_RETRYABLE:
                     blob.lease(1)
                 else:
                     blob.delete()
 
     def _handle_transmit_from_storage(self, envelopes: List[TelemetryItem], result: ExportResult) -> None:
@@ -198,26 +202,30 @@
                     if self._should_collect_stats():
                         _update_requests_map(_REQ_THROTTLE_NAME[1], value=response_error.status_code)
                     result = ExportResult.FAILED_NOT_RETRYABLE
                 elif _is_redirect_code(response_error.status_code):
                     self._consecutive_redirects = self._consecutive_redirects + 1
                     if self._consecutive_redirects < self.client._config.redirect_policy.max_redirects:  # pylint: disable=W0212
                         if response_error.response and response_error.response.headers:
+                            redirect_has_headers = True
                             location = response_error.response.headers.get("location")
-                            if location:
-                                url = urlparse(location)
-                                if url.scheme and url.netloc:
-                                    # Change the host to the new redirected host
-                                    self.client._config.host = "{}://{}".format(url.scheme, url.netloc)  # pylint: disable=W0212
-                                    # Attempt to export again
-                                    result =  self._transmit(envelopes)
-                        if not self._is_stats_exporter():
-                            logger.error(
-                                "Error parsing redirect information."
-                            )
+                            url = urlparse(location)
+                        else:
+                            redirect_has_headers = False
+                        if redirect_has_headers and url.scheme and url.netloc:
+                            # Change the host to the new redirected host
+                            self.client._config.host = "{}://{}".format(url.scheme, url.netloc)  # pylint: disable=W0212
+                            # Attempt to export again
+                            result = self._transmit(envelopes)
+                        else:
+                            if not self._is_stats_exporter():
+                                logger.error(
+                                    "Error parsing redirect information.",
+                                )
+                            result = ExportResult.FAILED_NOT_RETRYABLE
                     else:
                         if not self._is_stats_exporter():
                             logger.error(
                                 "Error sending telemetry because of circular redirects. " \
                                 "Please check the integrity of your connection string."
                             )
                         # If redirect but did not return, exception occurred
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 import logging
 
 from typing import Optional, Any
 
+from opentelemetry.sdk.metrics import (
+    Counter,
+    Histogram,
+    ObservableCounter,
+    ObservableGauge,
+    ObservableUpDownCounter,
+    UpDownCounter,
+)
 from opentelemetry.sdk.metrics.export import (
+    AggregationTemporality,
     DataPointT,
     HistogramDataPoint,
     MetricExporter,
     MetricExportResult,
     MetricsData as OTMetricsData,
     NumberDataPoint,
 )
@@ -28,22 +37,32 @@
 )
 
 _logger = logging.getLogger(__name__)
 
 __all__ = ["AzureMonitorMetricExporter"]
 
 
+APPLICATION_INSIGHTS_METRIC_TEMPORALITIES = {
+    Counter: AggregationTemporality.DELTA,
+    Histogram: AggregationTemporality.DELTA,
+    ObservableCounter: AggregationTemporality.DELTA,
+    ObservableGauge: AggregationTemporality.CUMULATIVE,
+    ObservableUpDownCounter: AggregationTemporality.CUMULATIVE,
+    UpDownCounter: AggregationTemporality.CUMULATIVE,
+}
+
+
 class AzureMonitorMetricExporter(BaseExporter, MetricExporter):
     """Azure Monitor Metric exporter for OpenTelemetry."""
 
     def __init__(self, **kwargs: Any) -> None:
         BaseExporter.__init__(self, **kwargs)
         MetricExporter.__init__(
             self,
-            preferred_temporality=kwargs.get("preferred_temporality"),
+            preferred_temporality=APPLICATION_INSIGHTS_METRIC_TEMPORALITIES,
             preferred_aggregation=kwargs.get("preferred_aggregation"),
         )
 
     def export(
         self,
         metrics_data: OTMetricsData,
         timeout_millis: float = 10_000,  # pylint: disable=unused-argument
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,30 +11,34 @@
     Sampler,
     SamplingResult,
     _get_parent_trace_state,
 )
 from opentelemetry.trace.span import TraceState
 from opentelemetry.util.types import Attributes
 
+from azure.monitor.opentelemetry.exporter._constants import _SAMPLE_RATE_KEY
+
 
 _HASH = 5381
 _INTEGER_MAX = Int32.maxval
 _INTEGER_MIN = Int32.minval
 
 
 # Sampler is responsible for the following:
 # Implements same trace id hashing algorithm so that traces are sampled the same across multiple nodes (via AI SDKS)
 # Adds item count to span attribute if span is sampled (needed for ingestion service)
 # Inherits from the Sampler interface as defined by OpenTelemetry
 # https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/trace/sdk.md#sampler
 class ApplicationInsightsSampler(Sampler):
     """Sampler that implements the same probability sampling algorithm as the ApplicationInsights SDKs."""
 
-    # sampling_ratio takes values in the range [0,1]
+    # sampling_ratio must take a value in the range [0,1]
     def __init__(self, sampling_ratio: float = 1.0):
+        if not 0.0 <= sampling_ratio <= 1.0:
+            raise ValueError("sampling_ratio must be in the range [0,1]")
         self._ratio = sampling_ratio
         self._sample_rate = round(sampling_ratio * 100)
 
     # pylint:disable=C0301
     # See https://github.com/microsoft/Telemetry-Collection-Spec/blob/main/OpenTelemetry/trace/ApplicationInsightsSampler.md
     def should_sample(
         self,
@@ -56,15 +60,15 @@
             if sample_score < self._ratio:
                 decision = Decision.RECORD_AND_SAMPLE
             else:
                 decision = Decision.DROP
         # Add sample rate as span attribute
         if attributes is None:
             attributes = {}
-        attributes["sampleRate"] = self._sample_rate
+        attributes[_SAMPLE_RATE_KEY] = self._sample_rate
         return SamplingResult(
             decision,
             attributes,
             _get_parent_trace_state(parent_context),
         )
 
     # pylint:disable=R0201
@@ -81,7 +85,15 @@
 
         # divide by _INTEGER_MAX for value between 0 and 1 for sampling score
         return float(hash_value) / _INTEGER_MAX
 
 
     def get_description(self) -> str:
         return "ApplicationInsightsSampler{}".format(self._ratio)
+
+
+def azure_monitor_opentelemetry_sampler_factory(sampler_argument):
+    try:
+        rate = float(sampler_argument)
+        return ApplicationInsightsSampler(rate)
+    except ValueError:
+        return ApplicationInsightsSampler()
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from opentelemetry.util.types import Attributes
 from opentelemetry.semconv.trace import DbSystemValues, SpanAttributes
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SpanExporter, SpanExportResult
 from opentelemetry.trace import SpanKind
 
+from azure.monitor.opentelemetry.exporter._constants import _SAMPLE_RATE_KEY
 from azure.monitor.opentelemetry.exporter import _utils
 from azure.monitor.opentelemetry.exporter._generated.models import (
     MessageData,
     MonitorBase,
     RemoteDependencyData,
     RequestData,
     TelemetryExceptionData,
@@ -41,14 +42,18 @@
     "peer.",
     "exception.",
     "thread.",
     "fass.",
     "code.",
 ]
 
+_STANDARD_AZURE_MONITOR_ATTRIBUTES = [
+    _SAMPLE_RATE_KEY,
+]
+
 
 class AzureMonitorTraceExporter(BaseExporter, SpanExporter):
     """Azure Monitor Trace exporter for OpenTelemetry."""
 
     def export(self, spans: Sequence[ReadableSpan], **kwargs: Any) -> SpanExportResult: # pylint: disable=unused-argument
         """Export span data
         :param spans: Open Telemetry Spans to export.
@@ -416,17 +421,21 @@
         if data.data:
             data.data = str(data.data)[:8192]
         if data.type:
             data.type = str(data.type)[:1024]
         if target:
             data.target = str(target)[:1024]
 
+    # sampleRate
+    if _SAMPLE_RATE_KEY in span.attributes:
+        envelope.sample_rate = span.attributes[_SAMPLE_RATE_KEY]
+
     data.properties = _utils._filter_custom_properties(
         span.attributes,
-        lambda key, val: not _is_opentelemetry_standard_attribute(key)
+        lambda key, val: not _is_standard_attribute(key)
     )
     if span.links:
         # Max length for value is 8192
         # Since links are a fixed length (80) in json, max number of links would be 102
         links = []
         for link in span.links:
             if len(links) > 102:
@@ -446,15 +455,15 @@
         envelope.tags["ai.operation.id"] = "{:032x}".format(span.context.trace_id)
         if span.context and span.context.span_id:
             envelope.tags["ai.operation.parentId"] = "{:016x}".format(
                 span.context.span_id
             )
         properties = _utils._filter_custom_properties(
             event.attributes,
-            lambda key, val: not _is_opentelemetry_standard_attribute(key)
+            lambda key, val: not _is_standard_attribute(key)
         )
         if event.name == "exception":
             envelope.name = 'Microsoft.ApplicationInsights.Exception'
             exc_type = event.attributes.get(SpanAttributes.EXCEPTION_TYPE)
             exc_message = event.attributes.get(SpanAttributes.EXCEPTION_MESSAGE)
             if exc_message is None or not exc_message:
                 exc_message = "Exception"
@@ -541,19 +550,20 @@
     if span.instrumentation_scope.name.startswith("opentelemetry.instrumentation."):
         # The string after the prefix is the name of the instrumentation
         name = span.instrumentation_scope.name.split("opentelemetry.instrumentation.", 1)[1]
         # Update the bit map to indicate instrumentation is being used
         _utils.add_instrumentation(name)
 
 
-def _is_opentelemetry_standard_attribute(key: str) -> bool:
+def _is_standard_attribute(key: str) -> bool:
     for prefix in _STANDARD_OPENTELEMETRY_ATTRIBUTE_PREFIXES:
         if key.startswith(prefix):
             return True
-    return False
+    return key in _STANDARD_AZURE_MONITOR_ATTRIBUTES
+
 
 def _get_azure_sdk_target_source(attributes: Attributes) -> Optional[str]:
     # Currently logic only works for ServiceBus and EventHub
     peer_address = attributes.get("peer.address")
     destination = attributes.get("message_bus.destination")
     if peer_address and destination:
         return peer_address + "/" + destination
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_state.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_state.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_statsbeat_metrics.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure/monitor/opentelemetry/exporter/statsbeat/_exporter.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_utils.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_utils.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_storage.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_storage.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_base_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_base_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         base = BaseExporter(
             api_version="2021-02-10_Preview",
             connection_string="InstrumentationKey=4321abcd-5678-4efa-8abc-1234567890ab;IngestionEndpoint=https://westus-0.in.applicationinsights.azure.com/",
             enable_local_storage=True,
             storage_maintenance_period=30,
             storage_max_size=1000,
             storage_min_retry_interval=100,
-            storage_path="test/path",
+            storage_directory="test/path",
             storage_retention_period=2000,
         )
         self.assertEqual(
             base._instrumentation_key,
             "4321abcd-5678-4efa-8abc-1234567890ab",
         )
         self.assertEqual(
@@ -98,42 +98,46 @@
         self.assertIsNotNone(base.storage)
         self.assertEqual(base.storage._max_size, 1000)
         self.assertEqual(base.storage._retention_period, 2000)
         self.assertEqual(base._storage_maintenance_period, 30)
         self.assertEqual(base._timeout, 10)
         self.assertEqual(base._api_version, "2021-02-10_Preview")
         self.assertEqual(base._storage_min_retry_interval, 100)
-        self.assertEqual(base._storage_path, "test/path")
+        self.assertEqual(base._storage_directory, "test/path")
 
-    def test_transmit_from_storage_success(self):
+    @mock.patch.object(TelemetryItem, "from_dict")
+    def test_transmit_from_storage_success(self, dict_patch):
         exporter = BaseExporter()
         exporter.storage = mock.Mock()
         blob_mock = mock.Mock()
         blob_mock.lease.return_value = True
         envelope_mock = {"name":"test","time":"time"}
         blob_mock.get.return_value = [envelope_mock]
+        dict_patch.return_value = {"name":"test","time":"time"}
         exporter.storage.gets.return_value = [blob_mock]
         with mock.patch.object(AzureMonitorClient, 'track') as post:
             post.return_value = TrackResponse(
                 items_received=1,
                 items_accepted=1,
                 errors=[],
             )
             exporter._transmit_from_storage()
         exporter.storage.gets.assert_called_once()
         blob_mock.lease.assert_called_once()
         blob_mock.delete.assert_called_once()
 
-    def test_transmit_from_storage_store_again(self):
+    @mock.patch.object(TelemetryItem, "from_dict")
+    def test_transmit_from_storage_store_again(self, dict_patch):
         exporter = BaseExporter()
         exporter.storage = mock.Mock()
         blob_mock = mock.Mock()
         blob_mock.lease.return_value = True
         envelope_mock = {"name":"test","time":"time"}
         blob_mock.get.return_value = [envelope_mock]
+        dict_patch.return_value = {"name":"test","time":"time"}
         exporter.storage.gets.return_value = [blob_mock]
         with mock.patch("azure.monitor.opentelemetry.exporter.export._base._is_retryable_code"):
             with mock.patch.object(AzureMonitorClient, 'track', throw(HttpResponseError)):
                 exporter._transmit_from_storage()
         exporter.storage.gets.assert_called_once()
         blob_mock.lease.assert_called()
         blob_mock.delete.assert_not_called()
@@ -184,14 +188,40 @@
             result = self._base._transmit(self._envelopes_to_export)
             self.assertEqual(result, ExportResult.FAILED_NOT_RETRYABLE)
             self.assertEqual(post.call_count, 2)
             self.assertEqual(self._base.client._config.host, "https://example.com")
         self._base.client._config.redirect_policy.max_redirects = prev_redirects
         self._base.client._config.host = prev_host
 
+    def test_transmit_http_error_redirect_missing_headers(self):
+        response = HttpResponse(None, None)
+        response.status_code = 307
+        response.headers = None
+        error = HttpResponseError(response=response)
+        prev_host = self._base.client._config.host
+        with mock.patch.object(AzureMonitorClient, 'track') as post:
+            post.side_effect = error
+            result = self._base._transmit(self._envelopes_to_export)
+            self.assertEqual(result, ExportResult.FAILED_NOT_RETRYABLE)
+            self.assertEqual(post.call_count, 1)
+            self.assertEqual(self._base.client._config.host, prev_host)
+
+    def test_transmit_http_error_redirect_invalid_location_header(self):
+        response = HttpResponse(None, None)
+        response.status_code = 307
+        response.headers = {"location":"123"}
+        error = HttpResponseError(response=response)
+        prev_host = self._base.client._config.host
+        with mock.patch.object(AzureMonitorClient, 'track') as post:
+            post.side_effect = error
+            result = self._base._transmit(self._envelopes_to_export)
+            self.assertEqual(result, ExportResult.FAILED_NOT_RETRYABLE)
+            self.assertEqual(post.call_count, 1)
+            self.assertEqual(self._base.client._config.host, prev_host)
+
     def test_transmit_request_error(self):
         with mock.patch.object(AzureMonitorClient, 'track', throw(ServiceRequestError, message="error")):
             result = self._base._transmit(self._envelopes_to_export)
         self.assertEqual(result, ExportResult.FAILED_RETRYABLE)
 
     @mock.patch.dict(
         os.environ,
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/conftest.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/test_connection_string_parser.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/test_connection_string_parser.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/perfstress_tests/trace_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/perfstress_tests/trace_exporter.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/logs/test_logs.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/logs/test_logs.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/metrics/test_metrics.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/metrics/test_metrics.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/trace/test_trace.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/trace/test_trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -972,14 +972,42 @@
         )
         span._status = Status(status_code=StatusCode.ERROR)
         span.start(start_time=start_time)
         span.end(end_time=end_time)
         envelope = exporter._span_to_envelope(span)
         self.assertFalse(envelope.data.base_data.success)
 
+    def test_span_to_envelope_sample_rate(self):
+        exporter = self._exporter
+        start_time = 1575494316027613500
+        end_time = start_time + 1001000000
+
+        span = trace._Span(
+            name="test",
+            context=SpanContext(
+                trace_id=36873507687745823477771305566750195431,
+                span_id=12030755672171557337,
+                is_remote=False,
+            ),
+            attributes={
+                "test": "asd",
+                "http.method": "GET",
+                "http.url": "https://www.wikipedia.org/wiki/Rabbit",
+                "http.status_code": 200,
+                "_MS.sampleRate": 50,
+            },
+            kind=SpanKind.CLIENT,
+        )
+        span._status = Status(status_code=StatusCode.OK)
+        span.start(start_time=start_time)
+        span.end(end_time=end_time)
+        envelope = exporter._span_to_envelope(span)
+        self.assertEqual(envelope.sample_rate, 50)
+        self.assertIsNone(envelope.data.base_data.properties.get("_MS.sampleRate"))
+
     def test_span_to_envelope_properties(self):
         exporter = self._exporter
         start_time = 1575494316027613500
         end_time = start_time + 1001000000
 
         # Properties
         span = trace._Span(
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_statsbeat.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_statsbeat.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/tests/statsbeat/test_exporter.py` & `azure-monitor-opentelemetry-exporter-1.0.0b9/tests/statsbeat/test_exporter.py`

 * *Files identical despite different names*

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-exporter-1.0.0b9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,9 @@
-Metadata-Version: 2.1
-Name: azure-monitor-opentelemetry-exporter
-Version: 1.0.0b8
-Summary: Microsoft Azure Monitor Opentelemetry Exporter Client Library for Python
-Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter
-Author: Microsoft Corporation
-Author-email: ascl@microsoft.com
-License: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Microsoft OpenTelemetry exporter for Azure Monitor
 
-[![Gitter chat](https://img.shields.io/gitter/room/Microsoft/azure-monitor-python)](https://gitter.im/Azure/azure-sdk-for-python)
-
 The exporter for Azure Monitor allows you to export data utilizing the OpenTelemetry SDK and send telemetry data to Azure Monitor for applications written in Python.
 
 [Source code](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter) | [Package (PyPi)][pypi] | [API reference documentation][api_docs] | [Product documentation][product_docs] | [Samples](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter/samples) | [Changelog](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/CHANGELOG.md)
 
 ## Getting started
 
 ### Install the package
@@ -39,15 +17,15 @@
 ### Prerequisites
 
 To use this package, you must have:
 
 * Azure subscription - [Create a free account][azure_sub]
 * Azure Monitor - [How to use application insights][application_insights_namespace]
 * OpenTelemetry SDK - [OpenTelemetry SDK for Python][ot_sdk_python]
-* Python 3.6 or later - [Install Python][python]
+* Python 3.7 or later - [Install Python][python]
 
 ### Instantiate the client
 
 Interaction with Azure monitor exporter starts with an instance of the `AzureMonitorTraceExporter` class for distributed tracing, `AzureMonitorLogExporter` for logging and `AzureMonitorMetricExporter` for metrics. You will need a **connection_string** to instantiate the object.
 Please find the samples linked below for demonstration as to how to construct the exporter using a connection string.
 
 #### Logging (experimental)
@@ -146,30 +124,44 @@
 
 * [Sampling][sampler_ref]: Sampling is a mechanism to control the noise and overhead introduced by OpenTelemetry by reducing the number of samples of traces collected and sent to the backend.
 
 * ApplicationInsightsSampler: Application Insights specific sampler used for consistent sampling across Application Insights SDKs and OpenTelemetry-based SDKs sending data to Application Insights. This sampler MUST be used whenever `AzureMonitorTraceExporter` is used.
 
 For more information about these resources, see [What is Azure Monitor?][product_docs].
 
+## Configuration
+
+All configuration options can be passed through the constructors of exporters through `kwargs`. Below is a list of configurable options.
+
+`connection_string`: The connection string used for your Application Insights resource.
+`disable_offline_storage`: Boolean value to determine whether to disable storing failed telemetry records for retry. Defaults to `False`.
+`storage_directory`: Storage directory in which to store retry files. Defaults to `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
+
 ## Examples
 
 ### Logging (experimental)
 
 NOTE: The logging signal for the `AzureMonitorLogExporter` is currently in an EXPERIMENTAL state. Possible breaking changes may ensue in the future.
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a log record](#export-hello-world-log)
 * [Exporting correlated log record](#export-correlated-log)
 * [Exporting log record with custom properties](#export-custom-properties-log)
 * [Exporting an exceptions log record](#export-exceptions-log)
 
+Review the [OpenTelemetry Logging SDK][ot_logging_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Log
 
 ```Python
+"""
+An example to show an application using Opentelemetry logging sdk. Logging calls to the standard Python
+logging library are tracked and telemetry is exported to application insights with the AzureMonitorLogExporter.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -196,14 +188,17 @@
 
 logger.warning("Hello World!")
 ```
 
 #### Export Correlated Log
 
 ```Python
+"""
+An example showing how to include context correlation information in logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry import trace
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
@@ -237,14 +232,17 @@
     logger.warning("WARNING: Inside of span")
 logger.error("ERROR: After span")
 ```
 
 #### Export Custom Properties Log
 
 ```Python
+"""
+An example showing how to add custom properties to logging telemetry.
+"""
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
     LogEmitterProvider,
     LoggingHandler,
     set_log_emitter_provider,
@@ -272,16 +270,14 @@
 # Custom properties
 logger.debug("DEBUG: Debug with properties", extra={"debug": "true"})
 ```
 
 #### Export Exceptions Log
 
 ```Python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example showing how to export exception telemetry using the AzureMonitorLogExporter.
 """
 import os
 import logging
 
 from opentelemetry.sdk._logs import (
@@ -325,19 +321,19 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Using different metric instruments](#metric-instrument-usage)
 * [Customizing outputted metrics with views](#metric-custom-views)
 * [Recording instruments with attributes](#metric-record-attributes)
 
+Review the [OpenTelemetry Metrics SDK][ot_metrics_sdk] to learn how to use OpenTelemetry components to collect metrics.
+
 #### Metric instrument usage
 
 ```python
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License.
 """
 An example to show an application using all instruments in the OpenTelemetry SDK. Metrics created
 and recorded using the sdk are tracked and telemetry is exported to application insights with the
 AzureMonitorMetricsExporter.
 """
 import os
 from typing import Iterable
@@ -399,14 +395,19 @@
 gauge = meter.create_observable_gauge("gauge", [observable_gauge_func])
 
 ```
 
 #### Metric custom views
 
 ```python
+"""
+This example shows how to customize the metrics that are output by the SDK using Views. Metrics created
+and recorded using the sdk are tracked and telemetry is exported to application insights with the
+AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import Counter, MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.metrics.view import View
 
@@ -436,17 +437,24 @@
 
 meter = metrics.get_meter_provider().get_meter("view-name-change")
 my_counter = meter.create_counter("my.counter")
 my_counter.add(100)
 
 ```
 
+More examples with the metrics `Views` SDK can be found [here](https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views).
+
 #### Metric record attributes
 
 ```python
+"""
+An example to show an application using different attributes with instruments in the OpenTelemetry SDK.
+Metrics created and recorded using the sdk are tracked and telemetry is exported to application insights
+with the AzureMonitorMetricsExporter.
+"""
 import os
 
 from opentelemetry import metrics
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 
 from azure.monitor.opentelemetry.exporter import AzureMonitorMetricExporter
@@ -491,17 +499,23 @@
 
 The following sections provide several code snippets covering some of the most common tasks, including:
 
 * [Exporting a custom span](#export-hello-world-trace)
 * [Using an instrumentation to track a library](#instrumentation-with-requests-library)
 * [Enabling sampling to limit the amount of telemetry sent](#enabling-sampling)
 
+Review the [OpenTelemetry Tracing SDK][ot_tracing_sdk] to learn how to use OpenTelemetry components to collect logs.
+
 #### Export Hello World Trace
 
 ```Python
+"""
+An example to show an application using Opentelemetry tracing api and sdk. Custom dependencies are
+tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 
 trace.set_tracer_provider(TracerProvider())
@@ -517,19 +531,28 @@
     print("Hello, World!")
 ```
 
 #### Instrumentation with requests library
 
 OpenTelemetry also supports several instrumentations which allows to instrument with third party libraries.
 
+For a list of instrumentations available in OpenTelemetry, visit the contrib [documentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/).
+
 This example shows how to instrument with the [requests](https://pypi.org/project/requests/) library.
 
-* Install the requests integration package using pip install opentelemetry-instrumentation-requests.
+* Install the requests instrumentation package using pip install opentelemetry-instrumentation-requests.
 
 ```Python
+"""
+An example to show an application instrumented with the OpenTelemetry requests instrumentation.
+Calls made with the requests library will be automatically tracked and telemetry is exported to 
+application insights with the AzureMonitorTraceExporter.
+See more info on the requests instrumentation here:
+https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
+"""
 import os
 import requests
 from opentelemetry import trace
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
@@ -547,15 +570,22 @@
 
 # This request will be traced
 response = requests.get(url="https://azure.microsoft.com/")
 ```
 
 #### Enabling sampling
 
+You can enable sampling to limit the amount of telemetry records you receive. In order to enable correct sampling in Application Insights, use the `ApplicationInsightsSampler` as shown below.
+
 ```Python
+"""
+An example to show an application using the ApplicationInsightsSampler to enable sampling for your telemetry.
+Specify a sampling rate for the sampler to limit the amount of telemetry records you receive. Custom dependencies
+ are tracked via spans and telemetry is exported to application insights with the AzureMonitorTraceExporter.
+"""
 import os
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import (
     ApplicationInsightsSampler,
     AzureMonitorTraceExporter,
@@ -590,14 +620,18 @@
 
 ### Additional documentation
 
 For more extensive documentation on the Azure Monitor service, see the [Azure Monitor documentation][product_docs] on docs.microsoft.com.
 
 For detailed overview of OpenTelemetry, visit their [overview](https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md) page.
 
+For the official OpenTelemetry Python documentation and how to enable other telemetry scenarios, visit the official OpenTelemetry [website](https://opentelemetry.io/docs/instrumentation/python/).
+
+For more information on the Azure Monitor OpenTelemetry Distro, which is a bundle of useful, pre-assembled components (one of them being this current package) that enable telemetry scenarios with Azure Monitor, visit the [README](https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry-distro).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
 When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
@@ -605,44 +639,41 @@
 provided by the bot. You will only need to do this once across all repos using our CLA.
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 <!-- LINKS -->
-[azure_cli]: https://docs.microsoft.com/cli/azure
 [api_docs]: https://azuresdkdocs.blob.core.windows.net/$web/python/azure-opentelemetry-exporter-azuremonitor/1.0.0b2/index.html
 [product_docs]: https://docs.microsoft.com/azure/azure-monitor/overview
-[azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
-[cloud_shell]: https://docs.microsoft.com/azure/cloud-shell/overview
-[cloud_shell_bash]: https://shell.azure.com/bash
 [pip]: https://pypi.org/project/pip/
 [pypi]: https://pypi.org/project/azure-monitor-opentelemetry-exporter/
 [python]: https://www.python.org/downloads/
-[venv]: https://docs.python.org/3/library/venv.html
-[virtualenv]: https://virtualenv.pypa.io
 [ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
 [application_insights_namespace]: https://docs.microsoft.com/azure/azure-monitor/app/app-insights-overview#how-do-i-use-application-insights
 [opentelemetry_spec]: https://opentelemetry.io/
 [instrumentation_library]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/overview.md#instrumentation-libraries
 [log_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#log-signal
 [log_record]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogRecord
 [log_emitter]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitter
 [log_emitter_provider]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogEmitterProvider
 [log_processor]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LogProcessor
 [logging_handler]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html#opentelemetry.sdk._logs.LoggingHandler
 [log_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/logs/_exporter.py
+[ot_logging_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/logs.html
 [metric_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#metric-signal
 [measurement]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#measurement
 [instrument]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#instrument
 [meter]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meter
 [meter_provider]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/api.md#meterprovider
 [metric_reader]:https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
 [metric_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/metrics/_exporter.py
+[ot_metrics_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.html
 [trace_concept]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/overview.md#tracing-signal
 [span]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Span
 [tracer]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.Tracer
 [tracer_provider]: https://opentelemetry-python.readthedocs.io/en/stable/api/trace.html?highlight=TracerProvider#opentelemetry.trace.TracerProvider
 [span_processor]: https://opentelemetry-python.readthedocs.io/en/stable/_modules/opentelemetry/sdk/trace.html?highlight=SpanProcessor#
 [trace_reference]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/monitor/azure-monitor-opentelemetry-exporter/azure/monitor/opentelemetry/exporter/export/trace/_exporter.py
+[ot_tracing_sdk]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/trace.html
 [sampler_ref]: https://github.com/open-telemetry/opentelemetry-specification/blob/master/specification/trace/sdk.md#sampling
```

## Comparing `azure-monitor-opentelemetry-exporter-1.0.0b8/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-exporter-1.0.0b9/azure_monitor_opentelemetry_exporter.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 samples/traces/sample_form_recognizer.py
 samples/traces/sample_jaeger.py
 samples/traces/sample_key_cert.py
 samples/traces/sample_key_keys.py
 samples/traces/sample_key_secret.py
 samples/traces/sample_psycopg2.py
 samples/traces/sample_requests.py
+samples/traces/sample_sampling.py
 samples/traces/sample_servicebus_receive.py
 samples/traces/sample_servicebus_send.py
 samples/traces/sample_span_event.py
 samples/traces/sample_storage_blob.py
 samples/traces/sample_text_analytics.py
 samples/traces/sample_trace.py
 samples/traces/collector/sample_collector.py
@@ -110,8 +111,9 @@
 tests/metrics/test_metrics.py
 tests/perfstress_tests/__init__.py
 tests/perfstress_tests/trace_exporter.py
 tests/statsbeat/__init__.py
 tests/statsbeat/test_exporter.py
 tests/statsbeat/test_statsbeat.py
 tests/trace/__init__.py
+tests/trace/test_sampling.py
 tests/trace/test_trace.py
```

