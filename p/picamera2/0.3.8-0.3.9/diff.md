# Comparing `tmp/picamera2-0.3.8.tar.gz` & `tmp/picamera2-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picamera2-0.3.8.tar", last modified: Thu Jan  5 14:58:34 2023, max compression
+gzip compressed data, was "picamera2-0.3.9.tar", last modified: Wed Mar  1 13:40:32 2023, max compression
```

## Comparing `picamera2-0.3.8.tar` & `picamera2-0.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.033145 picamera2-0.3.8/
--rw-rw-r--   0 david     (1000) david     (1000)     1322 2022-02-11 12:42:32.000000 picamera2-0.3.8/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-01-05 14:58:34.033145 picamera2-0.3.8/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6436 2023-01-05 14:53:32.000000 picamera2-0.3.8/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.029145 picamera2-0.3.8/picamera2/
--rw-rw-r--   0 david     (1000) david     (1000)      846 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4885 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/configuration.py
--rw-rw-r--   0 david     (1000) david     (1000)     3331 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/controls.py
--rw-rw-r--   0 david     (1000) david     (1000)     1173 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/converters.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.033145 picamera2-0.3.8/picamera2/encoders/
--rw-rw-r--   0 david     (1000) david     (1000)      194 2022-07-05 09:46:46.000000 picamera2-0.3.8/picamera2/encoders/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     5647 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/encoders/encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     1714 2022-12-01 09:14:04.000000 picamera2-0.3.8/picamera2/encoders/h264_encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     1943 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/encoders/jpeg_encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     1244 2022-12-01 09:14:04.000000 picamera2-0.3.8/picamera2/encoders/mjpeg_encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     2346 2022-12-01 09:14:04.000000 picamera2-0.3.8/picamera2/encoders/multi_encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     9174 2022-12-01 09:14:04.000000 picamera2-0.3.8/picamera2/encoders/v4l2_encoder.py
--rw-rw-r--   0 david     (1000) david     (1000)     1143 2022-12-01 09:14:04.000000 picamera2-0.3.8/picamera2/formats.py
--rw-rw-r--   0 david     (1000) david     (1000)     2921 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/job.py
--rw-rw-r--   0 david     (1000) david     (1000)      229 2022-07-05 09:46:46.000000 picamera2-0.3.8/picamera2/metadata.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.033145 picamera2-0.3.8/picamera2/outputs/
--rw-rw-r--   0 david     (1000) david     (1000)      144 2022-07-05 09:46:46.000000 picamera2-0.3.8/picamera2/outputs/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3188 2022-11-28 09:00:20.000000 picamera2-0.3.8/picamera2/outputs/circularoutput.py
--rw-rw-r--   0 david     (1000) david     (1000)     4189 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/outputs/ffmpegoutput.py
--rw-rw-r--   0 david     (1000) david     (1000)     4191 2022-11-28 09:00:20.000000 picamera2-0.3.8/picamera2/outputs/fileoutput.py
--rw-rw-r--   0 david     (1000) david     (1000)     1658 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/outputs/output.py
--rw-rw-r--   0 david     (1000) david     (1000)    74218 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/picamera2.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.033145 picamera2-0.3.8/picamera2/previews/
--rw-rw-r--   0 david     (1000) david     (1000)      122 2022-07-05 09:46:46.000000 picamera2-0.3.8/picamera2/previews/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     9006 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/drm_preview.py
--rw-rw-r--   0 david     (1000) david     (1000)     2109 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/gl_helpers.py
--rw-rw-r--   0 david     (1000) david     (1000)     2878 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/null_preview.py
--rw-rw-r--   0 david     (1000) david     (1000)    16667 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/q_gl_picamera2.py
--rw-rw-r--   0 david     (1000) david     (1000)     7815 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/q_picamera2.py
--rw-rw-r--   0 david     (1000) david     (1000)       87 2022-07-05 09:46:46.000000 picamera2-0.3.8/picamera2/previews/qt.py
--rw-rw-r--   0 david     (1000) david     (1000)     5197 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/previews/qt_previews.py
--rw-rw-r--   0 david     (1000) david     (1000)    12816 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/request.py
--rw-rw-r--   0 david     (1000) david     (1000)     1226 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/sensor_format.py
--rw-rw-r--   0 david     (1000) david     (1000)      426 2023-01-05 14:53:32.000000 picamera2-0.3.8/picamera2/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-01-05 14:58:34.029145 picamera2-0.3.8/picamera2.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-01-05 14:58:34.000000 picamera2-0.3.8/picamera2.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     1096 2023-01-05 14:58:34.000000 picamera2-0.3.8/picamera2.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-01-05 14:58:34.000000 picamera2-0.3.8/picamera2.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       85 2023-01-05 14:58:34.000000 picamera2-0.3.8/picamera2.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2023-01-05 14:58:34.000000 picamera2-0.3.8/picamera2.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-01-05 14:58:34.033145 picamera2-0.3.8/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     1417 2023-01-05 14:53:32.000000 picamera2-0.3.8/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/
+-rw-rw-r--   0 david     (1000) david     (1000)     1322 2022-02-11 12:42:32.000000 picamera2-0.3.9/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-03-01 13:40:32.902015 picamera2-0.3.9/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6436 2023-01-31 13:03:18.000000 picamera2-0.3.9/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/picamera2/
+-rw-rw-r--   0 david     (1000) david     (1000)      846 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4885 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/configuration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3331 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/controls.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1173 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/converters.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/picamera2/encoders/
+-rw-rw-r--   0 david     (1000) david     (1000)      194 2022-07-05 09:46:46.000000 picamera2-0.3.9/picamera2/encoders/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6231 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/encoders/encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3641 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/encoders/h264_encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2162 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/encoders/jpeg_encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1184 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/encoders/mjpeg_encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2346 2022-12-01 09:14:04.000000 picamera2-0.3.9/picamera2/encoders/multi_encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9837 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/encoders/v4l2_encoder.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1143 2022-12-01 09:14:04.000000 picamera2-0.3.9/picamera2/formats.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2921 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/job.py
+-rw-rw-r--   0 david     (1000) david     (1000)      229 2022-07-05 09:46:46.000000 picamera2-0.3.9/picamera2/metadata.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/picamera2/outputs/
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2022-07-05 09:46:46.000000 picamera2-0.3.9/picamera2/outputs/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3175 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/outputs/circularoutput.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4192 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/outputs/ffmpegoutput.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4304 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/outputs/fileoutput.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1658 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/outputs/output.py
+-rw-rw-r--   0 david     (1000) david     (1000)    74418 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/picamera2.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/picamera2/previews/
+-rw-rw-r--   0 david     (1000) david     (1000)      122 2022-07-05 09:46:46.000000 picamera2-0.3.9/picamera2/previews/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9006 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/previews/drm_preview.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2109 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/previews/gl_helpers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2878 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/previews/null_preview.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16667 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/previews/q_gl_picamera2.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7986 2023-03-01 13:36:34.000000 picamera2-0.3.9/picamera2/previews/q_picamera2.py
+-rw-rw-r--   0 david     (1000) david     (1000)      583 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/previews/qt.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5197 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/previews/qt_previews.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13072 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/request.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1226 2023-01-31 13:03:18.000000 picamera2-0.3.9/picamera2/sensor_format.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1532 2023-03-01 13:36:39.000000 picamera2-0.3.9/picamera2/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-03-01 13:40:32.902015 picamera2-0.3.9/picamera2.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     7276 2023-03-01 13:40:32.000000 picamera2-0.3.9/picamera2.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     1096 2023-03-01 13:40:32.000000 picamera2-0.3.9/picamera2.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-03-01 13:40:32.000000 picamera2-0.3.9/picamera2.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       85 2023-03-01 13:40:32.000000 picamera2-0.3.9/picamera2.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2023-03-01 13:40:32.000000 picamera2-0.3.9/picamera2.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-03-01 13:40:32.902015 picamera2-0.3.9/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     1417 2023-03-01 13:36:39.000000 picamera2-0.3.9/setup.py
```

### Comparing `picamera2-0.3.8/LICENSE` & `picamera2-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/PKG-INFO` & `picamera2-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picamera2
-Version: 0.3.8
+Version: 0.3.9
 Summary: The libcamera-based Python interface to Raspberry Pi cameras, based on the original Picamera library
 Home-page: https://github.com/RaspberryPi/picamera2
 Author: Raspberry Pi & Raspberry Pi Foundation
 Author-email: picamera2@raspberrypi.com
 License: BSD 2-Clause License
 Project-URL: Bug Tracker, https://github.com/RaspberryPi/picamera2/issues
 Platform: UNKNOWN
