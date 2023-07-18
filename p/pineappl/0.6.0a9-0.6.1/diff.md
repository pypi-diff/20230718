# Comparing `tmp/pineappl-0.6.0a9.tar.gz` & `tmp/pineappl-0.6.1.tar.gz`

## Comparing `pineappl-0.6.0a9.tar` & `pineappl-0.6.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/local_dependencies/pineappl/Cargo.toml
--rw-r--r--   0     1001      123      594 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/README.md
--rw-r--r--   0     1001      123    37886 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/bin.rs
--rw-r--r--   0     1001      123      256 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/convert.rs
--rw-r--r--   0     1001      123     2962 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/empty_subgrid.rs
--rw-r--r--   0     1001      123    22471 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/evolution.rs
--rw-r--r--   0     1001      123    15042 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/fk_table.rs
--rw-r--r--   0     1001      123    96582 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/grid.rs
--rw-r--r--   0     1001      123    25442 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123    43946 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lagrange_subgrid.rs
--rw-r--r--   0     1001      123      471 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lib.rs
--rw-r--r--   0     1001      123    16120 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lumi.rs
--rw-r--r--   0     1001      123     4853 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/ntuple_subgrid.rs
--rw-r--r--   0     1001      123    17098 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/pids.rs
--rw-r--r--   0     1001      123    36204 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/sparse_array3.rs
--rw-r--r--   0     1001      123    10342 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/subgrid.rs
--rw-r--r--   0     1001      123    16425 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/tests/drell_yan_lo.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/Cargo.toml
--rw-r--r--   0     1001      123      352 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/.gitignore
--rw-r--r--   0     1001      123      783 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/README.md
--rw-r--r--   0     1001      123      235 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/.gitignore
--rw-r--r--   0     1001      123      876 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/make.bat
--rw-r--r--   0     1001      123        0 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/_static/.gitkeep
--rw-r--r--   0     1001      123     6097 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/conf.py
--rw-r--r--   0     1001      123      886 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/implementation.rst
--rw-r--r--   0     1001      123     1295 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/index.rst
--rw-r--r--   0     1001      123       91 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/indices.rst
--rw-r--r--   0     1001      123     1148 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/installation.rst
--rw-r--r--   0     1001      123     2534 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/recipes.rst
--rw-r--r--   0     1001      123        0 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/refs.bib
--rw-r--r--   0     1001      123      951 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/shared/roles.rst
--rw-r--r--   0     1001      123      893 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/Containerfile
--rw-r--r--   0     1001      123     3584 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/README.md
--rwxr-xr-x   0     1001      123      219 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/maturin
--rw-r--r--   0     1001      123      115 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/__init__.py
--rw-r--r--   0     1001      123      516 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/bin.py
--rw-r--r--   0     1001      123     1688 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/fk_table.py
--rw-r--r--   0     1001      123    12585 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/grid.py
--rw-r--r--   0     1001      123      762 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/import_only_subgrid.py
--rw-r--r--   0     1001      123      379 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/lumi.py
--rw-r--r--   0     1001      123      254 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/subgrid.py
--rw-r--r--   0     1001      123      430 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/utils.py
--rw-r--r--   0     1001      123     1141 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pyproject.toml
--rw-r--r--   0     1001      123      674 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/bin.rs
--rw-r--r--   0     1001      123     1078 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/evolution.rs
--rw-r--r--   0     1001      123     6438 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/fk_table.rs
--rw-r--r--   0     1001      123    22338 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/grid.rs
--rw-r--r--   0     1001      123     1799 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123      874 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/lib.rs
--rw-r--r--   0     1001      123     1109 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/lumi.rs
--rw-r--r--   0     1001      123     4261 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/subgrid.rs
--rw-r--r--   0     1001      123      324 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/conftest.py
--rw-r--r--   0     1001      123      355 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_bin.py
--rw-r--r--   0     1001      123     6124 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_grid.py
--rw-r--r--   0     1001      123      237 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_lumi.py
--rw-r--r--   0     1001      123      868 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_sugrid.py
--rw-r--r--   0     1001      123    44640 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/Cargo.lock
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/PKG-INFO
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 pineappl-0.6.1/local_dependencies/pineappl/Cargo.toml
+-rw-r--r--   0     1001      123      594 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/README.md
+-rw-r--r--   0     1001      123    37830 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/bin.rs
+-rw-r--r--   0     1001      123      256 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/convert.rs
+-rw-r--r--   0     1001      123     2962 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/empty_subgrid.rs
+-rw-r--r--   0     1001      123    22593 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/evolution.rs
+-rw-r--r--   0     1001      123    15320 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/fk_table.rs
+-rw-r--r--   0     1001      123    97396 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/grid.rs
+-rw-r--r--   0     1001      123    25442 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123    43946 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/lagrange_subgrid.rs
+-rw-r--r--   0     1001      123      471 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/lib.rs
+-rw-r--r--   0     1001      123    16120 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/lumi.rs
+-rw-r--r--   0     1001      123     4968 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/ntuple_subgrid.rs
+-rw-r--r--   0     1001      123    17098 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/pids.rs
+-rw-r--r--   0     1001      123    36204 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/sparse_array3.rs
+-rw-r--r--   0     1001      123    10761 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/src/subgrid.rs
+-rw-r--r--   0     1001      123    16425 2023-07-18 07:02:15.000000 pineappl-0.6.1/local_dependencies/pineappl/tests/drell_yan_lo.rs
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 pineappl-0.6.1/Cargo.toml
+-rw-r--r--   0     1001      123      352 2023-07-18 07:02:15.000000 pineappl-0.6.1/.gitignore
+-rw-r--r--   0     1001      123      783 2023-07-18 07:02:15.000000 pineappl-0.6.1/README.md
+-rw-r--r--   0     1001      123      235 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/.gitignore
+-rw-r--r--   0     1001      123      876 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/make.bat
+-rw-r--r--   0     1001      123        0 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/_static/.gitkeep
+-rw-r--r--   0     1001      123     6097 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/conf.py
+-rw-r--r--   0     1001      123      886 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/implementation.rst
+-rw-r--r--   0     1001      123     1295 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/index.rst
+-rw-r--r--   0     1001      123       91 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/indices.rst
+-rw-r--r--   0     1001      123     1148 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/installation.rst
+-rw-r--r--   0     1001      123     2534 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/recipes.rst
+-rw-r--r--   0     1001      123        0 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/refs.bib
+-rw-r--r--   0     1001      123      951 2023-07-18 07:02:15.000000 pineappl-0.6.1/docs/source/shared/roles.rst
+-rw-r--r--   0     1001      123      893 2023-07-18 07:02:15.000000 pineappl-0.6.1/package/Containerfile
+-rw-r--r--   0     1001      123     3584 2023-07-18 07:02:15.000000 pineappl-0.6.1/package/README.md
+-rwxr-xr-x   0     1001      123      219 2023-07-18 07:02:15.000000 pineappl-0.6.1/package/maturin
+-rw-r--r--   0     1001      123      115 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/__init__.py
+-rw-r--r--   0     1001      123      516 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/bin.py
+-rw-r--r--   0     1001      123     1688 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/fk_table.py
+-rw-r--r--   0     1001      123    12585 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/grid.py
+-rw-r--r--   0     1001      123     1467 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/import_only_subgrid.py
+-rw-r--r--   0     1001      123      379 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/lumi.py
+-rw-r--r--   0     1001      123      359 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/subgrid.py
+-rw-r--r--   0     1001      123      430 2023-07-18 07:02:15.000000 pineappl-0.6.1/pineappl/utils.py
+-rw-r--r--   0     1001      123     1141 2023-07-18 07:02:15.000000 pineappl-0.6.1/pyproject.toml
+-rw-r--r--   0     1001      123      674 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/bin.rs
+-rw-r--r--   0     1001      123     1078 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/evolution.rs
+-rw-r--r--   0     1001      123     6438 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/fk_table.rs
+-rw-r--r--   0     1001      123    22338 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/grid.rs
+-rw-r--r--   0     1001      123     3465 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123     1001 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/lib.rs
+-rw-r--r--   0     1001      123     1109 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/lumi.rs
+-rw-r--r--   0     1001      123     5860 2023-07-18 07:02:15.000000 pineappl-0.6.1/src/subgrid.rs
+-rw-r--r--   0     1001      123      324 2023-07-18 07:02:15.000000 pineappl-0.6.1/tests/conftest.py
+-rw-r--r--   0     1001      123      355 2023-07-18 07:02:15.000000 pineappl-0.6.1/tests/test_bin.py
+-rw-r--r--   0     1001      123     6124 2023-07-18 07:02:15.000000 pineappl-0.6.1/tests/test_grid.py
+-rw-r--r--   0     1001      123      237 2023-07-18 07:02:15.000000 pineappl-0.6.1/tests/test_lumi.py
+-rw-r--r--   0     1001      123     2696 2023-07-18 07:02:15.000000 pineappl-0.6.1/tests/test_sugrid.py
+-rw-r--r--   0     1001      123    44356 2023-07-18 07:02:15.000000 pineappl-0.6.1/Cargo.lock
+-rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 pineappl-0.6.1/PKG-INFO
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/Cargo.toml` & `pineappl-0.6.1/local_dependencies/pineappl/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.9"
+version= "0.6.1"
 
 [dependencies]
 arrayvec = "0.7.2"
 bincode = "1.3.3"
 enum_dispatch = "0.3.7"
 float-cmp = "0.9.0"
 git-version = "0.3.5"
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/README.md` & `pineappl-0.6.1/local_dependencies/pineappl/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/bin.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/bin.rs`

 * *Files 1% similar despite different names*

```diff
@@ -165,16 +165,15 @@
                     if split.len() == 1 {
                         // there's no colon
                         continue;
                     }
 
                     if split.len() != 2 {
                         return Err(ParseBinRemapperError(format!(
-                            "too many ':' found: '{}'",
-                            string
+                            "too many ':' found: '{string}'"
                         )));
                     }
 
                     (split[0].parse::<usize>(), split[1].parse::<usize>())
                 };
 
                 if let Ok(num) = rhs {
@@ -183,16 +182,15 @@
 
                 if let Ok(num) = lhs {
                     vec.drain(0..num);
                 }
 
                 if lhs.is_err() && rhs.is_err() {
                     return Err(ParseBinRemapperError(format!(
-                        "unable to parse ':' syntax from: '{}'",
-                        string
+                        "unable to parse ':' syntax from: '{string}'"
                     )));
                 }
 
                 if vec.len() <= 1 {
                     return Err(ParseBinRemapperError(
                         "no limits due to ':' syntax".to_string(),
                     ));
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/empty_subgrid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/empty_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/evolution.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/evolution.rs`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,23 @@
                     .iter()
                     .any(|entry| entry.entry().iter().any(|&(a, b, _)| (a == 0) || (b == 0)))
             })
         })
         .unwrap_or(false)
 }
 
+type Pid01IndexTuples = Vec<(usize, usize)>;
+type Pid01Tuples = Vec<(i32, i32)>;
+
 pub(crate) fn pids(
     operator: &ArrayView5<f64>,
     info: &OperatorInfo,
     gluon_has_pid_zero: bool,
     pid1_nonzero: &dyn Fn(i32) -> bool,
-) -> Result<(Vec<(usize, usize)>, Vec<(i32, i32)>), GridError> {
+) -> Result<(Pid01IndexTuples, Pid01Tuples), GridError> {
     // list of all non-zero PID indices
     let pid_indices: Vec<_> = (0..operator.dim().3)
         .cartesian_product(0..operator.dim().1)
         .filter(|&(pid0_idx, pid1_idx)| {
             // 1) at least one element of the operator must be non-zero, and 2) the pid must be
             // contained in the lumi somewhere
             operator
@@ -220,20 +223,22 @@
                 .into_owned()
         })
         .collect();
 
     Ok(operators)
 }
 
+type Fac1X1aX1bOp3Tuple = (Vec<f64>, Vec<f64>, Vec<f64>, Array3<f64>);
+
 pub(crate) fn ndarray_from_subgrid_orders(
     info: &OperatorInfo,
     subgrids: &ArrayView1<SubgridEnum>,
     orders: &[Order],
     order_mask: &[bool],
-) -> Result<(Vec<f64>, Vec<f64>, Vec<f64>, Array3<f64>), GridError> {
+) -> Result<Fac1X1aX1bOp3Tuple, GridError> {
     // TODO: skip empty subgrids
 
     let mut fac1: Vec<_> = subgrids
         .iter()
         .flat_map(|subgrid| {
             subgrid
                 .mu2_grid()
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/fk_table.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/fk_table.rs`

 * *Files 1% similar despite different names*

```diff
@@ -127,21 +127,30 @@
 impl FkTable {
     /// Returns the [`Grid`] object for this `FkTable`.
     #[must_use]
     pub const fn grid(&self) -> &Grid {
         &self.grid
     }
 
+    // TODO: when trying to convert the following function to `const` as per clippy's suggestion,
+    // the compiler errors out with: 'the destructor for this type cannot be evaluated in constant
+    // functions'
+
     /// Converts the `FkTable` back to a [`Grid`].
+    #[must_use]
     pub fn into_grid(self) -> Grid {
         self.grid
     }
 
     /// Returns the FK table represented as a four-dimensional array indexed by `bin`, `lumi`,
     /// `x1` and `x2`, in this order.
+    ///
+    /// # Panics
+    ///
+    /// TODO
     #[must_use]
     pub fn table(&self) -> Array4<f64> {
         let has_pdf1 = self.grid.has_pdf1();
         let has_pdf2 = self.grid.has_pdf2();
         let x_grid = self.x_grid();
 
         let mut result = Array4::zeros((
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/grid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/grid.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1887,15 +1887,15 @@
             subgrid_params: SubgridParams::default(),
             more_members: self.more_members.clone(),
         };
 
         // write additional metadata
         grid.set_key_value("lumi_id_types", &info.lumi_id_types);
 
-        Ok(FkTable::try_from(grid).unwrap())
+        Ok(FkTable::try_from(grid).unwrap_or_else(|_| unreachable!()))
     }
 
     /// Deletes bins with the corresponding `bin_indices`. Repeated indices and indices larger or
     /// equal the bin length are ignored.
     pub fn delete_bins(&mut self, bin_indices: &[usize]) {
         let mut bin_indices: Vec<_> = bin_indices
             .iter()
@@ -2001,14 +2001,38 @@
                         })
                         .collect(),
                 )
             })
             .collect();
     }
 
+    /// Splits the grid such that the luminosity function contains only a single combination per
+    /// channel.
+    pub fn split_lumi(&mut self) {
+        let indices: Vec<_> = self
+            .lumi
+            .iter()
+            .enumerate()
+            .flat_map(|(index, entry)| iter::repeat(index).take(entry.entry().len()))
+            .collect();
+
+        self.subgrids = self.subgrids.select(Axis(2), &indices);
+        self.lumi = self
+            .lumi
+            .iter()
+            .flat_map(|entry| {
+                entry
+                    .entry()
+                    .iter()
+                    .copied()
+                    .map(move |entry| LumiEntry::new(vec![entry]))
+            })
+            .collect();
+    }
+
     /// Returns `true` if the first initial state needs a convolution, `false` otherwise.
     #[must_use]
     pub fn has_pdf1(&self) -> bool {
         let initial_state_1 = self.initial_state_1();
 
         !self
             .lumi()
@@ -2025,27 +2049,35 @@
             .lumi()
             .iter()
             .all(|entry| entry.entry().iter().all(|&(_, b, _)| b == initial_state_2))
     }
 
     /// Returns the particle identifier of the first initial state. This is usually but not always
     /// a proton, which is represented by the PDG ID `2212`.
+    ///
+    /// # Panics
+    ///
+    /// TODO
     #[must_use]
     pub fn initial_state_1(&self) -> i32 {
         self.key_values()
             .map_or(Some("2212"), |kv| {
                 kv.get("initial_state_1").map(String::as_str)
             })
             .map(str::parse)
             .unwrap()
             .unwrap()
     }
 
     /// Returns the particle identifier of the second initial state. This is usually but not always
     /// a proton, which is represented by the PDG ID `2212`.
+    ///
+    /// # Panics
+    ///
+    /// TODO
     #[must_use]
     pub fn initial_state_2(&self) -> i32 {
         self.key_values()
             .map_or(Some("2212"), |kv| {
                 kv.get("initial_state_2").map(String::as_str)
             })
             .map(str::parse)
@@ -2552,16 +2584,16 @@
         let lumi_id_types = "pdg_mc_ids".to_owned();
 
         let eko_info = EkoInfo {
             muf2_0: 1.,
             alphas: vec![1.],
             xir: 1.,
             xif: 1.,
-            target_x_grid: target_x_grid.clone(),
-            target_pids: target_pids.clone(),
+            target_x_grid,
+            target_pids,
             grid_axes: GridAxes {
                 x_grid: axes.x_grid,
                 pids: axes.pids,
                 mur2_grid: axes.mur2_grid.clone(),
                 muf2_grid: axes.muf2_grid,
             },
             lumi_id_types,
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/import_only_subgrid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/import_only_subgrid.rs`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
             x.array_mut()[[0, 7, 1]] = 8.0;
         } else {
             unreachable!();
         }
 
         assert!(!grid1.is_empty());
 
-        assert_eq!(grid1.indexed_iter().nth(0), Some(((0, 1, 2), 1.0)));
+        assert_eq!(grid1.indexed_iter().next(), Some(((0, 1, 2), 1.0)));
         assert_eq!(grid1.indexed_iter().nth(1), Some(((0, 1, 3), 2.0)));
         assert_eq!(grid1.indexed_iter().nth(2), Some(((0, 4, 3), 4.0)));
         assert_eq!(grid1.indexed_iter().nth(3), Some(((0, 7, 1), 8.0)));
 
         // symmetric luminosity function
         let lumi =
             &mut (|ix1, ix2, _| x[ix1] * x[ix2]) as &mut dyn FnMut(usize, usize, usize) -> f64;
@@ -512,15 +512,15 @@
             x.array_mut()[[0, 3, 4]] = 4.0;
             x.array_mut()[[0, 1, 7]] = 8.0;
         } else {
             unreachable!();
         }
         assert_eq!(grid2.convolute(&x, &x, &mu2, lumi), 0.228515625);
 
