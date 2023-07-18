# Comparing `tmp/sierras-0.2.4.tar.gz` & `tmp/sierras-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierras-0.2.4.tar", last modified: Wed Jul 12 18:50:05 2023, max compression
+gzip compressed data, was "sierras-0.2.5.tar", last modified: Tue Jul 18 17:45:02 2023, max compression
```

## Comparing `sierras-0.2.4.tar` & `sierras-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:05.949802 sierras-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 18:49:45.000000 sierras-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 18:49:45.000000 sierras-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-12 18:50:05.949802 sierras-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-12 18:49:45.000000 sierras-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-12 18:49:45.000000 sierras-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:50:05.949802 sierras-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:50:05.945802 sierras-0.2.4/sierras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 18:50:05.000000 sierras-0.2.4/sierras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-12 18:49:45.000000 sierras-0.2.4/sierras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-12 18:49:45.000000 sierras-0.2.4/test_sierras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:45:02.504798 sierras-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 17:44:45.000000 sierras-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 17:44:45.000000 sierras-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-18 17:45:02.504798 sierras-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-18 17:44:45.000000 sierras-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-18 17:44:45.000000 sierras-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:45:02.504798 sierras-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:45:02.504798 sierras-0.2.5/sierras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-18 17:45:02.000000 sierras-0.2.5/sierras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-18 17:45:02.000000 sierras-0.2.5/sierras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:45:02.000000 sierras-0.2.5/sierras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 17:45:02.000000 sierras-0.2.5/sierras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 17:45:02.000000 sierras-0.2.5/sierras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-18 17:44:45.000000 sierras-0.2.5/sierras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-07-18 17:44:45.000000 sierras-0.2.5/test_sierras.py
```

### Comparing `sierras-0.2.4/LICENSE` & `sierras-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sierras-0.2.4/PKG-INFO` & `sierras-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.4
+Version: 0.2.5
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/fernandezfran/sierras/badge.svg)](https://coveralls.io/github/fernandezfran/sierras)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
 [![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
 [![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
 [![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
@@ -70,24 +71,29 @@
 
 
 ## Usage
 
 A simple example of use:
 
 ```python
-import sierras
+from sierras import ArrheniusRegressor
 
-areg = sierras.ArrheniusRegressor()
+# default constant is Boltzmann in eV/K
+areg = ArrheniusRegressor()
 
+# temperatures and target_process arrays-like as usually used in scikit-learn 
 areg.fit(Temperatures, target_process)
 
-areg.activation_energy_  # in this case in eV
-areg.extrapolated_process_  # extrapolated process at room temperature
-
-areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
+# print the activation energy ([eV] in the default case) and the extrapolated 
+# process at room temperatures values (in the same units as target_process is)
+print(areg.activation_energy_, areg.extrapolated_process_)
+
+# plot the fitting
+fig, ax = plt.subplots()
+areg.plot(ax=ax)
 ```
 
 
 For a more detailed explanation you can read the 
 [tutorial](https://sierras.readthedocs.io/en/latest/tutorial.html) 
 and the [API](https://sierras.readthedocs.io/en/latest/api.html).
```

### Comparing `sierras-0.2.4/README.md` & `sierras-0.2.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/fernandezfran/sierras/badge.svg)](https://coveralls.io/github/fernandezfran/sierras)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
 [![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
 [![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
 [![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
@@ -29,24 +30,29 @@
 
 
 ## Usage
 
 A simple example of use:
 
 ```python
-import sierras
+from sierras import ArrheniusRegressor
 
-areg = sierras.ArrheniusRegressor()
+# default constant is Boltzmann in eV/K
+areg = ArrheniusRegressor()
 
+# temperatures and target_process arrays-like as usually used in scikit-learn 
 areg.fit(Temperatures, target_process)
 
-areg.activation_energy_  # in this case in eV
-areg.extrapolated_process_  # extrapolated process at room temperature
-
-areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
+# print the activation energy ([eV] in the default case) and the extrapolated 
+# process at room temperatures values (in the same units as target_process is)
+print(areg.activation_energy_, areg.extrapolated_process_)
+
+# plot the fitting
+fig, ax = plt.subplots()
+areg.plot(ax=ax)
 ```
 
 
 For a more detailed explanation you can read the 
 [tutorial](https://sierras.readthedocs.io/en/latest/tutorial.html) 
 and the [API](https://sierras.readthedocs.io/en/latest/api.html).
```

### Comparing `sierras-0.2.4/pyproject.toml` & `sierras-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sierras"
-version = "0.2.4"
+version = "0.2.5"
 authors = [{name = "Francisco Fernandez", email = "ffernandev@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes."
 keywords = [
     "arrhenius-process",
     "arrhenius-equation",
```

### Comparing `sierras-0.2.4/sierras.egg-info/PKG-INFO` & `sierras-0.2.5/sierras.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.4
+Version: 0.2.5
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
 Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/fernandezfran/sierras/badge.svg)](https://coveralls.io/github/fernandezfran/sierras)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
 [![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
 [![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
 [![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
@@ -70,24 +71,29 @@
 
 
 ## Usage
 
 A simple example of use:
 
 ```python
-import sierras
+from sierras import ArrheniusRegressor
 
-areg = sierras.ArrheniusRegressor()
+# default constant is Boltzmann in eV/K
+areg = ArrheniusRegressor()
 
+# temperatures and target_process arrays-like as usually used in scikit-learn 
 areg.fit(Temperatures, target_process)
 
-areg.activation_energy_  # in this case in eV
-areg.extrapolated_process_  # extrapolated process at room temperature
-
-areg.plot.arrhenius(Temperatures, target_process)  # plot the fitting
+# print the activation energy ([eV] in the default case) and the extrapolated 
+# process at room temperatures values (in the same units as target_process is)
+print(areg.activation_energy_, areg.extrapolated_process_)
+
+# plot the fitting
+fig, ax = plt.subplots()
+areg.plot(ax=ax)
 ```
 
 
 For a more detailed explanation you can read the 
 [tutorial](https://sierras.readthedocs.io/en/latest/tutorial.html) 
 and the [API](https://sierras.readthedocs.io/en/latest/api.html).
```

### Comparing `sierras-0.2.4/sierras.py` & `sierras-0.2.5/sierras.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
 import matplotlib.pyplot as plt
 
 import numpy as np
 
 import pandas as pd
 
-import sklearn.linear_model
 from sklearn.base import BaseEstimator, RegressorMixin
+from sklearn.linear_model import LinearRegression
 
 # =============================================================================
 # CONSTANTS
 # =============================================================================
 
 __all__ = ["ArrheniusRegressor"]
 
@@ -126,15 +126,15 @@
         sample_weight : array-like of shape (n_samples,), defualt=None
             Individual weight of each thermally-induced value.
 
         **kwargs
             Keyword arguments that are passed and are documented in
             ``sklearn.linear_model.LinearRegression``.
         """
-        self.reg_ = sklearn.linear_model.LinearRegression(**kwargs)
+        self.reg_ = LinearRegression(**kwargs)
 
         self._X = 1 / X
         self._y = np.log(y)
         self._sample_weight = (
             sample_weight / y if sample_weight is not None else None
         )
```

### Comparing `sierras-0.2.4/test_sierras.py` & `sierras-0.2.5/test_sierras.py`

 * *Files identical despite different names*

