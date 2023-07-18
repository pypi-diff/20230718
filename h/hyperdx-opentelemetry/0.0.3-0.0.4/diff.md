# Comparing `tmp/hyperdx_opentelemetry-0.0.3.tar.gz` & `tmp/hyperdx_opentelemetry-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdx_opentelemetry-0.0.3.tar", max compression
+gzip compressed data, was "hyperdx_opentelemetry-0.0.4.tar", max compression
```

## Comparing `hyperdx_opentelemetry-0.0.3.tar` & `hyperdx_opentelemetry-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.3/LICENSE
--rw-r--r--   0        0        0     1184 2023-07-14 00:40:33.579362 hyperdx_opentelemetry-0.0.3/README.md
--rw-r--r--   0        0        0      820 2023-07-14 06:41:32.032971 hyperdx_opentelemetry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/baggage.py
--rw-r--r--   0        0        0     3072 2023-07-14 01:15:59.983930 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/distro.py
--rw-r--r--   0        0        0     1601 2023-07-14 00:22:56.721389 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/logs.py
--rw-r--r--   0        0        0     5499 2023-07-14 06:32:50.848960 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/manual.py
--rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/metrics.py
--rw-r--r--   0        0        0    18089 2023-07-14 01:13:04.588438 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/options.py
--rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/resource.py
--rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/sampler.py
--rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/trace.py
--rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/version.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 00:34:40.461547 hyperdx_opentelemetry-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1277 2023-07-18 00:14:38.846653 hyperdx_opentelemetry-0.0.4/README.md
+-rw-r--r--   0        0        0      820 2023-07-18 00:24:12.270245 hyperdx_opentelemetry-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-07-13 23:59:18.772014 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1373 2023-07-13 06:54:02.327463 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     3072 2023-07-14 01:15:59.983930 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/distro.py
+-rw-r--r--   0        0        0     1601 2023-07-18 00:09:01.879435 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/logs.py
+-rw-r--r--   0        0        0     5660 2023-07-18 00:14:38.847197 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/manual.py
+-rw-r--r--   0        0        0     1601 2023-07-13 06:39:14.131376 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    18672 2023-07-18 00:14:38.847568 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/options.py
+-rw-r--r--   0        0        0      826 2023-07-13 06:35:40.043017 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3172 2023-07-13 06:34:37.078271 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     1818 2023-07-13 06:33:47.851726 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/trace.py
+-rw-r--r--   0        0        0       99 2023-07-13 01:54:38.990328 hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/version.py
+-rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 hyperdx_opentelemetry-0.0.4/PKG-INFO
```

### Comparing `hyperdx_opentelemetry-0.0.3/LICENSE` & `hyperdx_opentelemetry-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/README.md` & `hyperdx_opentelemetry-0.0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # HyperDX OpenTelemetry Distro for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/hyperdxio/hyperdx-opentelemetry-python)](https://github.com/hyperdxio/home/blob/main/hyperdx-oss-lifecycle-and-practices.md)
 [![CircleCI](https://circleci.com/gh/hyperdxio/hyperdx-opentelemetry-python.svg?style=shield)](https://circleci.com/gh/hyperdxio/hyperdx-opentelemetry-python)
 [![PyPi](https://img.shields.io/pypi/v/hyperdx-opentelemetry)](https://pypi.org/project/hyperdx-opentelemetry/)
 
+> This project is a fork from https://github.com/honeycombio/honeycomb-opentelemetry-python
+
 **STATUS: this library is BETA.**
 You're welcome to try it, and let us know your feedback in the issues!
 
 This is HyperDX's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and HyperDX easier!
 
 Latest release built with:
```

### Comparing `hyperdx_opentelemetry-0.0.3/pyproject.toml` & `hyperdx_opentelemetry-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperdx-opentelemetry"
-version = "0.0.3"
+version = "0.0.4"
 description = "HyperDX OpenTelemetry Distro for Python"
 authors = ["HyperDX <support@hyperdx.io>"]
 readme = "README.md"
 packages = [{include = "hyperdx", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
```

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/baggage.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/distro.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/distro.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/logs.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/logs.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/manual.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/manual.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,34 +125,37 @@
             tracer_provider=tracer_provider,
         )
     except ImportError as e:
         pass
 
 
 def configure_custom_env_vars(options: HyperDXOptions, resource: Resource):
-    os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_REQUEST"] = os.getenv(
-        "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_REQUEST", ".*"
-    )
-    os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_RESPONSE"] = os.getenv(
-        "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_RESPONSE", ".*"
-    )
-    os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST"] = os.getenv(
-        "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST", ".*"
-    )
-    os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_RESPONSE"] = os.getenv(
-        "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_RESPONSE", ".*"
-    )
+    if options.enable_advanced_network_capture:
+        os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_REQUEST"] = os.getenv(
+            "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_REQUEST", ".*"
+        )
+        os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_RESPONSE"] = os.getenv(
+            "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_CLIENT_RESPONSE", ".*"
+        )
+        os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST"] = os.getenv(
+            "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_REQUEST", ".*"
+        )
+        os.environ["OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_RESPONSE"] = os.getenv(
+            "OTEL_INSTRUMENTATION_HTTP_CAPTURE_HEADERS_SERVER_RESPONSE", ".*"
+        )
+
     os.environ["OTEL_PYTHON_LOG_CORRELATION"] = os.getenv(
         "OTEL_PYTHON_LOG_CORRELATION", "true"
     )
 
 
 def instrument_custom_libs(
     options: HyperDXOptions,
     resource: Resource,
     tracer_provider: TracerProvider,
     meter_provider: MeterProvider,
 ):
-    _instrument_urllib(options, tracer_provider, meter_provider)
-    _instrument_requests(options, tracer_provider, meter_provider)
-    _instrument_flask(options, tracer_provider, meter_provider)
-    _instrument_fastapi(options, tracer_provider, meter_provider)
+    if options.enable_advanced_network_capture:
+        _instrument_urllib(options, tracer_provider, meter_provider)
+        _instrument_requests(options, tracer_provider, meter_provider)
+        _instrument_flask(options, tracer_provider, meter_provider)
+        _instrument_fastapi(options, tracer_provider, meter_provider)
```

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/metrics.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/options.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     OTEL_SERVICE_NAME,
 )
 from grpc import ssl_channel_credentials
 
 # Environment Variable Names
 DEBUG = "DEBUG"
 HYPERDX_ENABLE_LOCAL_VISUALIZATIONS = "HYPERDX_ENABLE_LOCAL_VISUALIZATIONS"
+HYPERDX_ENABLE_ADVANCED_NETWORK_CAPTURE = "HYPERDX_ENABLE_ADVANCED_NETWORK_CAPTURE"
 OTEL_SERVICE_VERSION = "OTEL_SERVICE_VERSION"
 SAMPLE_RATE = "SAMPLE_RATE"
 
 # HNY Credential Names
 HYPERDX_API_ENDPOINT = "HYPERDX_API_ENDPOINT"
 HYPERDX_API_KEY = "HYPERDX_API_KEY"
 HYPERDX_DATASET = "HYPERDX_DATASET"
@@ -48,14 +49,19 @@
     "Unable to parse " + "OTEL_EXPORTER_OTLP_INSECURE. Defaulting to False."
 )
 INVALID_LOCAL_VIS_ERROR = (
     "Unable to parse "
     + "HYPERDX_ENABLE_LOCAL_VISUALIZATIONS environment variable. "
     + "Defaulting to false."
 )
+INVALID_LOCAL_ADVANCED_NETWORK_CAPTURE_ERROR = (
+    "Unable to parse "
+    + "HYPERDX_ENABLE_ADVANCED_NETWORK_CAPTURE environment variable. "
+    + "Defaulting to false."
+)
 INVALID_LOGS_INSECURE_ERROR = (
     "Unable to parse " + "OTEL_EXPORTER_OTLP_LOGS_INSECURE. Defaulting to False."
 )
 INVALID_METRICS_INSECURE_ERROR = (
     "Unable to parse " + "OTEL_EXPORTER_OTLP_METRICS_INSECURE. Defaulting to False."
 )
 INVALID_TRACES_INSECURE_ERROR = (
@@ -239,14 +245,15 @@
     logs_exporter_protocol = DEFAULT_EXPORTER_PROTOCOL
     sample_rate = DEFAULT_SAMPLE_RATE
     debug = False
     log_level = DEFAULT_LOG_LEVEL
     dataset = None
     metrics_dataset = None
     enable_local_visualizations = False
+    enable_advanced_network_capture = False
 
     # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     def __init__(
         self,
         apikey: str = None,
         traces_apikey: str = None,
         metrics_apikey: str = None,
@@ -267,14 +274,15 @@
         dataset: str = None,
         metrics_dataset: str = None,
         enable_local_visualizations: bool = False,
         exporter_protocol: str = EXPORTER_PROTOCOL_HTTP_PROTO,
         traces_exporter_protocol: str = None,
         metrics_exporter_protocol: str = None,
         logs_exporter_protocol: str = None,
+        enable_advanced_network_capture: bool = False,
     ):
         self.debug = parse_bool(DEBUG, (debug or False), INVALID_DEBUG_ERROR)
         if self.debug:
             self.log_level = "DEBUG"
         else:
             log_level = os.environ.get(OTEL_LOG_LEVEL, log_level)
             if log_level and log_level.upper() in log_levels:
@@ -429,14 +437,20 @@
 
         self.enable_local_visualizations = parse_bool(
             HYPERDX_ENABLE_LOCAL_VISUALIZATIONS,
             enable_local_visualizations,
             INVALID_LOCAL_VIS_ERROR,
         )
 
+        self.enable_advanced_network_capture = parse_bool(
+            HYPERDX_ENABLE_ADVANCED_NETWORK_CAPTURE,
+            enable_advanced_network_capture,
+            INVALID_LOCAL_ADVANCED_NETWORK_CAPTURE_ERROR,
+        )
+
     def get_traces_endpoint(self) -> str:
         """
         Returns the OTLP traces endpoint to send spans to.
         """
         return self.traces_endpoint
 
     def get_metrics_endpoint(self) -> str:
```

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/resource.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/sampler.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/src/hyperdx/opentelemetry/trace.py` & `hyperdx_opentelemetry-0.0.4/src/hyperdx/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `hyperdx_opentelemetry-0.0.3/PKG-INFO` & `hyperdx_opentelemetry-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdx-opentelemetry
-Version: 0.0.3
+Version: 0.0.4
 Summary: HyperDX OpenTelemetry Distro for Python
 Author: HyperDX
 Author-email: support@hyperdx.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,16 @@
 
 # HyperDX OpenTelemetry Distro for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/hyperdxio/hyperdx-opentelemetry-python)](https://github.com/hyperdxio/home/blob/main/hyperdx-oss-lifecycle-and-practices.md)
 [![CircleCI](https://circleci.com/gh/hyperdxio/hyperdx-opentelemetry-python.svg?style=shield)](https://circleci.com/gh/hyperdxio/hyperdx-opentelemetry-python)
 [![PyPi](https://img.shields.io/pypi/v/hyperdx-opentelemetry)](https://pypi.org/project/hyperdx-opentelemetry/)
 
+> This project is a fork from https://github.com/honeycombio/honeycomb-opentelemetry-python
+
 **STATUS: this library is BETA.**
 You're welcome to try it, and let us know your feedback in the issues!
 
 This is HyperDX's Distribution of OpenTelemetry for Python.
 It makes getting started with OpenTelemetry and HyperDX easier!
 
 Latest release built with:
```