-        assert_eq!(grid2.indexed_iter().nth(0), Some(((0, 1, 7), 8.0)));
+        assert_eq!(grid2.indexed_iter().next(), Some(((0, 1, 7), 8.0)));
         assert_eq!(grid2.indexed_iter().nth(1), Some(((0, 2, 1), 1.0)));
         assert_eq!(grid2.indexed_iter().nth(2), Some(((0, 3, 1), 2.0)));
         assert_eq!(grid2.indexed_iter().nth(3), Some(((0, 3, 4), 4.0)));
 
         grid1.merge(&mut grid2, false);
 
         assert_eq!(grid1.convolute(&x, &x, &mu2, lumi), 2.0 * 0.228515625);
@@ -580,15 +580,15 @@
             x.array_mut()[[0, 7, 1]] = 8.0;
         } else {
             unreachable!();
         }
 
         assert!(!grid1.is_empty());
 
-        assert_eq!(grid1.indexed_iter().nth(0), Some(((0, 1, 2), 1.0)));
+        assert_eq!(grid1.indexed_iter().next(), Some(((0, 1, 2), 1.0)));
         assert_eq!(grid1.indexed_iter().nth(1), Some(((0, 1, 3), 2.0)));
         assert_eq!(grid1.indexed_iter().nth(2), Some(((0, 4, 3), 4.0)));
         assert_eq!(grid1.indexed_iter().nth(3), Some(((0, 7, 1), 8.0)));
 
         // symmetric luminosity function
         let lumi =
             &mut (|ix1, ix2, _| x[ix1] * x[ix2]) as &mut dyn FnMut(usize, usize, usize) -> f64;
