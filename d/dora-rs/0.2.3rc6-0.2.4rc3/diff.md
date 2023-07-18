# Comparing `tmp/dora_rs-0.2.3rc6.tar.gz` & `tmp/dora_rs-0.2.4rc3.tar.gz`

## Comparing `dora_rs-0.2.3rc6.tar` & `dora_rs-0.2.4rc3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-download/Cargo.toml
--rw-r--r--   0     1001      123     1285 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-download/src/lib.rs
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      123     3249 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      123     7334 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      123     2010 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/lib.rs
--rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/Cargo.toml
--rw-r--r--   0     1001      123     1620 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/lib.rs
--rw-r--r--   0     1001      123     2248 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/telemetry.rs
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/Cargo.toml
--rw-r--r--   0     1001      123    13111 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/lib.rs
--rw-r--r--   0     1001      123     4296 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/channel.rs
--rw-r--r--   0     1001      123     2461 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/mod.rs
--rw-r--r--   0     1001      123    12448 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/python.rs
--rw-r--r--   0     1001      123     9727 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/shared_lib.rs
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/Cargo.toml
--rw-r--r--   0     1001      123     5862 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/src/lib.rs
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-metrics/Cargo.toml
--rw-r--r--   0     1001      123     1483 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-metrics/src/lib.rs
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/Cargo.toml
--rw-r--r--   0     1001      123     9127 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/config.rs
--rw-r--r--   0     1001      123      957 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/coordinator_messages.rs
--rw-r--r--   0     1001      123     6485 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/daemon_messages.rs
--rw-r--r--   0     1001      123     8967 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/mod.rs
--rw-r--r--   0     1001      123     7313 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/validate.rs
--rw-r--r--   0     1001      123     6705 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      123      974 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/lib.rs
--rw-r--r--   0     1001      123     1970 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-core/src/topics.rs
--rw-r--r--   0        0        0      424 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/Cargo.toml
--rw-r--r--   0     1001      123     2396 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/src/lib.rs
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/Cargo.toml
--rw-r--r--   0     1001      123      360 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/build.rs
--rw-r--r--   0     1001      123      229 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/schema/message.capnp
--rw-r--r--   0     1001      123     3225 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/src/lib.rs
--rw-r--r--   0     1001      123     7447 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-message/src/message_capnp.rs
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/Cargo.toml
--rw-r--r--   0     1001      123     2216 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      123     2082 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      123     2209 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/event.rs
--rw-r--r--   0     1001      123     6484 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/mod.rs
--rw-r--r--   0     1001      123     8588 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/thread.rs
--rw-r--r--   0     1001      123      267 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/lib.rs
--rw-r--r--   0     1001      123     3153 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/control_channel.rs
--rw-r--r--   0     1001      123     5186 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/drop_stream.rs
--rw-r--r--   0     1001      123    10789 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/mod.rs
--rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/Cargo.toml
--rw-r--r--   0     1001      123      204 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/README.md
--rw-r--r--   0     1001      123      372 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/dora/__init__.py
--rw-r--r--   0     1001      123      153 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/pyproject.toml
--rw-r--r--   0     1001      123     2076 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/src/lib.rs
--rw-r--r--   0     1001      123   144347 2023-05-05 02:34:52.000000 dora_rs-0.2.3rc6/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 dora_rs-0.2.3rc6/PKG-INFO
+-rw-r--r--   0        0        0      705 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/Cargo.toml
+-rw-r--r--   0     1001      123     1620 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/lib.rs
+-rw-r--r--   0     1001      123     2248 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/telemetry.rs
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      123     3249 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      123     7334 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      123     2010 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/lib.rs
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/Cargo.toml
+-rw-r--r--   0     1001      123     2429 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      123     2149 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      123     2209 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/event.rs
+-rw-r--r--   0     1001      123     7008 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/mod.rs
+-rw-r--r--   0     1001      123     9248 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/thread.rs
+-rw-r--r--   0     1001      123      673 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/lib.rs
+-rw-r--r--   0     1001      123     3649 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/control_channel.rs
+-rw-r--r--   0     1001      123     5795 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/drop_stream.rs
+-rw-r--r--   0     1001      123    12329 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/mod.rs
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/Cargo.toml
+-rw-r--r--   0     1001      123    13208 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/lib.rs
+-rw-r--r--   0     1001      123     4296 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      123     2568 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      123    12634 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/python.rs
+-rw-r--r--   0     1001      123     9727 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/shared_lib.rs
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-metrics/Cargo.toml
+-rw-r--r--   0     1001      123     1483 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-metrics/src/lib.rs
+-rw-r--r--   0        0        0      409 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/Cargo.toml
+-rw-r--r--   0     1001      123     2396 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/src/lib.rs
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/Cargo.toml
+-rw-r--r--   0     1001      123     5862 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/src/lib.rs
+-rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/Cargo.toml
+-rw-r--r--   0     1001      123     9127 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/config.rs
+-rw-r--r--   0     1001      123      957 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      123     6695 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/daemon_messages.rs
+-rw-r--r--   0     1001      123     8998 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      123     7001 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      123     6705 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      123      974 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/lib.rs
+-rw-r--r--   0     1001      123     2066 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-core/src/topics.rs
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-download/Cargo.toml
+-rw-r--r--   0     1001      123     1285 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-download/src/lib.rs
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/Cargo.toml
+-rw-r--r--   0     1001      123      360 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/build.rs
+-rw-r--r--   0     1001      123      229 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/schema/message.capnp
+-rw-r--r--   0     1001      123     3225 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/src/lib.rs
+-rw-r--r--   0     1001      123     7447 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/local_dependencies/dora-message/src/message_capnp.rs
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/Cargo.toml
+-rw-r--r--   0     1001      123      204 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/README.md
+-rw-r--r--   0     1001      123      518 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/dora/__init__.py
+-rw-r--r--   0     1001      123      153 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/pyproject.toml
+-rw-r--r--   0     1001      123     3399 2023-07-18 10:52:18.000000 dora_rs-0.2.4rc3/src/lib.rs
+-rw-r--r--   0     1001      123   142629 2023-07-18 10:52:39.000000 dora_rs-0.2.4rc3/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 dora_rs-0.2.4rc3/PKG-INFO
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-download/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-download/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-download"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-download/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "shared-memory-server"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/shared-memory-server/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/shared-memory-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-tracing"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-tracing/src/telemetry.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-runtime"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
@@ -31,14 +31,15 @@
 pyo3 = { version = "0.18", features = ["eyre", "abi3-py37"], optional = true }
 tracing = "0.1.36"
 tracing-subscriber = "0.3.15"
 dora-download = { path = "../dora-download" }
 flume = "0.10.14"
 clap = { version = "4.0.3", features = ["derive"] }
 tracing-opentelemetry = { version = "0.18.0", optional = true }
+pythonize = { version = "0.18.0", optional = true }
 
 [features]
 default = ["tracing"]
 tracing = ["dora-tracing"]
 telemetry = ["tracing", "opentelemetry", "tracing-opentelemetry"]
 metrics = ["opentelemetry", "opentelemetry-system-metrics", "dora-metrics"]
-python = ["pyo3", "dora-operator-api-python"]
+python = ["pyo3", "dora-operator-api-python", "pythonize"]
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         node: config,
         operators,
     } = config;
     let node_id = config.node_id.clone();
     #[cfg(feature = "tracing")]
     set_up_tracing(&node_id.to_string()).context("failed to set up tracing subscriber")?;
 
