# Comparing `tmp/manim_lamination_builder-0.2.7.tar.gz` & `tmp/manim_lamination_builder-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_lamination_builder-0.2.7.tar", last modified: Tue Jun 27 19:52:45 2023, max compression
+gzip compressed data, was "manim_lamination_builder-0.2.8.tar", last modified: Tue Jul 18 02:44:17 2023, max compression
```

## Comparing `manim_lamination_builder-0.2.7.tar` & `manim_lamination_builder-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/LICENSE
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.7/README.md
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.277353 manim_lamination_builder-0.2.7/manim_lamination_builder/
--rw-r--r--   0 forrest   (1000) forrest   (1000)     1054 2023-05-17 21:22:09.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/__init__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)      506 2023-05-17 21:59:01.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/__main__.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/animation.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3132 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/chord.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2846 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/custom_json.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4443 2023-06-21 01:11:35.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     3470 2023-05-14 20:26:30.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/lamination.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     2035 2023-06-13 23:38:46.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/leaf_polygon_conversion.py
--rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1144 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/main.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     4225 2023-06-20 23:53:08.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/morph.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     1039 2023-06-19 18:18:30.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/new_generate.py
--rw-r--r--   0 forrest   (1000) forrest   (1000)     6900 2023-06-13 21:43:04.000000 manim_lamination_builder-0.2.7/manim_lamination_builder/points.py
-drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/
--rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/PKG-INFO
--rw-r--r--   0 forrest   (1000) forrest   (1000)      728 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/SOURCES.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/dependency_links.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/requires.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-06-27 19:52:45.000000 manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/top_level.txt
--rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-06-27 19:44:53.000000 manim_lamination_builder-0.2.7/pyproject.toml
--rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-06-27 19:52:45.280686 manim_lamination_builder-0.2.7/setup.cfg
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-07-18 02:44:17.835428 manim_lamination_builder-0.2.8/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    34523 2023-05-14 20:25:53.000000 manim_lamination_builder-0.2.8/LICENSE
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-07-18 02:44:17.835428 manim_lamination_builder-0.2.8/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3590 2023-05-17 01:50:11.000000 manim_lamination_builder-0.2.8/README.md
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-07-18 02:44:17.835428 manim_lamination_builder-0.2.8/manim_lamination_builder/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     1070 2023-07-03 21:49:50.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/__init__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      506 2023-05-17 21:59:01.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/__main__.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4412 2023-07-02 19:04:53.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/animation.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     3199 2023-07-03 19:06:54.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/chord.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     2920 2023-07-03 19:19:16.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/custom_json.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4443 2023-07-02 19:04:53.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6138 2023-07-11 02:29:29.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/lamination.py
+-rwxr-xr-x   0 forrest   (1000) forrest   (1000)     1124 2023-07-11 01:52:35.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/main.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4225 2023-07-02 19:04:53.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/morph.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     4157 2023-07-11 14:54:38.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/new_generate.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)     6900 2023-07-03 19:06:53.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/points.py
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      467 2023-07-18 02:42:23.000000 manim_lamination_builder-0.2.8/manim_lamination_builder/visual_settings.py
+drwxr-xr-x   0 forrest   (1000) forrest   (1000)        0 2023-07-18 02:44:17.835428 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/
+-rw-r--r--   0 forrest   (1000) forrest   (1000)    43957 2023-07-18 02:44:17.000000 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/PKG-INFO
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      720 2023-07-18 02:44:17.000000 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)        1 2023-07-18 02:44:17.000000 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       12 2023-07-18 02:44:17.000000 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/requires.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       25 2023-07-18 02:44:17.000000 manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/top_level.txt
+-rw-r--r--   0 forrest   (1000) forrest   (1000)      693 2023-07-18 02:44:04.000000 manim_lamination_builder-0.2.8/pyproject.toml
+-rw-r--r--   0 forrest   (1000) forrest   (1000)       38 2023-07-18 02:44:17.835428 manim_lamination_builder-0.2.8/setup.cfg
```

### Comparing `manim_lamination_builder-0.2.7/LICENSE` & `manim_lamination_builder-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/PKG-INFO` & `manim_lamination_builder-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_lamination_builder
-Version: 0.2.7
+Version: 0.2.8
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.7/README.md` & `manim_lamination_builder-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/__init__.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This is a re-implementation of lamination-builder that runs in python without dependencies on a browser and focusing on animations and convenient generation of figures. Instead it uses Manim, which has several dependencies, which you are responsible for installing in accordance with Manim's installation instructions.
 """
-from manim_lamination_builder.lamination import Lamination
+from manim_lamination_builder.lamination import Lamination, LeafLamination
 from manim_lamination_builder.custom_json import (
     custom_dump,
     custom_parse,
     read_file_to_laminations,
     parse_lamination,
 )
 from manim_lamination_builder.points import FloatWrapper, UnitPoint, NaryFraction, sigma
```

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/animation.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/animation.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/chord.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         if a.to_float() < b.to_float():
             self.min = a
             self.max = b
         else:
             self.min = b
             self.max = a
 
+    def __hash__(self):
+        return hash((self.min, self.max))
+
     def crosses(self, other: "Chord") -> bool:
         if (
             self.max.to_float() <= other.min.to_float()
             or self.min.to_float() >= other.max.to_float()
         ):
             return False
         if (
```

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/custom_json.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/custom_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 import json5
 
 
 class CustomEncoder(json.JSONEncoder):
     def default(self, v):
         types = {"NaryFraction": lambda v: v.to_string()}
         vtype = type(v).__name__
-        if vtype == "Lamination":
+        if vtype in ["LeafLamination", "Lamination"]:
             ret = v.__dict__.copy()
             ret.pop("colorizer")
             return ret
         if vtype == "Chord":
             return list(v.__dict__.values())
         if vtype == "FloatWrapper":
             return v.value
         if vtype in types:
             return types[type(v).__name__](v)
+        if vtype == "set":
+            return list(v)
         else:
             return json.JSONEncoder.default(self, v)
 
 
 class CustomDecoder(json.JSONDecoder):
     def __init__(self, *args, **kwargs):
         super().__init__(object_hook=self.object_hook, *args, **kwargs)
```

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/generate.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/generate.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/main.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,35 +6,30 @@
 
 from manim_lamination_builder.custom_json import custom_dump, read_file_to_laminations
 from typing import List
 from manim import (
     WHITE,
     Scene,
     Group,
-    tempconfig,
 )
-import sys
-import os
 
 from manim.utils.file_ops import config
 
-from manim_lamination_builder.lamination import Lamination
+from manim_lamination_builder.lamination import AbstractLamination
 
-def group(laminations: List[Lamination]):
+def group(laminations: List[AbstractLamination]):
     group = Group(*[lamination.build() for lamination in laminations])
     group = group.arrange_in_grid()
     group.scale(
         1
         / max(group.width / config.frame_width + 0.01, group.height / config.frame_height + 0.01)
     )
     return group
 
 class Main(Scene):
-    def __init__(self, laminations: List[Lamination]):
+    def __init__(self, laminations: List[AbstractLamination]):
         self.laminations = laminations
         super().__init__()
 
     def construct(self):
-        self.camera.background_color = WHITE
+        config.background_color = WHITE
         self.add(group(self.laminations))
-
-
```

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/morph.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/morph.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder/points.py` & `manim_lamination_builder-0.2.8/manim_lamination_builder/points.py`

 * *Files identical despite different names*

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/PKG-INFO` & `manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-lamination-builder
-Version: 0.2.7
+Version: 0.2.8
 Summary: a replacement to lamination builder that uses manim instead of the browser
 Author-email: Forrest Hilton <forrestmhilton@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `manim_lamination_builder-0.2.7/manim_lamination_builder.egg-info/SOURCES.txt` & `manim_lamination_builder-0.2.8/manim_lamination_builder.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 manim_lamination_builder/__init__.py
 manim_lamination_builder/__main__.py
 manim_lamination_builder/animation.py
 manim_lamination_builder/chord.py
 manim_lamination_builder/custom_json.py
 manim_lamination_builder/generate.py
 manim_lamination_builder/lamination.py
-manim_lamination_builder/leaf_polygon_conversion.py
 manim_lamination_builder/main.py
 manim_lamination_builder/morph.py
 manim_lamination_builder/new_generate.py
 manim_lamination_builder/points.py
+manim_lamination_builder/visual_settings.py
 manim_lamination_builder.egg-info/PKG-INFO
 manim_lamination_builder.egg-info/SOURCES.txt
 manim_lamination_builder.egg-info/dependency_links.txt
 manim_lamination_builder.egg-info/requires.txt
 manim_lamination_builder.egg-info/top_level.txt
```

### Comparing `manim_lamination_builder-0.2.7/pyproject.toml` & `manim_lamination_builder-0.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "manim_lamination_builder"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Forrest Hilton", email="forrestmhilton@gmail.com" },
 ]
 description = "a replacement to lamination builder that uses manim instead of the browser"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