@@ -609,15 +609,15 @@
             x.array_mut()[[0, 3, 4]] = 4.0;
             x.array_mut()[[0, 1, 7]] = 8.0;
         } else {
             unreachable!();
         }
         assert_eq!(grid2.convolute(&x, &x, &mu2, lumi), 0.228515625);
 
-        assert_eq!(grid2.indexed_iter().nth(0), Some(((0, 1, 7), 8.0)));
+        assert_eq!(grid2.indexed_iter().next(), Some(((0, 1, 7), 8.0)));
         assert_eq!(grid2.indexed_iter().nth(1), Some(((0, 2, 1), 1.0)));
         assert_eq!(grid2.indexed_iter().nth(2), Some(((0, 3, 1), 2.0)));
         assert_eq!(grid2.indexed_iter().nth(3), Some(((0, 3, 4), 4.0)));
 
         grid1.merge(&mut grid2, false);
 
         assert_eq!(grid1.convolute(&x, &x, &mu2, lumi), 2.0 * 0.228515625);
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/lagrange_subgrid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/lagrange_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/lumi.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/ntuple_subgrid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/ntuple_subgrid.rs`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     use super::*;
     use crate::lagrange_subgrid::LagrangeSubgridV2;
     use crate::subgrid::{ExtraSubgridParams, SubgridParams};
 
     #[test]
     #[should_panic(expected = "NtupleSubgridV1 doesn't support the convolute operation")]
     fn convolute() {
-        let _ = NtupleSubgridV1::new().convolute(&[], &[], &[], &mut |_, _, _| 0.0);
+        NtupleSubgridV1::new().convolute(&[], &[], &[], &mut |_, _, _| 0.0);
     }
 
     #[test]
     fn fill_zero() {
         let mut subgrid = NtupleSubgridV1::new();
 
         subgrid.fill(&Ntuple {
@@ -119,15 +119,17 @@
 
         assert!(subgrid.is_empty());
     }
 
     #[test]
     #[should_panic(expected = "NtupleSubgridV1 doesn't support the indexed_iter operation")]
     fn indexed_iter() {
-        let _ = NtupleSubgridV1::new().indexed_iter();
+        // `next` isn't called because `indexed_iter` panics, but it suppresses a warning about an
+        // unused result
+        NtupleSubgridV1::new().indexed_iter().next();
     }
 
     #[test]
     fn stats() {
         let subgrid = NtupleSubgridV1::new();
         assert_eq!(
             subgrid.stats(),
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/pids.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/pids.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/sparse_array3.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/sparse_array3.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/src/subgrid.rs` & `pineappl-0.6.1/local_dependencies/pineappl/src/subgrid.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 use super::empty_subgrid::EmptySubgridV1;
 use super::grid::Ntuple;
 use super::import_only_subgrid::{ImportOnlySubgridV1, ImportOnlySubgridV2};
 use super::lagrange_subgrid::{LagrangeSparseSubgridV1, LagrangeSubgridV1, LagrangeSubgridV2};
 use super::ntuple_subgrid::NtupleSubgridV1;
 use enum_dispatch::enum_dispatch;
+use ndarray::Array3;
 use serde::{Deserialize, Serialize};
 use std::borrow::Cow;
 
 /// Enum which lists all possible `Subgrid` variants possible.
 #[enum_dispatch(Subgrid)]
 #[derive(Clone, Deserialize, Serialize)]
 pub enum SubgridEnum {
@@ -113,14 +114,30 @@
     /// Return statistics for this subgrid.
     fn stats(&self) -> Stats;
 
     /// Return the static (single) scale, if this subgrid has one.
     fn static_scale(&self) -> Option<Mu2>;
 }
 
+impl From<&SubgridEnum> for Array3<f64> {
+    fn from(subgrid: &SubgridEnum) -> Self {
+        let mut result = Self::zeros((
+            subgrid.mu2_grid().len(),
+            subgrid.x1_grid().len(),
+            subgrid.x2_grid().len(),
+        ));
+
+        for ((imu2, ix1, ix2), value) in subgrid.indexed_iter() {
+            result[[imu2, ix1, ix2]] = value;
+        }
+
+        result
+    }
+}
+
 /// Type to iterate over the non-zero contents of a subgrid. The tuple contains the indices of the
 /// `mu2_grid`, the `x1_grid` and finally the `x2_grid`.
 pub type SubgridIndexedIter<'a> = Box<dyn Iterator<Item = ((usize, usize, usize), f64)> + 'a>;
 
 /// Subgrid creation parameters for subgrids that perform interpolation.
 #[derive(Clone, Debug, Deserialize, Serialize)]
 pub struct SubgridParams {
```

