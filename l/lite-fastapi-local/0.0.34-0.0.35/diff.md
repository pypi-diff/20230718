# Comparing `tmp/lite_fastapi_local-0.0.34.tar.gz` & `tmp/lite_fastapi_local-0.0.35.tar.gz`

## Comparing `lite_fastapi_local-0.0.34.tar` & `lite_fastapi_local-0.0.35.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/ledModel.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/ledModel.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import FastAPI, status
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse, PlainTextResponse, Response, FileResponse
 from fastapi_utils.tasks import repeat_every
 
 import asyncio, json, subprocess, sys, os, time, shutil, threading, requests, uvicorn
-import QR_CHK_dep as CHKF
+import lite_fastapi_local.QR_CHK_dep as CHKF
 
 from common.variable import common
 from common.function import find_camera_index_list, save_cctv, find_camera_index, find_lidar_sensor_port_number, upload_video_to_s3
 from settings import Logger, mqtt
 from router import setupRouter, motorRouter, sensorRouter
 from model.motorModel import motor
 from model.ledModel import led
```

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/function.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/motorModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/setupModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/solModel.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/motorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/setupRouter.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/LICENSE` & `lite_fastapi_local-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.34/pyproject.toml` & `lite_fastapi_local-0.0.35/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.34"
+version = "0.0.35"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.34/PKG-INFO` & `lite_fastapi_local-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.34
+Version: 0.0.35
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

