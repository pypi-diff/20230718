# Comparing `tmp/webuiapi-0.9.4-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13148 bytes, number of entries: 7
--rw-r--r--  2.0 unx      574 b- defN 23-Jul-15 03:54 webuiapi/__init__.py
--rw-r--r--  2.0 unx    36360 b- defN 23-Jul-15 03:54 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    13790 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Jul-15 03:55 webuiapi-0.9.4.dist-info/RECORD
-7 files, 52449 bytes uncompressed, 12186 bytes compressed:  76.8%
+Zip file size: 13211 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      574 b- defN 23-Jul-18 05:00 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    36512 b- defN 23-Jul-18 04:59 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-18 05:01 webuiapi-0.9.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13773 b- defN 23-Jul-18 05:01 webuiapi-0.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 05:01 webuiapi-0.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-18 05:01 webuiapi-0.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-Jul-18 05:01 webuiapi-0.9.5.dist-info/RECORD
+7 files, 52584 bytes uncompressed, 12249 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.4.dist-info/LICENSE
+Filename: webuiapi-0.9.5.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.4.dist-info/METADATA
+Filename: webuiapi-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.4.dist-info/WHEEL
+Filename: webuiapi-0.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.4.dist-info/top_level.txt
+Filename: webuiapi-0.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.4.dist-info/RECORD
+Filename: webuiapi-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -9,15 +9,15 @@
     ModelKeywordInterface,
     InstructPix2PixInterface,
     ControlNetInterface,
     ControlNetUnit,
     RemBGInterface,
 )
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -581,18 +581,22 @@
         payload = {
             "image": b64_img(image),
         }
 
         response = self.session.post(url=f"{self.baseurl}/png-info", json=payload)
         return self._to_api_result(response)
 
-    # XXX always returns empty info (2022/12/26)
-    def interrogate(self, image):
+    """
+    :param image pass base64 encoded image or PIL Image
+    :param model "clip" or "deepdanbooru"
+    """
+    def interrogate(self, image, model="clip"):
         payload = {
-            "image": b64_img(image),
+            "image": b64_img(image) if isinstance(image, Image.Image) else image,
+            "model": model,
         }
 
         response = self.session.post(url=f"{self.baseurl}/interrogate", json=payload)
         return self._to_api_result(response)
 
     def interrupt(self):
         response = self.session.post(url=f"{self.baseurl}/interrupt")
```

## Comparing `webuiapi-0.9.4.dist-info/LICENSE` & `webuiapi-0.9.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.4.dist-info/METADATA` & `webuiapi-0.9.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.4
+Version: 0.9.5
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: Pillow
 
 # sdwebuiapi
 API client for AUTOMATIC1111/stable-diffusion-webui
 
 Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
@@ -440,13 +440,13 @@
 ```
 
 
 ### Extension support - RemBG (contributed by webcoderz)
 ```
 # https://github.com/AUTOMATIC1111/stable-diffusion-webui-rembg
 rembg = webuiapi.RemBGInterface(api)
-rembg.rembg()
-
 r = rembg.rembg(input_image=img, model='u2net', return_mask=False)
 r.image
 ```
 
+
+
```