### Comparing `pineappl-0.6.0a9/local_dependencies/pineappl/tests/drell_yan_lo.rs` & `pineappl-0.6.1/local_dependencies/pineappl/tests/drell_yan_lo.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/Cargo.toml` & `pineappl-0.6.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.9"
+version= "0.6.1"
 
 [package.metadata.maturin]
 name = "pineappl"
 
 [lib]
 name = "pineappl"
 crate-type = ["cdylib"]
 
 [dependencies]
 itertools = "0.10.1"
 ndarray = "0.15.4"
 numpy = "0.16.2"
-pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.9" }
+pineappl = { path = "local_dependencies/pineappl", version = "0.6.1" }
 pyo3 = { features = ["extension-module"], version = "0.16.4" }
```

### Comparing `pineappl-0.6.0a9/README.md` & `pineappl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/Makefile` & `pineappl-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/make.bat` & `pineappl-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/conf.py` & `pineappl-0.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/implementation.rst` & `pineappl-0.6.1/docs/source/implementation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/index.rst` & `pineappl-0.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/installation.rst` & `pineappl-0.6.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/recipes.rst` & `pineappl-0.6.1/docs/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/docs/source/shared/roles.rst` & `pineappl-0.6.1/docs/source/shared/roles.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/package/Containerfile` & `pineappl-0.6.1/package/Containerfile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/package/README.md` & `pineappl-0.6.1/package/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/pineappl/bin.py` & `pineappl-0.6.1/pineappl/bin.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/pineappl/fk_table.py` & `pineappl-0.6.1/pineappl/fk_table.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/pineappl/grid.py` & `pineappl-0.6.1/pineappl/grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/pineappl/import_only_subgrid.py` & `pineappl-0.6.1/pineappl/import_only_subgrid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 from .pineappl import PyImportOnlySubgridV1
+from .pineappl import PyImportOnlySubgridV2
 from .utils import PyWrapper
 
 
 class ImportOnlySubgridV1(PyWrapper):
     """
     Python wrapper object to :class:`~pineappl.pineappl.PyImportOnlySubgridV1`.
 
@@ -20,7 +21,28 @@
             interpolation grid for :math:`x_2`
     """
 
     def __init__(self, array, q2_grid, x1_grid, x2_grid):
         self._raw = PyImportOnlySubgridV1(
             np.array(array), np.array(q2_grid), np.array(x1_grid), np.array(x2_grid)
         )
