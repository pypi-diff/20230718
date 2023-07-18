# Comparing `tmp/lite_fastapi_local-0.0.31.tar.gz` & `tmp/lite_fastapi_local-0.0.32.tar.gz`

## Comparing `lite_fastapi_local-0.0.31.tar` & `lite_fastapi_local-0.0.32.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/QR_READ_dep.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/requirements.txt
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/settings.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/common/function.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/common/variable.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/boxDoorModel.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/ledModel.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/motorModel.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/setupModel.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/solModel.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/sprayModel.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/motorRouter.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/sensorRouter.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/QR_READ_dep.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/requirements.txt
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/settings.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/common/function.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/common/variable.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/boxDoorModel.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/ledModel.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/motorModel.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/setupModel.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/solModel.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/model/sprayModel.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/motorRouter.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/sensorRouter.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/src/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.32/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/QR_CHK_dep.py` & `lite_fastapi_local-0.0.32/src/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/QR_READ_dep.py` & `lite_fastapi_local-0.0.32/src/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/main.py` & `lite_fastapi_local-0.0.32/src/main.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/requirements.txt` & `lite_fastapi_local-0.0.32/src/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/settings.py` & `lite_fastapi_local-0.0.32/src/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/common/function.py` & `lite_fastapi_local-0.0.32/src/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/common/variable.py` & `lite_fastapi_local-0.0.32/src/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/motorModel.py` & `lite_fastapi_local-0.0.32/src/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/setupModel.py` & `lite_fastapi_local-0.0.32/src/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/model/solModel.py` & `lite_fastapi_local-0.0.32/src/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/motorRouter.py` & `lite_fastapi_local-0.0.32/src/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/sensorRouter.py` & `lite_fastapi_local-0.0.32/src/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/src/lite_fastapi_local_ver_greengrass/router/setupRouter.py` & `lite_fastapi_local-0.0.32/src/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/LICENSE` & `lite_fastapi_local-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.31/pyproject.toml` & `lite_fastapi_local-0.0.32/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.31/PKG-INFO` & `lite_fastapi_local-0.0.32/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.31
+Version: 0.0.32
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

