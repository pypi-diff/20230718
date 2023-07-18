# Comparing `tmp/evogression-0.8.1.tar.gz` & `tmp/evogression-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evogression-0.8.1.tar", last modified: Sun Jan 15 22:27:22 2023, max compression
+gzip compressed data, was "evogression-0.9.0.tar", last modified: Tue Jul 18 15:14:25 2023, max compression
```

## Comparing `evogression-0.8.1.tar` & `evogression-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 22:27:22.583052 evogression-0.8.1/
--rw-rw-rw-   0        0        0      404 2023-01-08 01:29:14.000000 evogression-0.8.1/Cargo.toml
--rw-rw-rw-   0        0        0     1090 2019-02-09 22:27:10.000000 evogression-0.8.1/LICENSE.txt
--rw-rw-rw-   0        0        0       85 2023-01-02 21:01:32.000000 evogression-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3402 2023-01-15 22:27:22.577865 evogression-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2815 2023-01-02 21:01:32.000000 evogression-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-15 22:27:22.182230 evogression-0.8.1/evogression/
--rw-rw-rw-   0        0        0      324 2023-01-14 23:01:34.000000 evogression-0.8.1/evogression/__init__.py
--rw-rw-rw-   0        0        0       25 2023-01-15 22:24:28.000000 evogression-0.8.1/evogression/_version.py
--rw-rw-rw-   0        0        0     2635 2023-01-14 22:51:09.000000 evogression-0.8.1/evogression/data.py
--rw-rw-rw-   0        0        0     5117 2023-01-14 23:01:34.000000 evogression-0.8.1/evogression/evolution.py
--rw-rw-rw-   0        0        0    12557 2023-01-15 22:24:28.000000 evogression-0.8.1/evogression/groups.py
-drwxrwxrwx   0        0        0        0 2023-01-15 22:27:22.262057 evogression-0.8.1/evogression.egg-info/
--rw-rw-rw-   0        0        0     3402 2023-01-15 22:27:21.000000 evogression-0.8.1/evogression.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-01-15 22:27:21.000000 evogression-0.8.1/evogression.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 22:27:21.000000 evogression-0.8.1/evogression.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-15 22:27:21.000000 evogression-0.8.1/evogression.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-15 22:27:21.000000 evogression-0.8.1/evogression.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       71 2023-01-02 21:01:32.000000 evogression-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-15 22:27:22.583052 evogression-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-01-08 01:46:47.000000 evogression-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-15 22:27:22.377316 evogression-0.8.1/src/
--rw-rw-rw-   0        0        0    25192 2023-01-08 01:29:14.000000 evogression-0.8.1/src/creature.rs
--rw-rw-rw-   0        0        0    17166 2023-01-08 01:29:14.000000 evogression-0.8.1/src/evolution.rs
--rw-rw-rw-   0        0        0     1014 2023-01-08 01:46:47.000000 evogression-0.8.1/src/lib.rs
--rw-rw-rw-   0        0        0     4005 2023-01-08 01:46:47.000000 evogression-0.8.1/src/standardize.rs
-drwxrwxrwx   0        0        0        0 2023-01-15 22:27:22.561874 evogression-0.8.1/tests/
--rw-rw-rw-   0        0        0       44 2019-03-14 04:19:52.000000 evogression-0.8.1/tests/__init__.py
--rw-rw-rw-   0        0        0   385324 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/data_examples.py
--rw-rw-rw-   0        0        0     2726 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/evolution_test.py
--rw-rw-rw-   0        0        0     1402 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/fitting_test.py
--rw-rw-rw-   0        0        0     3400 2023-01-15 22:24:28.000000 evogression-0.8.1/tests/group_test.py
--rw-rw-rw-   0        0        0      946 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/parameter_pruning_test.py
--rw-rw-rw-   0        0        0      989 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/surface_evolution_test.py
--rw-rw-rw-   0        0        0     1009 2023-01-14 23:01:34.000000 evogression-0.8.1/tests/surface_group_test.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:14:25.737995 evogression-0.9.0/
+-rw-rw-rw-   0        0        0      461 2023-07-18 14:54:35.000000 evogression-0.9.0/Cargo.toml
+-rw-rw-rw-   0        0        0     1090 2019-02-09 22:27:10.000000 evogression-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       85 2023-01-02 21:01:32.000000 evogression-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3402 2023-07-18 15:14:25.737995 evogression-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2815 2023-01-02 21:01:32.000000 evogression-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 15:14:25.726996 evogression-0.9.0/evogression/
+-rw-rw-rw-   0        0        0      330 2023-07-16 15:25:33.000000 evogression-0.9.0/evogression/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-07-18 14:53:43.000000 evogression-0.9.0/evogression/_version.py
+-rw-rw-rw-   0        0        0     2635 2023-04-25 03:26:58.000000 evogression-0.9.0/evogression/data.py
+-rw-rw-rw-   0        0        0     6305 2023-07-18 14:56:01.000000 evogression-0.9.0/evogression/evolution.py
+-rw-rw-rw-   0        0        0    12616 2023-07-15 22:25:30.000000 evogression-0.9.0/evogression/groups.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:14:25.729996 evogression-0.9.0/evogression.egg-info/
+-rw-rw-rw-   0        0        0     3402 2023-07-18 15:14:25.000000 evogression-0.9.0/evogression.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-07-18 15:14:25.000000 evogression-0.9.0/evogression.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 15:14:25.000000 evogression-0.9.0/evogression.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 15:14:25.000000 evogression-0.9.0/evogression.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-18 15:14:25.000000 evogression-0.9.0/evogression.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       71 2023-01-02 21:01:32.000000 evogression-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 15:14:25.737995 evogression-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1121 2023-01-08 01:46:47.000000 evogression-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 15:14:25.731995 evogression-0.9.0/src/
+-rw-rw-rw-   0        0        0    25506 2023-07-18 15:06:58.000000 evogression-0.9.0/src/creature.rs
+-rw-rw-rw-   0        0        0    17869 2023-07-18 15:07:49.000000 evogression-0.9.0/src/evolution.rs
+-rw-rw-rw-   0        0        0     1174 2023-07-16 15:24:58.000000 evogression-0.9.0/src/lib.rs
+-rw-rw-rw-   0        0        0     4113 2023-07-18 15:08:50.000000 evogression-0.9.0/src/standardize.rs
+drwxrwxrwx   0        0        0        0 2023-07-18 15:14:25.736995 evogression-0.9.0/tests/
+-rw-rw-rw-   0        0        0       44 2019-03-14 04:19:52.000000 evogression-0.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0   385324 2023-01-14 23:01:34.000000 evogression-0.9.0/tests/data_examples.py
+-rw-rw-rw-   0        0        0     3058 2023-07-18 14:46:34.000000 evogression-0.9.0/tests/evolution_test.py
+-rw-rw-rw-   0        0        0     1402 2023-01-14 23:01:34.000000 evogression-0.9.0/tests/fitting_test.py
+-rw-rw-rw-   0        0        0     3400 2023-01-15 22:24:28.000000 evogression-0.9.0/tests/group_test.py
+-rw-rw-rw-   0        0        0      946 2023-01-14 23:01:34.000000 evogression-0.9.0/tests/parameter_pruning_test.py
+-rw-rw-rw-   0        0        0      989 2023-01-14 23:01:34.000000 evogression-0.9.0/tests/surface_evolution_test.py
+-rw-rw-rw-   0        0        0     1009 2023-04-26 03:30:59.000000 evogression-0.9.0/tests/surface_group_test.py
```

### Comparing `evogression-0.8.1/LICENSE.txt` & `evogression-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/PKG-INFO` & `evogression-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evogression
-Version: 0.8.1
+Version: 0.9.0
 Summary: Evolutionary Regression
 Home-page: https://github.com/zachbateman/evogression.git