+
+class ImportOnlySubgridV2(PyWrapper):
+    """
+    Python wrapper object to :class:`~pineappl.pineappl.PyImportOnlySubgridV2`.
+
+    Parameters
+    ----------
+        array : numpy.ndarray(float, dim=3)
+            3-dimensional subgrid content
+        mu2_grid : sequence(float)
+            scale grid
+        x1_grid : sequence(float)
+            interpolation grid for :math:`x_1`
+        x2_grid : sequence(float)
+            interpolation grid for :math:`x_2`
+    """
+
+    def __init__(self, array, mu2_grid, x1_grid, x2_grid):
+        self._raw = PyImportOnlySubgridV2(
+            np.array(array), mu2_grid, np.array(x1_grid), np.array(x2_grid)
+        )
```

### Comparing `pineappl-0.6.0a9/pyproject.toml` & `pineappl-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/src/bin.rs` & `pineappl-0.6.1/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/src/evolution.rs` & `pineappl-0.6.1/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/src/fk_table.rs` & `pineappl-0.6.1/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/src/grid.rs` & `pineappl-0.6.1/src/grid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/src/import_only_subgrid.rs` & `pineappl-0.6.1/src/import_only_subgrid.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,72 @@
 use super::subgrid::PySubgridEnum;
 
 use numpy::{PyReadonlyArray1, PyReadonlyArray3};
 use pineappl::import_only_subgrid::ImportOnlySubgridV1;