```

### Comparing `picamera2-0.3.8/README.md` & `picamera2-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/__init__.py` & `picamera2-0.3.9/picamera2/__init__.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/configuration.py` & `picamera2-0.3.9/picamera2/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             target = self._FORWARD_FIELDS[name]
             self.__getattribute__(target).__setattr__(name, value)
         elif name in self._ALLOWED_FIELDS:
             if name in self._FIELD_CLASS_MAP and isinstance(value, dict):
                 value = self._FIELD_CLASS_MAP[name](value)
             super().__setattr__(name, value)
         else:
-            raise RuntimeError(f"Invalid field '{name}'")
+            raise RuntimeError(f"Invalid field {name!r}")
 
     def __getattribute__(self, name):
         if name in super().__getattribute__("_FORWARD_FIELDS"):
             return super().__getattribute__(self._FORWARD_FIELDS[name]).__getattribute__(name)
         else:
             return super().__getattribute__(name)
```

### Comparing `picamera2-0.3.8/picamera2/controls.py` & `picamera2-0.3.9/picamera2/controls.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/converters.py` & `picamera2-0.3.9/picamera2/converters.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/encoders/encoder.py` & `picamera2-0.3.9/picamera2/encoders/encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         self._format = None
         self._output = []
         self._running = False
         self._lock = threading.Lock()
         self.firsttimestamp = None
 
     @property
+    def running(self):
+        return self._running
+
+    @property
     def width(self):
         """Gets width
 
         :return: Width of frames
         :rtype: int
         """
         return self._width