-Download-URL: https://github.com/zachbateman/evogression/archive/v_0.8.1.tar.gz
+Download-URL: https://github.com/zachbateman/evogression/archive/v_0.9.0.tar.gz
 Author: Zach Bateman
 License: MIT
 Keywords: REGRESSION,MACHINE,LEARNING,EVOLUTION
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `evogression-0.8.1/README.md` & `evogression-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/evogression/data.py` & `evogression-0.9.0/evogression/data.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/evogression/evolution.py` & `evogression-0.9.0/evogression/evolution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''
 Module containing evolution algorithm for regression.
 '''
 from collections import defaultdict
 import os
+import pickle
 from pandas import DataFrame
 from . import data as data_funcs
 from . import rust_evogression
 
 
 class Evolution:
     '''
@@ -98,7 +99,34 @@
                 for d, clean_row in zip(data, generate_clean_data(data)):
                     d[prediction_key] = self.model.predict_point(clean_row)
             case dict():
                 data[prediction_key] = self.model.predict_point(generate_clean_data([data])[0])
             case _:
                 print('Error!  "data" arg provided to .predict() must be a dict or list of dicts or DataFrame.')
         return data
+
+    def save(self, filename: str="model.evo") -> None:
+        self._model_serialized = self.model.to_json()
+        self.model = None  # Delete actual Rust object as can't pickle it
+
+        self._best_creature_serialized = self.best_creature.to_json()
+        self.best_creature = None  # Delete actual Rust object as can't pickle it
+
+        self.all_data = None  # Shrink object size - full data is not needed once initialized
+
+        cleaned_name = filename + '.evo' if '.' not in filename else filename
+
+        with open(cleaned_name, 'wb') as file:
+            pickle.dump(self, file)
+
+
+def load(filename: str="model.evo") -> Evolution:
+    cleaned_name = filename + '.evo' if '.' not in filename else filename
+
+    try:
+        with open(cleaned_name, 'rb') as file:
+            evo = pickle.load(file)
+        evo.model = rust_evogression.load_evolution_from_json(evo._model_serialized)
+        evo.best_creature = rust_evogression.load_creature_from_json(evo._best_creature_serialized)
+        return evo
+    except FileNotFoundError:
+        print(f'Saved model not found.  Please check that it is spelled correctly: "{filename}"')
```