+use pineappl::import_only_subgrid::ImportOnlySubgridV2;
 use pineappl::sparse_array3::SparseArray3;
-
+use pineappl::subgrid::Mu2;
 use pyo3::prelude::*;
 
+/// PyO3 wrapper to :rustdoc:`pineappl::import_only_subgrid::ImportOnlySubgridV2 <import_only_subgrid/struct.ImportOnlySubgridV2.html>`
+///
+/// **Usage**: `pineko`
+#[pyclass]
+#[derive(Clone)]
+#[repr(transparent)]
+pub struct PyImportOnlySubgridV2 {
+    pub(crate) import_only_subgrid: ImportOnlySubgridV2,
+}
+
+#[pymethods]
+impl PyImportOnlySubgridV2 {
+    #[new]
+    pub fn new(
+        array: PyReadonlyArray3<f64>,
+        mu2_grid: Vec<(f64, f64)>,
+        x1_grid: PyReadonlyArray1<f64>,
+        x2_grid: PyReadonlyArray1<f64>,
+    ) -> Self {
+        let mut sparse_array = SparseArray3::new(mu2_grid.len(), x1_grid.len(), x2_grid.len());
+
+        for ((imu2, ix1, ix2), value) in array
+            .as_array()
+            .indexed_iter()
+            .filter(|((_, _, _), value)| **value != 0.0)
+        {
+            sparse_array[[imu2, ix1, ix2]] = *value;
+        }
+        Self{
+            import_only_subgrid: ImportOnlySubgridV2::new(
+            sparse_array,
+            mu2_grid
+                .iter()
+                .map(|(ren, fac)| Mu2 {
+                    ren: *ren,
+                    fac: *fac,
+                })
+                .collect(),
+            x1_grid.to_vec().unwrap(),
+            x2_grid.to_vec().unwrap(),
+        )}
+    }
+
+    /// Wrapper to match :meth:`pineappl.pineappl.PyGrid.set_subgrid()`
+    ///
+    /// Returns
+    /// -------
+    ///     PySubgridEnum :
+    ///         casted object
+    pub fn into(&self) -> PySubgridEnum {
+        PySubgridEnum {
+            subgrid_enum: self.import_only_subgrid.clone().into(),
+        }
+    }
+}
+
 /// PyO3 wrapper to :rustdoc:`pineappl::import_only_subgrid::ImportOnlySubgridV1 <import_only_subgrid/struct.ImportOnlySubgridV1.html>`
 ///
 /// **Usage**: `yadism`
 #[pyclass]
 #[derive(Clone)]
 #[repr(transparent)]
 pub struct PyImportOnlySubgridV1 {
```

### Comparing `pineappl-0.6.0a9/src/lib.rs` & `pineappl-0.6.1/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#![warn(missing_docs)]
 use pyo3::prelude::*;
 
 pub mod bin;
 pub mod evolution;
 pub mod fk_table;
 pub mod grid;
 pub mod import_only_subgrid;
@@ -15,15 +16,17 @@
 fn pineappl(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<bin::PyBinRemapper>()?;
     m.add_class::<evolution::PyEvolveInfo>()?;
     m.add_class::<grid::PyGrid>()?;
     m.add_class::<grid::PyOrder>()?;
     m.add_class::<lumi::PyLumiEntry>()?;
     m.add_class::<import_only_subgrid::PyImportOnlySubgridV1>()?;
+    m.add_class::<import_only_subgrid::PyImportOnlySubgridV2>()?;
     m.add_class::<fk_table::PyFkTable>()?;
     m.add_class::<fk_table::PyFkAssumptions>()?;
     m.add_class::<subgrid::PySubgridEnum>()?;
     m.add_class::<subgrid::PySubgridParams>()?;
+    m.add_class::<subgrid::PyMu2>()?;
     m.add("version", env!("CARGO_PKG_VERSION"))?;
 
     Ok(())
 }
```

### Comparing `pineappl-0.6.0a9/src/lumi.rs` & `pineappl-0.6.1/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/tests/test_grid.py` & `pineappl-0.6.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a9/Cargo.lock` & `pineappl-0.6.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -441,25 +441,14 @@
  "proc-macro2",
  "quote",
  "syn 1.0.107",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys 0.45.0",
@@ -488,15 +477,15 @@
 name = "filetime"
 version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e884668cd0c7480504233e951174ddc3b382f7c2666e3b7310b5c4e7b0c37f9"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -684,15 +673,15 @@
 name = "is-terminal"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "256017f749ab3117e93acb91063009e1f1bb56d03965b14c2c8df4eb02c524d8"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
- "rustix 0.37.4",
+ "rustix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -738,20 +727,14 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
-
-[[package]]
-name = "linux-raw-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd550e73688e6d578f0ac2119e32b797a327631a42f9433e59d02e139c8df60d"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
@@ -838,14 +821,20 @@
  "num-complex",
  "num-traits",
  "py_literal",
  "zip",
 ]
 
 [[package]]
