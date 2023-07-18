# Comparing `tmp/mediaify-3.0.1.tar.gz` & `tmp/mediaify-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-3.0.1.tar", last modified: Wed Apr 26 00:08:51 2023, max compression
+gzip compressed data, was "mediaify-3.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mediaify-3.0.1.tar` & `mediaify-3.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1147 2023-04-26 00:08:32.929485 mediaify-3.0.1/LICENSE
--rw-r--r--   0        0        0     3830 2023-04-26 00:08:32.929485 mediaify-3.0.1/README.md
--rw-r--r--   0        0        0     1770 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/__init__.py
--rw-r--r--   0        0        0      198 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/__init__.py
--rw-r--r--   0        0        0     2397 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/encode.py
--rw-r--r--   0        0        0     1272 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/exports.py
--rw-r--r--   0        0        0     2559 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/formats.py
--rw-r--r--   0        0        0     1280 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/animation/utils.py
--rw-r--r--   0        0        0      143 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/__init__.py
--rw-r--r--   0        0        0      914 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/encode.py
--rw-r--r--   0        0        0      989 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/exports.py
--rw-r--r--   0        0        0     2046 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/audio/formats.py
--rw-r--r--   0        0        0     1243 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/animation.py
--rw-r--r--   0        0        0      884 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/audio.py
--rw-r--r--   0        0        0      599 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/base.py
--rw-r--r--   0        0        0     2119 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/codecs.py
--rw-r--r--   0        0        0     1387 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/image.py
--rw-r--r--   0        0        0      770 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/resize.py
--rw-r--r--   0        0        0      486 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/shared.py
--rw-r--r--   0        0        0     2418 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/configs/video.py
--rw-r--r--   0        0        0     3672 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/files.py
--rw-r--r--   0        0        0        0 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/format.py
--rw-r--r--   0        0        0      162 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/__init__.py
--rw-r--r--   0        0        0     1948 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/encode.py
--rw-r--r--   0        0        0     1149 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/exports.py
--rw-r--r--   0        0        0     2078 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/image/formats.py
--rw-r--r--   0        0        0      977 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/resize.py
--rw-r--r--   0        0        0      995 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/utils.py
--rw-r--r--   0        0        0      175 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/__init__.py
--rw-r--r--   0        0        0     2330 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/codecs.py
--rw-r--r--   0        0        0     1212 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/encode.py
--rw-r--r--   0        0        0     1424 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/exports.py
--rw-r--r--   0        0        0     2752 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/formats.py
--rw-r--r--   0        0        0     1303 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/info.py
--rw-r--r--   0        0        0     2822 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/process.py
--rw-r--r--   0        0        0     1451 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/summary.py
--rw-r--r--   0        0        0     1057 2023-04-26 00:08:33.045485 mediaify-3.0.1/mediaify/video/thumbnail.py
--rw-r--r--   0        0        0     1743 2023-04-26 00:08:33.045485 mediaify-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     5318 1970-01-01 00:00:00.000000 mediaify-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-07-18 09:25:04.806435 mediaify-3.0.2/LICENSE
+-rw-r--r--   0        0        0     3856 2023-07-18 09:25:04.806435 mediaify-3.0.2/README.md
+-rw-r--r--   0        0        0     1816 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/__init__.py
+-rw-r--r--   0        0        0      198 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/animation/__init__.py
+-rw-r--r--   0        0        0     2397 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/animation/encode.py
+-rw-r--r--   0        0        0     1272 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/animation/exports.py
+-rw-r--r--   0        0        0     2559 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/animation/formats.py
+-rw-r--r--   0        0        0     1280 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/animation/utils.py
+-rw-r--r--   0        0        0      143 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/audio/__init__.py
+-rw-r--r--   0        0        0      914 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/audio/encode.py
+-rw-r--r--   0        0        0      989 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/audio/exports.py
+-rw-r--r--   0        0        0     2046 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/audio/formats.py
+-rw-r--r--   0        0        0     1243 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/__init__.py
+-rw-r--r--   0        0        0     1021 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/animation.py
+-rw-r--r--   0        0        0      884 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/audio.py
+-rw-r--r--   0        0        0      599 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/base.py
+-rw-r--r--   0        0        0     2119 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/codecs.py
+-rw-r--r--   0        0        0     1387 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/image.py
+-rw-r--r--   0        0        0      770 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/resize.py
+-rw-r--r--   0        0        0      486 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/shared.py
+-rw-r--r--   0        0        0     2509 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/configs/video.py
+-rw-r--r--   0        0        0     3672 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/files.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/format.py
+-rw-r--r--   0        0        0      162 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/image/__init__.py
+-rw-r--r--   0        0        0     1948 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/image/encode.py
+-rw-r--r--   0        0        0     1149 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/image/exports.py
+-rw-r--r--   0        0        0     2078 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/image/formats.py
+-rw-r--r--   0        0        0      977 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/resize.py
+-rw-r--r--   0        0        0     1070 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/utils.py
+-rw-r--r--   0        0        0      175 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/__init__.py
+-rw-r--r--   0        0        0     2330 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/codecs.py
+-rw-r--r--   0        0        0     1212 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/encode.py
+-rw-r--r--   0        0        0     1424 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/exports.py
+-rw-r--r--   0        0        0     2752 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/formats.py
+-rw-r--r--   0        0        0     1303 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/info.py
+-rw-r--r--   0        0        0     2822 2023-07-18 09:25:04.922437 mediaify-3.0.2/mediaify/video/process.py
+-rw-r--r--   0        0        0     1451 2023-07-18 09:25:04.926437 mediaify-3.0.2/mediaify/video/summary.py
+-rw-r--r--   0        0        0     1057 2023-07-18 09:25:04.926437 mediaify-3.0.2/mediaify/video/thumbnail.py
+-rw-r--r--   0        0        0     1743 2023-07-18 09:25:04.926437 mediaify-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5344 1970-01-01 00:00:00.000000 mediaify-3.0.2/PKG-INFO
```

### Comparing `mediaify-3.0.1/LICENSE` & `mediaify-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/README.md` & `mediaify-3.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,35 +67,35 @@
     encoding=mediaify.WEBPImageFormat(
         resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=80,
     ),
 )
 preview = mediaify.VideoPreviewAnimationEncoding(
     encoding=mediaify.WEBPAnimationFormat(
+        resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=50,
         lossless=False,
-        resize=mediaify.TargetResolutionResize(width=640, height=360)
     ),
     framerate=5,
     frames=60,
 )
 video_360p = mediaify.WEBMFormat(
+    resize=mediaify.TargetResolutionResize(width=640, height=360),
     video_codec=mediaify.AV1Codec(crf=50, preset=7),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=640, height=360),
 )
 video_720p = mediaify.WEBMFormat(
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
     video_codec=mediaify.AV1Codec(crf=45, preset=6),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
 fallback = mediaify.MP4Format(
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
     video_codec=mediaify.H264Codec(crf=21, preset="medium"),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
 
 
 configs = [thumbnail, preview, video_360p, video_720p, fallback]
 with open('./examples/input/video.mp4', 'rb') as f:
     data = f.read()
 
@@ -137,13 +137,14 @@
 
 If you want any of these features to be developed, just flag an issue and I'll work on it.
 
 - New Encoders
     - [x] Video
         - [X] WEBM
         - [X] MP4
+        - [ ] DASH Video
         - [ ] Video to Animation
         - [ ] Video to Audio
     - [x] Audio Support
 - Better Resizing
     - [ ] Blackbars
     - [ ] Cropping
```

### Comparing `mediaify-3.0.1/mediaify/__init__.py` & `mediaify-3.0.2/mediaify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,19 @@
     AnimationFile,
 )
 from .video import (
     encode_video,
     batch_encode_video,
     VideoFile,
 )
+from .files import MediaFile
 
 __all__ = [
     "guess_type",
+    "MediaFile",
 
     "encode_audio",
     "batch_encode_audio",
     "AudioFile",
 
     "encode_image",
     "batch_encode_image",
```

### Comparing `mediaify-3.0.1/mediaify/animation/encode.py` & `mediaify-3.0.2/mediaify/animation/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/animation/exports.py` & `mediaify-3.0.2/mediaify/animation/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/animation/formats.py` & `mediaify-3.0.2/mediaify/animation/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/animation/utils.py` & `mediaify-3.0.2/mediaify/animation/utils.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/audio/encode.py` & `mediaify-3.0.2/mediaify/audio/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/audio/exports.py` & `mediaify-3.0.2/mediaify/audio/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/audio/formats.py` & `mediaify-3.0.2/mediaify/audio/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/__init__.py` & `mediaify-3.0.2/mediaify/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/animation.py` & `mediaify-3.0.2/mediaify/configs/animation.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/audio.py` & `mediaify-3.0.2/mediaify/configs/audio.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/base.py` & `mediaify-3.0.2/mediaify/configs/base.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/codecs.py` & `mediaify-3.0.2/mediaify/configs/codecs.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/image.py` & `mediaify-3.0.2/mediaify/configs/image.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/resize.py` & `mediaify-3.0.2/mediaify/configs/resize.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/configs/video.py` & `mediaify-3.0.2/mediaify/configs/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from .base import VideoFormat, AnimationFormat
 from . import (
     ResizeConfig,
     UnencodedEncoding,
     ThumbnailEncoding,
 )
 from . import H264Codec, OpusCodec, VP9Codec, AV1Codec
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Union
 
 
 @dataclass
 class WEBMFormat(VideoFormat):
     "Encode as a .webm video"
     resize: "ResizeConfig | None" = None
     "How to resize the video, None to disable resizing. Defaults to None."
     framerate: "float|None" = None
     """
     The framerate to encode the video at, None to use the original framerate.
     Defaults to None.
     """
-    video_codec: "VP9Codec|AV1Codec" = VP9Codec()
+    video_codec: "VP9Codec|AV1Codec" = field(default_factory=VP9Codec)
     "The video codec to use, defaults to VP9EncodeConfig"
-    audio_codec: "OpusCodec|None" = OpusCodec()
+    audio_codec: "OpusCodec|None" = field(default_factory=OpusCodec)
     "The audio codec to use, defaults to OpusEncodeConfig"
 
     def __repr__(self) -> str:
         if self.audio_codec is None:
             audio = ""
         else:
             audio = f" {self.audio_codec}"
@@ -44,17 +44,17 @@
     resize: "ResizeConfig | None" = None
     "How to resize the video, None to disable resizing. Defaults to None."
     framerate: "float|None" = None
     """
     The framerate to encode the video at, None to use the original framerate.
     Defaults to None.
     """
-    video_codec: "H264Codec|AV1Codec" = H264Codec()
+    video_codec: "H264Codec|AV1Codec" = field(default_factory=H264Codec)
     "The video codec to use, defaults to H264EncodeConfig"
-    audio_codec: "OpusCodec|None" = OpusCodec()
+    audio_codec: "OpusCodec|None" = field(default_factory=OpusCodec)
     "The audio codec to use, defaults to OpusEncodeConfig"
 
     def __repr__(self) -> str:
         if self.audio_codec is None:
             audio = ""
         else:
             audio = f" {self.audio_codec}"
```

### Comparing `mediaify-3.0.1/mediaify/files.py` & `mediaify-3.0.2/mediaify/files.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/image/encode.py` & `mediaify-3.0.2/mediaify/image/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/image/exports.py` & `mediaify-3.0.2/mediaify/image/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/image/formats.py` & `mediaify-3.0.2/mediaify/image/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/resize.py` & `mediaify-3.0.2/mediaify/resize.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/utils.py` & `mediaify-3.0.2/mediaify/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from magic import Magic
 import io
 from typing import Literal
 
 
 def is_animated_sequence(data: bytes) -> bool:
     pil_img = PILImage.open(io.BytesIO(data))
-    return pil_img.is_animated
+    if hasattr(pil_img, 'is_animated'):
+        return pil_img.is_animated
+    else:
+        return False
 
 
 def guess_mimetype(data: bytes) -> str:
     magic = Magic(mime=True)
     return magic.from_buffer(data)
```

### Comparing `mediaify-3.0.1/mediaify/video/codecs.py` & `mediaify-3.0.2/mediaify/video/codecs.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/encode.py` & `mediaify-3.0.2/mediaify/video/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/exports.py` & `mediaify-3.0.2/mediaify/video/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/formats.py` & `mediaify-3.0.2/mediaify/video/formats.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/info.py` & `mediaify-3.0.2/mediaify/video/info.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/process.py` & `mediaify-3.0.2/mediaify/video/process.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/summary.py` & `mediaify-3.0.2/mediaify/video/summary.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/mediaify/video/thumbnail.py` & `mediaify-3.0.2/mediaify/video/thumbnail.py`

 * *Files identical despite different names*

### Comparing `mediaify-3.0.1/pyproject.toml` & `mediaify-3.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "3.0.1"
+version = "3.0.2"
 description = "Media encoding made simple"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
```

### Comparing `mediaify-3.0.1/PKG-INFO` & `mediaify-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaify
-Version: 3.0.1
+Version: 3.0.2
 Summary: Media encoding made simple
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -105,35 +105,35 @@
     encoding=mediaify.WEBPImageFormat(
         resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=80,
     ),
 )
 preview = mediaify.VideoPreviewAnimationEncoding(
     encoding=mediaify.WEBPAnimationFormat(
+        resize=mediaify.TargetResolutionResize(width=640, height=360),
         quality=50,
         lossless=False,
-        resize=mediaify.TargetResolutionResize(width=640, height=360)
     ),
     framerate=5,
     frames=60,
 )
 video_360p = mediaify.WEBMFormat(
+    resize=mediaify.TargetResolutionResize(width=640, height=360),
     video_codec=mediaify.AV1Codec(crf=50, preset=7),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=640, height=360),
 )
 video_720p = mediaify.WEBMFormat(
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
     video_codec=mediaify.AV1Codec(crf=45, preset=6),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
 fallback = mediaify.MP4Format(
+    resize=mediaify.TargetResolutionResize(width=1280, height=720),
     video_codec=mediaify.H264Codec(crf=21, preset="medium"),
     audio_codec=mediaify.OpusCodec(bitrate=128_000),
-    resize=mediaify.TargetResolutionResize(width=1280, height=720),
 )
 
 
 configs = [thumbnail, preview, video_360p, video_720p, fallback]
 with open('./examples/input/video.mp4', 'rb') as f:
     data = f.read()
 
@@ -175,14 +175,15 @@
 
 If you want any of these features to be developed, just flag an issue and I'll work on it.
 
 - New Encoders
     - [x] Video
         - [X] WEBM
         - [X] MP4
+        - [ ] DASH Video
         - [ ] Video to Animation
         - [ ] Video to Audio
     - [x] Audio Support
 - Better Resizing
     - [ ] Blackbars
     - [ ] Cropping
```

