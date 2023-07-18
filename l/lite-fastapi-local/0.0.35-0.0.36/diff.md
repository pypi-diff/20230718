# Comparing `tmp/lite_fastapi_local-0.0.35.tar.gz` & `tmp/lite_fastapi_local-0.0.36.tar.gz`

## Comparing `lite_fastapi_local-0.0.35.tar` & `lite_fastapi_local-0.0.36.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/readme.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_CHK_dep.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_END_dep.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_READ_dep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/__init__.py
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/main.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/requirements.txt
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/__init__.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/function.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/variable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/boxDoorModel.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/ledModel.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/motorModel.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/setupModel.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/solModel.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/sprayModel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/__init__.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/motorRouter.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/sensorRouter.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/setupRouter.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/schema/qrSchema.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/src/lite_fastapi_local/schema/setupSchema.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/readme.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/QR_CHK_dep.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/QR_END_dep.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/QR_READ_dep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/__init__.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/main.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/requirements.txt
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/common/__init__.py
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/common/function.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/common/variable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/boxDoorModel.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/ledModel.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/motorModel.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/setupModel.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/solModel.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/sprayModel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/__init__.py
+-rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/motorRouter.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/sensorRouter.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/setupRouter.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/schema/qrSchema.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/src/lite_fastapi_local/schema/setupSchema.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 lite_fastapi_local-0.0.36/PKG-INFO
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_CHK_dep.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/QR_CHK_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/QR_READ_dep.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/QR_READ_dep.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/main.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import JSONResponse, PlainTextResponse, Response, FileResponse
 from fastapi_utils.tasks import repeat_every
 
 import asyncio, json, subprocess, sys, os, time, shutil, threading, requests, uvicorn
 import lite_fastapi_local.QR_CHK_dep as CHKF
 
-from common.variable import common
-from common.function import find_camera_index_list, save_cctv, find_camera_index, find_lidar_sensor_port_number, upload_video_to_s3
-from settings import Logger, mqtt
-from router import setupRouter, motorRouter, sensorRouter
-from model.motorModel import motor
-from model.ledModel import led
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.common.function import find_camera_index_list, save_cctv, find_camera_index, find_lidar_sensor_port_number, upload_video_to_s3
+from lite_fastapi_local.settings import Logger, mqtt
+from lite_fastapi_local.router import setupRouter, motorRouter, sensorRouter
+from lite_fastapi_local.model.motorModel import motor
+from lite_fastapi_local.model.ledModel import led
 
 
 app = FastAPI()
 app.include_router(setupRouter.router)
 app.include_router(motorRouter.router)
 app.include_router(sensorRouter.router)
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/requirements.txt` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/requirements.txt`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/settings.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/settings.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/function.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/common/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 
 from datetime import datetime
 from pygrabber.dshow_graph import FilterGraph
 from skimage.metrics import structural_similarity as ssim
 from serial.tools import list_ports
 
-from common.variable import common
+from lite_fastapi_local.common.variable import common
 # from settings import trigger_lambda, s3_connection
 
 
 # aws
 def update_cctv_list():
     mac_address = common.get_MACHINE_MAC()
     url = f"https://44qasvgllj.execute-api.ap-northeast-2.amazonaws.com/test_run/macAddress/{mac_address}"
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/common/variable.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/common/variable.py`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/motorModel.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/motorModel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from common.variable import common
-from settings import mqtt
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.settings import mqtt
 
 class Motor:
 
     def send_qr_result(self, qr_code: str, result: str):
         mac = common.get_MACHINE_MAC()
         mqtt.publish(f'tg/{mac}/qr_result', json.dumps({
             "qr_code": qr_code,
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/setupModel.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/setupModel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from common.variable import common
-from settings import mqtt
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.settings import mqtt
 
 class Setup():
 
     def change_volume(self, volume: int):
         mac = common.get_MACHINE_MAC()
         mqtt.publish(f'tg/{mac}/setup', json.dumps({
             'volume': str(volume)
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/model/solModel.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/model/solModel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from common.variable import common
-from settings import mqtt
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.settings import mqtt
 
 class Sol():
 
     def turn_on_sol(self, index):
         mac = common.get_MACHINE_MAC()
         mqtt.publish(f'tg/{mac}/control', json.dumps({
             "do":{
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/motorRouter.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/motorRouter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import asyncio, threading
 from datetime import datetime
 
 from fastapi import APIRouter, status, BackgroundTasks
 from fastapi.responses import JSONResponse
 
-from common.variable import common
-from common.function import capture_image, save_cctv, create_directory
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.common.function import capture_image, save_cctv, create_directory
+from lite_fastapi_local.model.motorModel import motor
+from lite_fastapi_local.model.ledModel import led
+from lite_fastapi_local.model.setupModel import setup
+from lite_fastapi_local.model.sprayModel import spray
+from lite_fastapi_local.model.boxDoorModel import box_door
+from lite_fastapi_local.model.solModel import sol
 
-from model.motorModel import motor
-from model.ledModel import led
-from model.setupModel import setup
-from model.sprayModel import spray
-from model.boxDoorModel import box_door
-from model.solModel import sol
-
-from schema.qrSchema import QrCode
+from lite_fastapi_local.schema.qrSchema import QrCode
 
 router = APIRouter(
     prefix="/motor",
     tags=["motors"],
     responses={404: {"description": "Not found"}}
 )
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/sensorRouter.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/sensorRouter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import serial
 
 from fastapi import APIRouter, status
 from fastapi.responses import JSONResponse
 
-from common.variable import common
+from lite_fastapi_local.common.variable import common
 
 router = APIRouter(
     prefix="/sensor",
     tags=["sensors"],
     responses={404: {"description": "Not found"}}
 )
```

### Comparing `lite_fastapi_local-0.0.35/src/lite_fastapi_local/router/setupRouter.py` & `lite_fastapi_local-0.0.36/src/lite_fastapi_local/router/setupRouter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from fastapi import APIRouter, status
 from fastapi.responses import JSONResponse
 
-from common.variable import common
-
-from model.setupModel import setup
-from schema.setupSchema import Volume, MotorMovement, CountMax, CountSet, DoorOpenPower, DoorHoldingPower
+from lite_fastapi_local.common.variable import common
+from lite_fastapi_local.model.setupModel import setup
+from lite_fastapi_local.schema.setupSchema import Volume, MotorMovement, CountMax, CountSet, DoorOpenPower, DoorHoldingPower
 
 router = APIRouter(
     prefix="/setup",
     tags=["setups"],
     responses={404: {"description": "Not found"}}
 )
```

### Comparing `lite_fastapi_local-0.0.35/LICENSE` & `lite_fastapi_local-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `lite_fastapi_local-0.0.35/pyproject.toml` & `lite_fastapi_local-0.0.36/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lite_fastapi_local"
-version = "0.0.35"
+version = "0.0.36"
 authors = [
   { name="dohyung102", email="dohyung102@thegreet.co.kr" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lite_fastapi_local-0.0.35/PKG-INFO` & `lite_fastapi_local-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lite_fastapi_local
-Version: 0.0.35
+Version: 0.0.36
 Summary: A small example package
 Author-email: dohyung102 <dohyung102@thegreet.co.kr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