+name = "normalize-line-endings"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
+
+[[package]]
 name = "num-bigint"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -929,15 +918,15 @@
 name = "parking_lot_core"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "pest"
 version = "2.5.2"
@@ -980,15 +969,15 @@
  "once_cell",
  "pest",
  "sha1",
 ]
 
 [[package]]
 name = "pineappl"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "anyhow",
  "arrayvec",
  "bincode",
  "enum_dispatch",
  "float-cmp",
  "git-version",
@@ -1004,73 +993,75 @@
  "serde",
  "serde_yaml",
  "thiserror",
 ]
 
 [[package]]
 name = "pineappl_applgrid"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "cc",
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_capi"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "itertools",
  "pineappl",
 ]
 
 [[package]]
 name = "pineappl_cli"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "base64",
  "clap",
  "clap_mangen",
  "cxx",
  "either",
  "enum_dispatch",
  "flate2",
  "float-cmp",
  "git-version",
+ "is-terminal",
  "itertools",
  "lhapdf",
- "libc",
  "lz4_flex",
  "ndarray",
  "ndarray-npy",
  "pineappl",
  "pineappl_applgrid",
  "pineappl_fastnlo",
+ "predicates",
  "prettytable-rs",
  "rayon",
- "scopeguard",
  "serde",
  "serde_yaml",
  "tar",