@@ -77,14 +81,35 @@
         :raises RuntimeError: Failed to set height
         """
         if not isinstance(value, int):
             raise RuntimeError("Height must be integer")
         self._height = value
 
     @property
+    def size(self):
+        """Gets size
+
+        :return: Size of frames as (width, height)
+        :rtype: tuple
+        """
+        return (self._width, self._height)
+
+    @size.setter
+    def size(self, value):
+        """Sets size
+
+        :param value: Size
+        :type value: tuple
+        :raises RuntimeError: Failed to set size
+        """
+        if not isinstance(value, tuple) or len(value) != 2:
+            raise RuntimeError("Size must be a tuple of two integers")
+        self.width, self.height = value
+
+    @property
     def stride(self):
         """Gets stride
 
         :return: Stride
         :rtype: int
         """
         return self._stride
@@ -123,19 +148,16 @@
         elif value == "YUV420":
             self._format = V4L2_PIX_FMT_YUV420
         elif value == "XBGR8888":
             self._format = V4L2_PIX_FMT_BGR32
         elif value == "XRGB8888":
             self._format = V4L2_PIX_FMT_RGBA32
         else:
-            if type(self) is Encoder:
-                formats.assert_format_valid(value)
-                self._format = value
-            else:
-                raise RuntimeError("Invalid format")
+            formats.assert_format_valid(value)
+            self._format = value
 
     @property
     def output(self):
         """Gets output objects
 
         :return: Output object list or single Output object
         :rtype: List[Output]
@@ -190,14 +212,16 @@
             self._start()
 
     def _start(self):
         pass
 
     def stop(self):
         with self._lock:
+            if not self._running:
+                raise RuntimeError("Encoder already stopped")
             self._running = False
             for out in self._output:
                 out.stop()
             self._stop()
 
     def _stop(self):
         pass
```

### Comparing `picamera2-0.3.8/picamera2/encoders/h264_encoder.py` & `picamera2-0.3.9/picamera2/encoders/mjpeg_encoder.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,33 @@
-"""H264 encoder functionality"""
+"""MJPEG encoder functionality utilising V4L2"""
 
 from math import sqrt
 
-from v4l2 import (V4L2_CID_MPEG_VIDEO_H264_I_PERIOD,
-                  V4L2_CID_MPEG_VIDEO_REPEAT_SEQ_HEADER, V4L2_PIX_FMT_H264)
+from v4l2 import V4L2_PIX_FMT_MJPEG
 
 from picamera2.encoders import Quality
 from picamera2.encoders.v4l2_encoder import V4L2Encoder
 
 
-class H264Encoder(V4L2Encoder):
-    """Uses functionality from V4L2Encoder"""
+class MJPEGEncoder(V4L2Encoder):
+    """MJPEG encoder utilsing V4L2 functionality"""
 
-    def __init__(self, bitrate=None, repeat=True, iperiod=None):
-        """H264 Encoder
+    def __init__(self, bitrate=None):
+        """Creates MJPEG encoder
 
         :param bitrate: Bitrate, default None
         :type bitrate: int
-        :param repeat: Repeat seq header, defaults to True
-        :type repeat: bool, optional
-        :param iperiod: Iperiod, defaults to None
-        :type iperiod: int, optional
         """
-        super().__init__(bitrate, V4L2_PIX_FMT_H264)
-        if iperiod is not None:
-            self._controls += [(V4L2_CID_MPEG_VIDEO_H264_I_PERIOD, iperiod)]
-        if repeat:
-            self._controls += [(V4L2_CID_MPEG_VIDEO_REPEAT_SEQ_HEADER, 1)]
+        super().__init__(bitrate, V4L2_PIX_FMT_MJPEG)
 
     def _setup(self, quality):
-        if self._requested_bitrate is None:
+        if getattr(self, "bitrate", None) is None:
             # These are suggested bitrates for 1080p30 in Mbps
-            BITRATE_TABLE = {Quality.VERY_LOW: 2,
-                             Quality.LOW: 4,
-                             Quality.MEDIUM: 6,
-                             Quality.HIGH: 9,
-                             Quality.VERY_HIGH: 15}
+            BITRATE_TABLE = {Quality.VERY_LOW: 6,
+                             Quality.LOW: 12,
+                             Quality.MEDIUM: 18,
+                             Quality.HIGH: 27,
+                             Quality.VERY_HIGH: 45}
             reference_complexity = 1920 * 1080 * 30
             actual_complexity = self.width * self.height * self.framerate
             reference_bitrate = BITRATE_TABLE[quality] * 1000000
-            self._bitrate = int(reference_bitrate * sqrt(actual_complexity / reference_complexity))
-        else:
-            self._bitrate = self._requested_bitrate
+            self.bitrate = int(reference_bitrate * sqrt(actual_complexity / reference_complexity))
```

### Comparing `picamera2-0.3.8/picamera2/encoders/jpeg_encoder.py` & `picamera2-0.3.9/picamera2/encoders/jpeg_encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,50 +5,55 @@
 from picamera2.encoders import Quality
 from picamera2.encoders.multi_encoder import MultiEncoder
 
 
 class JpegEncoder(MultiEncoder):
     """Uses functionality from MultiEncoder"""
 
-    def __init__(self, num_threads=4, q=None, colour_space='RGBX', colour_subsampling='420'):
+    FORMAT_TABLE = {"XBGR8888": "RGBX",
+                    "XRGB8888": "BGRX",
+                    "BGR888": "RGB",
+                    "RGB888": "BGR"}
+
+    def __init__(self, num_threads=4, q=None, colour_space=None, colour_subsampling='420'):
         """Initialises Jpeg encoder
 
         :param num_threads: Number of threads to use, defaults to 4
         :type num_threads: int, optional
         :param q: Quality, defaults to None
         :type q: int, optional
         :param colour_space: Colour space, defaults to 'RGBX'
         :type colour_space: str, optional
         :param colour_subsampling: Colour subsampling, allows choice of YUV420, YUV422 or YUV444
             outputs. Defaults to '420'.
         :type colour_subsampling: str, optional
         """
         super().__init__(num_threads=num_threads)
-        self.requested_q = q
+        self.q = q
         self.colour_space = colour_space
         self.colour_subsampling = colour_subsampling
 
     def encode_func(self, request, name):
         """Performs encoding
 
         :param request: Request
         :type request: request
         :param name: Name
         :type name: str
         :return: Jpeg image
         :rtype: bytes
         """
+        if self.colour_space is None:
+            self.colour_space = self.FORMAT_TABLE[request.config[name]["format"]]
         array = request.make_array(name)
         return simplejpeg.encode_jpeg(array, quality=self.q, colorspace=self.colour_space,
                                       colorsubsampling=self.colour_subsampling)
 
     def _setup(self, quality):
-        if self.requested_q is None:
+        if getattr(self, "q", None) is None:
             # Image size and framerate isn't an issue here, you just get what you get.
             Q_TABLE = {Quality.VERY_LOW: 20,
                        Quality.LOW: 40,
                        Quality.MEDIUM: 60,
                        Quality.HIGH: 75,
                        Quality.VERY_HIGH: 90}
             self.q = Q_TABLE[quality]
-        else:
-            self.q = self.requested_q
```

### Comparing `picamera2-0.3.8/picamera2/encoders/multi_encoder.py` & `picamera2-0.3.9/picamera2/encoders/multi_encoder.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/encoders/v4l2_encoder.py` & `picamera2-0.3.9/picamera2/encoders/v4l2_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,36 +22,38 @@
         :type bitrate: int
         :param pixformat: Pixel format
         :type pixformat: int
         """
         super().__init__()
         self.bufs = {}
         # The encoder's _setup method will calculate the final bitrate.
