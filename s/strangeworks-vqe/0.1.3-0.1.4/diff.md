# Comparing `tmp/strangeworks_vqe-0.1.3.tar.gz` & `tmp/strangeworks_vqe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_vqe-0.1.3.tar", max compression
+gzip compressed data, was "strangeworks_vqe-0.1.4.tar", max compression
```

## Comparing `strangeworks_vqe-0.1.3.tar` & `strangeworks_vqe-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       19 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/README.md
--rw-r--r--   0        0        0      659 2023-05-01 16:14:49.365245 strangeworks_vqe-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      126 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/__init__.py
--rw-r--r--   0        0        0    11090 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/sdk.py
--rw-r--r--   0        0        0      691 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/serializer.py
--rw-r--r--   0        0        0     5714 2023-05-01 16:14:33.265433 strangeworks_vqe-0.1.3/strangeworks_vqe/utils.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      121 2023-07-18 10:56:23.507099 strangeworks_vqe-0.1.4/README.md
+-rw-r--r--   0        0        0      659 2023-07-18 10:56:39.703329 strangeworks_vqe-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-07-18 10:56:23.507099 strangeworks_vqe-0.1.4/strangeworks_vqe/__init__.py
+-rw-r--r--   0        0        0    11091 2023-07-18 10:56:23.507099 strangeworks_vqe-0.1.4/strangeworks_vqe/sdk.py
+-rw-r--r--   0        0        0      691 2023-07-18 10:56:23.507099 strangeworks_vqe-0.1.4/strangeworks_vqe/serializer.py
+-rw-r--r--   0        0        0     5714 2023-07-18 10:56:23.507099 strangeworks_vqe-0.1.4/strangeworks_vqe/utils.py
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.4/PKG-INFO
```

### Comparing `strangeworks_vqe-0.1.3/pyproject.toml` & `strangeworks_vqe-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "strangeworks-vqe"
-version = "0.1.3"
+version = "0.1.4"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_vqe"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "^0.4.0"
+strangeworks = "^0.4.4"
 tweedledum = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
```

### Comparing `strangeworks_vqe-0.1.3/strangeworks_vqe/sdk.py` & `strangeworks_vqe-0.1.4/strangeworks_vqe/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         all_backends = strangeworks.backends(backend_type_slugs=["sw-vqe"])
 
         aws_backends = []
         aws_sim_backends = []
         ibmq_backends = []
         ibm_cloud_backends = []
         ibm_sim_backends = []
+
         for bb in range(len(all_backends)):
             try:
                 arn_str = all_backends[bb].remote_backend_id[0:3]
                 # print(arn_str)
                 if arn_str == "arn" and all_backends[bb].remote_status != "retired":
                     if (
                         all_backends[bb].name == "SV1"
```

### Comparing `strangeworks_vqe-0.1.3/strangeworks_vqe/serializer.py` & `strangeworks_vqe-0.1.4/strangeworks_vqe/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_vqe-0.1.3/strangeworks_vqe/utils.py` & `strangeworks_vqe-0.1.4/strangeworks_vqe/utils.py`

 * *Files identical despite different names*