### Comparing `evogression-0.8.1/evogression/groups.py` & `evogression-0.9.0/evogression/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 class EvoGroup:
     def __init__(self, models: list[Evolution]):
         self.models: list[Evolution] = models
 
     def __iter__(self):
         return (model for model in self.models)
 
+    def __len__(self):
+        return len(self.models)
+
     def output_regression(self, directory: str='regression_modules') -> None:
         '''Output each Evolution's regression as a new Python module.'''
         for model in self.models:
             model.output_regression(directory=directory, add_error_value=True)
 
     @property
     def parameter_usage(self) -> dict[str, int]:
```

### Comparing `evogression-0.8.1/evogression.egg-info/PKG-INFO` & `evogression-0.9.0/evogression.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: evogression
-Version: 0.8.1
+Version: 0.9.0
 Summary: Evolutionary Regression
 Home-page: https://github.com/zachbateman/evogression.git
-Download-URL: https://github.com/zachbateman/evogression/archive/v_0.8.1.tar.gz
+Download-URL: https://github.com/zachbateman/evogression/archive/v_0.9.0.tar.gz
 Author: Zach Bateman
 License: MIT
 Keywords: REGRESSION,MACHINE,LEARNING,EVOLUTION
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `evogression-0.8.1/evogression.egg-info/SOURCES.txt` & `evogression-0.9.0/evogression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/setup.py` & `evogression-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/src/creature.rs` & `evogression-0.9.0/src/creature.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,40 @@
 use rand_distr::{Normal, Triangular};
 use std::collections::{HashMap, HashSet};
 use std::fmt;
 use std::ops;
 use std::cmp;
 use itertools::izip;
 use rayon::prelude::*;
+use serde::{Serialize, Deserialize};
 use pyo3::prelude::*;
 
 use crate::standardize::Standardizer;
 
 
 fn num_layers() -> u8 {
     // Generate a random number of Creature modifier layers
     *[1, 1, 1, 2, 2, 3].choose(&mut rand::thread_rng()).unwrap()
 }
 
 
+#[pyfunction]
+pub fn load_creature_from_json(json: &str) -> Creature {
+    serde_json::from_str(&json).unwrap()
+}
+
+
 /**
 A "Creature" is essentially a randomly generated function.
 The equation of a creature can be one or more Coefficients in one or more
 LayerModifiers which function as one or more layers for a simple neural network.
 */
 #[pyclass]
 #[derive(Clone)]
+#[derive(Serialize, Deserialize)]
 pub struct Creature {
     equation: Vec<LayerModifiers>,
     pub cached_error_sum: Option<f32>,
     #[pyo3(get)]
     pub generation: u8,
     #[pyo3(get)]
     pub offspring: u8,
@@ -343,14 +351,18 @@
             }
 
             // Add in the bias "layer_bias" to the current layer's calculation.
             total = inner_total + layer_modifiers.layer_bias;
         }
         total
     }
+
+    fn to_json(&self) -> String {
+        serde_json::to_string(&self).unwrap()
+    }
 }
 
 impl Creature {
     // Create a string which creates a Python module with callable regression function
     pub fn python_regression_module_string(&self, standardizer: &Standardizer, target: &String) -> String {
         let mut s = "'''\nPython regression function module generated by Evogression\n'''\n\n".to_string();
         s += "def regression(parameters: dict) -> float:\n";
@@ -430,17 +442,17 @@
     }
 }
 
 /// Each "LayerModifiers" represents a full neural network layer.
 /// "modifiers" is a collection of Coefficents applied to certain input parameters.
 /// The "previous_layer_coefficients" field is Coefficients applied to a previous layer's output, if applicable.
 /// The "layer_bias" field is a bias added to the layer's calculation.
-#[derive(Clone)]
-#[derive(Debug)]
-#[derive(PartialEq)]
+
+#[derive(Debug, Clone, PartialEq)]
+#[derive(Serialize, Deserialize)]
 struct LayerModifiers {
     modifiers: HashMap<String, Coefficients>,
     previous_layer_coefficients: Option<Coefficients>,
     layer_bias: f32,
 }
 
 impl LayerModifiers {
@@ -480,17 +492,16 @@
         Ok(())
     }
 }
 
 /// A "Coefficients" struct contains 4 values which
 /// are used to form the following equation given input "param":
 /// Value = C * (B * param + Z) ^ X
-#[derive(Clone)]
-#[derive(Debug)]
-#[derive(PartialEq)]
+#[derive(Debug, Clone, PartialEq)]
+#[derive(Serialize, Deserialize)]
 struct Coefficients { c: f32, b: f32, z: f32, x: u8 }
 
 impl Coefficients {
     fn calculate(&self, &param_value: &f32) -> f32 {
         self.c * (self.b * param_value + self.z).powi(self.x as i32)
     }
```