-        self._requested_bitrate = bitrate
+        self.bitrate = bitrate
         self._pixformat = pixformat
         self._controls = []
         self.vd = None
+        self._framerate = None
 
     def _start(self):
         self.vd = open('/dev/video11', 'rb+', buffering=0)
 
         self.buf_available = queue.Queue()
         self.buf_frame = queue.Queue()
 
         self.thread = threading.Thread(target=self.thread_poll, args=(self.buf_available,))
         self.thread.setDaemon(True)
         self.thread.start()
 
         cp = v4l2_capability()
         fcntl.ioctl(self.vd, VIDIOC_QUERYCAP, cp)
 
-        ctrl = v4l2_control()
-        ctrl.id = V4L2_CID_MPEG_VIDEO_BITRATE
-        ctrl.value = self._bitrate
-        fcntl.ioctl(self.vd, VIDIOC_S_CTRL, ctrl)
+        if self.bitrate is not None:
+            ctrl = v4l2_control()
+            ctrl.id = V4L2_CID_MPEG_VIDEO_BITRATE
+            ctrl.value = self.bitrate
+            fcntl.ioctl(self.vd, VIDIOC_S_CTRL, ctrl)
 
         fmt = v4l2_format()
         fmt.type = V4L2_BUF_TYPE_VIDEO_OUTPUT_MPLANE
         fmt.fmt.pix_mp.width = self._width
         fmt.fmt.pix_mp.height = self._height
         fmt.fmt.pix_mp.pixelformat = self.format
         fmt.fmt.pix_mp.plane_fmt[0].bytesperline = self.stride
@@ -68,14 +70,24 @@
         fmt.fmt.pix_mp.field = V4L2_FIELD_ANY
         fmt.fmt.pix_mp.colorspace = V4L2_COLORSPACE_DEFAULT
         fmt.fmt.pix_mp.num_planes = 1
         fmt.fmt.pix_mp.plane_fmt[0].bytesperline = 0
         fmt.fmt.pix_mp.plane_fmt[0].sizeimage = 512 << 10
         fcntl.ioctl(self.vd, VIDIOC_S_FMT, fmt)
 
+        if self._framerate is not None and self._enable_framerate:
+            # Some codecs, such as H264, support this parameter. Our other codecs do not,
+            # and do not allow you to set the _framerate property.
+            sparm = v4l2_streamparm()
+            sparm.type = V4L2_BUF_TYPE_VIDEO_OUTPUT_MPLANE
+            sparm.parm.output.capabilities = V4L2_CAP_TIMEPERFRAME
+            sparm.parm.output.timeperframe.numerator = 1000
+            sparm.parm.output.timeperframe.denominator = round(self._framerate * 1000)
+            fcntl.ioctl(self.vd, VIDIOC_S_PARM, sparm)
+
         if len(self._controls) > 0:
             controlarr = (v4l2_ext_control * len(self._controls))()
             ext = v4l2_ext_controls()
             for i, tup in enumerate(self._controls):
                 idv, value = tup
                 controlarr[i].id = idv
                 controlarr[i].value = value
