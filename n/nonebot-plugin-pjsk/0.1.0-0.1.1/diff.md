# Comparing `tmp/nonebot_plugin_pjsk-0.1.0.tar.gz` & `tmp/nonebot_plugin_pjsk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_pjsk-0.1.0.tar` & `nonebot_plugin_pjsk-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2202 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/README.md
--rw-r--r--   0        0        0     1070 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/LICENSE
--rw-r--r--   0        0        0     1148 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     1581 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     4225 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0      951 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1078 2023-07-13 09:45:45.960801 nonebot_plugin_pjsk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2202 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/README.md
+-rw-r--r--   0        0        0     1070 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/LICENSE
+-rw-r--r--   0        0        0     1186 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     1581 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     5014 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0      951 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1078 2023-07-18 15:40:46.096094 nonebot_plugin_pjsk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.1.0/README.md` & `nonebot_plugin_pjsk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/LICENSE` & `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from nonebot.plugin import PluginMetadata
 
 from .draw import make_ramdom
 from .utils import check_res
 
 driver = get_driver()
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __plugin_meta__ = PluginMetadata(
     name="pjsk表情",
     description="pjsk表情包生成,适配nonebot2的插件",
     usage="pjsk 【text】",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     supported_adapters={"~onebot.v11"},
@@ -27,15 +27,17 @@
 
 pjsk = on_command("pjsk", aliases={"啤酒烧烤"}, priority=10)
 
 
 @pjsk.handle()
 async def _(matcher: Matcher, arg: Message = CommandArg()) -> None:
     if text := arg.extract_plain_text():
-        await matcher.send(MessageSegment.image(await make_ramdom(text)))
+        img = await make_ramdom(text)
+        if img:
+            await matcher.send(MessageSegment.image(img))
 
 
 @driver.on_startup
 async def _():
     logger.info("检查pjsk资源")
     msg = await check_res()
     logger.success(msg)
```

### Comparing `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/draw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from io import BytesIO
 from pathlib import Path
-from typing import Tuple
+from typing import Tuple, Optional
 
 from PIL import Image, ImageDraw, ImageFont
 from pydantic import BaseModel
 
 from .config import (
     template,
     stroke_color,
@@ -24,25 +24,25 @@
     text_color: str = "grey"
     font_start: Tuple[int, int] = (0, 0)
     stroke_width: int = 7
     rotation_angle: int = 10
     font_size: int
 
 
-async def make_ramdom(text: str) -> bytes:
+async def make_ramdom(text: str):
     """生成图片"""
     text_list = text.split(" ")
     role: Path = random.choice(list(template.keys()))
     random_img: Path = random.choice(template[role])
     image: Image.Image = Image.open(random_img)
     text_image = Image.new("RGBA", image.size, (0, 0, 0, 0))
     draw = ImageDraw.Draw(text_image)
-
+    text_config: Optional[TextConfig] = None
     if len(text_list) == 1:
-        text_config:TextConfig = await text_draw(text, image.size, draw, role)
+        text_config = await text_draw(text, image.size, draw, role)
         text_position = text_config.font_start
         draw.text(
             text_position,
             text_config.text,
             font=font_style,
             fill=stroke_color,
             stroke_width=text_config.stroke_width,
@@ -52,47 +52,65 @@
             text=text_config.text,
             font=font_style,
             fill=text_config.text_color,
         )
 
     elif len(text_list) >= 2:
         for i, one_text in enumerate(text_list, start=0):
-            text_config:TextConfig = await text_draw(one_text, image.size, draw, role)
+            text_config = await text_draw(one_text, image.size, draw, role)
             text_position = text_config.font_start
-            text_position = (text_position[0],(text_position[-1] + (i * text_config.font_size)))
+            text_position = (
+                text_position[0],
+                (text_position[-1] + (i * text_config.font_size)),
+            )
             draw.text(
                 text_position,
                 text_config.text,
                 font=font_style,
                 fill=stroke_color,
                 stroke_width=text_config.stroke_width,
             )
             draw.text(
                 xy=text_position,
                 text=text_config.text,
                 font=font_style,
                 fill=text_config.text_color,
             )
-
     else:
-        ...
+        return
 
+    if not text_config:
+        return
     # print(text_config.font_start)
 
     # 旋转
+    if text_config.rotation_angle:
+        text_bbox = draw.textbbox((0, 0), text_config.text, font_style)
+        center = (
+            (text_bbox[0] + text_bbox[2]) * 2,
+            (text_bbox[1] + text_bbox[3]) * 2,
+        )
+        print(center)
+        text_image = text_image.rotate(
+            text_config.rotation_angle,
+            expand=True,
+            center=center,
+            resample=Image.BICUBIC,
+        )
+
     # if text_config.rotation_angle:
     #     text_bbox = draw.textbbox((0, 0), text_config.text, font_style)
     #     center = (
     #         (text_bbox[0] + text_bbox[2]) // 2,
     #         (text_bbox[1] + text_bbox[3]) // 2,
     #     )
-    #     print(center)
-    #     text_image = text_image.rotate(
-    #         text_config.rotation_angle, expand=True, center=center
-    #     )
+    #     text_image = text_image.resize((text_image.width * 2, text_image.height * 2), Image.ANTIALIAS)
+    #     text_image = text_image.filter(ImageFilter.SMOOTH)
+    #     text_image = text_image.rotate(text_config.rotation_angle, expand=True,center=center, resample=Image.BICUBIC)
+    #     text_image = text_image.resize((text_image.width // 2, text_image.height // 2), Image.ANTIALIAS)
 
     image.paste(text_image, (0, 0), mask=text_image)
     bytes_data = BytesIO()
     image.save(bytes_data, format="png")
     return bytes_data.getvalue()
```

### Comparing `nonebot_plugin_pjsk-0.1.0/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.1.1/nonebot_plugin_pjsk/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.1.0/pyproject.toml` & `nonebot_plugin_pjsk-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_pjsk"
-version = "0.1.0"
+version = "0.1.1"
 description = "PJSK表情包for Nonebot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 repository = "https://github.com/Agnes4m/nonebot_plugin_pjsk"
 keywords = ["pjsk", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_pjsk-0.1.0/PKG-INFO` & `nonebot_plugin_pjsk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.1.0
+Version: 0.1.1
 Summary: PJSK表情包for Nonebot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 License: MIT
 Keywords: pjsk,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.1.1 Summary:
 PJSKè¡¨æåfor Nonebot2 Home-page: https://github.com/Agnes4m/
 nonebot_plugin_pjsk License: MIT Keywords: pjsk,nonebot2,plugin Author:
 Agnes_Digital Author-email: Z735803792@163.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