### Comparing `evogression-0.8.1/src/evolution.rs` & `evogression-0.9.0/src/evolution.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 use rand::prelude::*;
 use std::collections::HashMap;
 use std::time::Instant;
 use crate::standardize::Standardizer;
 use crate::creature::{Creature, MutateSpeed};
 use rayon::prelude::*;
+use serde::{Serialize, Deserialize};
 use pyo3::prelude::*;
 
 #[pyclass]
+#[derive(Serialize, Deserialize)]
 pub struct Evolution {
     #[pyo3(get)]
     target: String,
     #[pyo3(get)]
     num_creatures: u32,
     #[pyo3(get)]
     num_cycles: u16,
@@ -36,15 +38,25 @@
     fn best_error(&self) -> f32 {
         self.best_creature.cached_error_sum.unwrap_or(999.9)
     }
 
     fn python_regression_module_string(&self) -> String {
         self.generate_python_regression_module_string()
     }
+
+    fn to_json(&self) -> String {
+        serde_json::to_string(&self).unwrap()
+    }
 }
+
+#[pyfunction]
+pub fn load_evolution_from_json(json: &str) -> Evolution {
+    serde_json::from_str(&json).unwrap()
+}
+
 impl Evolution {
     // Have this non-pymethods function as passing in &self.standardizer
     // was causing issues in the pymethods impl block
     fn generate_python_regression_module_string(&self) -> String {
         self.best_creature.python_regression_module_string(&self.standardizer, &self.target)
     }
 }
@@ -227,30 +239,44 @@
         // Now DON'T include any anomalous NaN calculations in resulting errors!
         match creature.cached_error_sum.unwrap() {
             x if !x.is_nan() => errors.push(x),
             _ => (),
         }
     }
     errors.sort_by(|a, b| a.total_cmp(b));