```

### Comparing `picamera2-0.3.8/picamera2/formats.py` & `picamera2-0.3.9/picamera2/formats.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/job.py` & `picamera2-0.3.9/picamera2/job.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/outputs/circularoutput.py` & `picamera2-0.3.9/picamera2/outputs/circularoutput.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,22 +69,21 @@
             else:
                 with self._lock:
                     frame, keyframe = self._circular.popleft()
                 self._write(frame, timestamp)
 
     def stop(self):
         """Close file handle and prevent recording"""
-        self.recording = False
-        key = False
+        if not self.recording or self._fileoutput is None:
+            return
         with self._lock:
             while self._circular:
                 frame, keyframe = self._circular.popleft()
-                if not self.outputtofile:
-                    if not key:
-                        if keyframe:
-                            self._write(frame)
-                            key = True
-                    else:
+                if self._firstframe:
+                    if keyframe:
                         self._write(frame)
+                        self._firstframe = False
                 else:
                     self._write(frame)
+        self.recording = False
+        self._firstframe = False
         self.close()
```

### Comparing `picamera2-0.3.8/picamera2/outputs/ffmpegoutput.py` & `picamera2-0.3.9/picamera2/outputs/ffmpegoutput.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                        '-i', '-']
         video_codec = ['-c:v', 'copy']
         audio_input = []
         audio_codec = []
         if self.audio:
             audio_input = ['-itsoffset', str(self.audio_sync),
                            '-f', 'pulse',
-                           '-sample_rate', str(self.audio_bitrate),
+                           '-sample_rate', str(self.audio_samplerate),
                            '-thread_queue_size', '512',  # necessary to prevent warnings
                            '-i', self.audio_device]
             audio_codec = ['-b:a', str(self.audio_bitrate),
                            '-c:a', self.audio_codec]
 
         command = ['ffmpeg'] + general_options + audio_input + video_input + \
             audio_codec + video_codec + self.output_filename.split()
```

### Comparing `picamera2-0.3.8/picamera2/outputs/fileoutput.py` & `picamera2-0.3.9/picamera2/outputs/fileoutput.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,19 +34,21 @@
         return self._fileoutput
 
     @fileoutput.setter
     def fileoutput(self, file):
         """Change file to output frames to"""
         self._split = False
         self._firstframe = True
+        self._needs_close = False
         if file is None:
             self._fileoutput = None
         else:
             if isinstance(file, str):
                 self._fileoutput = open(file, "wb")
+                self._needs_close = True
             elif isinstance(file, io.BufferedIOBase):
                 self._fileoutput = file
             else:
                 raise RuntimeError("Must pass io.BufferedIOBase")
             if hasattr(self._fileoutput, "raw") and isinstance(self._fileoutput.raw, socket.SocketIO) and \
                     self._fileoutput.raw._sock.type == socket.SocketKind.SOCK_DGRAM:
                 self._split = True
@@ -91,15 +93,16 @@
         """Close file handle and prevent recording"""
         super().stop()
         self.close()
 
     def close(self):
         """Closes all files"""
         try:
-            self._fileoutput.close()
+            if self._needs_close:
+                self._fileoutput.close()
         except (ConnectionResetError, ConnectionRefusedError, BrokenPipeError) as e:
             self.dead = True
             if self._connectiondead is not None:
                 self._connectiondead(e)
 
     def _write(self, frame, timestamp=None):
         try:
```

### Comparing `picamera2-0.3.8/picamera2/outputs/output.py` & `picamera2-0.3.9/picamera2/outputs/output.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/picamera2.py` & `picamera2-0.3.9/picamera2/picamera2.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 
 import libcamera
 import numpy as np
 from libcamera import controls
 from PIL import Image
 
 import picamera2.formats as formats
+import picamera2.utils as utils
 from picamera2.encoders import Encoder, H264Encoder, MJPEGEncoder, Quality
 from picamera2.outputs import FfmpegOutput, FileOutput
 from picamera2.previews import DrmPreview, NullPreview, QtGlPreview, QtPreview
 
 from .configuration import CameraConfiguration
 from .controls import Controls
 from .job import Job
 from .request import CompletedRequest, Helpers
 from .sensor_format import SensorFormat
-from .utils import convert_from_libcamera_type
 
 STILL = libcamera.StreamRole.StillCapture
 RAW = libcamera.StreamRole.Raw
 VIDEO = libcamera.StreamRole.VideoRecording
 VIEWFINDER = libcamera.StreamRole.Viewfinder
 
 _log = logging.getLogger(__name__)
