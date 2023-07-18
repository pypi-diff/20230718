# Comparing `tmp/sees-0.0.5.tar.gz` & `tmp/sees-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sees-0.0.5.tar", last modified: Mon Jul 17 07:46:19 2023, max compression
+gzip compressed data, was "sees-0.0.6.tar", last modified: Tue Jul 18 15:41:04 2023, max compression
```

## Comparing `sees-0.0.5.tar` & `sees-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2624 2023-07-17 07:46:19.476706 sees-0.0.5/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2215 2023-07-17 00:57:14.000000 sees-0.0.5/README.md
--rw-r--r--   0 claudio   (1001) claudio   (1001)      819 2023-07-17 07:46:07.000000 sees-0.0.5/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-17 07:46:19.476706 sees-0.0.5/setup.cfg
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.466706 sees-0.0.5/src/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.466706 sees-0.0.5/src/sees/
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    24801 2023-07-16 22:33:32.000000 sees-0.0.5/src/sees/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3203 2023-07-17 01:36:29.000000 sees-0.0.5/src/sees/__main__.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.5/src/sees/_render.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/src/sees/canvas/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.5/src/sees/canvas/canvas.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2620 2023-07-16 22:33:00.000000 sees-0.0.5/src/sees/canvas/gltflib.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.5/src/sees/canvas/mpl.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     4894 2023-07-16 22:33:14.000000 sees-0.0.5/src/sees/canvas/ply.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.5/src/sees/canvas/tri.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5687 2023-07-17 01:34:09.000000 sees-0.0.5/src/sees/cli.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.5/src/sees/config.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.5/src/sees/consolidate.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.5/src/sees/core.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     5707 2023-07-17 01:25:18.000000 sees-0.0.5/src/sees/section.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/src/sees/solid/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/src/sees/solid/convert/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.5/src/sees/solid/convert/convert.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.5/src/sees/solid/convert/example.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.5/src/sees/solid/ops.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.5/src/sees/solid/plt.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.5/src/sees/structure.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      569 2023-07-17 01:57:03.000000 sees-0.0.5/src/sees/tcl.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/src/sees/utilities/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.5/src/sees/utilities/alpha_shape.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.5/src/sees/views.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/src/sees.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2624 2023-07-17 07:46:19.000000 sees-0.0.5/src/sees.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      683 2023-07-17 07:46:19.000000 sees-0.0.5/src/sees.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-17 07:46:19.000000 sees-0.0.5/src/sees.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-17 07:46:19.000000 sees-0.0.5/src/sees.egg-info/entry_points.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2023-07-17 07:46:19.000000 sees-0.0.5/src/sees.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-17 07:46:19.476706 sees-0.0.5/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.5/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2624 2023-07-18 15:41:04.376706 sees-0.0.6/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2215 2023-07-17 00:57:14.000000 sees-0.0.6/README.md
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      844 2023-07-18 15:40:24.000000 sees-0.0.6/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-18 15:41:04.376706 sees-0.0.6/setup.cfg
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.356706 sees-0.0.6/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.366706 sees-0.0.6/src/sees/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    24909 2023-07-17 15:58:28.000000 sees-0.0.6/src/sees/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3214 2023-07-17 15:52:15.000000 sees-0.0.6/src/sees/__main__.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.6/src/sees/_render.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/src/sees/canvas/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      714 2023-07-16 22:32:53.000000 sees-0.0.6/src/sees/canvas/canvas.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2620 2023-07-16 22:33:00.000000 sees-0.0.6/src/sees/canvas/gltflib.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1543 2023-07-16 22:33:08.000000 sees-0.0.6/src/sees/canvas/mpl.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4894 2023-07-16 22:33:14.000000 sees-0.0.6/src/sees/canvas/ply.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1458 2023-07-16 22:33:22.000000 sees-0.0.6/src/sees/canvas/tri.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5687 2023-07-17 01:34:09.000000 sees-0.0.6/src/sees/cli.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.6/src/sees/config.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)     5608 2023-07-16 22:18:49.000000 sees-0.0.6/src/sees/consolidate.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-16 06:07:59.000000 sees-0.0.6/src/sees/core.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     5760 2023-07-18 14:45:02.000000 sees-0.0.6/src/sees/section.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/src/sees/solid/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/src/sees/solid/convert/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.6/src/sees/solid/convert/convert.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.6/src/sees/solid/convert/example.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.6/src/sees/solid/ops.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.6/src/sees/solid/plt.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.6/src/sees/structure.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      614 2023-07-17 15:37:20.000000 sees-0.0.6/src/sees/tcl.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/src/sees/utilities/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.6/src/sees/utilities/alpha_shape.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      202 2023-07-16 06:08:31.000000 sees-0.0.6/src/sees/views.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.366706 sees-0.0.6/src/sees.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2624 2023-07-18 15:41:03.000000 sees-0.0.6/src/sees.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      683 2023-07-18 15:41:04.000000 sees-0.0.6/src/sees.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-18 15:41:03.000000 sees-0.0.6/src/sees.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-18 15:41:03.000000 sees-0.0.6/src/sees.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       12 2023-07-18 15:41:03.000000 sees-0.0.6/src/sees.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-18 15:41:04.376706 sees-0.0.6/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.6/tests/test.py
```

### Comparing `sees-0.0.5/PKG-INFO` & `sees-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.5
+Version: 0.0.6
 Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Description-Content-Type: text/markdown
 
 # `sees`
