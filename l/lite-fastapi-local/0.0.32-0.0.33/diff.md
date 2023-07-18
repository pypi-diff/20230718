# Comparing `tmp/lite_fastapi_local-0.0.32.tar.gz` & `tmp/lite_fastapi_local-0.0.33.tar.gz`

## Comparing `lite_fastapi_local-0.0.32.tar` & `lite_fastapi_local-0.0.33.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_READ_dep.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/requirements.txt
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/settings.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/common/function.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/common/variable.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/boxDoorModel.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/ledModel.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/motorModel.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/setupModel.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/solModel.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/sprayModel.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/motorRouter.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/sensorRouter.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/ledModel.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.33/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.32/src/QR_CHK_dep.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/QR_READ_dep.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/main.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/main.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/requirements.txt` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/settings.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/common/function.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/common/variable.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/model/motorModel.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/model/setupModel.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/model/solModel.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/router/motorRouter.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/router/sensorRouter.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/src/router/setupRouter.py` & `lite_fastapi_local-0.0.33/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/LICENSE` & `lite_fastapi_local-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.32/pyproject.toml` & `lite_fastapi_local-0.0.33/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.32"
+version = "0.0.33"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.32/PKG-INFO` & `lite_fastapi_local-0.0.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.32
+Version: 0.0.33
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