+    let dataflow_descriptor = config.dataflow_descriptor.clone();
+
     let operator_definition = if operators.is_empty() {
         bail!("no operators");
     } else if operators.len() > 1 {
         bail!("multiple operators are not supported");
     } else {
         let mut ops = operators;
         ops.remove(0)
@@ -86,14 +88,15 @@
     let operator_id = operator_definition.id.clone();
     run_operator(
         &node_id,
         operator_definition,
         incoming_events,
         operator_events_tx,
         init_done_tx,
+        &dataflow_descriptor,
     )
     .wrap_err_with(|| format!("failed to run operator {operator_id}"))?;
 
     match main_task.join() {
         Ok(result) => result.wrap_err("main task failed")?,
         Err(panic) => std::panic::resume_unwind(panic),
     }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use dora_core::{
     config::{DataId, NodeId},
-    descriptor::{OperatorDefinition, OperatorSource},
+    descriptor::{Descriptor, OperatorDefinition, OperatorSource},
     message::MetadataParameters,
 };
 use dora_node_api::{DataSample, Event};
 use eyre::{Context, Result};
 use std::any::Any;
 use tokio::sync::{mpsc::Sender, oneshot};
 
@@ -15,14 +15,15 @@
 
 pub fn run_operator(
     node_id: &NodeId,
     operator_definition: OperatorDefinition,
     incoming_events: flume::Receiver<Event>,
     events_tx: Sender<OperatorEvent>,
     init_done: oneshot::Sender<Result<()>>,
+    dataflow_descriptor: &Descriptor,
 ) -> eyre::Result<()> {
     match &operator_definition.config.source {
         OperatorSource::SharedLibrary(source) => {
             shared_lib::run(
                 node_id,
                 &operator_definition.id,
                 source,
@@ -43,14 +44,15 @@
             python::run(
                 node_id,
                 &operator_definition.id,
                 source,
                 events_tx,
                 incoming_events,
                 init_done,
+                dataflow_descriptor,
             )
             .wrap_err_with(|| {
                 format!(
                     "failed to spawn Python operator for {}",
                     operator_definition.id
                 )
             })?;
@@ -63,14 +65,15 @@
             tracing::error!("WASM operators are not supported yet");
         }
     }
     Ok(())
 }
 
 #[derive(Debug)]
+#[allow(dead_code)]
 pub enum OperatorEvent {
     AllocateOutputSample {
         len: usize,
         sample: oneshot::Sender<eyre::Result<DataSample>>,
     },
     Output {
         output_id: DataId,
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/python.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/python.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(clippy::borrow_deref_ref)] // clippy warns about code generated by #[pymethods]
 
 use super::{OperatorEvent, StopReason};
 use dora_core::{
     config::{NodeId, OperatorId},
-    descriptor::source_is_url,
+    descriptor::{source_is_url, Descriptor},
 };
 use dora_download::download_file;
 use dora_node_api::Event;
 use dora_operator_api_python::PyEvent;
 use dora_operator_api_types::DoraStatus;
 use eyre::{bail, eyre, Context, Result};
 use pyo3::{
@@ -35,14 +35,15 @@
 pub fn run(
     node_id: &NodeId,
     operator_id: &OperatorId,
     source: &str,
     events_tx: Sender<OperatorEvent>,
     incoming_events: flume::Receiver<Event>,
     init_done: oneshot::Sender<Result<()>>,
+    dataflow_descriptor: &Descriptor,
 ) -> eyre::Result<()> {
     let path = if source_is_url(source) {
         let target_path = Path::new("build")
             .join(node_id.to_string())
             .join(format!("{}.py", operator_id));
         // try to download the shared library
         let rt = tokio::runtime::Builder::new_current_thread()
@@ -94,14 +95,19 @@
             .getattr("Operator")
             .wrap_err("no `Operator` class found in module")?;
 
         let locals = [("Operator", operator_class)].into_py_dict(py);
         let operator = py
             .eval("Operator()", None, Some(locals))
             .map_err(traceback)?;
+        operator.setattr(
+            "dataflow_descriptor",
+            pythonize::pythonize(py, dataflow_descriptor)?,
+        )?;
+
         Result::<_, eyre::Report>::Ok(Py::from(operator))
     };
 
     let python_runner = move || {
         let mut operator =
             match Python::with_gil(init_operator).wrap_err("failed to init python operator") {
                 Ok(op) => {
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-runtime/src/operator/shared_lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-operator-api-python"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-python/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-metrics/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-metrics/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-metrics"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-metrics/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-metrics/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-core"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/config.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/coordinator_messages.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/coordinator_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/daemon_messages.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/daemon_messages.rs`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,27 @@
     collections::{BTreeMap, BTreeSet},
     fmt,
     net::SocketAddr,
     path::PathBuf,
 };
 
 use crate::{
-    config::{CommunicationConfig, DataId, NodeId, NodeRunConfig, OperatorId},
-    descriptor::{OperatorDefinition, ResolvedNode},
+    config::{DataId, NodeId, NodeRunConfig, OperatorId},
+    descriptor::{Descriptor, OperatorDefinition, ResolvedNode},
 };
-use dora_message::Metadata;
+use dora_message::{uhlc, Metadata};
 use uuid::Uuid;
 
 #[derive(Debug, serde::Serialize, serde::Deserialize)]
 pub struct NodeConfig {
     pub dataflow_id: DataflowId,
     pub node_id: NodeId,
     pub run_config: NodeRunConfig,
     pub daemon_communication: DaemonCommunication,
+    pub dataflow_descriptor: Descriptor,
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 pub enum DaemonCommunication {
     Shmem {
         daemon_control_region_id: SharedMemoryId,
         daemon_drop_region_id: SharedMemoryId,
@@ -127,20 +128,26 @@
 type SharedMemoryId = String;
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 #[must_use]
 pub enum DaemonReply {
     Result(Result<(), String>),
     PreparedMessage { shared_memory_id: SharedMemoryId },
-    NextEvents(Vec<NodeEvent>),
-    NextDropEvents(Vec<NodeDropEvent>),
+    NextEvents(Vec<Timestamped<NodeEvent>>),
+    NextDropEvents(Vec<Timestamped<NodeDropEvent>>),
     Empty,
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
+pub struct Timestamped<T> {
+    pub inner: T,
+    pub timestamp: uhlc::Timestamp,
+}
+
+#[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
 pub enum NodeEvent {
     Stop,
     Reload {
         operator_id: Option<OperatorId>,
     },
     Input {
         id: DataId,
@@ -246,10 +253,10 @@
 pub type DataflowId = Uuid;
 
 #[derive(Debug, serde::Deserialize, serde::Serialize)]
 pub struct SpawnDataflowNodes {
     pub dataflow_id: DataflowId,
     pub working_dir: PathBuf,
     pub nodes: Vec<ResolvedNode>,
-    pub communication: CommunicationConfig,
     pub machine_listen_ports: BTreeMap<String, SocketAddr>,
+    pub dataflow_descriptor: Descriptor,
 }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -236,28 +236,28 @@
 
 pub fn source_is_url(source: &str) -> bool {
     source.contains("://")
 }
 
 pub fn resolve_path(source: &str, working_dir: &Path) -> Result<PathBuf> {
     let path = Path::new(&source);
-    if path.extension().is_none() {
+    let path = if path.extension().is_none() {
         path.with_extension(EXE_EXTENSION)
     } else {
         path.to_owned()
     };
 
     // Search path within current working directory
-    if let Ok(abs_path) = working_dir.join(path).canonicalize() {
+    if let Ok(abs_path) = working_dir.join(&path).canonicalize() {
         Ok(abs_path)
     // Search path within $PATH
-    } else if let Ok(abs_path) = which::which(path) {
+    } else if let Ok(abs_path) = which::which(&path) {
         Ok(abs_path)
     } else {
-        bail!("Could not find source path.")
+        bail!("Could not find source path {}", path.display())
     }
 }
 
 #[derive(Debug, Serialize, Deserialize, Clone)]
 #[serde(deny_unknown_fields)]
 pub struct PythonOperatorConfig {
     pub path: PathBuf,
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/validate.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/validate.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 use crate::{
     adjust_shared_library_path,
     config::{DataId, Input, InputMapping, OperatorId, UserInputMapping},
     descriptor::{self, source_is_url, CoreNodeKind, OperatorSource},
 };
 
 use eyre::{bail, eyre, Context};
-use std::{env::consts::EXE_EXTENSION, path::Path, process::Command};
+use std::{path::Path, process::Command};
 use tracing::info;
 
-use super::{Descriptor, SHELL_SOURCE};
+use super::{resolve_path, Descriptor, SHELL_SOURCE};
 const VERSION: &str = env!("CARGO_PKG_VERSION");
 
 pub fn check_dataflow(dataflow: &Descriptor, working_dir: &Path) -> eyre::Result<()> {
     if dataflow.daemon_config.is_some() {
         tracing::warn!("ignoring deprecated `daemon_config` key in dataflow config");
     }
     if dataflow.communication.zenoh.is_some() {
@@ -27,24 +27,16 @@
         match &node.kind {
             descriptor::CoreNodeKind::Custom(node) => match node.source.as_str() {
                 SHELL_SOURCE => (),
                 source => {
                     if source_is_url(source) {
                         info!("{source} is a URL."); // TODO: Implement url check.
                     } else {
-                        let raw = Path::new(source);
-                        let path = if raw.extension().is_none() {
-                            raw.with_extension(EXE_EXTENSION)
-                        } else {
-                            raw.to_owned()
-                        };
-                        working_dir
-                            .join(&path)
-                            .canonicalize()
-                            .wrap_err_with(|| format!("no node exists at `{}`", path.display()))?;
+                        resolve_path(source, working_dir)
+                            .wrap_err_with(|| format!("Could not find source path `{}`", source))?;
                     };
                 }
             },
             descriptor::CoreNodeKind::Runtime(node) => {
                 for operator_definition in &node.operators {
                     match &operator_definition.config.source {
                         OperatorSource::SharedLibrary(path) => {
@@ -162,15 +154,15 @@
         format!("Please reinstall it with: `pip install dora-rs=={VERSION} --force`");
     let mut command = Command::new("python3");
     command.args([
         "-c",
         &format!(
             "
 import dora;
-assert dora.__version__=='{VERSION}',  'Python dora-rs should be {VERSION}. {reinstall_command}'
+assert dora.__version__=='{VERSION}',  'Python dora-rs should be {VERSION}, but current version is %s. {reinstall_command}' % (dora.__version__)
         "
         ),
     ]);
     let mut result = command
         .spawn()
         .wrap_err("Could not spawn python dora-rs command.")?;
     let status = result
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/descriptor/visualize.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-core/src/topics.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-core/src/topics.rs`

 * *Files 5% similar despite different names*

```diff
@@ -49,22 +49,32 @@
     },
     Destroy,
     List,
     DaemonConnected,
     ConnectedMachines,
 }
 
-#[derive(Debug, serde::Deserialize, serde::Serialize)]
+#[derive(Debug, Clone, serde::Deserialize, serde::Serialize)]
 pub enum ControlRequestReply {
     Error(String),
     CoordinatorStopped,
-    DataflowStarted { uuid: Uuid },
-    DataflowReloaded { uuid: Uuid },
-    DataflowStopped { uuid: Uuid },
-    DataflowList { dataflows: Vec<DataflowId> },
+    DataflowStarted {
+        uuid: Uuid,
+    },
+    DataflowReloaded {
+        uuid: Uuid,
+    },
+    DataflowStopped {
+        uuid: Uuid,
+        result: Result<(), String>,
+    },
+
+    DataflowList {
+        dataflows: Vec<DataflowId>,
+    },
     DestroyOk,
     DaemonConnected(bool),
     ConnectedMachines(BTreeSet<String>),
     Logs(Vec<u8>),
 }
 
 #[derive(Debug, Clone, serde::Serialize, serde::Deserialize)]
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-operator-api-types/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-operator-api-types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-message/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-message"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # Building capnp schema script is disabled by default as it requires to install capnp.
 # To change the schema install capnp at: https://capnproto.org/install.html
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-message/src/lib.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-message/src/message_capnp.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-message/src/message_capnp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/Cargo.toml` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dora-node-api"
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 [features]
 default = ["tracing"]
@@ -23,7 +23,8 @@
 flume = "0.10.14"
 uuid = { version = "1.1.2", features = ["v4"] }
 capnp = "0.14.11"
 bincode = "1.3.3"
 shared_memory = "0.12.0"
 dora-tracing = { optional = true , path = "../dora-tracing" }
 arrow = "35.0.0"
+futures = "0.3.28"
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 use dora_core::{
     config::NodeId,
-    daemon_messages::{DaemonReply, DaemonRequest, DataflowId},
+    daemon_messages::{DaemonReply, DaemonRequest, DataflowId, Timestamped},
+    message::uhlc::Timestamp,
 };
 use eyre::{bail, eyre, Context};
 use shared_memory_server::{ShmemClient, ShmemConf};
 use std::{
     net::{SocketAddr, TcpStream},
     time::Duration,
 };
 
 mod tcp;
 
 pub enum DaemonChannel {
-    Shmem(ShmemClient<DaemonRequest, DaemonReply>),
+    Shmem(ShmemClient<Timestamped<DaemonRequest>, DaemonReply>),
     Tcp(TcpStream),
 }
 
 impl DaemonChannel {
     #[tracing::instrument(level = "trace")]
     pub fn new_tcp(socket_addr: SocketAddr) -> eyre::Result<Self> {
         let stream = TcpStream::connect(socket_addr).wrap_err("failed to open TCP connection")?;
@@ -33,33 +34,41 @@
         let channel = DaemonChannel::Shmem(
             unsafe { ShmemClient::new(daemon_events_region, Some(Duration::from_secs(5))) }
                 .wrap_err("failed to create ShmemChannel")?,
         );
         Ok(channel)
     }
 
-    pub fn register(&mut self, dataflow_id: DataflowId, node_id: NodeId) -> eyre::Result<()> {
-        let msg = DaemonRequest::Register {
-            dataflow_id,
-            node_id,
-            dora_version: env!("CARGO_PKG_VERSION").to_owned(),
+    pub fn register(
+        &mut self,
+        dataflow_id: DataflowId,
+        node_id: NodeId,
+        timestamp: Timestamp,
+    ) -> eyre::Result<()> {
+        let msg = Timestamped {
+            inner: DaemonRequest::Register {
+                dataflow_id,
+                node_id,
+                dora_version: env!("CARGO_PKG_VERSION").to_owned(),
+            },
+            timestamp,
         };
         let reply = self
             .request(&msg)
             .wrap_err("failed to send register request to dora-daemon")?;
 
         match reply {
             dora_core::daemon_messages::DaemonReply::Result(result) => result
                 .map_err(|e| eyre!(e))
                 .wrap_err("failed to register node with dora-daemon")?,
             other => bail!("unexpected register reply: {other:?}"),
         }
         Ok(())
     }
 
-    pub fn request(&mut self, request: &DaemonRequest) -> eyre::Result<DaemonReply> {
+    pub fn request(&mut self, request: &Timestamped<DaemonRequest>) -> eyre::Result<DaemonReply> {
         match self {
             DaemonChannel::Shmem(client) => client.request(request),
             DaemonChannel::Tcp(stream) => tcp::request(stream, request),
         }
     }
 }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/daemon_connection/tcp.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-use dora_core::daemon_messages::{DaemonReply, DaemonRequest};
+use dora_core::daemon_messages::{DaemonReply, DaemonRequest, Timestamped};
 use eyre::{eyre, Context};
 use std::{
     io::{Read, Write},
     net::TcpStream,
 };
 
-pub fn request(connection: &mut TcpStream, request: &DaemonRequest) -> eyre::Result<DaemonReply> {
+pub fn request(
+    connection: &mut TcpStream,
+    request: &Timestamped<DaemonRequest>,
+) -> eyre::Result<DaemonReply> {
     send_message(connection, request)?;
-    if request.expects_tcp_reply() {
+    if request.inner.expects_tcp_reply() {
         receive_reply(connection)
             .and_then(|reply| reply.ok_or_else(|| eyre!("server disconnected unexpectedly")))
     } else {
         Ok(DaemonReply::Empty)
     }
 }
 
-fn send_message(connection: &mut TcpStream, message: &DaemonRequest) -> eyre::Result<()> {
+fn send_message(
+    connection: &mut TcpStream,
+    message: &Timestamped<DaemonRequest>,
+) -> eyre::Result<()> {
     let serialized = bincode::serialize(&message).wrap_err("failed to serialize DaemonRequest")?;
     tcp_send(connection, &serialized).wrap_err("failed to send DaemonRequest")?;
     Ok(())
 }
 
 fn receive_reply(connection: &mut TcpStream) -> eyre::Result<Option<DaemonReply>> {
     let raw = match tcp_receive(connection) {
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/event.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/mod.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+use std::sync::Arc;
+
 pub use event::{Data, Event, MappedInputData};
+use futures::{Stream, StreamExt};
 
 use self::thread::{EventItem, EventStreamThreadHandle};
 use crate::daemon_connection::DaemonChannel;
 use dora_core::{
     config::NodeId,
-    daemon_messages::{self, DaemonCommunication, DaemonRequest, DataflowId, NodeEvent},
+    daemon_messages::{
+        self, DaemonCommunication, DaemonRequest, DataflowId, NodeEvent, Timestamped,
+    },
+    message::uhlc,
 };
 use eyre::{eyre, Context};
 
 mod event;
 mod thread;
 
 pub struct EventStream {
     node_id: NodeId,
-    receiver: flume::Receiver<EventItem>,
+    receiver: flume::r#async::RecvStream<'static, EventItem>,
     _thread_handle: EventStreamThreadHandle,
     close_channel: DaemonChannel,
+    clock: Arc<uhlc::HLC>,
 }
 
 impl EventStream {
-    #[tracing::instrument(level = "trace")]
+    #[tracing::instrument(level = "trace", skip(clock))]
     pub(crate) fn init(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         daemon_communication: &DaemonCommunication,
+        clock: Arc<uhlc::HLC>,
     ) -> eyre::Result<Self> {
         let channel = match daemon_communication {
             DaemonCommunication::Shmem {
                 daemon_events_region_id,
                 ..
             } => unsafe { DaemonChannel::new_shmem(daemon_events_region_id) }.wrap_err_with(
                 || format!("failed to create shmem event stream for node `{node_id}`"),
@@ -45,70 +53,66 @@
             )?,
             DaemonCommunication::Tcp { socket_addr } => DaemonChannel::new_tcp(*socket_addr)
                 .wrap_err_with(|| {
                     format!("failed to connect event close channel for node `{node_id}`")
                 })?,
         };
 
-        Self::init_on_channel(dataflow_id, node_id, channel, close_channel)
+        Self::init_on_channel(dataflow_id, node_id, channel, close_channel, clock)
     }
 
     pub(crate) fn init_on_channel(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         mut channel: DaemonChannel,
         mut close_channel: DaemonChannel,
+        clock: Arc<uhlc::HLC>,
     ) -> eyre::Result<Self> {
-        channel.register(dataflow_id, node_id.clone())?;
+        channel.register(dataflow_id, node_id.clone(), clock.new_timestamp())?;
         let reply = channel
-            .request(&DaemonRequest::Subscribe)
+            .request(&Timestamped {
+                inner: DaemonRequest::Subscribe,
+                timestamp: clock.new_timestamp(),
+            })
             .map_err(|e| eyre!(e))
             .wrap_err("failed to create subscription with dora-daemon")?;
 
         match reply {
             daemon_messages::DaemonReply::Result(Ok(())) => {}
             daemon_messages::DaemonReply::Result(Err(err)) => {
                 eyre::bail!("subscribe failed: {err}")
             }
             other => eyre::bail!("unexpected subscribe reply: {other:?}"),
         }
 
-        close_channel.register(dataflow_id, node_id.clone())?;
+        close_channel.register(dataflow_id, node_id.clone(), clock.new_timestamp())?;
 
         let (tx, rx) = flume::bounded(0);
-        let thread_handle = thread::init(node_id.clone(), tx, channel)?;
+        let thread_handle = thread::init(node_id.clone(), tx, channel, clock.clone())?;
 
         Ok(EventStream {
             node_id: node_id.clone(),
-            receiver: rx,
+            receiver: rx.into_stream(),
             _thread_handle: thread_handle,
             close_channel,
+            clock,
         })
     }
 
+    /// wait for the next event on the events stream.
     pub fn recv(&mut self) -> Option<Event> {
-        let event = self.receiver.recv();
-        self.recv_common(event)
+        futures::executor::block_on(self.recv_async())
     }
 
     pub async fn recv_async(&mut self) -> Option<Event> {
-        let event = self.receiver.recv_async().await;
-        self.recv_common(event)
+        self.receiver.next().await.map(Self::convert_event_item)
     }
 
-    #[tracing::instrument(skip(self), fields(%self.node_id))]
-    fn recv_common(&mut self, event: Result<EventItem, flume::RecvError>) -> Option<Event> {
-        let event = match event {
-            Ok(event) => event,
-            Err(flume::RecvError::Disconnected) => {
-                tracing::trace!("event channel disconnected");
-                return None;
-            }
-        };
-        let event = match event {
+    fn convert_event_item(item: EventItem) -> Event {
+        match item {
             EventItem::NodeEvent { event, ack_channel } => match event {
                 NodeEvent::Stop => Event::Stop,
                 NodeEvent::Reload { operator_id } => Event::Reload { operator_id },
                 NodeEvent::InputClosed { id } => Event::InputClosed { id },
                 NodeEvent::Input { id, metadata, data } => {
                     let data = match data {
                         None => Ok(None),
@@ -135,29 +139,45 @@
                     let err = eyre!(
                         "received `AllInputsClosed` event, which should be handled by background task"
                     );
                     tracing::error!("{err:?}");
                     Event::Error(err.wrap_err("internal error").to_string())
                 }
             },
+
             EventItem::FatalError(err) => {
                 Event::Error(format!("fatal event stream error: {err:?}"))
             }
-        };
+        }
+    }
+}
 
-        Some(event)
+impl Stream for EventStream {
+    type Item = Event;
+
+    fn poll_next(
+        mut self: std::pin::Pin<&mut Self>,
+        cx: &mut std::task::Context<'_>,
+    ) -> std::task::Poll<Option<Self::Item>> {
+        self.receiver
+            .poll_next_unpin(cx)
+            .map(|item| item.map(Self::convert_event_item))
     }
 }
 
 impl Drop for EventStream {
     #[tracing::instrument(skip(self), fields(%self.node_id))]
     fn drop(&mut self) {
+        let request = Timestamped {
+            inner: DaemonRequest::EventStreamDropped,
+            timestamp: self.clock.new_timestamp(),
+        };
         let result = self
             .close_channel
-            .request(&DaemonRequest::EventStreamDropped)
+            .request(&request)
             .map_err(|e| eyre!(e))
             .wrap_err("failed to signal event stream closure to dora-daemon")
             .and_then(|r| match r {
                 daemon_messages::DaemonReply::Result(Ok(())) => Ok(()),
                 daemon_messages::DaemonReply::Result(Err(err)) => {
                     Err(eyre!("EventStreamClosed failed: {err}"))
                 }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/event_stream/thread.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/event_stream/thread.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 use dora_core::{
     config::NodeId,
-    daemon_messages::{DaemonReply, DaemonRequest, DropToken, NodeEvent},
+    daemon_messages::{DaemonReply, DaemonRequest, DropToken, NodeEvent, Timestamped},
+    message::uhlc::{self, Timestamp},
 };
 use eyre::{eyre, Context};
 use flume::RecvTimeoutError;
-use std::time::{Duration, Instant};
+use std::{
+    sync::Arc,
+    time::{Duration, Instant},
+};
 
 use crate::daemon_connection::DaemonChannel;
 
 pub fn init(
     node_id: NodeId,
     tx: flume::Sender<EventItem>,
     channel: DaemonChannel,
+    clock: Arc<uhlc::HLC>,
 ) -> eyre::Result<EventStreamThreadHandle> {
     let node_id_cloned = node_id.clone();
-    let join_handle = std::thread::spawn(|| event_stream_loop(node_id_cloned, tx, channel));
+    let join_handle = std::thread::spawn(|| event_stream_loop(node_id_cloned, tx, channel, clock));
     Ok(EventStreamThreadHandle::new(node_id, join_handle))
 }
 
 #[derive(Debug)]
 pub enum EventItem {
     NodeEvent {
         event: NodeEvent,
@@ -64,47 +69,61 @@
             Err(RecvTimeoutError::Disconnected) => {
                 tracing::warn!("event stream thread result channel closed unexpectedly");
             }
         }
     }
 }
 
-#[tracing::instrument(skip(tx, channel))]
-fn event_stream_loop(node_id: NodeId, tx: flume::Sender<EventItem>, mut channel: DaemonChannel) {
+#[tracing::instrument(skip(tx, channel, clock))]
+fn event_stream_loop(
+    node_id: NodeId,
+    tx: flume::Sender<EventItem>,
+    mut channel: DaemonChannel,
+    clock: Arc<uhlc::HLC>,
+) {
     let mut tx = Some(tx);
     let mut pending_drop_tokens: Vec<(DropToken, flume::Receiver<()>, Instant, u64)> = Vec::new();
     let mut drop_tokens = Vec::new();
 
     let result = 'outer: loop {
         if let Err(err) = handle_pending_drop_tokens(&mut pending_drop_tokens, &mut drop_tokens) {
             break 'outer Err(err);
         }
 
-        let daemon_request = DaemonRequest::NextEvent {
-            drop_tokens: std::mem::take(&mut drop_tokens),
+        let daemon_request = Timestamped {
+            inner: DaemonRequest::NextEvent {
+                drop_tokens: std::mem::take(&mut drop_tokens),
+            },
+            timestamp: clock.new_timestamp(),
         };
         let events = match channel.request(&daemon_request) {
-            Ok(DaemonReply::NextEvents(events)) if events.is_empty() => {
-                tracing::trace!("event stream closed for node `{node_id}`");
-                break Ok(());
+            Ok(DaemonReply::NextEvents(events)) => {
+                if events.is_empty() {
+                    tracing::trace!("event stream closed for node `{node_id}`");
+                    break Ok(());
+                } else {
+                    events
+                }
             }
-            Ok(DaemonReply::NextEvents(events)) => events,
             Ok(other) => {
                 let err = eyre!("unexpected control reply: {other:?}");
                 tracing::warn!("{err:?}");
                 continue;
             }
             Err(err) => {
                 let err = eyre!(err).wrap_err("failed to receive incoming event");
                 tracing::warn!("{err:?}");
                 continue;
             }
         };
-        for event in events {
-            let drop_token = match &event {
+        for Timestamped { inner, timestamp } in events {
+            if let Err(err) = clock.update_with_timestamp(&timestamp) {
+                tracing::warn!("failed to update HLC: {err}");
+            }
+            let drop_token = match &inner {
                 NodeEvent::Input {
                     data: Some(data), ..
                 } => data.drop_token(),
                 NodeEvent::AllInputsClosed => {
                     // close the event stream
                     tx = None;
                     // skip this internal event
@@ -112,15 +131,15 @@
                 }
                 _ => None,
             };
 
             if let Some(tx) = tx.as_ref() {
                 let (drop_tx, drop_rx) = flume::bounded(0);
                 match tx.send(EventItem::NodeEvent {
-                    event,
+                    event: inner,
                     ack_channel: drop_tx,
                 }) {
                     Ok(()) => {}
                     Err(send_error) => {
                         let event = send_error.into_inner();
                         tracing::trace!(
                             "event channel was closed already, could not forward `{event:?}`"
@@ -130,15 +149,15 @@
                     }
                 }
 
                 if let Some(token) = drop_token {
                     pending_drop_tokens.push((token, drop_rx, Instant::now(), 1));
                 }
             } else {
-                tracing::warn!("dropping event because event `tx` was already closed: `{event:?}`");
+                tracing::warn!("dropping event because event `tx` was already closed: `{inner:?}`");
             }
         }
     };
     if let Err(err) = result {
         if let Some(tx) = tx.as_ref() {
             if let Err(flume::SendError(item)) = tx.send(EventItem::FatalError(err)) {
                 let err = match item {
@@ -148,16 +167,21 @@
                 tracing::error!("failed to report fatal EventStream error: {err:?}");
             }
         } else {
             tracing::error!("received error event after `tx` was closed: {err:?}");
         }
     }
 
-    if let Err(err) = report_remaining_drop_tokens(channel, drop_tokens, pending_drop_tokens)
-        .context("failed to report remaining drop tokens")
+    if let Err(err) = report_remaining_drop_tokens(
+        channel,
+        drop_tokens,
+        pending_drop_tokens,
+        clock.new_timestamp(),
+    )
+    .context("failed to report remaining drop tokens")
     {
         tracing::warn!("{err:?}");
     }
 }
 
 fn handle_pending_drop_tokens(
     pending_drop_tokens: &mut Vec<(DropToken, flume::Receiver<()>, Instant, u64)>,
@@ -184,17 +208,18 @@
     Ok(())
 }
 
 fn report_remaining_drop_tokens(
     mut channel: DaemonChannel,
     mut drop_tokens: Vec<DropToken>,
     mut pending_drop_tokens: Vec<(DropToken, flume::Receiver<()>, Instant, u64)>,
+    timestamp: Timestamp,
 ) -> eyre::Result<()> {
     while !(pending_drop_tokens.is_empty() && drop_tokens.is_empty()) {
-        report_drop_tokens(&mut drop_tokens, &mut channel)?;
+        report_drop_tokens(&mut drop_tokens, &mut channel, timestamp)?;
 
         let mut still_pending = Vec::new();
         for (token, rx, since, _) in pending_drop_tokens.drain(..) {
             match rx.recv_timeout(Duration::from_millis(100)) {
                 Ok(()) => return Err(eyre!("Node API should not send anything on ACK channel")),
                 Err(flume::RecvTimeoutError::Disconnected) => {
                     // the event was dropped -> add the drop token to the list
@@ -221,19 +246,23 @@
 
     Ok(())
 }
 
 fn report_drop_tokens(
     drop_tokens: &mut Vec<DropToken>,
     channel: &mut DaemonChannel,
+    timestamp: Timestamp,
 ) -> Result<(), eyre::ErrReport> {
     if drop_tokens.is_empty() {
         return Ok(());
     }
-    let daemon_request = DaemonRequest::ReportDropTokens {
-        drop_tokens: std::mem::take(drop_tokens),
+    let daemon_request = Timestamped {
+        inner: DaemonRequest::ReportDropTokens {
+            drop_tokens: std::mem::take(drop_tokens),
+        },
+        timestamp,
     };
     match channel.request(&daemon_request)? {
         dora_core::daemon_messages::DaemonReply::Empty => Ok(()),
         other => Err(eyre!("unexpected ReportDropTokens reply: {other:?}")),
     }
 }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/control_channel.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/control_channel.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,79 @@
+use std::sync::Arc;
+
 use crate::daemon_connection::DaemonChannel;
 use dora_core::{
     config::{DataId, NodeId},
-    daemon_messages::{DaemonCommunication, DaemonRequest, Data, DataflowId},
-    message::Metadata,
+    daemon_messages::{DaemonCommunication, DaemonRequest, Data, DataflowId, Timestamped},
+    message::{uhlc::HLC, Metadata},
 };
 use eyre::{bail, eyre, Context};
 
 pub(crate) struct ControlChannel {
     channel: DaemonChannel,
+    clock: Arc<HLC>,
 }
 
 impl ControlChannel {
-    #[tracing::instrument(level = "trace")]
+    #[tracing::instrument(level = "trace", skip(clock))]
     pub(crate) fn init(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         daemon_communication: &DaemonCommunication,
+        clock: Arc<HLC>,
     ) -> eyre::Result<Self> {
         let channel = match daemon_communication {
             DaemonCommunication::Shmem {
                 daemon_control_region_id,
                 ..
             } => unsafe { DaemonChannel::new_shmem(daemon_control_region_id) }
                 .wrap_err("failed to create shmem control channel")?,
             DaemonCommunication::Tcp { socket_addr } => DaemonChannel::new_tcp(*socket_addr)
                 .wrap_err("failed to connect control channel")?,
         };
 
-        Self::init_on_channel(dataflow_id, node_id, channel)
+        Self::init_on_channel(dataflow_id, node_id, channel, clock)
     }
 
-    #[tracing::instrument(skip(channel), level = "trace")]
+    #[tracing::instrument(skip(channel, clock), level = "trace")]
     pub fn init_on_channel(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         mut channel: DaemonChannel,
+        clock: Arc<HLC>,
     ) -> eyre::Result<Self> {
-        channel.register(dataflow_id, node_id.clone())?;
+        channel.register(dataflow_id, node_id.clone(), clock.new_timestamp())?;
 
-        Ok(Self { channel })
+        Ok(Self { channel, clock })
     }
 
     pub fn report_outputs_done(&mut self) -> eyre::Result<()> {
         let reply = self
             .channel
-            .request(&DaemonRequest::OutputsDone)
+            .request(&Timestamped {
+                inner: DaemonRequest::OutputsDone,
+                timestamp: self.clock.new_timestamp(),
+            })
             .wrap_err("failed to report outputs done to dora-daemon")?;
         match reply {
             dora_core::daemon_messages::DaemonReply::Result(result) => result
                 .map_err(|e| eyre!(e))
                 .wrap_err("failed to report outputs done event to dora-daemon")?,
             other => bail!("unexpected outputs done reply: {other:?}"),
         }
         Ok(())
     }
 
     pub fn report_closed_outputs(&mut self, outputs: Vec<DataId>) -> eyre::Result<()> {
         let reply = self
             .channel
-            .request(&DaemonRequest::CloseOutputs(outputs))
+            .request(&Timestamped {
+                inner: DaemonRequest::CloseOutputs(outputs),
+                timestamp: self.clock.new_timestamp(),
+            })
             .wrap_err("failed to report closed outputs to dora-daemon")?;
         match reply {
             dora_core::daemon_messages::DaemonReply::Result(result) => result
                 .map_err(|e| eyre!(e))
                 .wrap_err("failed to receive closed outputs reply from dora-daemon")?,
             other => bail!("unexpected closed outputs reply: {other:?}"),
         }
@@ -78,15 +89,18 @@
         let request = DaemonRequest::SendMessage {
             output_id,
             metadata,
             data,
         };
         let reply = self
             .channel
-            .request(&request)
+            .request(&Timestamped {
+                inner: request,
+                timestamp: self.clock.new_timestamp(),
+            })
             .wrap_err("failed to send SendMessage request to dora-daemon")?;
         match reply {
             dora_core::daemon_messages::DaemonReply::Empty => Ok(()),
             other => bail!("unexpected SendMessage reply: {other:?}"),
         }
     }
 }
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/drop_stream.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/drop_stream.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-use std::time::Duration;
+use std::{sync::Arc, time::Duration};
 
 use crate::daemon_connection::DaemonChannel;
 use dora_core::{
     config::NodeId,
     daemon_messages::{
-        self, DaemonCommunication, DaemonReply, DaemonRequest, DataflowId, DropToken, NodeDropEvent,
+        self, DaemonCommunication, DaemonReply, DaemonRequest, DataflowId, DropToken,
+        NodeDropEvent, Timestamped,
     },
+    message::uhlc,
 };
 use eyre::{eyre, Context};
 use flume::RecvTimeoutError;
 
 pub struct DropStream {
     receiver: flume::Receiver<DropToken>,
     _thread_handle: DropStreamThreadHandle,
 }
 
 impl DropStream {
-    #[tracing::instrument(level = "trace")]
+    #[tracing::instrument(level = "trace", skip(hlc))]
     pub(crate) fn init(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         daemon_communication: &DaemonCommunication,
+        hlc: Arc<uhlc::HLC>,
     ) -> eyre::Result<Self> {
         let channel = match daemon_communication {
             DaemonCommunication::Shmem {
                 daemon_drop_region_id,
                 ..
             } => {
                 unsafe { DaemonChannel::new_shmem(daemon_drop_region_id) }.wrap_err_with(|| {
                     format!("failed to create shmem drop stream for node `{node_id}`")
                 })?
             }
             DaemonCommunication::Tcp { socket_addr } => DaemonChannel::new_tcp(*socket_addr)
                 .wrap_err_with(|| format!("failed to connect drop stream for node `{node_id}`"))?,
         };
 
-        Self::init_on_channel(dataflow_id, node_id, channel)
+        Self::init_on_channel(dataflow_id, node_id, channel, hlc)
     }
 
     pub fn init_on_channel(
         dataflow_id: DataflowId,
         node_id: &NodeId,
         mut channel: DaemonChannel,
+        clock: Arc<uhlc::HLC>,
     ) -> eyre::Result<Self> {
-        channel.register(dataflow_id, node_id.clone())?;
+        channel.register(dataflow_id, node_id.clone(), clock.new_timestamp())?;
 
         let reply = channel
-            .request(&DaemonRequest::SubscribeDrop)
+            .request(&Timestamped {
+                inner: DaemonRequest::SubscribeDrop,
+                timestamp: clock.new_timestamp(),
+            })
             .map_err(|e| eyre!(e))
             .wrap_err("failed to create subscription with dora-daemon")?;
 
         match reply {
             daemon_messages::DaemonReply::Result(Ok(())) => {}
             daemon_messages::DaemonReply::Result(Err(err)) => {
                 eyre::bail!("drop subscribe failed: {err}")
             }
             other => eyre::bail!("unexpected drop subscribe reply: {other:?}"),
         }
 
         let (tx, rx) = flume::bounded(0);
         let node_id_cloned = node_id.clone();
 
-        let handle = std::thread::spawn(|| drop_stream_loop(node_id_cloned, tx, channel));
+        let handle = std::thread::spawn(|| drop_stream_loop(node_id_cloned, tx, channel, clock));
 
         Ok(Self {
             receiver: rx,
             _thread_handle: DropStreamThreadHandle::new(node_id.clone(), handle),
         })
     }
 }
@@ -74,37 +81,51 @@
     type Target = flume::Receiver<DropToken>;
 
     fn deref(&self) -> &Self::Target {
         &self.receiver
     }
 }
 
-#[tracing::instrument(skip(tx, channel))]
-fn drop_stream_loop(node_id: NodeId, tx: flume::Sender<DropToken>, mut channel: DaemonChannel) {
+#[tracing::instrument(skip(tx, channel, clock))]
+fn drop_stream_loop(
+    node_id: NodeId,
+    tx: flume::Sender<DropToken>,
+    mut channel: DaemonChannel,
+    clock: Arc<uhlc::HLC>,
+) {
     'outer: loop {
-        let daemon_request = DaemonRequest::NextFinishedDropTokens;
+        let daemon_request = Timestamped {
+            inner: DaemonRequest::NextFinishedDropTokens,
+            timestamp: clock.new_timestamp(),
+        };
         let events = match channel.request(&daemon_request) {
-            Ok(DaemonReply::NextDropEvents(events)) if events.is_empty() => {
-                tracing::trace!("drop stream closed for node `{node_id}`");
-                break;
+            Ok(DaemonReply::NextDropEvents(events)) => {
+                if events.is_empty() {
+                    tracing::trace!("drop stream closed for node `{node_id}`");
+                    break;
+                } else {
+                    events
+                }
             }
-            Ok(DaemonReply::NextDropEvents(events)) => events,
             Ok(other) => {
                 let err = eyre!("unexpected drop reply: {other:?}");
                 tracing::warn!("{err:?}");
                 continue;
             }
             Err(err) => {
                 let err = eyre!(err).wrap_err("failed to receive incoming drop event");
                 tracing::warn!("{err:?}");
                 continue;
             }
         };
-        for event in events {
-            match event {
+        for Timestamped { inner, timestamp } in events {
+            if let Err(err) = clock.update_with_timestamp(&timestamp) {
+                tracing::warn!("failed to update HLC: {err}");
+            }
+            match inner {
                 NodeDropEvent::OutputDropped { drop_token } => {
                     if tx.send(drop_token).is_err() {
                         tracing::warn!(
                             "drop channel was closed already, could not forward \
                             drop token`{drop_token:?}`"
                         );
                         break 'outer;
```

### Comparing `dora_rs-0.2.3rc6/local_dependencies/dora-node-api/src/node/mod.rs` & `dora_rs-0.2.4rc3/local_dependencies/dora-node-api/src/node/mod.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 use crate::EventStream;
 
 use self::{control_channel::ControlChannel, drop_stream::DropStream};
 use dora_core::{
     config::{DataId, NodeId, NodeRunConfig},
     daemon_messages::{Data, DropToken, NodeConfig},
+    descriptor::Descriptor,
     message::{uhlc, Metadata, MetadataParameters},
 };
 use eyre::{bail, WrapErr};
 use shared_memory::{Shmem, ShmemConf};
 use std::{
     collections::{HashMap, VecDeque},
     ops::{Deref, DerefMut},
+    sync::Arc,
     time::Duration,
 };
 
 #[cfg(feature = "tracing")]
 use dora_tracing::set_up_tracing;
 
 mod control_channel;
@@ -22,22 +24,32 @@
 
 const ZERO_COPY_THRESHOLD: usize = 4096;
 
 pub struct DoraNode {
     id: NodeId,
     node_config: NodeRunConfig,
     control_channel: ControlChannel,
-    hlc: uhlc::HLC,
+    clock: Arc<uhlc::HLC>,
 
     sent_out_shared_memory: HashMap<DropToken, ShmemHandle>,
     drop_stream: DropStream,
     cache: VecDeque<ShmemHandle>,
+
+    dataflow_descriptor: Descriptor,
 }
 
 impl DoraNode {
+    /// Initiate a node from environment variables set by `dora-coordinator`
+    ///
+    /// ```no_run
+    /// use dora_node_api::DoraNode;
+    ///
+    /// let (mut node, mut events) = DoraNode::init_from_env().expect("Could not init node.");
+    /// ```
+    ///
     pub fn init_from_env() -> eyre::Result<(Self, EventStream)> {
         let node_config: NodeConfig = {
             let raw = std::env::var("DORA_NODE_CONFIG")
                 .wrap_err("env variable DORA_NODE_CONFIG must be set")?;
             serde_yaml::from_str(&raw).context("failed to deserialize operator config")?
         };
         #[cfg(feature = "tracing")]
@@ -49,35 +61,66 @@
     #[tracing::instrument]
     pub fn init(node_config: NodeConfig) -> eyre::Result<(Self, EventStream)> {
         let NodeConfig {
             dataflow_id,
             node_id,
             run_config,
             daemon_communication,
+            dataflow_descriptor,
         } = node_config;
 
-        let event_stream = EventStream::init(dataflow_id, &node_id, &daemon_communication)
-            .wrap_err("failed to init event stream")?;
-        let drop_stream = DropStream::init(dataflow_id, &node_id, &daemon_communication)
-            .wrap_err("failed to init drop stream")?;
-        let control_channel = ControlChannel::init(dataflow_id, &node_id, &daemon_communication)
-            .wrap_err("failed to init control channel")?;
+        let clock = Arc::new(uhlc::HLC::default());
+
+        let event_stream =
+            EventStream::init(dataflow_id, &node_id, &daemon_communication, clock.clone())
+                .wrap_err("failed to init event stream")?;
+        let drop_stream =
+            DropStream::init(dataflow_id, &node_id, &daemon_communication, clock.clone())
+                .wrap_err("failed to init drop stream")?;
+        let control_channel =
+            ControlChannel::init(dataflow_id, &node_id, &daemon_communication, clock.clone())
+                .wrap_err("failed to init control channel")?;
 
         let node = Self {
             id: node_id,
             node_config: run_config,
             control_channel,
-            hlc: uhlc::HLC::default(),
+            clock,
             sent_out_shared_memory: HashMap::new(),
             drop_stream,
             cache: VecDeque::new(),
+
+            dataflow_descriptor,
         };
         Ok((node, event_stream))
     }
 
+    /// Send data from the node to the other nodes.
+    /// We take a closure as an input to enable zero copy on send.
+    ///
+    /// ```no_run
+    /// use dora_node_api::{DoraNode, MetadataParameters};
+    /// use dora_core::config::DataId;
+    ///
+    /// let (mut node, mut events) = DoraNode::init_from_env().expect("Could not init node.");
+    ///
+    /// let output = DataId::from("output_id".to_owned());
+    ///
+    /// let data: &[u8] = &[0, 1, 2, 3];
+    /// let parameters = MetadataParameters::default();
+    ///
+    /// node.send_output(
+    ///    output,
+    ///    parameters,
+    ///    data.len(),
+    ///    |out| {
+    ///         out.copy_from_slice(data);
+    ///     }).expect("Could not send output");
+    /// ```
+    ///
     pub fn send_output<F>(
         &mut self,
         output_id: DataId,
         parameters: MetadataParameters,
         data_len: usize,
         data: F,
     ) -> eyre::Result<()>
@@ -97,15 +140,16 @@
         sample: Option<DataSample>,
     ) -> eyre::Result<()> {
         self.handle_finished_drop_tokens()?;
 
         if !self.node_config.outputs.contains(&output_id) {
             eyre::bail!("unknown output");
         }
-        let metadata = Metadata::from_parameters(self.hlc.new_timestamp(), parameters.into_owned());
+        let metadata =
+            Metadata::from_parameters(self.clock.new_timestamp(), parameters.into_owned());
 
         let (data, shmem) = match sample {
             Some(sample) => sample.finalize(),
             None => (None, None),
         };
 
         self.control_channel
@@ -204,14 +248,21 @@
         const MAX_CACHE_SIZE: usize = 20;
 
         self.cache.push_back(memory);
         while self.cache.len() > MAX_CACHE_SIZE {
             self.cache.pop_front();
         }
     }
+
+    /// Returns the full dataflow descriptor that this node is part of.
+    ///
+    /// This method returns the parsed dataflow YAML file.
+    pub fn dataflow_descriptor(&self) -> &Descriptor {
+        &self.dataflow_descriptor
+    }
 }
 
 impl Drop for DoraNode {
     #[tracing::instrument(skip(self), fields(self.id = %self.id), level = "trace")]
     fn drop(&mut self) {
         // close all outputs first to notify subscribers as early as possible
         if let Err(err) = self
```

### Comparing `dora_rs-0.2.3rc6/Cargo.toml` & `dora_rs-0.2.4rc3/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [package]
-version= "0.2.3-rc6"
+version= "0.2.4-rc3"
 name = "dora-node-api-python"
 edition = "2021"
 documentation= "https://dora.carsmos.ai/dora/"
 description= "`dora` goal is to be a low latency, composable, and distributed data flow."
 license= "Apache-2.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
@@ -18,11 +18,12 @@
 dora-operator-api-python = { path = "local_dependencies/dora-operator-api-python" }
 pyo3 = { version = "0.18", features = ["eyre", "abi3-py37"] }
 eyre = "0.6"
 serde_yaml = "0.8.23"
 flume = "0.10.14"
 dora-runtime = { features = ["tracing", "python"] , path = "local_dependencies/dora-runtime" }
 arrow = { version = "35.0.0", features = ["pyarrow"] }
+pythonize = "0.18.0"
 
 [lib]
 name = "dora"
 crate-type = ["cdylib"]
```

### Comparing `dora_rs-0.2.3rc6/Cargo.lock` & `dora_rs-0.2.4rc3/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,26 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.18"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e37cfd5e7657ada45f742d6e99ca5788580b5c529dc78faf11ece6dc702656f"
+checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "aho-corasick"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android_system_properties"
 version = "0.1.5"
@@ -56,18 +65,67 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7db9d9767fde724f83933a716ee182539788f293828244e9d999695ce0f7ba1e"
 dependencies = [
  "rgb",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e765fd216e48e067936442276d1d57399e37bce53c264d6fefbe298080cb57ee"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "array-init"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
 
@@ -246,15 +304,15 @@
 
 [[package]]
 name = "arrow-schema"
 version = "35.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf6b26f6a6f8410e3b9531cbd1886399b99842701da77d4b4cf2013f7708f20f"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "arrow-select"
 version = "35.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "83deb30a09afdf654d346092ef03e965f9c05d9b0753164d531f41d290d553f4"
@@ -274,47 +332,47 @@
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "async-attributes"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3203e79f4dd9bdda415ed03cf14dae5a2bf775c683a00f94e9cd1faf0f596e5"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "async-channel"
-version = "1.6.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2114d64672151c0c5eaa5e131ec84a74f06e1e559830dabba01ca30605d66319"
+checksum = "cf46fee83e5ccffc220104713af3292ff9bc7c64c7de289f66dae8e38d826833"
 dependencies = [
- "concurrent-queue 1.2.2",
+ "concurrent-queue",
  "event-listener",
  "futures-core",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.5.0"
+version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17adb73da160dfb475c183343c8cccd80721ea5a605d3eb57125f0a7b7a92d0b"
+checksum = "6fa3dc5f2a8564f07759c008b9109dc0d39de92a88d5588b8a5036d286383afb"
 dependencies = [
  "async-lock",
  "async-task",
- "concurrent-queue 2.1.0",
+ "concurrent-queue",
  "fastrand",
  "futures-lite",
  "slab",
 ]
 
 [[package]]
 name = "async-global-executor"
@@ -330,65 +388,67 @@
  "futures-lite",
  "once_cell",
  "tokio",
 ]
 
 [[package]]
 name = "async-io"
-version = "1.6.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a811e6a479f2439f0c04038796b5cfb3d2ad56c230e0f2d3f7b04d68cfee607b"
+checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
 dependencies = [
- "concurrent-queue 1.2.2",
+ "async-lock",
+ "autocfg",
+ "cfg-if",
+ "concurrent-queue",
  "futures-lite",
- "libc",
  "log",
- "once_cell",
  "parking",
  "polling",
+ "rustix",
  "slab",
  "socket2",
  "waker-fn",
- "winapi",
 ]
 
 [[package]]
 name = "async-lock"
 version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa24f727524730b077666307f2734b4a1a1c57acb79193127dcc8914d5242dd7"
 dependencies = [
  "event-listener",
 ]
 
 [[package]]
 name = "async-process"
-version = "1.3.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83137067e3a2a6a06d67168e49e68a0957d215410473a740cea95a2425c0b7c6"
+checksum = "7a9d28b1d97e08915212e2e45310d47854eafa69600756fc735fb788f75199c9"
 dependencies = [
  "async-io",
+ "async-lock",
+ "autocfg",
  "blocking",
  "cfg-if",
  "event-listener",
  "futures-lite",
- "libc",
- "once_cell",
+ "rustix",
  "signal-hook",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-rustls"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93b21a03b7c21702a0110f9f8d228763a533570deb376119042dabf33c37a01a"
 dependencies = [
  "futures-io",
- "rustls",
+ "rustls 0.20.8",
  "webpki",
 ]
 
 [[package]]
 name = "async-std"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -414,55 +474,56 @@
  "pin-utils",
  "slab",
  "wasm-bindgen-futures",
 ]
 
 [[package]]
 name = "async-stream"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dad5c83079eae9969be7fadefe640a1c566901f05ff91ab221de4b6f68d9507e"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
+ "pin-project-lite",
 ]
 
 [[package]]
 name = "async-stream-impl"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10f203db73a71dfa2fb6dd22763990fa26f3d2625a6da2da900d23b87d26be27"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.2.0"
+version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30696a84d817107fc028e049980e09d5e140e8da8f1caeb17e8e950658a3cea9"
+checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
 
 [[package]]
 name = "async-trait"
-version = "0.1.64"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd7fce9ba8c3c042128ce72d8b2ddbf3a05747efb67ea0313c635e10bda47a2"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "atomic-waker"
-version = "1.0.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065374052e7df7ee4047b1160cca5e1467a12351a40b3da123c870ba0b8eda2a"
+checksum = "1181e1e0d1fce796a03db1ae795d67167da795f9cf4a39c37589e85ef57f26d3"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
@@ -481,17 +542,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "3f1e31e207a6b8fb791a38ea3105e6cb541f55e4d029902d3039a4ad07cc4105"
 
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
@@ -502,56 +563,56 @@
 checksum = "fd4b13b0233143ae151a66e0135d715b65f631d1028c40502cc88182bcb9f4fa"
 dependencies = [
  "ansi_colours",
  "atty",
  "bincode",
  "bugreport",
  "bytesize",
- "clap 4.1.11",
+ "clap 4.3.0",
  "clircle",
  "console",
  "content_inspector",
- "dirs 5.0.0",
+ "dirs 5.0.1",
  "encoding",
  "flate2",
  "git2",
  "globset",
  "grep-cli",
  "nu-ansi-term 0.47.0",
  "once_cell",
  "path_abs",
  "plist",
  "regex",
  "semver",
  "serde",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
  "shell-words",
  "syntect",
  "thiserror",
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -567,80 +628,54 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "bitflags"
-version = "2.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07d1372b52fa64b8af7cf6e3848cfa2dadb81c21e810f144bdd9c26e21895235"
-
-[[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
  "funty",
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
 name = "block-buffer"
-version = "0.7.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0940dc441f31689269e10ac70eb1002a3a1d3ad1390e030043662eb7fe4688b"
-dependencies = [
- "block-padding",
- "byte-tools",
- "byteorder",
- "generic-array 0.12.4",
-]
-
-[[package]]
-name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
- "generic-array 0.14.5",
-]
-
-[[package]]
-name = "block-padding"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa79dedbb091f449f1f39e53edf88d5dbe95f895dae6135a8d7b881fb5af73f5"
-dependencies = [
- "byte-tools",
+ "generic-array",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.2.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6ccb65d468978a086b69884437ded69a90faab3bbe6e67f242173ea728acccc"
+checksum = "77231a1c8f801696fc0123ec6150ce92cffb8e164a02afb9c8ddee0e9b65ad65"
 dependencies = [
  "async-channel",
+ "async-lock",
  "async-task",
  "atomic-waker",
  "fastrand",
  "futures-lite",
- "once_cell",
+ "log",
 ]
 
 [[package]]
 name = "bstr"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
  "once_cell",
  "regex-automata",
  "serde",
 ]
 
@@ -653,23 +688,17 @@
  "git-version",
  "shell-escape",
  "sys-info",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
-
-[[package]]
-name = "byte-tools"
-version = "0.3.1"
+version = "3.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b5ca7a04898ad4bcd41c90c5285445ff5b791899bb1b0abdd2a2aa791211d7"
+checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
@@ -677,50 +706,50 @@
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.1.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4872d67bab6358e59559027aa3b9157c53d9358c51423c17554809a8858e0f8"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "bytesize"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38fcc2979eff34a4b84e1cf9a1e3da42a7d44b3b690a40cdcb23e3d556cfb2e5"
 
 [[package]]
 name = "cache-padded"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1db59621ec70f09c5e9b597b220c7a2b43611f4710dc03ceb8748637775692c"
+checksum = "981520c98f422fcc584dc1a95c334e6953900b9106bc47a9839b81790009eb21"
 
 [[package]]
 name = "capnp"
 version = "0.14.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dca085c2c7d9d65ad749d450b19b551efaa8e3476a439bdca07aca8533097f3"
 
 [[package]]
 name = "capnpc"
-version = "0.14.7"
+version = "0.14.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7ed9b80f792ac01a8b328ccbc509c2bd756fb5dec18af0163e7963dde23c0b5"
+checksum = "bdc9f1dc84666d4ff007b1a16c8f97db80764a624625979be05d869bcff43aaa"
 dependencies = [
  "capnp",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.73"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fff2a6927b3bb87f9595d67196a70493f627687a71d87a0d692242c33f58c11"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 dependencies = [
  "jobserver",
 ]
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
@@ -753,88 +782,94 @@
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
- "bitflags 1.3.2",
- "clap_derive 3.2.18",
+ "bitflags",
+ "clap_derive 3.2.25",
  "clap_lex 0.2.4",
  "indexmap",
  "once_cell",
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap"
-version = "4.1.11"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42dfd32784433290c51d92c438bb72ea5063797fc3cc9a21a8c4346bebbb2098"
+checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
 dependencies = [
- "bitflags 2.2.0",
- "clap_derive 4.1.9",
- "clap_lex 0.3.0",
- "is-terminal",
+ "clap_builder",
+ "clap_derive 4.3.0",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "bitflags",
+ "clap_lex 0.5.0",
  "once_cell",
  "strsim",
- "termcolor",
  "terminal_size",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.18"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
+checksum = "ae6371b8bdc8b7d3959e9cf7b22d4435ef3e79e138688421ec654acf8c81b008"
 dependencies = [
- "heck 0.4.0",
+ "heck 0.4.1",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.1.9"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fddf67631444a3a3e3e5ac51c36a5e01335302de677bd78759eaa90ab1f46644"
+checksum = "191d9573962933b4027f932c600cd252ce27a8ad5979418fe78e43c07996f27b"
 dependencies = [
- "heck 0.4.0",
- "proc-macro-error",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d4198f73e42b4936b35b5bb248d81d2b595ecb170da0bac7655c54eedfa8da8"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "clircle"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e68bbd985a63de680ab4d1ad77b6306611a8f961b282c8b5ab513e6de934e396"
 dependencies = [
@@ -851,64 +886,61 @@
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "combine"
 version = "4.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "flume",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 
 [[package]]
 name = "concurrent-queue"
-version = "1.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30ed07550be01594c6026cff2a1d7fe9c8f683caa798e12b68694ac9e88286a3"
-dependencies = [
- "cache-padded",
-]
-
-[[package]]
-name = "concurrent-queue"
-version = "2.1.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
+checksum = "62ec6771ecfa0762d24683ee5a32ad78487a3d3afdc0fb8cae19d2c5deb50b7c"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "console"
-version = "0.15.5"
+version = "0.15.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d79fbe8970a77e3e34151cc13d3b3e248aa0faaecb9f6091fa07ebefe5ad60"
+checksum = "c926e00cc70edefdc64d3a5ff31cc65bb97a3460097762bd23afb4d8145fccf8"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
  "unicode-width",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "const-oid"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "520fbf3c07483f94e3e3ca9d0cfd913d7718ef2483d2cfd91c0d9e91474ab913"
@@ -952,23 +984,23 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.2"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59a6001667ab124aebae2a495118e11d30984c3a653e99d86d58971708cf5e4b"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -976,44 +1008,43 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.4"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aaa7bd5fb665c6864b5f963dd9097905c54125909c7aa94c9e18507cdbe6c53"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6455c0ca19f0d2fbf751b908d5c55c1f5cbc65e03c4225427254b46890bdde1e"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.8"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1145cf131a2c6ba0615079ab6a638f7e1973ac9c2634fcbeaaad6114246efe8c"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "lazy_static",
- "memoffset 0.6.5",
+ "memoffset 0.8.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1024,15 +1055,15 @@
 
 [[package]]
 name = "crossterm"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot",
  "signal-hook",
  "signal-hook-mio",
  "winapi",
@@ -1055,15 +1086,15 @@
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
- "generic-array 0.14.5",
+ "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "csv"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1082,101 +1113,97 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.1.22"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f877be4f7c9f246b183111634f75baa039715e3f46ce860677d3b19a69fb229c"
+checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "ctrlc"
-version = "3.2.5"
+version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbcf33c2a618cbe41ee43ae6e9f2e48368cd9f9db2896f10167d8d762679f639"
+checksum = "04d778600249295e82b6ab12e291ed9029407efee0cfb7baf67157edc65964df"
 dependencies = [
  "nix 0.26.2",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "cty"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b365fabc795046672053e29c954733ec3b05e4be654ab130fe8f1f94d7051f35"
-
-[[package]]
 name = "cxx"
-version = "1.0.85"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5add3fc1717409d029b20c5b6903fc0c0b02fa6741d820054f4a2efa5e5816fd"
+checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
 dependencies = [
  "cc",
  "cxxbridge-flags",
  "cxxbridge-macro",
  "link-cplusplus",
 ]
 
 [[package]]
 name = "cxx-build"
-version = "1.0.73"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b49edea7163bbc7a39e3d829b4b0b66a9d30486973152842b7413f2c7b5632bf"
+checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
-version = "1.0.85"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69a3e162fde4e594ed2b07d0f83c6c67b745e7f28ce58c6df5e6b6bef99dfb59"
+checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
 
 [[package]]
 name = "cxxbridge-macro"
-version = "1.0.85"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e7e2adeb6a0d4a282e581096b06e1791532b7d576dcde5ccd9382acf55db8e6"
+checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "dashmap"
 version = "4.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e77a43b28d0668df09411cb0bc9a8c2adc40f9a048afe863e05fd43251e8e39c"
 dependencies = [
  "cfg-if",
  "num_cpus",
 ]
 
 [[package]]
 name = "dashmap"
-version = "5.2.0"
+version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8858831f7781322e539ea39e72449c46b059638250c14344fec8d0aa6e539c"
+checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
- "num_cpus",
- "parking_lot",
+ "hashbrown 0.12.3",
+ "lock_api",
+ "once_cell",
+ "parking_lot_core",
 ]
 
 [[package]]
 name = "der"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1a467a65c5e759bce6e65eaf91cc29f466cdc57cb65777bd646872a8a1fd4de"
@@ -1184,28 +1211,19 @@
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
 name = "digest"
-version = "0.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3d0c8c8752312f9713efd397ff63acb9f85585afbf179282e720e7704954dd5"
-dependencies = [
- "generic-array 0.12.4",
-]
-
-[[package]]
-name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
- "block-buffer 0.10.4",
+ "block-buffer",
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dirs"
@@ -1214,29 +1232,19 @@
 checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
 dependencies = [
  "dirs-sys 0.3.7",
 ]
 
 [[package]]
 name = "dirs"
-version = "5.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
-dependencies = [
- "dirs-sys 0.4.0",
-]
-
-[[package]]
-name = "dirs-next"
-version = "2.0.0"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b98cf8ebf19c3d1b223e151f99a4f9f0690dca41414773390fc824184ac833e1"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
- "cfg-if",
- "dirs-sys-next",
+ "dirs-sys 0.4.1",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
@@ -1244,290 +1252,282 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
-dependencies = [
- "libc",
- "redox_users",
- "windows-sys 0.45.0",
-]
-
-[[package]]
-name = "dirs-sys-next"
-version = "0.1.2"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ebda144c4fe02d1f7ea1a7d9641b6fc6b580adcfa024ae48797ecdeb6825b4d"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
- "atty",
  "bat",
- "clap 4.1.11",
+ "clap 4.3.0",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-core",
  "dora-node-api-c",
  "dora-operator-api-c",
  "dora-tracing",
  "eyre",
  "inquire",
  "notify",
  "serde",
  "serde_json",
- "serde_yaml 0.9.19",
+ "serde_yaml 0.9.21",
  "termcolor",
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
- "clap 3.2.23",
+ "clap 3.2.25",
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
  "futures-concurrency",
+ "names",
  "rand",
  "serde",
  "serde_json",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
  "thiserror",
  "tokio",
  "tokio-stream",
  "tracing",
  "uuid",
  "which",
  "zenoh",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
- "serde_yaml 0.9.19",
+ "serde_yaml 0.9.21",
  "tokio",
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "async-trait",
  "bincode",
- "clap 3.2.23",
+ "clap 3.2.25",
  "ctrlc",
  "dora-core",
  "dora-download",
  "dora-runtime",
  "dora-tracing",
  "eyre",
  "flume",
  "futures",
  "futures-concurrency",
  "serde",
  "serde_json",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
  "shared-memory-server",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
  "uuid",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "dora-examples"
 version = "0.0.0"
 dependencies = [
- "clap 4.1.11",
+ "clap 4.3.0",
  "dora-coordinator",
  "dora-core",
  "dora-daemon",
  "dunce",
  "eyre",
  "futures",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "capnp",
  "capnpc",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "futures",
  "opentelemetry 0.17.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "tokio",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "bincode",
  "capnp",
  "dora-core",
  "dora-tracing",
  "eyre",
  "flume",
+ "futures",
  "once_cell",
  "serde",
  "serde_json",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
  "shared-memory-server",
  "shared_memory",
  "thiserror",
  "tokio",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "flume",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-runtime",
  "eyre",
  "flume",
  "pyo3",
- "serde_yaml 0.8.23",
+ "pythonize",
+ "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "arrow",
  "dora-node-api",
  "eyre",
  "flume",
  "pyo3",
- "serde_yaml 0.8.23",
+ "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
- "clap 4.1.11",
+ "clap 4.3.0",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-operator-api-types",
  "dora-tracing",
@@ -1535,52 +1535,53 @@
  "flume",
  "futures",
  "futures-concurrency",
  "libloading",
  "opentelemetry 0.18.0",
  "opentelemetry-system-metrics",
  "pyo3",
- "serde_yaml 0.8.23",
+ "pythonize",
+ "serde_yaml 0.8.26",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tokio",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "dunce"
-version = "1.0.2"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453440c271cf5577fd2a40e4942540cb7d0d2f85e27c8d07dd0023c925a67541"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f94fa09c2aeea5b8839e414b7b841bf429fd25b9c522116ac97ee87856d88b2"
+checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
 
 [[package]]
 name = "either"
-version = "1.6.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -1646,17 +1647,17 @@
 name = "encoding_index_tests"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a246d82be1c9d791c5dfde9a2bd045fc3cbba3fa2b11ad558f27d01712f00569"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.31"
+version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9852635589dc9f9ea1b6fe9f05b50ef208c85c834a562f0c6abb1c475736ec2b"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.10.0"
@@ -1668,25 +1669,14 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys 0.48.0",
@@ -1721,15 +1711,15 @@
 name = "ext-trait-proc_macros"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ab7934152eaf26aa5aa9f7371408ad5af4c31357073c9e84c3b9d7f11ad639a"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "extension-traits"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a296e5a895621edf9fa8329c83aa1cb69a964643e36cf54d8d7a69b789089537"
@@ -1744,61 +1734,55 @@
 checksum = "4c2b6b5a29c02cdc822728b7d7b8ae1bab3e3b05d44522770ddd49722eeac7eb"
 dependencies = [
  "indenter",
  "once_cell",
 ]
 
 [[package]]
-name = "fake-simd"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88a8acf291dafb59c2d96e8f59828f3838bb1a70398823ade51a84de6a6deed"
-
-[[package]]
 name = "fastrand"
-version = "1.7.0"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3fcf0cee53519c866c09b5de1f6c56ff9d647101f81c1964fa632e148896cdf"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.2.12",
- "windows-sys 0.45.0",
+ "redox_syscall 0.2.16",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "fixedbitset"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "279fb028e20b3c4c320317955b77c5e0c9701f05a1d309905d6fc702cdc5053e"
+checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flatbuffers"
 version = "23.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77f5399c2c9c50ae9418e522842ad362f61ee48b346ac106807bd355a8a7c619"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "rustc_version",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
@@ -1806,15 +1790,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
 dependencies = [
  "futures-core",
  "futures-sink",
  "nanorand",
  "pin-project",
- "spin 0.9.2",
+ "spin 0.9.8",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
@@ -1841,114 +1825,114 @@
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "futures"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38390104763dc37a5145a53c29c63c1290b5d316d6086ec32c293f6736051bb0"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52ba265a92256105f45b719605a571ffe2d1f0fea3807304b522c1d778f79eed"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-concurrency"
-version = "7.1.0"
+version = "7.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e06f199437c8a435c12ad153c5a1f4e131871cf6f6025585bb15e8cbb414f0dc"
+checksum = "30ce9739c5655304eced9aaea4220e4393b8f60a3a5f1b84d09a206d6a5078a9"
 dependencies = [
  "bitvec",
  "futures-core",
  "pin-project",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04909a7a7e4633ae6c4a9ab280aeb86da1236243a77b694a49eacd659a4bd3ac"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7acc85df6714c176ab5edf386123fafe217be88c0840ec11f199441134a074e2"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00f5fb52a06bdcadeb54e8d3671f8888a39697dcb0b81b23b55174030427f4eb"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-lite"
-version = "1.12.0"
+version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
+checksum = "49a9d51ce47660b1e808d3c990b4709f2f415d928835a17dfd16991515c46bce"
 dependencies = [
  "fastrand",
  "futures-core",
  "futures-io",
  "memchr",
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdfb8ce053d86b91919aad980c220b1fb8401a9394410e1c289ed7e66b61835d"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39c15cf1a4aa79df40f1bb462fb39676d0ad9e366c2a33b590d7c66f4f81fcf9"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ffb393ac5d9a6eaa9d3fdf37ae2776656b706e200c8e16b1bdb227f5198e6ea"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.25"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197676987abd2f9cadff84926f410af1c183608d36641465df73ae8211dc65d6"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -1956,26 +1940,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.12.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffdf9f34f1447443d37393cc6c2b8313aebddcd96906caf34e54c68d8e57d7bd"
-dependencies = [
- "typenum",
-]
-
-[[package]]
-name = "generic-array"
-version = "0.14.5"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd48d33ec7f05fbfa152300fdad764757cbded343c1aa1cff2fbaf4134851803"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
@@ -1988,21 +1963,21 @@
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghost"
-version = "0.1.6"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb19fe8de3ea0920d282f7b77dd4227aea6b8b999b42cdf0ca41b2472b14443a"
+checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "git-version"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6b0decc02f4636b9ccad390dcbe77b722a77efedfa393caf8379a51d5c61899"
@@ -2016,54 +1991,54 @@
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe69f1cbdb6e28af2bac214e943b99ce8a0a06b447d15d3e61161b0423139f3f"
 dependencies = [
  "proc-macro-hack",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "git2"
 version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccf7f68c2995f392c49fffb4f95ae2c873297830eb25c6bc4c114ce8f4562acc"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "libc",
  "libgit2-sys",
  "log",
  "url",
 ]
 
 [[package]]
 name = "glob"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b919933a397b79c37e33b77bb2aa3dc8eb6e165ad809e58ff75bc7db2e34574"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "globset"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d74589adefde59de1a0c4f4732695c32805624aec7b68d91503d4dba79afc"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 0.7.20",
  "bstr",
  "fnv",
  "log",
  "regex",
 ]
 
 [[package]]
 name = "gloo-timers"
-version = "0.2.3"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d12a7f4e95cfe710f1d624fb1210b7d961a5fb05c4fd942f4feab06e61f590e"
+checksum = "9b995a66bb87bebce9a0f4a95aed01daca4872c050bfcb21653361c03bc35e5c"
 dependencies = [
  "futures-channel",
  "futures-core",
  "js-sys",
  "wasm-bindgen",
 ]
 
@@ -2082,28 +2057,28 @@
  "same-file",
  "termcolor",
  "winapi-util",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.17"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66b91535aa35fea1523ad1b86cb6b53c28e0ae566ba4a460f4457e936cad7c6f"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
  "indexmap",
  "slab",
  "tokio",
- "tokio-util 0.7.1",
+ "tokio-util 0.7.8",
  "tracing",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2132,17 +2107,17 @@
 checksum = "6d621efb26863f0e9924c6ac577e8275e5e6b77455db64ffa6c65c904e9e132c"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "heck"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
@@ -2172,31 +2147,31 @@
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "digest 0.10.6",
+ "digest",
 ]
 
 [[package]]
 name = "home"
-version = "0.5.3"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2456aef2e6b6a9784192ae780c0f15bc57df0e918585282325e8c8ac27737654"
+checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
 dependencies = [
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75f43d41e26995c17e71ee126451dd3941010b0514a81a9d11f3b341debc2399"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -2208,17 +2183,17 @@
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
-version = "1.7.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "496ce29bb5a52785b44e0f7ca2847ae0bb839c9bd28f69acac9b99d461c0c04c"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
 
@@ -2226,17 +2201,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.19"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42dc3c131584288d375f2d07f822b0cb012d8c6fb899a5b9fdb3cb7eb9b6004f"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -2271,70 +2246,65 @@
 checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows 0.48.0",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.2.3"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "418a0a6fab821475f634efe3ccc45c013f742efe03d853e8d3355d5cb850ecf8"
+checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
- "matches",
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indenter"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce23b50ad8242c51a442f3ff322d56b02f08852c77e4c0b4d3fd684abc89c683"
 
 [[package]]
 name = "indexmap"
-version = "1.9.1"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10a35a97730320ffe8e2d410b5d3b69279b98d2c14bdb8b70ea89ecf7888d41e"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.4"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7906a9fababaeacb774f72410e497a1d18de916322e33797bb2cd29baa23c9e"
-dependencies = [
- "unindent",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inotify"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8069d3ec154eb856955c1c0fbffefbf5f3c40a104ec912d4797314c1801abff"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "inotify-sys",
  "libc",
 ]
 
 [[package]]
 name = "inotify-sys"
 version = "0.1.5"
@@ -2346,24 +2316,24 @@
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
- "generic-array 0.14.5",
+ "generic-array",
 ]
 
 [[package]]
 name = "inquire"
-version = "0.5.2"
+version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6055ce38cac9b10ac819ed4a509d92ccbc60808152c19ff9121c98198964272"
+checksum = "f3a94f0659efe59329832ba0452d3ec753145fc1fb12a8e1d60de4ccf99f5364"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossterm",
  "dyn-clone",
  "lazy_static",
  "newline-converter",
  "thiserror",
  "unicode-segmentation",
  "unicode-width",
@@ -2376,17 +2346,17 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "integer-encoding"
-version = "3.0.3"
+version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e85a1509a128c855368e135cffcde7eac17d8e1083f41e2b98c58bc1a5074be"
+checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
 name = "inventory"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0eb5160c60ba1e809707918ee329adb99d222888155835c6feedba19f6c3fd4"
 dependencies = [
@@ -2399,81 +2369,84 @@
 name = "inventory-impl"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e41b53715c6f0c4be49510bb82dee2c1e51c8586d885abe65396e82ed518548"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.6"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfa919a82ea574332e2de6e74b4c36e74d41982b335080fa59d4ef31be20fdf3"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ipnet"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "879d54834c8c76457ef4293a689b2a8c59b076067ad77b15efafbb05f92a592b"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
 
 [[package]]
 name = "ipnetwork"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f84f1612606f3753f205a4e9a2efd6fe5b4c573a6269b2cc6c3003d44a0d127"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.4"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21b6b32576413a8e69b90e952e4a026476040d81017b80445deda5f2d3921857"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
- "rustix 0.36.9",
- "windows-sys 0.45.0",
+ "rustix",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.1"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1aab8fc367588b89dcee83ab0fd66b72b50b72fa1904d7095045ace2b0c81c35"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "jni"
-version = "0.20.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "039022cdf4d7b1cf548d31f60ae783138e5fd42013f6271049d7df7afadef96c"
+checksum = "1a87aa2bb7d2af34197c04845522473242e1aa17c12f4935d5856491a7fb8c97"
 dependencies = [
  "cesu8",
+ "cfg-if",
  "combine",
  "jni-sys",
  "log",
  "thiserror",
  "walkdir",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
@@ -2485,17 +2458,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.56"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a38fc24e30fd564ce974c02bf1d337caddff65be6cc4735a1f7eab22a7440f04"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json5"
 version = "0.4.1"
@@ -2505,17 +2478,20 @@
  "pest",
  "pest_derive",
  "serde",
 ]
 
 [[package]]
 name = "keccak"
-version = "0.1.0"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67c21572b4949434e4fc1e1978b99c5f77064153c59d998bf13ecd96fb5ecba7"
+checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
+dependencies = [
+ "cpufeatures",
+]
 
 [[package]]
 name = "kqueue"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c8fc60ba15bf51257aa9807a48a61013db043fcf3a78cb0d916e8e396dcad98"
 dependencies = [
@@ -2525,15 +2501,15 @@
 
 [[package]]
 name = "kqueue-sys"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8367585489f01bc55dd27404dcf56b95e6da061a256a666ab23be9ba96a2e587"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "libc",
 ]
 
 [[package]]
 name = "kv-log-macro"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2613,17 +2589,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libgit2-sys"
 version = "0.14.2+1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f3d95f6b51075fe9810a7ae22c7095f12b98005ab364d8544797a825ce946a4"
 dependencies = [
@@ -2641,23 +2617,23 @@
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libm"
-version = "0.2.2"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33a33a362ce288760ec6a508b94caaec573ae7d3bbbd91b87aa0bad4456839db"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -2668,45 +2644,40 @@
 checksum = "f30344350a2a51da54c1d53be93fade8a237e545dbcc4bdbe635413f2117cab9"
 dependencies = [
  "safemem",
 ]
 
 [[package]]
 name = "link-cplusplus"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8cae2cd7ba2f3f63938b9c724475dfb7b9861b545a90324476324ed21dbc8c8"
+checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linked-hash-map"
-version = "0.5.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fb9b38af92608140b86b693604b9ffcc5824240a484d1ecd4795bacb2fe88f3"
-
-[[package]]
-name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.2"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f508063cc7bb32987c71511216bd5a32be15bccb6a80b52df8b9d7f01fc3aa2"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.6"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88943dd7ef4a2e5a4bfa2753aaab3013e34ce2533d1996fb18ef591e315e2b3b"
+checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
+ "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2738,39 +2709,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb907fe88d54d8d9ce32a3cceab4218ed2f6b7d35617cafe9adf84e43919cb"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "maplit"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e2e65a1a2e43cfcb47a895c4c8b10d1f4a61097f9f254f183aee60cad9c651d"
-
-[[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
 
 [[package]]
-name = "matches"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e378b66a060d48947b590737b30a1be76706c8dd7b8ba0f2fe3989c68a853f"
-
-[[package]]
 name = "memchr"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "308cc39be01b73d0d18f82a0e7b2a3df85245f84af96fdddc5d202d27e47b86a"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
@@ -2793,72 +2752,82 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57ee1c23c7c63b0c9250c339ffdc69255f110b298b901b9f6c82547b7b87caaf"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys 0.36.1",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
+name = "names"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bddcd3bf5144b6392de80e04c347cd7fab2508f6df16a85fc496ecd5cec39bc"
+dependencies = [
+ "clap 3.2.25",
+ "rand",
+]
+
+[[package]]
 name = "nanorand"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
 dependencies = [
  "getrandom",
 ]
@@ -2876,45 +2845,32 @@
 checksum = "1f71d09d5c87634207f894c6b31b6a2b2c64ea3bdcf71bd5599fdbbe1600c00f"
 dependencies = [
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "nix"
-version = "0.22.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4916f159ed8e5de0082076562152a76b7a1f64a01fd9d1e0fea002c37624faf"
-dependencies = [
- "bitflags 1.3.2",
- "cc",
- "cfg-if",
- "libc",
- "memoffset 0.6.5",
-]
-
-[[package]]
-name = "nix"
-version = "0.23.1"
+version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f866317acbd3a240710c63f065ffb1e4fd466259045ccb504130b7f668f35c6"
+checksum = "8f3790c00a0150112de0f4cd161e3d7fc4b2d8a5542ffc35f099a2562aecb35c"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "cc",
  "cfg-if",
  "libc",
  "memoffset 0.6.5",
 ]
 
 [[package]]
 name = "nix"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "cfg-if",
  "libc",
  "memoffset 0.7.1",
  "pin-utils",
  "static_assertions",
 ]
 
@@ -2922,35 +2878,35 @@
 name = "no-std-net"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43794a0ace135be66a25d3ae77d41b91615fb68ae937f904090203e81f755b65"
 
 [[package]]
 name = "notify"
-version = "5.1.0"
+version = "5.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ea850aa68a06e48fdb069c0ec44d0d64c8dbffa49bf3b6f7f0a901fdea1ba9"
+checksum = "729f63e1ca555a43fe3efa4f3efdf4801c479da85b432242a7b726f353c88486"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "crossbeam-channel",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
  "mio",
  "walkdir",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "ntapi"
-version = "0.3.7"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c28774a7fd2fbb4f0babd8237ce554b73af68021b5f695a3cebd6c59bac0980f"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
@@ -3019,17 +2975,17 @@
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2cc698a63b549a70bc047073d2949cce27cd1c7b0a4a862d08a8031bc2801db"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
@@ -3052,17 +3008,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a64b1ec5cda2586e284722486d802acf1f7dbdc623e2bfc57e65ca1cd099290"
+checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -3091,15 +3047,15 @@
 
 [[package]]
 name = "onig"
 version = "6.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c4b31c8722ad9171c6d77d3557db078cab2bd50afcc9d09c8b315c59df8ca4f"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "libc",
  "once_cell",
  "onig_sys",
 ]
 
 [[package]]
 name = "onig_sys"
@@ -3108,20 +3064,14 @@
 checksum = "7b829e3d7e9cc74c7e315ee8edb185bf4190da5acde74afd7fc59c35b1f086e7"
 dependencies = [
  "cc",
  "pkg-config",
 ]
 
 [[package]]
-name = "opaque-debug"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2839e79665f131bdb5782e51f2c6c9599c133c6098982a54c794358bf432529c"
-
-[[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "opentelemetry"
@@ -3198,17 +3148,17 @@
 checksum = "9b02e0230abb0ab6636d18e2ba8fa02903ea63772281340ccac18e0af3ec9eeb"
 dependencies = [
  "opentelemetry 0.18.0",
 ]
 
 [[package]]
 name = "opentelemetry-system-metrics"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a848fb2d43cc8e5adabdedc6b37a88b45653d3a23b000a3d047e6953d5af42ea"
+checksum = "d425a3381784debcefe6c609c031b8f99ff1e56cb11ee783016970999f30c565"
 dependencies = [
  "indexmap",
  "opentelemetry 0.17.0",
  "sysinfo",
 ]
 
 [[package]]
@@ -3231,85 +3181,91 @@
 name = "opentelemetry_sdk"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ca41c4933371b61c2a2f214bf16931499af4ec90543604ec828f7a625c09113"
 dependencies = [
  "async-trait",
  "crossbeam-channel",
- "dashmap 5.2.0",
+ "dashmap 5.4.0",
  "fnv",
  "futures-channel",
  "futures-executor",
  "futures-util",
  "once_cell",
  "opentelemetry_api",
  "percent-encoding",
  "rand",
  "thiserror",
  "tokio",
  "tokio-stream",
 ]
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "ordered-float"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3305af35278dd29f46fcdd139e0b1fbfae2153f0e5928b39b035542dd31e37b7"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "ordered-float"
-version = "3.4.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d84eb1409416d254e4a9c8fa56cc24701755025b458f0fcd8e59e1f5f40c23bf"
+checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "os_str_bytes"
-version = "6.0.0"
+version = "6.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e22443d1643a904602595ba1cd8f7d896afe56d26712531c5ff73a15b2fbf64"
+checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
 
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
+checksum = "14f2252c834a40ed9bb5422029649578e63aa341ac401f74e719dd1afda8394e"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87f5ec2493a61ac0506c0f4199f99070cbe83857b0337006a30f3e6719b8ef58"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.1"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28141e0cc4143da2443301914478dc976a61ffdb3f043058310c70df2fed8954"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.2.12",
+ "redox_syscall 0.2.16",
  "smallvec",
- "windows-sys 0.32.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
@@ -3336,83 +3292,84 @@
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "pest"
-version = "2.1.3"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10f4872ae94d7b90ae48754df22fd42ad52ce740b8f370b03da4835417403e53"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
+ "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.1.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "833d1ae558dc601e9a60366421196a8d94bc0ac980476d0b67e1d0988d72b2d0"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.1.3"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99b8db626e31e5b81787b9783425769681b347011cc59471e33ea46d2ea0cf55"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.1.3"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54be6e404f5317079812fc8f9f5279de376d8856929e21c184ecf6bbd692a11d"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
- "maplit",
+ "once_cell",
  "pest",
- "sha-1",
+ "sha2",
 ]
 
 [[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.0.10"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ad3879ad3baf4e44784bc6a718a8698867bb991f8ce24d1bcbe2cfb4c3a75e"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.10"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "744b6f092ba29c3650faf274db506afd39944f48420f6c86b17cfe0ee1cb36bb"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -3443,25 +3400,25 @@
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plist"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9bd9647b268a3d3e14ff09c23201133a62589c658db02bb7388c7246aafe0590"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.1",
  "indexmap",
  "line-wrap",
  "quick-xml",
  "serde",
  "time",
 ]
 
@@ -3504,15 +3461,15 @@
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "48dd52a5211fac27e7acb14cfc9f30ae16ae0e956b7b779c8214c74559cef4c3"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pnet_macros_support"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89de095dc7739349559913aed1ef6a11e73ceade4897dadc77c5e09de6740750"
@@ -3552,51 +3509,54 @@
  "pnet_base",
  "pnet_packet",
  "pnet_sys",
 ]
 
 [[package]]
 name = "polling"
-version = "2.2.0"
+version = "2.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685404d509889fade3e86fe3a5803bca2ec09b0c0778d5ada6ec8bf7a8de5259"
+checksum = "4b2d323e8ca7996b3e23126511a523f7e62924d93ecd5ae73b333815b0eb3dce"
 dependencies = [
+ "autocfg",
+ "bitflags",
  "cfg-if",
+ "concurrent-queue",
  "libc",
  "log",
- "wepoll-ffi",
- "winapi",
+ "pin-project-lite",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "ppv-lite86"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb9f9e6e233e5c4a35559a617bf40a4ec447db2e84c20b55a6f83167b7e57872"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.1.24"
+version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ebcd279d20a4a0a2404a33056388e950504d891c855c7975b9a8fef75f3bf04"
+checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
 dependencies = [
  "proc-macro2",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3605,23 +3565,23 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-hack"
-version = "0.5.19"
+version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbf0c48bc1d91375ae5c3cd81e3722dff1abcf81a30960240640d223f59fe0e5"
+checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.9.0"
@@ -3658,32 +3618,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9cc1a3263e07e0bf68e96268f37665207b49560d98739662cdfaae215c720fe"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "prost-types"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "534b7a0e836e3c482d2693070f982e39e7611da9695d4d1f5a4b186b51faef0a"
 dependencies = [
  "bytes",
  "prost",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "eyre",
  "indoc",
  "libc",
  "memoffset 0.8.0",
  "parking_lot",
@@ -3691,53 +3651,63 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "pythonize"
+version = "0.18.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
+dependencies = [
+ "pyo3",
+ "serde",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
@@ -3752,32 +3722,32 @@
 checksum = "445cbfe2382fa023c4f2f3c7e1c95c03dcc1df2bf23cebcb2b13e1402c4394d1"
 dependencies = [
  "bytes",
  "pin-project-lite",
  "quinn-proto",
  "quinn-udp",
  "rustc-hash",
- "rustls",
+ "rustls 0.20.8",
  "thiserror",
  "tokio",
  "tracing",
  "webpki",
 ]
 
 [[package]]
 name = "quinn-proto"
-version = "0.9.2"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72ef4ced82a24bb281af338b9e8f94429b6eca01b4e66d899f40031f074e74c9"
+checksum = "67c10f662eee9c94ddd7135043e544f3c82fa839a1e7b865911331961b53186c"
 dependencies = [
  "bytes",
  "rand",
  "ring",
  "rustc-hash",
- "rustls",
+ "rustls 0.20.8",
  "rustls-native-certs",
  "slab",
  "thiserror",
  "tinyvec",
  "tracing",
  "webpki",
 ]
@@ -3793,17 +3763,17 @@
  "socket2",
  "tracing",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -3829,130 +3799,130 @@
 dependencies = [
  "ppv-lite86",
  "rand_core",
 ]
 
 [[package]]
 name = "rand_core"
-version = "0.6.3"
+version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d34f1408f55294453790c48b2f1ebbb1c5b4b7563eb1f418bcfcfdbb06ebb4e7"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "raw-window-handle"
-version = "0.5.0"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed7e3d950b66e19e0c372f3fa3fbbcf85b1746b571f74e0c2af6042a5c93420a"
-dependencies = [
- "cty",
-]
+checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
 name = "raw_sync_2"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f067b45fa17e31d15636789c2638bd562da5496d498876cf0495df78f7e4fdcb"
 dependencies = [
  "cfg-if",
  "libc",
- "nix 0.23.1",
+ "nix 0.23.2",
  "rand",
  "winapi",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.5.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c06aca804d41dbc8ba42dfd964f0d01334eceb64314b9ecf7c5fad5188a06d90"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
- "autocfg",
- "crossbeam-deque",
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.9.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d78120e2c850279833f1dd3582f730c4ab53ed95aeaaaa862a2a5c71b1656d8e"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
- "lazy_static",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.12"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae183fc1b06c149f0c1793e1eb447c8b04bfe46d48e9e48bfb8d2d7ed64ecf0"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7776223e2696f1aa4c6b0170e83212f47296a00424305117d013dfe86fb0fe55"
+checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall 0.2.12",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
- "aho-corasick",
+ "aho-corasick 1.0.1",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "reqwest"
-version = "0.11.12"
+version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "431949c384f4e2ae07605ccaa56d1d9d2ecdb5cadd4f9577ccfab29f2e5149fc"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
- "base64 0.13.1",
+ "base64 0.21.1",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -3960,15 +3930,15 @@
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls",
+ "rustls 0.21.1",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tower-service",
  "url",
  "wasm-bindgen",
@@ -4014,15 +3984,15 @@
 [[package]]
 name = "rsa"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "094052d5470cbcef561cb848a7209968c9f12dfa6d668f4bca048ac5de51099c"
 dependencies = [
  "byteorder",
- "digest 0.10.6",
+ "digest",
  "num-bigint-dig",
  "num-integer",
  "num-iter",
  "num-traits",
  "pkcs1",
  "pkcs8",
  "rand_core",
@@ -4030,33 +4000,33 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-operator"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rustc-hash"
@@ -4071,50 +4041,48 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.9"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd5c6ff11fecd55b40746d1995a02f2eb375bf8c00d192d521ee09f42bef37bc"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
- "bitflags 1.3.2",
- "errno 0.2.8",
+ "bitflags",
+ "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys 0.1.4",
- "windows-sys 0.45.0",
+ "linux-raw-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "rustix"
-version = "0.37.3"
+name = "rustls"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b24138615de35e32031d041a09032ef3487a616d901ca4db224e7d557efae2"
+checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
 dependencies = [
- "bitflags 1.3.2",
- "errno 0.3.1",
- "io-lifetimes",
- "libc",
- "linux-raw-sys 0.3.2",
- "windows-sys 0.45.0",
+ "log",
+ "ring",
+ "sct",
+ "webpki",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.20.6"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aab8ee6c7097ed6057f43c187a62418d0c05a4bd5f18b3571db50ee0f9ce033"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
 dependencies = [
  "log",
  "ring",
+ "rustls-webpki",
  "sct",
- "webpki",
 ]
 
 [[package]]
 name = "rustls-native-certs"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0167bac7a9f490495f3c33013e7722b53cb087ecbe082fb0c6387c96f634ea50"
@@ -4127,22 +4095,32 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.1",
+]
+
+[[package]]
+name = "rustls-webpki"
+version = "0.100.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.9"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73b4b750c782965c211b42f022f59af1fbceabdd026623714f104152f1ec149f"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "safemem"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef703b7cb59335eae2eb93ceb664c0eb7ea6bf567079d843e09420219668e072"
 
@@ -4169,122 +4147,121 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1438fb328c52f5148ea02a317603efd802f2cd6eb9e721adfd51b94bb55d9ddb"
 dependencies = [
  "macro_rules_attribute",
  "prettyplease",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "schannel"
-version = "0.1.19"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f05ba609c234e60bee0d547fe94a4c7e9da733d1c962cf6e59efa4cd9c8bc75"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
- "lazy_static",
- "winapi",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scratch"
-version = "1.0.2"
+version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
+checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
 
 [[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.6.1"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dc14f172faf8a0194a3aded622712b0de276821addc574fa54fc0a1167e10dc"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.6.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0160a13a177a45bfb43ce71c01580998474f556ad854dcbca936dd2841a5c556"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.7"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d65bd28f48be7196d222d95b9243287f48d27aca604e08497513019ff0502cc4"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-with-expand-env"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "888d884a3be3a209308d0b66f1918ff18f60e93db837259e53ea7d8dd14e7e98"
 dependencies = [
  "serde",
- "shellexpand 2.1.0",
+ "shellexpand 2.1.2",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.89"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "020ff22c755c2ed3f8cf162dbb41a7268d934702f3ed3631656ea597e08fc3db"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -4297,91 +4274,90 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.8.23"
+version = "0.8.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a521f2940385c165a24ee286aa8599633d162077a54bdcae2a6fd5a7bfa7a0"
+checksum = "578a7433b776b56a35785ed5ce9a7e777ac0598aac5a6dd1b4b18a307c7fc71b"
 dependencies = [
  "indexmap",
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.19"
+version = "0.9.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f82e6c8c047aa50a7328632d067bcae6ef38772a79e28daf32f735e0e4f3dd10"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
-name = "sha-1"
-version = "0.8.2"
+name = "sha2"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7d94d0bede923b3cea61f3f1ff57ff8cdfd77b400fb8f9998949e0cf04163df"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
- "block-buffer 0.7.3",
- "digest 0.8.1",
- "fake-simd",
- "opaque-debug",
+ "cfg-if",
+ "cpufeatures",
+ "digest",
 ]
 
 [[package]]
 name = "sha3"
-version = "0.10.6"
+version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf0c33fae925bdc080598b84bc15c55e7b9a4a43b3c704da051f977469691c9"
+checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
 dependencies = [
- "digest 0.10.6",
+ "digest",
  "keccak",
 ]
 
 [[package]]
 name = "sharded-slab"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory",
  "tracing",
 ]
 
 [[package]]
 name = "shared_memory"
-version = "0.12.0"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "681a9e90340f748af3a1cc52eb2c040eee29f976b763e99ad90fc0c5df6f9791"
+checksum = "ba8593196da75d9dc4f69349682bd4c2099f8cde114257d1ef7ef1b33d1aba54"
 dependencies = [
  "cfg-if",
  "libc",
- "nix 0.22.3",
+ "nix 0.23.2",
  "rand",
- "winapi",
+ "win-sys",
 ]
 
 [[package]]
 name = "shell-escape"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "45bb67a18fa91266cc7807181f62f9178a6873bfad7dc788c42e6430db40184f"
@@ -4390,35 +4366,35 @@
 name = "shell-words"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24188a676b6ae68c3b2cb3a01be17fbf7240ce009799bb56d5b1409051e78fde"
 
 [[package]]
 name = "shellexpand"
-version = "2.1.0"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83bdb7831b2d85ddf4a7b148aa19d0587eddbe8671a436b7bd1182eaad0f2829"
+checksum = "7ccc8076840c4da029af4f87e4e8daeb0fca6b87bbb02e10cb60b791450e11e4"
 dependencies = [
- "dirs-next",
+ "dirs 4.0.0",
 ]
 
 [[package]]
 name = "shellexpand"
-version = "3.0.0"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd1c7ddea665294d484c39fd0c0d2b7e35bbfe10035c5fe1854741a57f6880e1"
+checksum = "da03fa3b94cc19e3ebfc88c4229c49d8f08cdbd1228870a45f0ffdf84988e14b"
 dependencies = [
- "dirs 4.0.0",
+ "dirs 5.0.1",
 ]
 
 [[package]]
 name = "signal-hook"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "647c97df271007dcea485bb74ffdb57f2e683f1306c854f468a0c244badabf2d"
+checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-mio"
@@ -4429,36 +4405,39 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "signature"
 version = "1.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
 dependencies = [
- "digest 0.10.6",
+ "digest",
  "rand_core",
 ]
 
 [[package]]
 name = "slab"
-version = "0.4.5"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9def91fd1e018fe007022791f865d0ccc9b3a0d5001e01aabb8b40e46000afb5"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
+dependencies = [
+ "autocfg",
+]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
@@ -4476,17 +4455,17 @@
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
 name = "spin"
-version = "0.9.2"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "511254be0c5bcf062b019a6c89c01a664aa359ded62f78aa72c6fc137c0590e5"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "spki"
 version = "0.6.0"
@@ -4525,44 +4504,55 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syntect"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6c454c27d9d7d9a84c7803aaa3c50cd088d2906fe3c6e42da3209aa623576a8"
 dependencies = [
  "bincode",
- "bitflags 1.3.2",
+ "bitflags",
  "flate2",
  "fnv",
  "lazy_static",
  "once_cell",
  "onig",
  "plist",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "serde",
  "serde_derive",
  "serde_json",
  "thiserror",
  "walkdir",
  "yaml-rust",
 ]
@@ -4575,17 +4565,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.24.5"
+version = "0.26.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d80929a3b477bce3a64360ca82bfb361eacce1dcb7b1fb31e8e5e181e37c212"
+checksum = "5c18a6156d1f27a9592ee18c1a846ca8dd5c258b7179fc193ae87c74ebb666f5"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "rayon",
@@ -4596,82 +4586,83 @@
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.4"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
- "rustix 0.37.3",
+ "rustix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "terminal_size"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e6bf6f19e9f8ed8d4048dc22981458ebcf406d67e94cd422e5ecd73d63b3237"
 dependencies = [
- "rustix 0.37.3",
+ "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10deb33631e3c9018b9baf9dcbbc4f737320d2b576bac10f6aefa048fa407e3e"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.37"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "982d17546b47146b28f7c22e3d08465f6b8903d0ea13c1660d9d84a6e7adcdbb"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.4"
+version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
+checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
+ "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "threadpool"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4691,35 +4682,35 @@
  "log",
  "ordered-float 1.1.1",
  "threadpool",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
@@ -4727,73 +4718,72 @@
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
 name = "tinyvec"
-version = "1.5.1"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c1c1d5a42b6245520c249549ec267180beaffcc0615401ac8e31853d4b6d8d2"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
 dependencies = [
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.7.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b557f72f448c511a979e2564e55d74e6c4432fc96ff4f6241bc6bded342643b7"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.11"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d660770404473ccd7bc9f8b28494a811bc18542b915c0855c51e8f419d5223ce"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
@@ -4808,17 +4798,17 @@
  "log",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.1"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0edfdeb067411dba2044da6d1cb2df793dd35add7888d73c16e3381ded401764"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -4860,48 +4850,48 @@
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9403f1bafde247186684b230dc6f38b5cd514584e8bec1dd32514be4745fa757"
 dependencies = [
  "proc-macro2",
  "prost-build",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "tower"
-version = "0.4.12"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89fd63ad6adf737582df5db40d286574513c69a11dac5214dc3b5603d6713e"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
  "indexmap",
  "pin-project",
  "pin-project-lite",
  "rand",
  "slab",
  "tokio",
- "tokio-util 0.7.1",
+ "tokio-util 0.7.8",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "tower-layer"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "343bc9466d3fe6b0f960ef45960509f84480bf4fd96f92901afe7ff3df9d3a62"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
 
 [[package]]
 name = "tower-service"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "360dfd1d6d30e05fda32ace2c8c70e9c0a9da713275777f5a4dbb8a1893930c6"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
@@ -4910,28 +4900,28 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-futures"
@@ -4966,17 +4956,17 @@
  "tracing-core",
  "tracing-log",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "nu-ansi-term 0.46.0",
  "once_cell",
  "regex",
  "sharded-slab",
  "smallvec",
@@ -4984,97 +4974,98 @@
  "tracing",
  "tracing-core",
  "tracing-log",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59547bce71d9c38b83d9c0e92b6066c4253371f15005def0c30d9657f50c7642"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
 
 [[package]]
 name = "typenum"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf81ac59edc17cc8697ff311e8f5ef2d99fcbd9817b34cec66f90b6c3dfd987"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ucd-trie"
-version = "0.1.3"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56dee185309b50d1f11bfedef0fe6d036842e3fb77413abef29f8f8d1c5d4c1c"
+checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "uhlc"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7908438f98a5824af02b34c2b31fb369c5764ef835d26df0badbb9897fb28245"
+checksum = "8d291a7454d390b753ef68df8145da18367e32883ec2fa863959f0aefb915cdb"
 dependencies = [
  "hex",
  "humantime",
  "lazy_static",
  "log",
  "serde",
+ "spin 0.9.8",
  "uuid",
 ]
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.8"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "099b7128301d285f79ddd55b9a83d5e6b9e97c92e0ea0daebee7263e932de992"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.3"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4f5b37a154999a8f3f98cc23a628d850e154479cd94decf3414696e12e31aaf"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "854cbdc4f7bc6ae19c820d44abdc3277ac3e1b2b93db20a636825d9322fb60e6"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.0"
+version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdbf052a0783de01e944a6ce7a8cb939e295b1e7be835a1112c3b9a7f047a5a"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
 [[package]]
 name = "unindent"
-version = "0.1.8"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "514672a55d7380da379785a4d70ca8386c8883ff7eaae877be4d2081cebe73d8"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "uninit"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e130f2ed46ca5d8ec13c7ff95836827f92f5f5f37fd2b2bf16f33c408d98bb6"
 dependencies = [
  "extension-traits",
 ]
 
 [[package]]
 name = "unsafe-libyaml"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad2024452afd3874bf539695e04af6732ba06517424dbf958fdb16a01f3bef6c"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
@@ -5088,34 +5079,39 @@
 name = "unzip-n"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e7e85a0596447f0f2ac090e16bc4c516c6fe91771fb0c0ccf7fa3dae896b9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "url"
-version = "2.2.2"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507c383b2d33b5fc35d1861e77e6b383d158b2da5e14fe51b83dfedf6fd578c"
+checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
 dependencies = [
  "form_urlencoded",
  "idna",
- "matches",
  "percent-encoding",
 ]
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "validated_struct"
@@ -5133,15 +5129,15 @@
 name = "validated_struct_macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d4444a980afa9ef0d29c2a3f4d952ec0495a7a996a9c78b52698b71bc21edb4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "unzip-n",
 ]
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5179,20 +5175,19 @@
 name = "waker-fn"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d5b2c62b4012a3e1eca5a7e077d13b3bf498c4073e33ccd58626607748ceeca"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5206,105 +5201,103 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.79"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25f1af7423d8588a3d840681122e72e6a24ddbcb3f0ec385cac0d12d24256c06"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.79"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b21c0df030f5a177f3cba22e9bc4322695ec43e7257d865302900290bcdedca"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
- "lazy_static",
  "log",
+ "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.29"
+version = "0.4.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2eb6ec270a31b1d3c7e266b999739109abce8b6c87e4b31fcfcd788b65267395"
+checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.79"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f4203d69e40a52ee523b2529a773d5ffc1dc0071801c87b3d270b471b80ed01"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.79"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa8a30d46208db204854cadbb5d4baf5fcf8071ba5bf48190c3e59937962ebc"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.79"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d958d035c4438e28c70e4321a2911302f10135ce78a9c7834c0cab4123d06a2"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.56"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c060b319f29dd25724f09a2ba1418f142f539b2be99fbf4d2d5a8f7330afb8eb"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webbrowser"
-version = "0.8.3"
+version = "0.8.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa61ff77f695a94d9c8558e0bb5c362a8fd1f27c74663770fbc633acbafedbb6"
+checksum = "fd222aa310eb7532e3fd427a5d7db7e44bc0b0cf1c1e21139c345325511a85b6"
 dependencies = [
  "core-foundation",
- "dirs 4.0.0",
+ "home",
  "jni",
  "log",
  "ndk-context",
  "objc",
  "raw-window-handle",
  "url",
  "web-sys",
- "widestring",
- "winapi",
 ]
 
 [[package]]
 name = "webpki"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f095d78192e208183081cc07bc5515ef55216397af48b873e5edcd72637fa1bd"
@@ -5319,49 +5312,43 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
 dependencies = [
  "webpki",
 ]
 
 [[package]]
-name = "wepoll-ffi"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d743fdedc5c64377b5fc2bc036b01c7fd642205a0d96356034ae3404d49eb7fb"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "which"
-version = "4.3.0"
+version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c831fbbee9e129a8cf93e7747a82da9d95ba8e16621cae60ec2cdc849bacb7b"
+checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
 dependencies = [
  "either",
  "libc",
  "once_cell",
 ]
 
 [[package]]
-name = "widestring"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "653f141f39ec16bba3c5abe400a0c60da7468261cc2cbf36805022876bc721a8"
-
-[[package]]
 name = "wild"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05b116685a6be0c52f5a103334cbff26db643826c7b3735fc0a3ba9871310a74"
 dependencies = [
  "glob",
 ]
 
 [[package]]
+name = "win-sys"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b7b128a98c1cfa201b09eb49ba285887deb3cbe7466a98850eb1adabb452be5"
+dependencies = [
+ "windows 0.34.0",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -5386,93 +5373,80 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
-dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-sys"
-version = "0.32.0"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3df6e476185f92a12c072be4a189a0210dcdcf512a1891d6dff9edb874deadc6"
+checksum = "45296b64204227616fdbf2614cefa4c236b98ee64dfaaaa435207ed99fe7829f"
 dependencies = [
- "windows_aarch64_msvc 0.32.0",
- "windows_i686_gnu 0.32.0",
- "windows_i686_msvc 0.32.0",
- "windows_x86_64_gnu 0.32.0",
- "windows_x86_64_msvc 0.32.0",
+ "windows_aarch64_msvc 0.34.0",
+ "windows_i686_gnu 0.34.0",
+ "windows_i686_msvc 0.34.0",
+ "windows_x86_64_gnu 0.34.0",
+ "windows_x86_64_msvc 0.34.0",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.36.1"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_msvc 0.36.1",
- "windows_i686_gnu 0.36.1",
- "windows_i686_msvc 0.36.1",
- "windows_x86_64_gnu 0.36.1",
- "windows_x86_64_msvc 0.36.1",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.1",
- "windows_aarch64_msvc 0.42.1",
- "windows_i686_gnu 0.42.1",
- "windows_i686_msvc 0.42.1",
- "windows_x86_64_gnu 0.42.1",
- "windows_x86_64_gnullvm 0.42.1",
- "windows_x86_64_msvc 0.42.1",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets 0.42.1",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.1",
- "windows_aarch64_msvc 0.42.1",
- "windows_i686_gnu 0.42.1",
- "windows_i686_msvc 0.42.1",
- "windows_x86_64_gnu 0.42.1",
- "windows_x86_64_gnullvm 0.42.1",
- "windows_x86_64_msvc 0.42.1",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
@@ -5484,149 +5458,119 @@
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
  "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.32.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8e92753b1c443191654ec532f14c199742964a061be25d77d7a96f09db20bf5"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.36.1"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9bb8c3fd39ade2d67e9874ac4f3db21f0d710bee00fe7cab16949ec184eeaa47"
+checksum = "17cffbe740121affb56fad0fc0e421804adf0ae00891205213b5cecd30db881d"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.32.0"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a711c68811799e017b6038e0922cb27a5e2f43a2ddb609fe0b6f3eeda9de615"
+checksum = "2564fde759adb79129d9b4f54be42b32c89970c18ebf93124ca8870a498688ed"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.36.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180e6ccf01daf4c426b846dfc66db1fc518f074baa793aa7d9b9aaeffad6a3b6"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.42.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.32.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "146c11bb1a02615db74680b32a68e2d61f553cc24c4eb5b4ca10311740e44172"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.36.1"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2e7917148b2812d1eeafaeb22a97e4813dfa60a3f8f78ebe204bcc88f12f024"
+checksum = "9cd9d32ba70453522332c14d38814bceeb747d80b3958676007acadd7e166956"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.32.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c912b12f7454c6620635bbff3450962753834be2a594819bd5e945af18ec64bc"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.36.1"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dcd171b8776c41b97521e5da127a2d86ad280114807d0b2ab1e462bc764d9e1"
+checksum = "cfce6deae227ee8d356d19effc141a509cc503dfd1f850622ec4b0f84428e1f4"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.32.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "504a2476202769977a040c6364301a3f65d0cc9e3fb08600b2bda150a0488316"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.36.1"
+version = "0.34.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c811ca4a8c853ef420abd8592ba53ddbbac90410fab6903b3e79972a631f7680"
+checksum = "d19538ccc21819d01deaf88d6a17eae6596a12e9aafdbb97916fb49896d89de9"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
@@ -5652,15 +5596,15 @@
 name = "with_builtin_macros-proc_macros"
 version = "0.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15bd7679c15e22924f53aee34d4e448c45b674feb6129689af88593e129f8f42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
@@ -5692,15 +5636,15 @@
  "flume",
  "form_urlencoded",
  "futures",
  "git-version",
  "hex",
  "lazy_static",
  "log",
- "ordered-float 3.4.0",
+ "ordered-float 3.7.0",
  "petgraph",
  "rand",
  "regex",
  "rustc_version",
  "serde",
  "serde_json",
  "socket2",
@@ -5766,15 +5710,15 @@
 checksum = "bad1ff61abf28c57e8879ec4286fa29becf7e9bf12555df9a7faddff3bc9ea1b"
 dependencies = [
  "flume",
  "json5",
  "num_cpus",
  "serde",
  "serde_json",
- "serde_yaml 0.9.19",
+ "serde_yaml 0.9.21",
  "validated_struct",
  "zenoh-cfg-properties",
  "zenoh-core",
  "zenoh-protocol-core",
  "zenoh-util",
 ]
 
@@ -5848,15 +5792,15 @@
 checksum = "a9f1354094eb4d5e4b864b5aa385efce46f94a43f6ba57dd9ea9a017e6e74176"
 dependencies = [
  "async-std",
  "async-trait",
  "futures",
  "log",
  "quinn",
- "rustls",
+ "rustls 0.20.8",
  "rustls-native-certs",
  "rustls-pemfile",
  "webpki",
  "zenoh-cfg-properties",
  "zenoh-config",
  "zenoh-core",
  "zenoh-link-commons",
@@ -5938,29 +5882,29 @@
  "zenoh-link-commons",
  "zenoh-protocol-core",
  "zenoh-sync",
 ]
 
 [[package]]
 name = "zenoh-logger"
-version = "0.2.3-rc6"
+version = "0.2.4-rc3"
 dependencies = [
  "zenoh",
 ]
 
 [[package]]
 name = "zenoh-macros"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3a9ac20b120990778cca204ee46c43a37ed4ffbc331e95702615490f9c169de8"
 dependencies = [
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
  "unzip-n",
 ]
 
 [[package]]
 name = "zenoh-plugin-trait"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -6049,32 +5993,32 @@
 [[package]]
 name = "zenoh-util"
 version = "0.7.0-rc"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54646455dad3940535e97cce03f1b604265177349133903d989bc72e00011404"
 dependencies = [
  "async-std",
- "clap 3.2.23",
+ "clap 3.2.25",
  "futures",
  "hex",
  "home",
  "humantime",
  "lazy_static",
  "libc",
  "libloading",
  "log",
  "pnet",
  "pnet_datalink",
- "shellexpand 3.0.0",
+ "shellexpand 3.1.0",
  "winapi",
  "zenoh-cfg-properties",
  "zenoh-collections",
  "zenoh-core",
  "zenoh-crypto",
  "zenoh-sync",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
```