```

### Comparing `sees-0.0.5/README.md` & `sees-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/pyproject.toml` & `sees-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sees"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
   {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
 description="A modern OpenSees renderer"
 
 readme = "README.md"
@@ -16,22 +16,24 @@
   "earthquake-engineering",
 ] 
 
 [options]
 #packages = find
 install_requires = [
   "sdof",
+  "ssid",
   "opensees",
   "quakeio",
 
   "pyyaml",
   "scipy",
   "numpy",
   "plotly",
-  "trimesh",
+# "trimesh",
+  "pygltflib",
   "matplotlib"
 ]
 
 [project.urls]
 repository = "http://github.com/BRACE2/sees"
 # documentation = "https://brace2.github.io/sees"
```

### Comparing `sees-0.0.5/src/sees/__init__.py` & `sees-0.0.6/src/sees/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,22 +105,25 @@
     R = np.array(((0,-1),
                   (1, 0))).T
 
     # Treat aggregated sections
     if "section" in section:
         if section["section"] not in outlines:
             outlines[section["name"]] = get_section_shape(sections[section["section"]], sections, outlines)
+        else:
+            outlines[section["name"]] = outlines[section["section"]]
 
     elif "bounding_polygon" in section:
         outlines[section["name"]] = [R@s for s in section["bounding_polygon"]]
 
     elif "fibers" in section:
         #outlines[section["name"]] = _alpha_shape(np.array([f["coord"] for f in section["fibers"]]))
         points = np.array([f["coord"] for f in section["fibers"]])
         outlines[section["name"]] = points[ConvexHull(points).vertices]
+
     return outlines[section["name"]]
 
 def get_section_geometries(model, renderer=None):
 
     sections, outlines = {}, {}
     for name,section in model["sections"].items():
         get_section_shape(section, model["sections"], outlines)
@@ -660,14 +663,15 @@
         if "extrude" in self.config["show_objects"]:
             displ = None
             if len(self.response_layers) == 1:
                 displ = next(iter(self.response_layers.values()))
             try:
                 self.plot_extruded_frames(displ)
             except Exception as e:
+                raise e
                 print("Warning -- ", e, file=sys.stderr)
 
         self.canvas.build()
         return self
 
     def write(self, filename):
         self.canvas.write(filename)
```

### Comparing `sees-0.0.5/src/sees/__main__.py` & `sees-0.0.6/src/sees/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import numpy as np
 import sees
 from sees import RenderError
 from sees.cli import parse_args
 from sees.views import VIEWS
 
