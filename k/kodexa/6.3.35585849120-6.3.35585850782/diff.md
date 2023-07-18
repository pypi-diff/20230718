# Comparing `tmp/kodexa-6.3.35585849120.tar.gz` & `tmp/kodexa-6.3.35585850782.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35585849120.tar", max compression
+gzip compressed data, was "kodexa-6.3.35585850782.tar", max compression
```

## Comparing `kodexa-6.3.35585849120.tar` & `kodexa-6.3.35585850782.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-07-18 09:43:14.359956 kodexa-6.3.35585849120/LICENSE
--rw-r--r--   0        0        0     2804 2023-07-18 09:43:14.359956 kodexa-6.3.35585849120/README.md
--rw-r--r--   0        0        0      847 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/model/__init__.py
--rw-r--r--   0        0        0      856 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/model/model.py
--rw-r--r--   0        0        0   118091 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/model/objects.py
--rw-r--r--   0        0        0    38744 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   112675 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/platform/client.py
--rw-r--r--   0        0        0    28020 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-07-18 09:43:14.367956 kodexa-6.3.35585849120/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 09:43:14.371956 kodexa-6.3.35585849120/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1260 2023-07-18 09:43:28.080004 kodexa-6.3.35585849120/pyproject.toml
--rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 kodexa-6.3.35585849120/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-18 09:43:25.496338 kodexa-6.3.35585850782/LICENSE
+-rw-r--r--   0        0        0     2804 2023-07-18 09:43:25.496338 kodexa-6.3.35585850782/README.md
+-rw-r--r--   0        0        0      847 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/model/model.py
+-rw-r--r--   0        0        0   118091 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38744 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112675 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28020 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:43:25.504338 kodexa-6.3.35585850782/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1261 2023-07-18 09:43:42.040584 kodexa-6.3.35585850782/pyproject.toml
+-rw-r--r--   0        0        0     4029 1970-01-01 00:00:00.000000 kodexa-6.3.35585850782/PKG-INFO
```

### Comparing `kodexa-6.3.35585849120/LICENSE` & `kodexa-6.3.35585850782/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/README.md` & `kodexa-6.3.35585850782/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/__init__.py` & `kodexa-6.3.35585850782/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/assistant/assistant.py` & `kodexa-6.3.35585850782/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/connectors/connectors.py` & `kodexa-6.3.35585850782/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/model/__init__.py` & `kodexa-6.3.35585850782/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/model/base.py` & `kodexa-6.3.35585850782/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/model/model.py` & `kodexa-6.3.35585850782/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/model/objects.py` & `kodexa-6.3.35585850782/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/model/persistence.py` & `kodexa-6.3.35585850782/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35585850782/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/platform/client.py` & `kodexa-6.3.35585850782/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/platform/kodexa.py` & `kodexa-6.3.35585850782/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/ast.py` & `kodexa-6.3.35585850782/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/core.py` & `kodexa-6.3.35585850782/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/lexrules.py` & `kodexa-6.3.35585850782/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/lextab.py` & `kodexa-6.3.35585850782/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/parserules.py` & `kodexa-6.3.35585850782/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/selectors/parsetab.py` & `kodexa-6.3.35585850782/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/spatial/azure_models.py` & `kodexa-6.3.35585850782/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35585850782/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35585850782/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/steps/common.py` & `kodexa-6.3.35585850782/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/testing/test_components.py` & `kodexa-6.3.35585850782/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/kodexa/testing/test_utils.py` & `kodexa-6.3.35585850782/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35585849120/pyproject.toml` & `kodexa-6.3.35585850782/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35585849120"
+version = "6.3.35585850782"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries',
     '''License :: OSI Approved :: Apache Software License''', # noqa
-    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 addict = "2.4.0"
 requests = "^2.28.1"
 msgpack = "1.0.5"
```

### Comparing `kodexa-6.3.35585849120/PKG-INFO` & `kodexa-6.3.35585850782/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35585849120
+Version: 6.3.35585850782
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