@@ -324,15 +324,17 @@
         :return: Camera properties
         :rtype: dict
         """
         return {} if self.camera is None else self.camera_properties_
 
     @property
     def camera_controls(self) -> dict:
-        return {k: (v[1].min, v[1].max, v[1].default) for k, v in self.camera_ctrl_info.items()}
+        return {k: (utils.convert_from_libcamera_type(v[1].min),
+                    utils.convert_from_libcamera_type(v[1].max),
+                    utils.convert_from_libcamera_type(v[1].default)) for k, v in self.camera_ctrl_info.items()}
 
     @property
     def title_fields(self):
         """The metadata fields reported in the title bar of any preview window."""
         return self._title_fields
 
     @title_fields.setter
@@ -406,15 +408,15 @@
         self.__identify_camera()
         # Re-generate the controls list to someting easer to use.
         for k, v in self.camera.controls.items():
             self.camera_ctrl_info[k.name] = (k, v)
 
         # Re-generate the properties list to someting easer to use.
         for k, v in self.camera.properties.items():
-            self.camera_properties_[k.name] = convert_from_libcamera_type(v)
+            self.camera_properties_[k.name] = utils.convert_from_libcamera_type(v)
 
         # These next lines could be placed elsewhere?
         raw_mode = self.camera.generate_configuration([RAW]).at(0)
         self.sensor_resolution = (raw_mode.size.width, raw_mode.size.height)
         self.sensor_format = str(raw_mode.pixel_format)
 
         _log.info('Initialization successful.')
@@ -590,15 +592,15 @@
             if isinstance(value, SensorFormat):
                 value = str(value)
             if key in valid:
                 stream_config[key] = value
             elif key in ignore_list:
                 pass  # allows us to pass items from the sensor_modes as a raw stream
             else:
-                raise ValueError(f"Bad key '{key}': valid stream configuration keys are {valid}")
+                raise ValueError(f"Bad key {key!r}: valid stream configuration keys are {valid}")
         return stream_config
 
     @staticmethod
     def _add_display_and_encode(config, display, encode) -> None:
         if display is not None and config.get(display, None) is None:
             raise RuntimeError(f"Display stream {display} was not defined")
         if encode is not None and config.get(encode, None) is None:
@@ -675,19 +677,15 @@
         self.align_stream(main, optimal=False)
         lores = self._make_initial_stream_config({"format": "YUV420", "size": main["size"]}, lores)
         if lores is not None:
             self.align_stream(lores, optimal=False)
         raw = self._make_initial_stream_config({"format": self.sensor_format, "size": main["size"]}, raw)
         if colour_space is None:
             # Choose default colour space according to the video resolution.
-            if formats.is_RGB(main["format"]):
-                # There's a bug down in some driver where it won't accept anything other than
-                # sRGB or JPEG as the colour space for an RGB stream. So until that is fixed:
-                colour_space = libcamera.ColorSpace.Sycc()
-            elif main["size"][0] < 1280 or main["size"][1] < 720:
+            if main["size"][0] < 1280 or main["size"][1] < 720:
                 colour_space = libcamera.ColorSpace.Smpte170m()
             else:
                 colour_space = libcamera.ColorSpace.Rec709()
         if "NoiseReductionMode" in self.camera_controls and "FrameDurationLimits" in self.camera_controls:
             controls = {"NoiseReductionMode": libcamera.controls.draft.NoiseReductionModeEnum.Fast,
                         "FrameDurationLimits": (33333, 33333)} | controls
         config = {"use_case": "video",
@@ -730,15 +728,15 @@
         if size[0] % 2 or size[1] % 2:
             raise RuntimeError("width and height should be even")
 
     def check_camera_config(self, camera_config: dict) -> None:
         required_keys = ["colour_space", "transform", "main", "lores", "raw"]
         for name in required_keys:
             if name not in camera_config:
-                raise RuntimeError(f"'{name}' key expected in camera configuration")
+                raise RuntimeError(f"{name!r} key expected in camera configuration")
 
         # Check the entire camera configuration for errors.
         if not isinstance(camera_config["colour_space"], libcamera._libcamera.ColorSpace):
             raise RuntimeError("Colour space has incorrect type")
         if not isinstance(camera_config["transform"], libcamera._libcamera.Transform):
             raise RuntimeError("Transform has incorrect type")
 
@@ -782,17 +780,20 @@
 
         # Make the libcamera configuration, and then we'll write all our parameters over
         # the ones it gave us.
         libcamera_config = self.camera.generate_configuration(roles)
         libcamera_config.transform = camera_config["transform"]
         buffer_count = camera_config["buffer_count"]
         self._update_libcamera_stream_config(libcamera_config.at(self.main_index), camera_config["main"], buffer_count)
-        libcamera_config.at(self.main_index).color_space = camera_config["colour_space"]
+        libcamera_config.at(self.main_index).color_space = utils.colour_space_to_libcamera(
+            camera_config["colour_space"],
+            camera_config["main"]["format"])
         if self.lores_index >= 0:
             self._update_libcamera_stream_config(libcamera_config.at(self.lores_index), camera_config["lores"], buffer_count)
+            # Must be YUV, so no need for colour_space_to_libcamera.
             libcamera_config.at(self.lores_index).color_space = camera_config["colour_space"]
         if self.raw_index >= 0:
             self._update_libcamera_stream_config(libcamera_config.at(self.raw_index), camera_config["raw"], buffer_count)
             libcamera_config.at(self.raw_index).color_space = libcamera.ColorSpace.Raw()
 
         return libcamera_config
 
@@ -852,15 +853,15 @@
 
         :param camera_config: Camera configuration
         :type camera_config: dict
         :param libcamera_config: libcamera configuration
         :type libcamera_config: dict
         """
         camera_config["transform"] = libcamera_config.transform
-        camera_config["colour_space"] = libcamera_config.at(0).color_space
+        camera_config["colour_space"] = utils.colour_space_from_libcamera(libcamera_config.at(0).color_space)
         self._update_stream_config(camera_config["main"], libcamera_config.at(0))
         if self.lores_index >= 0:
             self._update_stream_config(camera_config["lores"], libcamera_config.at(self.lores_index))
         if self.raw_index >= 0:
             self._update_stream_config(camera_config["raw"], libcamera_config.at(self.raw_index))
 
     def configure_(self, camera_config="preview") -> None:
@@ -868,14 +869,16 @@
 
         :param camera_config: Configuration, defaults to the 'preview' configuration
         :type camera_config: dict, string or CameraConfiguration, optional
         :raises RuntimeError: Failed to configure
         """
         if self.started:
             raise RuntimeError("Camera must be stopped before configuring")
+        if self.encoder is not None and self.encoder.running:
+            raise RuntimeError("Encoder must be stopped before configuring")
         initial_config = camera_config
         if isinstance(initial_config, str):
             if initial_config == "preview":
                 camera_config = self.preview_configuration
             elif initial_config == "still":
                 camera_config = self.still_configuration
             else:
@@ -915,15 +918,15 @@
 
         # Update the controls and properties list as some of the values may have changed.
         self.camera_ctrl_info = {}
         self.camera_properties_ = {}
         for k, v in self.camera.controls.items():
             self.camera_ctrl_info[k.name] = (k, v)
         for k, v in self.camera.properties.items():
-            self.camera_properties_[k.name] = convert_from_libcamera_type(v)
+            self.camera_properties_[k.name] = utils.convert_from_libcamera_type(v)
 
         # Record which libcamera stream goes with which of our names.
         self.stream_map = {"main": libcamera_config.at(0).stream}
         self.stream_map["lores"] = libcamera_config.at(self.lores_index).stream if self.lores_index >= 0 else None
         self.stream_map["raw"] = libcamera_config.at(self.raw_index).stream if self.raw_index >= 0 else None
         _log.debug(f"Streams: {self.stream_map}")
 
@@ -963,15 +966,15 @@
         if initial_config == "preview":
             self.preview_configuration.update(camera_config)
         elif initial_config == "still":
             self.still_configuration.update(camera_config)
         else:
             self.video_configuration.update(camera_config)
         # Set the controls directly so as to overwrite whatever is there.
-        self.controls.set_controls(self.camera_config['controls'])
+        self.controls = Controls(self, controls=self.camera_config['controls'])
         self.configure_count += 1
 
     def configure(self, camera_config="preview") -> None:
         """Configure the camera system with the given configuration."""
         self.configure_(camera_config)
 
     def camera_configuration(self) -> dict:
@@ -1425,15 +1428,15 @@
         def capture_image_and_switch_back_(self, preview_config, name) -> Image:
             _, result = self.capture_image_(name)
             self.switch_mode_(preview_config)
             return (True, result)
 
         functions = [partial(self.switch_mode_, camera_config),
                      partial(capture_image_and_switch_back_, self, preview_config, name)]
-        self.dispatch_functions(functions, wait, signal_function)
+        return self.dispatch_functions(functions, wait, signal_function)
 
     def start_encoder(self, encoder=None, output=None, pts=None, quality=Quality.MEDIUM) -> None:
         """Start encoder
 
         :param encoder: Sets encoder or uses existing, defaults to None
         :type encoder: Encoder, optional
         :raises RuntimeError: No encoder set or no stream
```

### Comparing `picamera2-0.3.8/picamera2/previews/drm_preview.py` & `picamera2-0.3.9/picamera2/previews/drm_preview.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/previews/gl_helpers.py` & `picamera2-0.3.9/picamera2/previews/gl_helpers.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/previews/null_preview.py` & `picamera2-0.3.9/picamera2/previews/null_preview.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/previews/q_gl_picamera2.py` & `picamera2-0.3.9/picamera2/previews/q_gl_picamera2.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/previews/q_picamera2.py` & `picamera2-0.3.9/picamera2/previews/q_picamera2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import numpy as np
 from libcamera import Transform
 from PyQt5.QtCore import (QRect, QRectF, QSize, QSocketNotifier, Qt,
                           pyqtSignal, pyqtSlot)
 from PyQt5.QtGui import QBrush, QColor, QImage, QPixmap, QTransform
 from PyQt5.QtWidgets import QGraphicsScene, QGraphicsView
 
@@ -167,22 +169,25 @@
         img = completed_request.make_array(display_stream_name)
         if stream_config["format"] in ("YUV420", "YUYV"):
             if cv2_available:
                 if stream_config["format"] == "YUV420":
                     img = cv2.cvtColor(img, cv2.COLOR_YUV420p2BGR)
                 else:
                     img = cv2.cvtColor(img, cv2.COLOR_YUV2RGB_YUYV)
-                width = stream_config["size"][0]
-                if width != stream_config["stride"]:
-                    img = img[:, :width, :]  # this will make it even more expensive!
             else:
-                raise RuntimeError("Qt preview cannot display YUV420/YUYV without cv2")
-        img = np.ascontiguousarray(img[..., :3])
-        shape = img.shape
-        qim = QImage(img.data, shape[1], shape[0], QImage.Format_RGB888)
+                logging.error("Qt preview cannot display YUV420/YUYV without cv2")
+                return
+
+        # Crop width for two reasons: (1) to remove "stride" padding from YUV images;
+        # (2) to ensure the RGB buffer passed to QImage has mandatory 4-byte alignment.
+        # [TODO: Consider QImage.Format_RGB32, if byte order can be made correct]
+        width = min(img.shape[1], stream_config["size"][0])
+        width -= width % 4
+        img = np.ascontiguousarray(img[:, :width, :3])
+        qim = QImage(img.data, width, img.shape[0], QImage.Format_RGB888)
         pix = QPixmap(qim)
         # Add the pixmap to the scene if there wasn't one, or replace it if the images have
         # changed size.
         if self.pixmap is None or pix.rect() != self.last_rect:
             if self.pixmap:
                 self.scene.removeItem(self.pixmap)
             self.last_rect = pix.rect()