-
+NAME="sees"
 EXAMPLES="""
 Examples:
     Plot the structural model defined in the file `sam.json`:
         $ {NAME} sam.json
 
     Plot displaced structure with unit translation at nodes
     5, 3 and 2 in direction 2 at scale of 100:
```

### Comparing `sees-0.0.5/src/sees/_render.py` & `sees-0.0.6/src/sees/_render.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/canvas/canvas.py` & `sees-0.0.6/src/sees/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/canvas/gltflib.py` & `sees-0.0.6/src/sees/canvas/gltflib.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/canvas/mpl.py` & `sees-0.0.6/src/sees/canvas/mpl.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/canvas/ply.py` & `sees-0.0.6/src/sees/canvas/ply.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/canvas/tri.py` & `sees-0.0.6/src/sees/canvas/tri.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/cli.py` & `sees-0.0.6/src/sees/cli.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/config.py` & `sees-0.0.6/src/sees/config.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/consolidate.py` & `sees-0.0.6/src/sees/consolidate.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/section.py` & `sees-0.0.6/src/sees/section.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.collections
 from math import sqrt
 
 def show(): plt.show()
 
-def section(s, ax=None, show=None, **kwds):
+def render(s, ax=None, show=None, **kwds):
     if isinstance(show, str):
         show = [show]
     elif show is None:
         show = ["fiber", "patch", "layer"]
 
     if isinstance(s, list):
         pass
@@ -146,22 +146,24 @@
                     ax.scatter(*zip(*(f.coord for patch in section.patches for f in patch.fibers)), s=0.1)
                 except:
                     pass
 
                 try:
                     ax.scatter(*zip(*(f.coord for patch in section.patches for f in patch.fibers)), s=0.1)
                 except Exception as e:
-                    print(e)
+                    # print(e)
+                    pass
 
 
                 try:
                     coords, areas = zip(*((f.coord, 20*f.area) for layer in section.layers for f in layer.fibers))
                     ax.scatter(*zip(*coords), s=areas, color="k")
                 except Exception as e:
-                    print(e)
+                    # print(e)
+                    pass
 
         # show centroid
         #ax.scatter(*section.centroid)
         # show origin
         # ax.scatter(0, 0)
         ax.axis("equal")
         #plt.show()
```

### Comparing `sees-0.0.5/src/sees/solid/convert/convert.py` & `sees-0.0.6/src/sees/solid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/solid/ops.py` & `sees-0.0.6/src/sees/solid/ops.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees/tcl.py` & `sees-0.0.6/src/sees/tcl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import sys
 import json
 from functools import partial
 from sees.cli import parse_args
 from sees import config, render, RenderError
 
 def _render(*args, rt=None):
-    config = parse_args(["render", *args])
-    if config is None:
-        return ""
-    if "verbose" in config and config["verbose"]:
-        print(config)
-
-    config["sam_file"] = rt.to_dict()
-
     try:
+        config = parse_args(["render", *args])
+#       print(config)
+        if config is None:
+            return ""
+        if "verbose" in config and config["verbose"]:
+            print(config)
+
+        config["sam_file"] = rt.to_dict()
         render(**config)
 
     except RenderError:
         print(e, file=sys.stderr)
 
     return ""
```

### Comparing `sees-0.0.5/src/sees/utilities/alpha_shape.py` & `sees-0.0.6/src/sees/utilities/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.5/src/sees.egg-info/PKG-INFO` & `sees-0.0.6/src/sees.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sees
-Version: 0.0.5
+Version: 0.0.6
 Summary: A modern OpenSees renderer
 Author-email: "Claudio M. Perez" <50180406+claudioperez@users.noreply.github.com>, Chrystal Chern <52893467+chrystalchern@users.noreply.github.com>
 Project-URL: repository, http://github.com/BRACE2/sees
 Keywords: seismic,post-processing,finite-element-analysis,earthquake-engineering
 Description-Content-Type: text/markdown
 
 # `sees`
```

### Comparing `sees-0.0.5/src/sees.egg-info/SOURCES.txt` & `sees-0.0.6/src/sees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

