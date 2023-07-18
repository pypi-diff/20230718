# Comparing `tmp/qcio-0.3.2.tar.gz` & `tmp/qcio-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcio-0.3.2.tar", max compression
+gzip compressed data, was "qcio-0.3.3.tar", max compression
```

## Comparing `qcio-0.3.2.tar` & `qcio-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2023-07-18 01:10:31.845509 qcio-0.3.2/LICENSE
--rw-r--r--   0        0        0      898 2023-07-18 01:10:31.845509 qcio-0.3.2/README.md
--rw-r--r--   0        0        0     1246 2023-07-18 01:10:31.845509 qcio-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      573 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/__init__.py
--rw-r--r--   0        0        0       89 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/constants.py
--rw-r--r--   0        0        0      346 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/helper_types.py
--rw-r--r--   0        0        0      272 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/__init__.py
--rw-r--r--   0        0        0     9738 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/base_models.py
--rw-r--r--   0        0        0     3082 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/inputs.py
--rw-r--r--   0        0        0     2236 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/inputs_base.py
--rw-r--r--   0        0        0     8354 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/molecule.py
--rw-r--r--   0        0        0     3585 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/outputs.py
--rw-r--r--   0        0        0     1935 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/outputs_base.py
--rw-r--r--   0        0        0     4462 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/models/results.py
--rw-r--r--   0        0        0     4413 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/qcel.py
--rw-r--r--   0        0        0      838 2023-07-18 01:10:31.845509 qcio-0.3.2/qcio/utils.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-18 02:24:27.790026 qcio-0.3.3/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-18 02:24:27.790026 qcio-0.3.3/README.md
+-rw-r--r--   0        0        0     1246 2023-07-18 02:24:27.790026 qcio-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      573 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/constants.py
+-rw-r--r--   0        0        0      483 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/helper_types.py
+-rw-r--r--   0        0        0      272 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/__init__.py
+-rw-r--r--   0        0        0     9738 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/base_models.py
+-rw-r--r--   0        0        0     3082 2023-07-18 02:24:27.790026 qcio-0.3.3/qcio/models/inputs.py
+-rw-r--r--   0        0        0     2236 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/inputs_base.py
+-rw-r--r--   0        0        0     8354 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/molecule.py
+-rw-r--r--   0        0        0     3585 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/outputs.py
+-rw-r--r--   0        0        0     1935 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/outputs_base.py
+-rw-r--r--   0        0        0     4794 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/models/results.py
+-rw-r--r--   0        0        0     4569 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/qcel.py
+-rw-r--r--   0        0        0      838 2023-07-18 02:24:27.794026 qcio-0.3.3/qcio/utils.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 qcio-0.3.3/PKG-INFO
```

### Comparing `qcio-0.3.2/LICENSE` & `qcio-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/README.md` & `qcio-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/pyproject.toml` & `qcio-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qcio"
-version = "0.3.2"
+version = "0.3.3"
 description = "Beautiful and user friendly data structures for quantum chemistry."
 authors = ["Colton Hicks <github@coltonhicks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `qcio-0.3.2/qcio/__init__.py` & `qcio-0.3.3/qcio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/base_models.py` & `qcio-0.3.3/qcio/models/base_models.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/inputs.py` & `qcio-0.3.3/qcio/models/inputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/inputs_base.py` & `qcio-0.3.3/qcio/models/inputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/molecule.py` & `qcio-0.3.3/qcio/models/molecule.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/outputs.py` & `qcio-0.3.3/qcio/models/outputs.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/outputs_base.py` & `qcio-0.3.3/qcio/models/outputs_base.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/qcio/models/results.py` & `qcio-0.3.3/qcio/models/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
 import numpy as np
 from pydantic import validator
 
-from qcio.helper_types import ArrayLike2D
+from qcio.helper_types import ArrayLike2D, ArrayLike3D
 
 from .base_models import QCIOModelBase
 from .molecule import Molecule
 from .outputs_base import ResultsBase
 
 __all__ = ["SinglePointResults", "Wavefunction", "OptimizationResults"]
 
@@ -54,15 +54,15 @@
         hessian: The hessian of the molecule in Hartrees/Bohr^2.
         nuclear_repulsion_energy: The nuclear repulsion energy of the molecule in
             Hartrees.
 
         wavefunction: Wavefunction data from the calculation.
 
         freqs_wavenumber: The frequencies of the molecule in wavenumbers.
-        normal_modes_cartesian: n_vibmodes*n_atoms length array containing
+        normal_modes_cartesian: n_vibmodes by n_atoms length array containing
             un-mass-weighted Cartesian displacements of each normal mode.
         gibbs_free_energy: Gibbs free energy (i.e. thermochemical analysis) in Hartrees
             of a system where translation / rotation / vibration degrees of freedom are
             approximated using ideal gas / rigid rotor / harmonic oscillator
             respectively.
     """
 
@@ -80,17 +80,24 @@
     nuclear_repulsion_energy: Optional[float] = None
 
     # Wavefunction data
     wavefunction: Optional[Wavefunction] = None
 
     # Frequency data
     freqs_wavenumber: List[float] = []
-    normal_modes_cartesian: List[float] = []
+    normal_modes_cartesian: Optional[ArrayLike3D] = None
     gibbs_free_energy: Optional[float] = None
 
+    @validator("normal_modes_cartesian")
+    def validate_normal_modes_cartesian_shape(cls, v: ArrayLike3D):
+        if v is not None:
+            # Assume array has length of the number of normal modes
+            n_normal_modes = len(v)
+            return np.asarray(v).reshape(n_normal_modes, -1, 3)
+
     @validator("gradient")
     def validate_gradient_shape(cls, v: ArrayLike2D):
         """Validate gradient is n x 3"""
         if v is not None:
             return np.asarray(v).reshape(-1, 3)
 
     @validator("hessian")
```

### Comparing `qcio-0.3.2/qcio/qcel.py` & `qcio-0.3.3/qcio/qcel.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
             qcel_key = qcio_to_qcel[key]
         else:
             qcel_key = key
         value = qcel_output["properties"].get(qcel_key)
         if value is not None:
             results[key] = value
 
+    # Override with return_result as qcel may not have save the key value to .properties
+    results[qcel_output["driver"]] = qcel_output["return_result"]
+
     if qcel_output["wavefunction"]:
         results["wavefunction"] = {
             key: value
             for key, value in qcel_output["wavefunction"].items()
             if key in Wavefunction.__annotations__
         }
```

### Comparing `qcio-0.3.2/qcio/utils.py` & `qcio-0.3.3/qcio/utils.py`

 * *Files identical despite different names*

### Comparing `qcio-0.3.2/PKG-INFO` & `qcio-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcio
-Version: 0.3.2
+Version: 0.3.3
 Summary: Beautiful and user friendly data structures for quantum chemistry.
 License: MIT
 Author: Colton Hicks
 Author-email: github@coltonhicks.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

