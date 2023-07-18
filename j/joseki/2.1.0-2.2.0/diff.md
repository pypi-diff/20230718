# Comparing `tmp/joseki-2.1.0.tar.gz` & `tmp/joseki-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joseki-2.1.0.tar", last modified: Fri Feb 17 12:42:35 2023, max compression
+gzip compressed data, was "joseki-2.2.0.tar", last modified: Tue Jul 18 07:38:20 2023, max compression
```

## Comparing `joseki-2.1.0.tar` & `joseki-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,65 @@
--rw-r--r--   0        0        0     1075 2023-02-17 12:42:20.344262 joseki-2.1.0/LICENSE
--rw-r--r--   0        0        0     1612 2023-02-17 12:42:20.344262 joseki-2.1.0/README.md
--rw-r--r--   0        0        0     1769 2023-02-17 12:42:20.348263 joseki-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      337 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/__init__.py
--rw-r--r--   0        0        0     3769 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/__main__.py
--rw-r--r--   0        0        0       22 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/__version__.py
--rw-r--r--   0        0        0    12451 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/accessor.py
--rw-r--r--   0        0        0     2606 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/core.py
--rw-r--r--   0        0        0       92 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/README.md
--rw-r--r--   0        0        0       22 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/__init__.py
--rw-r--r--   0        0        0      396 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/README.md
--rw-r--r--   0        0        0       84 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/__init__.py
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1a.csv
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1b.csv
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1c.csv
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1d.csv
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1e.csv
--rw-r--r--   0        0        0     3871 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_1f.csv
--rw-r--r--   0        0        0     3422 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_2a.csv
--rw-r--r--   0        0        0     3423 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_2b.csv
--rw-r--r--   0        0        0     3426 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_2c.csv
--rw-r--r--   0        0        0     3429 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/afgl_1986/table_2d.csv
--rw-r--r--   0        0        0     1788 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/mipas_2007/README.md
--rw-r--r--   0        0        0       93 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/mipas_2007/__init__.py
--rw-r--r--   0        0        0     5683 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/mipas_2007/extra.atm
--rw-r--r--   0        0        0    42274 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/mipas_2007/midlatitude_day.atm
--rw-r--r--   0        0        0    42276 2023-02-17 12:42:20.348263 joseki-2.1.0/src/joseki/data/mipas_2007/midlatitude_night.atm
--rw-r--r--   0        0        0    42270 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/data/mipas_2007/polar_summer.atm
--rw-r--r--   0        0        0    42270 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/data/mipas_2007/polar_winter.atm
--rw-r--r--   0        0        0    42270 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/data/mipas_2007/tropical.atm
--rw-r--r--   0        0        0      789 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/__init__.py
--rw-r--r--   0        0        0    13298 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/afgl_1986.py
--rw-r--r--   0        0        0     7713 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/core.py
--rw-r--r--   0        0        0     1921 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/factory.py
--rw-r--r--   0        0        0    11728 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/mipas_2007.py
--rw-r--r--   0        0        0    10285 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/schema.py
--rw-r--r--   0        0        0     2889 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/ussa_1976.py
--rw-r--r--   0        0        0      231 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/profiles/util.py
--rw-r--r--   0        0        0      979 2023-02-17 12:42:20.352263 joseki-2.1.0/src/joseki/units.py
--rw-r--r--   0        0        0       41 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/__init__.py
--rw-r--r--   0        0        0     1556 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/test_afgl_1986.py
--rw-r--r--   0        0        0     1290 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/test_core.py
--rw-r--r--   0        0        0      160 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/test_factory.py
--rw-r--r--   0        0        0     6159 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/test_mipas_2007.py
--rw-r--r--   0        0        0      233 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/profiles/test_ussa_1976.py
--rw-r--r--   0        0        0     6272 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/test_accessor.py
--rw-r--r--   0        0        0     4399 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/test_core.py
--rw-r--r--   0        0        0     2918 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/test_main.py
--rw-r--r--   0        0        0      808 2023-02-17 12:42:20.352263 joseki-2.1.0/tests/test_units.py
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 joseki-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-18 07:37:59.771823 joseki-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2042 2023-07-18 07:37:59.771823 joseki-2.2.0/README.md
+-rw-r--r--   0        0        0     1813 2023-07-18 07:37:59.775823 joseki-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      401 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__init__.py
+-rw-r--r--   0        0        0     3769 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__version__.py
+-rw-r--r--   0        0        0    15568 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/accessor.py
+-rw-r--r--   0        0        0     1741 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/constants.py
+-rw-r--r--   0        0        0     2899 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/core.py
+-rw-r--r--   0        0        0       92 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/README.md
+-rw-r--r--   0        0        0       22 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/README.md
+-rw-r--r--   0        0        0       84 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/__init__.py
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1a.csv
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1b.csv
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1c.csv
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1d.csv
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1e.csv
+-rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1f.csv
+-rw-r--r--   0        0        0     3422 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2a.csv
+-rw-r--r--   0        0        0     3423 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2b.csv
+-rw-r--r--   0        0        0     3426 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2c.csv
+-rw-r--r--   0        0        0     3429 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2d.csv
+-rw-r--r--   0        0        0      151 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/ecmwf/README.md
+-rw-r--r--   0        0        0     4542 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/ecmwf/model_levels_60.csv
+-rw-r--r--   0        0        0     1788 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/README.md
+-rw-r--r--   0        0        0       93 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/__init__.py
+-rw-r--r--   0        0        0     5683 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/extra.atm
+-rw-r--r--   0        0        0    42274 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_day.atm
+-rw-r--r--   0        0        0    42276 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_night.atm
+-rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/polar_summer.atm
+-rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/polar_winter.atm
+-rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/tropical.atm
+-rw-r--r--   0        0        0      789 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/profiles/__init__.py
+-rw-r--r--   0        0        0    13295 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/profiles/afgl_1986.py
+-rw-r--r--   0        0        0    27398 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/cams.py
+-rw-r--r--   0        0        0    13343 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/core.py
+-rw-r--r--   0        0        0     1921 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/factory.py
+-rw-r--r--   0        0        0    11728 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/mipas_2007.py
+-rw-r--r--   0        0        0    10466 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/schema.py
+-rw-r--r--   0        0        0     2887 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/ussa_1976.py
+-rw-r--r--   0        0        0     4404 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/util.py
+-rw-r--r--   0        0        0      393 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/tests_util.py
+-rw-r--r--   0        0        0     3325 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/units.py
+-rw-r--r--   0        0        0       41 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2168 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc
+-rw-r--r--   0        0        0    11316 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip
+-rw-r--r--   0        0        0    54028 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc
+-rw-r--r--   0        0        0     1496 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc
+-rw-r--r--   0        0        0    55752 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip
+-rw-r--r--   0        0        0     2046 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_afgl_1986.py
+-rw-r--r--   0        0        0     7227 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_cams.py
+-rw-r--r--   0        0        0     7018 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_core.py
+-rw-r--r--   0        0        0      160 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_factory.py
+-rw-r--r--   0        0        0     6159 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_mipas_2007.py
+-rw-r--r--   0        0        0      233 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_ussa_1976.py
+-rw-r--r--   0        0        0      767 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_util.py
+-rw-r--r--   0        0        0     7066 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_accessor.py
+-rw-r--r--   0        0        0     4582 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_core.py
+-rw-r--r--   0        0        0     2918 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     1972 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_units.py
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 joseki-2.2.0/PKG-INFO
```

### Comparing `joseki-2.1.0/LICENSE` & `joseki-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/README.md` & `joseki-2.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Reference atmosphere's thermophysical profiles for radiative transfer
 applications in Earth's atmosphere.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![code-style-black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/joseki)](https://pypi.python.org/pypi/joseki/)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/joseki)](https://anaconda.org/conda-forge/joseki)
 [![Coverage](https://codecov.io/gh/nollety/joseki/branch/main/graph/badge.svg)](https://codecov.io/gh/nollety/joseki)
 
 
 This package gathers together datasets of thermophysical properties of the
 Earth's atmosphere relevant for radiative transfer applications, and provides
 utilities to compute common caracteristic quantities as well as to perform
 different operations, such as interpolation and rescaling, on a dataset.
@@ -45,8 +46,16 @@
 
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
-Visit https://nollety.github.io/joseki/.
+Visit https://nollety.github.io/joseki/.
+
+## Ikigai
+
+*Joseki* was born in the context of the development of the 
+[Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
+the need to collect, document and trace, integrate and modify *popular* 
+thermophysical profiles.
+As such, its features evolve in close relationship to those of *Eradiate*.
```

### Comparing `joseki-2.1.0/pyproject.toml` & `joseki-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "xarray>=2022.12.0",
     "ussa1976>=0.3.4",
     "attrs>=22.2.0",
     "importlib-resources>=5.10.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "2.1.0"
+version = "2.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Changelog = "https://github.com/nollety/joseki/blob/main/docs/changelog.md"
 homepage = "https://github.com/nollety/joseki"
@@ -40,19 +40,21 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "jupyterlab>=3.5.3",
     "ipykernel>=6.21.0",
     "ipython>=8.9.0",
     "matplotlib>=3.6.3",
+    "nbstripout>=0.6.1",
 ]
 docs = [
     "mkdocs>=1.4.2",
     "mkdocstrings[python]>=0.20.0",
     "mkdocs-material>=9.0.10",
+    "mike>=1.1.2",
 ]
 test = [
     "pytest>=7.2.1",
     "coverage>=7.1.0",
 ]
 
 [tool.pdm.version]
```

### Comparing `joseki-2.1.0/src/joseki/__main__.py` & `joseki-2.2.0/src/joseki/__main__.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/core.py` & `joseki-2.2.0/src/joseki/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 """Core module."""
+from __future__ import annotations
+
 import logging
 import os
 import typing as t
 
 import pint
 import xarray as xr
 
 from .profiles.factory import factory
-from .profiles.core import represent_profile_in_cells, DEFAULT_METHOD
+from .profiles.core import (
+    DEFAULT_METHOD,
+    represent_profile_in_cells,
+    select_molecules,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def make(
     identifier: str,
-    z: t.Optional[pint.Quantity] = None,
-    interp_method: t.Optional[t.Mapping[str, str]] = DEFAULT_METHOD,
+    z: pint.Quantity | None = None,
+    interp_method: t.Mapping[str, str] | None = DEFAULT_METHOD,
     represent_in_cells: bool = False,
     conserve_column: bool = False,
+    molecules: t.List[str] | None = None,
     **kwargs: t.Any,
 ) -> xr.Dataset:
     """
     Create a profile with the specified identifier.
 
     Args:
         identifier: Profile identifier.
         z: Altitude values.
         interp_method: Mapping of variable and interpolation method.
         represent_in_cells: If `True`, compute the altitude layer centers and 
             interpolate the profile on the layer centers, and return the 
             interpolated profile.
         conserve_column: If `True`, ensure that column densities are conserved
             during interpolation.
+        molecules: List of molecules to include in the profile.
         kwargs: Additional keyword arguments passed to the profile constructor.
     
     Returns:
         Profile as xarray.Dataset.
     """
     logger.info("Creating profile %s", identifier)
     logger.debug("z: %s", z)
     logger.debug("interp_method: %s", interp_method)
     logger.debug("represent_in_cells: %s", represent_in_cells)
     logger.debug("conserve_column: %s", conserve_column)
+    logger.debug("molecules: %s", molecules)
     logger.debug("kwargs: %s", kwargs)
 
     profile = factory.create(identifier)
 
     logger.debug("exporting profile to xarray.Dataset")
     ds = profile.to_dataset(
         z=z,
@@ -57,14 +66,17 @@
     if represent_in_cells:
         ds = represent_profile_in_cells(
             ds,
             method=interp_method,
             conserve_column=conserve_column,
         )
     
+    if molecules is not None:
+        ds = select_molecules(ds, molecules)
+    
     return ds
 
 
 def open_dataset(path: os.PathLike, *args, **kwargs) -> xr.Dataset:
     """
     Thin wrapper around `xarray.open_dataset`.
     
@@ -93,8 +105,8 @@
 def identifiers() -> t.List[str]:
     """
     List all registered profile identifiers.
 
     Returns:
         List of all registered profile identifiers.
     """
-    return factory.registered_identifiers
+    return factory.registered_identifiers
```

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1a.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1b.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1c.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1d.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1e.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1e.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_1f.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_1f.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_2a.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_2a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_2b.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_2b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_2c.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_2c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/afgl_1986/table_2d.csv` & `joseki-2.2.0/src/joseki/data/afgl_1986/table_2d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/README.md` & `joseki-2.2.0/src/joseki/data/mipas_2007/README.md`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/extra.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/extra.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/midlatitude_day.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_day.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/midlatitude_night.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_night.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/polar_summer.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/polar_summer.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/polar_winter.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/polar_winter.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/data/mipas_2007/tropical.atm` & `joseki-2.2.0/src/joseki/data/mipas_2007/tropical.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/profiles/__init__.py` & `joseki-2.2.0/src/joseki/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/profiles/afgl_1986.py` & `joseki-2.2.0/src/joseki/profiles/afgl_1986.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,19 +149,19 @@
     data_vars["p"] = ureg.Quantity(df.p.values, "millibar").to("Pa")
     data_vars["t"] = ureg.Quantity(df.t.values, "K")
     data_vars["n"] = ureg.Quantity(df.n.values, "cm^-3").to("m^-3")
 
     for s in molecules:
         data_vars[f"x_{s}"] = (
             df[s].values * ureg.ppm
-        )  # raw data volume fraction are given in ppmv
+        )  # raw data mole fraction are given in ppmv
 
     # attributes
     pretty_identifier = f"AFGL (1986) {identifier.value.replace('_', '-')}"
-    pretty_title = f"{pretty_identifier} atmosphere thernmophysical profile"
+    pretty_title = f"{pretty_identifier} atmosphere thermophysical profile"
 
     attrs = {
         "Conventions": "CF-1.10",
         "title": pretty_title,
         "institution": INSTITUION,
         "source": SOURCE,
         "history": history(),
```

### Comparing `joseki-2.1.0/src/joseki/profiles/factory.py` & `joseki-2.2.0/src/joseki/profiles/factory.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/profiles/mipas_2007.py` & `joseki-2.2.0/src/joseki/profiles/mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/src/joseki/profiles/schema.py` & `joseki-2.2.0/src/joseki/profiles/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 import pint
 
 from ..__version__ import __version__
 from ..units import ureg
-from .util import utcnow
+from .util import utcnow, number_density
 
 logger = logging.getLogger(__name__)
 
 
 def history() -> str:
     return f"{utcnow()} dataset formatting by joseki version {__version__}."
 
 
-def volume_fraction_sum(ds: xr.Dataset) -> pint.Quantity:
-    """Compute the sum of volume mixing fractions.
+def mole_fraction_sum(ds: xr.Dataset) -> pint.Quantity:
+    """Compute the sum of mole fractions.
 
     Args:
         ds: Dataset.
 
     Returns:
-        The sum of volume fractions.
+        The sum of mole fractions.
     """
     return (
         sum([ds[c] for c in ds.data_vars if c.startswith("x_")]).values
         * ureg.dimensionless
     )
 
 @define(frozen=True)
@@ -62,22 +62,22 @@
         "url": str,
         "urldate": str,
     }
 
     def validate(
         self,
         ds: xr.Dataset,
-        check_volume_fraction_sum: bool = False,
+        check_x_sum: bool = False,
         ret_true_if_valid: bool = False,
     ) -> t.Optional[bool]:
         """Validate dataset.
 
         Args:
             ds: Dataset to validate.
-            check_volume_fraction_sum: if True, check that volume fraction sums
+            check_x_sum: if True, check that mole fraction sums
                 are never larger than one.
             ret_true_if_valid: make this method return True if the dataset is
                 valid.
 
         Raises:
             ValueError: If the dataset does not match the schema.
         
@@ -163,29 +163,29 @@
             if var.startswith("x_"):
                 m = var[2:]
                 if ds[var].attrs["units"] != "dimensionless":
                     raise ValueError(  # pragma: no cover
                         f"incorrect units for {var}. Expected dimensionless, "
                         f"got {ds[var].attrs['units']}"
                     )
-                if ds[var].attrs["standard_name"] != f"{m}_volume_fraction":
+                if ds[var].attrs["standard_name"] != f"{m}_mole_fraction":
                     raise ValueError(  # pragma: no cover
                         f"incorrect standard name for {var}. Expected "
-                        f"{m}_volume_fraction, got "
+                        f"{m}_mole_fraction, got "
                         f"{ds[var].attrs['standard_name']}"
                     )
 
-        if check_volume_fraction_sum:
+        if check_x_sum:
             logger.debug(
-                "Checking that volume fraction sums are never larger than one"
+                "Checking that mole fraction sums are never larger than one"
             )
-            vfs = volume_fraction_sum(ds)
+            vfs = mole_fraction_sum(ds)
             if np.any(vfs.m > 1):
                 raise ValueError(  # pragma: no cover
-                    "The rescaling factors lead to a profile where the volume "
+                    "The rescaling factors lead to a profile where the mole "
                     "fraction sum is larger than 1."
                 )
 
         logger.info("Dataset is valid")
 
         if ret_true_if_valid:  # pragma: no cover
             return True
@@ -207,16 +207,24 @@
             Dataset with schema-compliant data variables, coordinates, and
             attributes.
         """
         logger.debug("converting input to schema-compliant dataset")
 
         logger.debug("checking that all data variables are present")
         for var in self.data_vars:
-            if var not in data_vars:
-                raise ValueError(f"missing data variable: {var}")  # pragma: no cover
+            if var == "n" not in data_vars:
+                n = number_density(
+                    p=data_vars["p"],
+                    t=data_vars["t"],
+                )
+                data_vars["n"] = n
+            else:
+                if var not in data_vars:
+                    raise ValueError(f"missing data variable: {var}")  # pragma: no cover
+
 
         logger.debug("checking that there is at least one x_ data variable")
         if not any([name.startswith("x_") for name in data_vars]):
             raise ValueError("missing data variable starting with x_")  # pragma: no cover
 
         logger.debug("checking that all coordinates are present")
         for coord in self.coords:
@@ -244,16 +252,16 @@
         for var in data_vars:
             if var.startswith("x_"):
                 m = var[2:]
                 data_vars[var] = (
                     "z",
                     data_vars[var].m_as("dimensionless"),
                     {
-                        "standard_name": f"{m}_volume_fraction",
-                        "long_name": f"{m} volume fraction",
+                        "standard_name": f"{m}_mole_fraction",
+                        "long_name": f"{m} mole fraction",
                         "units": "dimensionless",
                     },
                 )
 
         logger.debug("converting coordinates")
         for attr, (_, _, units, standard_name) in self.coords.items():
             coords[attr] = (
```

### Comparing `joseki-2.1.0/src/joseki/profiles/ussa_1976.py` & `joseki-2.2.0/src/joseki/profiles/ussa_1976.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         coords = {"z": to_quantity(ds["z"]).to("km")}
 
         data_vars = {}
         data_vars["p"] = to_quantity(ds["p"]).to("Pa")
         data_vars["t"] = to_quantity(ds["t"]).to("K")
         data_vars["n"] = to_quantity(ds["n_tot"]).to("m^-3")
 
-        # compute volume fraction
+        # compute mole fraction
         for s in ds["s"].values:
             nx = to_quantity(ds["n"].sel(s=s))
             n_tot = to_quantity(ds["n_tot"])
             data_vars[f"x_{s}"] = (nx / n_tot).to("dimensionless")
 
         attrs = {
             "Conventions": "CF-1.10",
```

### Comparing `joseki-2.1.0/tests/profiles/test_afgl_1986.py` & `joseki-2.2.0/tests/profiles/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/tests/profiles/test_mipas_2007.py` & `joseki-2.2.0/tests/profiles/test_mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/tests/test_accessor.py` & `joseki-2.2.0/tests/test_accessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,18 +101,18 @@
 @pytest.mark.parametrize(
     "identifier, expected",
     [
         ("afgl_1986-us_standard", 0.000330 * ureg.dimensionless),
         ("mipas_2007-midlatitude_day", 0.0003685 * ureg.dimensionless)
     ]
 )
-def test_volume_fraction_at_sea_level(identifier: str, expected):
-    """CO2 volume mixing fraction at sea level matches expected value."""
+def test_mole_fraction_at_sea_level(identifier: str, expected):
+    """CO2 mole mixing fraction at sea level matches expected value."""
     ds = joseki.make(identifier)
-    value = ds.joseki.volume_fraction_at_sea_level["CO2"].to(ureg.dimensionless)
+    value = ds.joseki.mole_fraction_at_sea_level["CO2"].to(ureg.dimensionless)
     assert_approx_equal(value.m, expected.m)
 
 
 def test_scaling_factor():
     """Returns 2.0 when target amount is twice larger than initial amount."""
     initial = 5 * ureg.m
     target = 10 * ureg.m
@@ -176,9 +176,36 @@
 )
 def test_rescale_invalid(identifier: str):
     """A UserWarning is raised if invalid scaling factors are passed."""
     ds = joseki.make(identifier)
     with pytest.raises(ValueError):
         ds.joseki.rescale(
             factors={"O2": 2.0},
-            check_volume_fraction_sum=True,
+            check_x_sum=True,
         )
+
+def test_rescale_to_column_mass_density():
+    """Column mass density of H2O matches target value."""
+    ds = joseki.make("afgl_1986-midlatitude_summer")
+    target = {
+        "H2O": 20.0 * ureg.kg * ureg.m**-2,
+    }
+    rescaled = ds.joseki.rescale_to(target)
+    assert_approx_equal(
+        rescaled.joseki.column_mass_density["H2O"].m,
+        target["H2O"].m,
+        significant=3,
+    )
+
+@pytest.mark.parametrize(
+    "molecules",
+    [
+        ["H2O"],
+        ["H2O", "CO2"],
+    ]
+)
+def test_drop_molecules(molecules):
+    """x_M data variable is(are) dropped."""
+    ds = joseki.make("afgl_1986-midlatitude_summer")
+    assert all([m in ds.joseki.molecules for m in molecules])
+    dropped = ds.joseki.drop_molecules(molecules)
+    assert all([m not in dropped.joseki.molecules for m in molecules])
```

### Comparing `joseki-2.1.0/tests/test_core.py` & `joseki-2.2.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,19 @@
     for m in ds0.joseki.molecules:
         assert_approx_equal(
             ds0.joseki.column_number_density[m].m,
             ds1.joseki.column_number_density[m].m,
             significant=6
         )
 
+def test_select_molecules():
+    """Returns xr.Dataset."""
+    ds = make(identifier="afgl_1986-tropical", molecules=["H2O", "CO2"])
+    assert ds.joseki.molecules == ["H2O", "CO2"]
+
 def test_open_dataset(tmpdir):
     """Returns xr.Dataset."""
     ds = make(identifier="afgl_1986-tropical")
     path = tmpdir.join("test.nc")
     ds.to_netcdf(path)
     ds2 = open_dataset(path)
     assert ds2.joseki.is_valid
@@ -141,8 +146,8 @@
     path = tmpdir.join("test.nc")
     ds.to_netcdf(path)
     ds2 = load_dataset(path)
     assert ds2.joseki.is_valid
 
 def test_identifiers():
     """Returns list of identifiers."""
-    assert isinstance(identifiers(), list)
+    assert isinstance(identifiers(), list)
```

### Comparing `joseki-2.1.0/tests/test_main.py` & `joseki-2.2.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `joseki-2.1.0/PKG-INFO` & `joseki-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joseki
-Version: 2.1.0
+Version: 2.2.0
 Summary: Reference atmosphere's thermophysical profiles for radiative transfer applications in Earth's atmosphere.
 License: MIT
 Author-email: Yvan Nollet <yvan.nollet@rayference.eu>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -19,14 +19,15 @@
 Reference atmosphere's thermophysical profiles for radiative transfer
 applications in Earth's atmosphere.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![code-style-black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI](https://img.shields.io/pypi/v/joseki)](https://pypi.python.org/pypi/joseki/)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/joseki)](https://anaconda.org/conda-forge/joseki)
 [![Coverage](https://codecov.io/gh/nollety/joseki/branch/main/graph/badge.svg)](https://codecov.io/gh/nollety/joseki)
 
 
 This package gathers together datasets of thermophysical properties of the
 Earth's atmosphere relevant for radiative transfer applications, and provides
 utilities to compute common caracteristic quantities as well as to perform
 different operations, such as interpolation and rescaling, on a dataset.
@@ -62,7 +63,16 @@
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
 Visit https://nollety.github.io/joseki/.
+
+## Ikigai
+
+*Joseki* was born in the context of the development of the 
+[Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
+the need to collect, document and trace, integrate and modify *popular* 
+thermophysical profiles.
+As such, its features evolve in close relationship to those of *Eradiate*.
+
```

