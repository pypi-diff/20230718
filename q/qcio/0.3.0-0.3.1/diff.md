# Comparing `tmp/qcio-0.3.0.tar.gz` & `tmp/qcio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.3.0.tar", max compression
+gzip compressed data, was "qcio-0.3.1.tar", max compression
```

## Comparing `qcio-0.3.0.tar` & `qcio-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-07-17 21:07:13.766101 qcio-0.3.0/LICENSE
--rw-r--r--   0        0        0      898 2023-07-17 21:07:13.766101 qcio-0.3.0/README.md
--rw-r--r--   0        0        0     1246 2023-07-17 21:07:13.766101 qcio-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      573 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/constants.py
--rw-r--r--   0        0        0      346 2023-07-17 21:07:13.766101 qcio-0.3.0/qcio/helper_types.py
--rw-r--r--   0        0        0      272 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/__init__.py
--rw-r--r--   0        0        0     9738 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/base_models.py
--rw-r--r--   0        0        0     3082 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/inputs.py
--rw-r--r--   0        0        0     2236 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     7511 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/molecule.py
--rw-r--r--   0        0        0     3585 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/outputs.py
--rw-r--r--   0        0        0     1935 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/outputs_base.py
--rw-r--r--   0        0        0     4462 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/models/results.py
--rw-r--r--   0        0        0     4253 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/qcel.py
--rw-r--r--   0        0        0      793 2023-07-17 21:07:13.770101 qcio-0.3.0/qcio/utils.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-18 00:17:05.815752 qcio-0.3.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-18 00:17:05.815752 qcio-0.3.1/README.md
+-rw-r--r--   0        0        0     1246 2023-07-18 00:17:05.819753 qcio-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/constants.py
+-rw-r--r--   0        0        0      346 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/helper_types.py
+-rw-r--r--   0        0        0      272 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2236 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     8187 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/molecule.py
+-rw-r--r--   0        0        0     3585 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4462 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/models/results.py
+-rw-r--r--   0        0        0     4413 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/qcel.py
+-rw-r--r--   0        0        0      838 2023-07-18 00:17:05.819753 qcio-0.3.1/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.1/PKG-INFO
```

### Comparing `qcio-0.3.0/LICENSE` & `qcio-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/README.md` & `qcio-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/pyproject.toml` & `qcio-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.3.0"
+version = "0.3.1"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.3.0/qcio/__init__.py` & `qcio-0.3.1/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/base_models.py` & `qcio-0.3.1/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/inputs.py` & `qcio-0.3.1/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/inputs_base.py` & `qcio-0.3.1/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/molecule.py` & `qcio-0.3.1/qcio/models/molecule.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections import Counter
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 from pydantic import validator
 from typing_extensions import Self
 
 from qcio.constants import BOHR_TO_ANGSTROM
 from qcio.helper_types import ArrayLike2D
@@ -74,25 +74,29 @@
         symbols: The atomic symbols of the molecule.
         geometry: The geometry of the molecule in Cartesian coordinates. Units are (AU)
             Bohr.
         identifiers: Identifiers for the molecule such as name, smiles, etc.
         charge: The molecular charge.
         connectivity: Explicit description of the bonds between atoms.
         multiplicity: The molecular multiplicity.
+        connectivity: Explicit description of the bonds between atoms. Each tuple
+            contains the indices of the atoms in the bond and the order of the bond.
+            E.g., [(0, 1, 1.0), (1, 2, 2.0)] indicates a single bond between atoms 0
+            and 1 and a double bond between atoms 1 and 2.
         masses: Explicit masses for the atoms. If not set, default isotopic masses are
             used.
     """
 
     symbols: List[str]
     geometry: ArrayLike2D
     charge: int = 0
     multiplicity: int = 1
     identifiers: Identifiers = Identifiers()
+    connectivity: List[Tuple[int, int, float]] = []
     # masses: List[float] = []
-    # connectivity: List[Bond] = []
 
     def __repr_args__(self) -> "ReprArgs":
         """A helper for __repr__ that returns a list of tuples of the form
         (name, value).
         """
         return [  # pragma: no cover
             ("name", self.identifiers.name_common),
@@ -125,14 +129,23 @@
             sorted_elements = [("C", carbon_count)] + sorted_elements
 
         return "".join(
             f"{element}{count if count > 1 else ''}"
             for element, count in sorted_elements
         )
 
+    def dict(self, **kwargs) -> Dict[str, Any]:
+        """Handle tuple in connectivity"""
+        dict = super().dict(**kwargs)
+        # Must cast all values to floats as toml cannot handle mixed types
+        dict["connectivity"] = [
+            [float(val) for val in bond] for bond in dict["connectivity"]
+        ]
+        return dict
+
     @classmethod
     def open(cls, filepath: Union[Path, str]) -> Self:
         """Open a molecule from a file.
 
         Args:
             filepath: The path to the file to open. Maybe a path to a JSON file or an
                 XYZ file.
```

### Comparing `qcio-0.3.0/qcio/models/outputs.py` & `qcio-0.3.1/qcio/models/outputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/outputs_base.py` & `qcio-0.3.1/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/models/results.py` & `qcio-0.3.1/qcio/models/results.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.0/qcio/qcel.py` & `qcio-0.3.1/qcio/qcel.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,37 +7,41 @@
     Provenance,
     SinglePointOutput,
     SinglePointResults,
     Wavefunction,
 )
 
 
-def to_qcel_input(inp_obj: ProgramInput) -> Dict[str, Any]:
+def to_qcel_input(prog_input: ProgramInput) -> Dict[str, Any]:
     """Return the QCElemental v1 input schema representation of the input
     (AtomicInput dict).
 
+    Args:
+        prog_input: The input object to convert.
+
     Returns:
         The QCElemental v1 dict representation of an AtomicInput object.
     """
     return {
         "molecule": {
-            "symbols": inp_obj.molecule.symbols,
-            "geometry": inp_obj.molecule.geometry,
-            "molecular_charge": inp_obj.molecule.charge,
-            "molecular_multiplicity": inp_obj.molecule.multiplicity,
+            "symbols": prog_input.molecule.symbols,
+            "geometry": prog_input.molecule.geometry,
+            "molecular_charge": prog_input.molecule.charge,
+            "molecular_multiplicity": prog_input.molecule.multiplicity,
+            "connectivity": prog_input.molecule.connectivity or None,
             "identifiers": {
                 key: value
-                for key, value in inp_obj.molecule.identifiers.dict().items()
+                for key, value in prog_input.molecule.identifiers.dict().items()
                 if key not in ["name_IUPAC", "name_common"]  # not on qcel model
             },
         },
-        "driver": inp_obj.calctype,
-        "model": inp_obj.model.dict(),
-        "keywords": inp_obj.keywords,
-        "extras": inp_obj.extras,
+        "driver": prog_input.calctype,
+        "model": prog_input.model.dict(),
+        "keywords": prog_input.keywords,
+        "extras": prog_input.extras,
     }
 
 
 def from_qcel_output(
     qcio_input: ProgramInput,
     qcel_output: Dict[str, Any],
 ) -> Union[SinglePointOutput, ProgramFailure]:
```

### Comparing `qcio-0.3.0/PKG-INFO` & `qcio-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.3.0
+Version: 0.3.1
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