-    let median_error = errors[errors.len() / 2];
-    let min_error = errors[0];
-    (min_error, median_error)
+
+    match errors.len() {
+        x if x > 0 => {
+            let median_error = errors[errors.len() / 2];
+            let min_error = errors[0];
+            (min_error, median_error)
+        },
+        _ => {  // if an issue of no errors (very rare), throw huge errors instead of a panic
+            (99999.9, 99999.9)
+        }
+    }
+
 }
 
 fn error_results(creatures: &[Creature]) -> f32 {
     let mut errors = Vec::new();
     for creature in creatures.iter() {
         // Now DON'T include any anomalous NaN calculations in resulting errors!
         match creature.cached_error_sum.unwrap() {
             x if !x.is_nan() => errors.push(x),
             _ => (),
         }
     }
     errors.sort_by(|a, b| a.total_cmp(b));
-    errors[0]
+    match errors.len() {
+        x if x > 0 => {
+            errors[0]
+        },
+        _ => 99999.9  // if an issue of no errors (very rare), throw huge errors instead of a panic
+    }
 }
 
 fn kill_weak_creatures(creatures: Vec<Creature>, median_error: &f32) -> Vec<Creature> {
     creatures.into_par_iter()
              .filter(|creature| creature.cached_error_sum.unwrap() < *median_error)
              .collect()
 }
```

### Comparing `evogression-0.8.1/src/lib.rs` & `evogression-0.9.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -24,11 +24,13 @@
 }
 
 
 #[pymodule]
 fn rust_evogression(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(standardize_data, m)?)?;
     m.add_function(wrap_pyfunction!(run_evolution, m)?)?;
+    m.add_function(wrap_pyfunction!(evolution::load_evolution_from_json, m)?)?;
+    m.add_function(wrap_pyfunction!(creature::load_creature_from_json, m)?)?;
     m.add_class::<creature::Creature>()?;
     m.add_class::<evolution::Evolution>()?;
     Ok(())
 }
```

### Comparing `evogression-0.8.1/src/standardize.rs` & `evogression-0.9.0/src/standardize.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use std::collections::HashMap;
+use serde::{Serialize, Deserialize};
 
 
+#[derive(Serialize, Deserialize)]
 pub struct Standardizer {
     pub standardizers: HashMap<String, ParamStandardizer>,
 }
 
 impl Standardizer {
     pub fn new(data: &[HashMap<String, f32>]) -> Standardizer {
         let mut standardizers = HashMap::new();
@@ -45,14 +47,15 @@
         for (key, param_stand) in &self.standardizers {
             println!("Key: {}  ParamStand: {:?}", key, param_stand);
         }
     }
 }
 
 #[derive(Debug)]
+#[derive(Serialize, Deserialize)]
 pub struct ParamStandardizer {
     pub mean: f32,
     pub stdev: f32,
 }
 
 impl ParamStandardizer {
     fn new(values: &[&f32]) -> ParamStandardizer {
```

### Comparing `evogression-0.8.1/tests/data_examples.py` & `evogression-0.9.0/tests/data_examples.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/tests/evolution_test.py` & `evogression-0.9.0/tests/evolution_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import unittest
 import sys
 sys.path.insert(1, '..')
 import evogression
 from data_examples import linear_data, surface_3d_data, many_dimension_data
 import pandas
 
@@ -58,10 +59,19 @@
         test_data = linear_data
         test_data[1] = {'x': 5, 'y': None}
         test_data[4] = {'x': None, 'y': 11.2}
         test_data[5] = {'x': float('nan'), 'y': 11.2}
         test_data[6] = {'x': None, 'y': float('nan')}
         evogression.Evolution('y', test_data)
 
+    def test_save_and_load(self):
+        test_data = copy.deepcopy(linear_data)
+        evo = evogression.Evolution('y', test_data)
+        evo.save("test_save_data")
+
+        loaded_evo = evogression.load("test_save_data.evo")
+        prediction = loaded_evo.predict(test_data[0])
+        print(prediction)
+
 
 if __name__ == '__main__':
     unittest.main(buffer=True)
```

### Comparing `evogression-0.8.1/tests/fitting_test.py` & `evogression-0.9.0/tests/fitting_test.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/tests/group_test.py` & `evogression-0.9.0/tests/group_test.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/tests/parameter_pruning_test.py` & `evogression-0.9.0/tests/parameter_pruning_test.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/tests/surface_evolution_test.py` & `evogression-0.9.0/tests/surface_evolution_test.py`

 * *Files identical despite different names*

### Comparing `evogression-0.8.1/tests/surface_group_test.py` & `evogression-0.9.0/tests/surface_group_test.py`

 * *Files identical despite different names*