```

### Comparing `picamera2-0.3.8/picamera2/previews/qt_previews.py` & `picamera2-0.3.9/picamera2/previews/qt_previews.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2/request.py` & `picamera2-0.3.9/picamera2/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 import logging
 import threading
 import time
+from datetime import datetime
 
 import numpy as np
 import piexif
 from pidng.camdefs import Picamera2Camera
 from pidng.core import PICAM2DNG
 from PIL import Image
 
@@ -137,15 +138,15 @@
                 self.request = None
                 self.config = None
                 self.stream_map = None
 
     def make_buffer(self, name):
         """Make a 1d numpy array from the named stream's buffer."""
         if self.stream_map.get(name, None) is None:
-            raise RuntimeError(f'Stream "{name}" is not defined')
+            raise RuntimeError(f'Stream {name!r} is not defined')
         with _MappedBuffer(self, name) as b:
             return np.array(b, dtype=np.uint8)
 
     def get_metadata(self):
         """Fetch the metadata corresponding to this completed request."""
         metadata = {}
         for k, v in self.request.metadata.items():
@@ -252,19 +253,22 @@
         if format_str in ('jpg', 'jpeg'):
             if img.mode == "RGBA":
                 # Nasty hack. Qt doesn't understand RGBX so we have to use RGBA. But saving a JPEG
                 # doesn't like RGBA to we have to bodge that to RGBX.
                 img.mode = "RGBX"
             # Make up some extra EXIF data.
             if "AnalogueGain" in metadata and "DigitalGain" in metadata:
+                datetime_now = datetime.now().strftime("%Y:%m:%d %H:%M:%S")
                 zero_ifd = {piexif.ImageIFD.Make: "Raspberry Pi",
                             piexif.ImageIFD.Model: self.picam2.camera.id,
-                            piexif.ImageIFD.Software: "Picamera2"}
+                            piexif.ImageIFD.Software: "Picamera2",
+                            piexif.ImageIFD.DateTime: datetime_now}
                 total_gain = metadata["AnalogueGain"] * metadata["DigitalGain"]
-                exif_ifd = {piexif.ExifIFD.ExposureTime: (metadata["ExposureTime"], 1000000),
+                exif_ifd = {piexif.ExifIFD.DateTimeOriginal: datetime_now,
+                            piexif.ExifIFD.ExposureTime: (metadata["ExposureTime"], 1000000),
                             piexif.ExifIFD.ISOSpeedRatings: int(total_gain * 100)}
                 exif = piexif.dump({"0th": zero_ifd, "Exif": exif_ifd})
         # compress_level=1 saves pngs much faster, and still gets most of the compression.
         png_compress_level = self.picam2.options.get("compress_level", 1)
         jpeg_quality = self.picam2.options.get("quality", 90)
         keywords = {"compress_level": png_compress_level, "quality": jpeg_quality, "format": format}
         if exif != b'':
@@ -275,15 +279,15 @@
         _log.info(f"Time taken for encode: {(end_time-start_time)*1000} ms.")
 
     def save_dng(self, buffer, metadata, config, filename):
         """Save a DNG RAW image of the raw stream's buffer."""
         start_time = time.monotonic()
         raw = self.make_array(buffer, config)
 
-        camera = Picamera2Camera(config, metadata)
+        camera = Picamera2Camera(config.copy(), metadata)
         r = PICAM2DNG(camera)
 
         dng_compress_level = self.picam2.options.get("compress_level", 0)
 
         r.options(compress=dng_compress_level)
         r.convert(raw, filename)
```

### Comparing `picamera2-0.3.8/picamera2/sensor_format.py` & `picamera2-0.3.9/picamera2/sensor_format.py`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/picamera2.egg-info/PKG-INFO` & `picamera2-0.3.9/picamera2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picamera2
-Version: 0.3.8
+Version: 0.3.9
 Summary: The libcamera-based Python interface to Raspberry Pi cameras, based on the original Picamera library
 Home-page: https://github.com/RaspberryPi/picamera2
 Author: Raspberry Pi & Raspberry Pi Foundation
 Author-email: picamera2@raspberrypi.com
 License: BSD 2-Clause License
 Project-URL: Bug Tracker, https://github.com/RaspberryPi/picamera2/issues
 Platform: UNKNOWN
```

### Comparing `picamera2-0.3.8/picamera2.egg-info/SOURCES.txt` & `picamera2-0.3.9/picamera2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picamera2-0.3.8/setup.py` & `picamera2-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup
 
 with open("README.md") as readme:
     long_description = readme.read()
 
 setup(
     name='picamera2',
-    version='0.3.8',
+    version='0.3.9',
     description='The libcamera-based Python interface to Raspberry Pi cameras, based on the original Picamera library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Raspberry Pi & Raspberry Pi Foundation',
     author_email='picamera2@raspberrypi.com',
     url='https://github.com/RaspberryPi/picamera2',
     project_urls={
```

