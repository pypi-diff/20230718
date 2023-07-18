# Comparing `tmp/strangeworks_hybrid_optimize-0.1.1.tar.gz` & `tmp/strangeworks_hybrid_optimize-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_hybrid_optimize-0.1.1.tar", max compression
+gzip compressed data, was "strangeworks_hybrid_optimize-0.1.2.tar", max compression
```

## Comparing `strangeworks_hybrid_optimize-0.1.1.tar` & `strangeworks_hybrid_optimize-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       61 2023-07-16 11:08:20.398575 strangeworks_hybrid_optimize-0.1.1/README.md
--rw-r--r--   0        0        0      831 2023-07-16 11:08:33.614679 strangeworks_hybrid_optimize-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      346 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/__init__.py
--rw-r--r--   0        0        0    23978 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/sdk.py
--rw-r--r--   0        0        0    12428 2023-07-16 11:08:20.402575 strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/utils.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/README.md
+-rw-r--r--   0        0        0      831 2023-07-18 12:53:43.847948 strangeworks_hybrid_optimize-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      346 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/__init__.py
+-rw-r--r--   0        0        0    23979 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/sdk.py
+-rw-r--r--   0        0        0    12428 2023-07-18 12:53:25.808066 strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/utils.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strangeworks_hybrid_optimize-0.1.2/PKG-INFO
```

### Comparing `strangeworks_hybrid_optimize-0.1.1/pyproject.toml` & `strangeworks_hybrid_optimize-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "strangeworks-hybrid-optimize"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extension to strangeworks sdk to allow user to run the hybrid optimization service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_hybrid_optimize"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "0.4.0"
+strangeworks = "0.4.4"
 dimod = "^0.12.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
```

### Comparing `strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/sdk.py` & `strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
                 for rr in range(len(rsc_list)):
                     if rsc_list[rr].product.slug == self.product_slug:
                         self.rsc = rsc_list[rr]
             if self.rsc is None:
                 raise StrangeworksError(
                     "Unable to find resource. Please add resource on platform https://portal.strangeworks.com/products"  # noqa: E501
                 )
+
         except Exception as e:
             raise StrangeworksError(
                 f"Unable to find resource. Please add resource on platform https://portal.strangeworks.com/products: {e}"  # noqa: E501
             )
 
         self.backend_list = " "
```

### Comparing `strangeworks_hybrid_optimize-0.1.1/strangeworks_hybrid_optimize/utils.py` & `strangeworks_hybrid_optimize-0.1.2/strangeworks_hybrid_optimize/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_hybrid_optimize-0.1.1/PKG-INFO` & `strangeworks_hybrid_optimize-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: strangeworks-hybrid-optimize
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension to strangeworks sdk to allow user to run the hybrid optimization service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dimod (>=0.12.4,<0.13.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: qiskit (>=0.41.0,<0.42.0)
-Requires-Dist: strangeworks (==0.4.0)
+Requires-Dist: strangeworks (==0.4.4)
 Description-Content-Type: text/markdown
 
 # strangeworks-hybrid-optimize
 
 SDK extension for svc-hybrid
```

