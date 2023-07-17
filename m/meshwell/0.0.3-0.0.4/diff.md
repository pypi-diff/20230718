# Comparing `tmp/meshwell-0.0.3.tar.gz` & `tmp/meshwell-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshwell-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "meshwell-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meshwell-0.0.3.tar` & `meshwell-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-04 23:34:55.242387 meshwell-0.0.3/LICENSE
--rw-r--r--   0        0        0     2886 2023-07-04 23:34:55.242387 meshwell-0.0.3/README.md
--rw-r--r--   0        0        0      137 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/__init__.py
--rw-r--r--   0        0        0      465 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/config.py
--rw-r--r--   0        0        0     1608 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/gmsh_entity.py
--rw-r--r--   0        0        0     1315 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/labeledentity.py
--rw-r--r--   0        0        0    10545 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/model.py
--rw-r--r--   0        0        0     2180 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/polysurface.py
--rw-r--r--   0        0        0     5694 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/prism.py
--rw-r--r--   0        0        0      715 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/refinement.py
--rw-r--r--   0        0        0     2220 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/tag.py
--rw-r--r--   0        0        0      527 2023-07-04 23:34:55.250387 meshwell-0.0.3/meshwell/validation.py
--rw-r--r--   0        0        0     3235 2023-07-04 23:34:55.250387 meshwell-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 meshwell-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 23:34:56.292923 meshwell-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2927 2023-07-17 23:34:56.292923 meshwell-0.0.4/README.md
+-rw-r--r--   0        0        0      137 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/__init__.py
+-rw-r--r--   0        0        0      465 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/config.py
+-rw-r--r--   0        0        0     1608 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/gmsh_entity.py
+-rw-r--r--   0        0        0     1315 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/labeledentity.py
+-rw-r--r--   0        0        0    11397 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/model.py
+-rw-r--r--   0        0        0     2180 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/polysurface.py
+-rw-r--r--   0        0        0     5694 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/prism.py
+-rw-r--r--   0        0        0      715 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/refinement.py
+-rw-r--r--   0        0        0     2220 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/tag.py
+-rw-r--r--   0        0        0      527 2023-07-17 23:34:56.296923 meshwell-0.0.4/meshwell/validation.py
+-rw-r--r--   0        0        0     3235 2023-07-17 23:34:56.296923 meshwell-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4384 1970-01-01 00:00:00.000000 meshwell-0.0.4/PKG-INFO
```

### Comparing `meshwell-0.0.3/LICENSE` & `meshwell-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/README.md` & `meshwell-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,7 +42,8 @@
 * [gyptis](https://gyptis.gitlab.io/): uses basic gmsh for photonic geometries
 
 ### Acknowledgements
 
 * Simon Bilodeau (Princeton): maintainer
 * Helge Gehring (Google X): beta testing, use cases, bug fixes
 * Joaquin Matres Abril (Google X): code improvements
+* Niko Savola (Google): API improvements
```

### Comparing `meshwell-0.0.3/meshwell/gmsh_entity.py` & `meshwell-0.0.4/meshwell/gmsh_entity.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/labeledentity.py` & `meshwell-0.0.4/meshwell/labeledentity.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/model.py` & `meshwell-0.0.4/meshwell/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from os import cpu_count
 from typing import Dict, Optional
 
 import gmsh
 from meshwell.validation import validate_dimtags, unpack_dimtags
 from meshwell.labeledentity import LabeledEntities
 from meshwell.tag import tag_entities, tag_interfaces, tag_boundaries
 from meshwell.refinement import constant_refinement
@@ -15,21 +16,28 @@
 
 
 class Model:
     """Model class."""
 
     def __init__(
         self,
-        point_tolerance=1e-3,
+        point_tolerance: float = 1e-3,
+        n_threads: int = cpu_count(),
     ):
         # Initialize model
         if gmsh.is_initialized():
             gmsh.clear()
         gmsh.initialize()
 
+        # Set paralllel processing
+        gmsh.option.setNumber("General.NumThreads", n_threads)
+        gmsh.option.setNumber("Mesh.MaxNumThreads1D", n_threads)
+        gmsh.option.setNumber("Mesh.MaxNumThreads2D", n_threads)
+        gmsh.option.setNumber("Mesh.MaxNumThreads3D", n_threads)
+
         # Point snapping
         self.point_tolerance = point_tolerance
 
         # CAD engine
         self.model = gmsh.model
         self.occ = self.model.occ
 
@@ -121,41 +129,47 @@
     def mesh(
         self,
         entities_dict: OrderedDict,
         boundaries_dict: Dict = None,
         resolutions: Optional[Dict] = None,
         default_characteristic_length: float = 0.5,
         global_scaling: float = 1.0,
+        global_2D_algorithm: int = 6,
+        global_3D_algorithm: int = 1,
         filename: Optional[str] = None,
         verbosity: Optional[int] = 0,
         interface_delimiter: str = "___",
         boundary_delimiter: str = "None",
         finalize: bool = True,
     ):
         """Creates a GMSH mesh with proper physical tagging from a dict of {labels: list( (GMSH entity dimension, GMSH entity tag) )}.
 
         Args:
             entities_dict: OrderedDict of key: physical name, and value: meshwell entity
             resolutions (Dict): Pairs {"physical name": {"resolution": float, "distance": "float}}
             default_characteristic_length (float): if resolutions is not specified for this physical, will use this value instead
             global_scaling: factor to scale all mesh coordinates by (e.g. 1E-6 to go from um to m)
+            global_2D_algorithm: gmsh surface default meshing algorithm, see https://gmsh.info/doc/texinfo/gmsh.html#Mesh-options
+            global_3D_algorithm: gmsh volume default meshing algorithm, see https://gmsh.info/doc/texinfo/gmsh.html#Mesh-options
             filename (str, path): if True, filepath where to save the mesh
             verbosity: GMSH stdout while meshing (True or False)
             interface_delimiter: string characters to use when naming interfaces between entities
             boundary_delimiter: string characters to use when defining an interface between an entity and nothing (simulation boundary)
             finalize: if True (default), finalizes the GMSH model after execution
 
         Returns:
             meshio object with mesh information
         """
         resolutions = resolutions if resolutions else {}
         gmsh.option.setNumber("General.Terminal", verbosity)  # 1 verbose, 0 otherwise
         gmsh.option.setNumber(
             "Mesh.CharacteristicLengthMax", default_characteristic_length
         )
+        gmsh.option.setNumber("Mesh.Algorithm", global_2D_algorithm)
+        gmsh.option.setNumber("Mesh.Algorithm3D", global_3D_algorithm)
 
         # Initial synchronization
         self.occ.synchronize()
 
         # Parse strutural and boundary entities
         full_entities_dict = OrderedDict()
         keep = False
@@ -211,15 +225,15 @@
                                 current_dimtags_cut.extend(cut[0])
                             self.sync_model()
                     # Heal interfaces now that there are no volume conflicts
                     self.occ.removeAllDuplicates()
                     self.sync_model()
                     # Make sure the most up-to-date surfaces are logged as boundaries
                     previous_entities.update_boundaries()
-                current_entities.dimtags = current_dimtags_cut
+                current_entities.dimtags = list(set(current_dimtags_cut))
             current_entities.update_boundaries()
             final_entity_list.append(current_entities)
 
         # Tag entities, interfaces, and boundaries
         tag_entities(final_entity_list)
         final_entity_list = tag_interfaces(
             final_entity_list, max_dim, interface_delimiter
```

### Comparing `meshwell-0.0.3/meshwell/polysurface.py` & `meshwell-0.0.4/meshwell/polysurface.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/prism.py` & `meshwell-0.0.4/meshwell/prism.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/refinement.py` & `meshwell-0.0.4/meshwell/refinement.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/tag.py` & `meshwell-0.0.4/meshwell/tag.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/meshwell/validation.py` & `meshwell-0.0.4/meshwell/validation.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.3/pyproject.toml` & `meshwell-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version="0.0.3"
+version="0.0.4"
 authors = [
     {name = "Simon Bilodeau", email = "sb30@princeton.edu"},
 ]
 keywords = ["python"]
 license = {file = "LICENSE"}
 dependencies = [
     "shapely",
```

### Comparing `meshwell-0.0.3/PKG-INFO` & `meshwell-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshwell
-Version: 0.0.3
+Version: 0.0.4
 Summary: GMSH wrapper, with integrated photonics focus
 Keywords: python
 Author-email: Simon Bilodeau <sb30@princeton.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -81,8 +81,9 @@
 * [gyptis](https://gyptis.gitlab.io/): uses basic gmsh for photonic geometries
 
 ### Acknowledgements
 
 * Simon Bilodeau (Princeton): maintainer
 * Helge Gehring (Google X): beta testing, use cases, bug fixes
 * Joaquin Matres Abril (Google X): code improvements
+* Niko Savola (Google): API improvements
```