+ "tempfile",
 ]
 
 [[package]]
 name = "pineappl_fastnlo"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "cxx",
  "cxx-build",
+ "thiserror",
 ]
 
 [[package]]
 name = "pineappl_py"
-version = "0.6.0-alpha.9"
+version = "0.6.1"
 dependencies = [
  "itertools",
  "ndarray",
  "numpy",
  "pineappl",
  "pyo3",
 ]
@@ -1084,16 +1075,19 @@
 [[package]]
 name = "predicates"
 version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5aab5be6e4732b473071984b3164dbbfb7a3674d30ea5ff44410b6bcd960c3c"
 dependencies = [
  "difflib",
+ "float-cmp",
  "itertools",
+ "normalize-line-endings",
  "predicates-core",
+ "regex",
 ]
 
 [[package]]
 name = "predicates-core"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72f883590242d3c6fc5bf50299011695fa6590c2c70eac95ee1bdb9a733ad1a2"
@@ -1275,21 +1269,30 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
 dependencies = [
  "getrandom",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1322,37 +1325,23 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.36.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4feacf7db682c6c329c4ede12649cd36ecab0f3be5b7d74e6a20304725db4549"
-dependencies = [
- "bitflags",
- "errno 0.2.8",
- "io-lifetimes",
- "libc",
- "linux-raw-sys 0.1.4",
- "windows-sys 0.42.0",
-]
-
-[[package]]
-name = "rustix"
 version = "0.37.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c348b5dc624ecee40108aa2922fed8bad89d7fcc2b9f8cb18f632898ac4a37f9"
 dependencies = [
  "bitflags",
- "errno 0.3.0",
+ "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys 0.3.0",
+ "linux-raw-sys",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1484,23 +1473,23 @@
 name = "target-lexicon"
 version = "0.12.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
- "rustix 0.36.6",
- "windows-sys 0.42.0",
+ "redox_syscall 0.3.5",
+ "rustix",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "term"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
```

### Comparing `pineappl-0.6.0a9/PKG-INFO` & `pineappl-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pineappl
-Version: 0.6.0a9
+Version: 0.6.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: numpy>=1.16.0,<2.0.0
-Requires-Dist: sphinx; extra == 'docs'
-Requires-Dist: sphinx_rtd_theme; extra == 'docs'
-Requires-Dist: sphinxcontrib-bibtex; extra == 'docs'
-Requires-Dist: nbsphinx; extra == 'docs'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: numpy >=1.16.0, <2.0.0
+Requires-Dist: sphinx ; extra == 'docs'
+Requires-Dist: sphinx_rtd_theme ; extra == 'docs'
+Requires-Dist: sphinxcontrib-bibtex ; extra == 'docs'
+Requires-Dist: nbsphinx ; extra == 'docs'
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: pytest-cov ; extra == 'test'
 Provides-Extra: docs
 Provides-Extra: test
 Summary: Python bindings to PineAPPL
 Keywords: high-energy-physics,physics
 Author: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 Author-email: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 License: GPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/NNPDF/pineappl/blob/master/CHANGELOG.md
-Project-URL: documentation, https://pineappl.readthedocs.io/
 Project-URL: homepage, https://n3pdf.github.io/pineappl/
+Project-URL: documentation, https://pineappl.readthedocs.io/
+Project-URL: changelog, https://github.com/NNPDF/pineappl/blob/master/CHANGELOG.md
 
 [![PyPI version](https://badge.fury.io/py/pineappl.svg)](https://badge.fury.io/py/pineappl)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pineappl/badges/installer/conda.svg)](https://anaconda.org/conda-forge/pineappl)
 [![AUR](https://img.shields.io/aur/version/pineappl)](https://aur.archlinux.org/packages/pineappl)
 [![Documentation Status](https://readthedocs.org/projects/pineappl/badge/?version=latest)](https://pineappl.readthedocs.io/en/latest/?badge=latest)
 
 # Python bindings for PineAPPL
```

