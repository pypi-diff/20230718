# Comparing `tmp/egglog-0.4.0.tar.gz` & `tmp/egglog-0.5.1.tar.gz`

## Comparing `egglog-0.4.0.tar` & `egglog-0.5.1.tar`

### file list

```diff
@@ -1,57 +1,65 @@
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 egglog-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123      174 2023-05-03 14:45:46.000000 egglog-0.4.0/.flake8
--rw-r--r--   0     1001      123     4236 2023-05-03 14:45:46.000000 egglog-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      733 2023-05-03 14:45:46.000000 egglog-0.4.0/.gitignore
--rw-r--r--   0     1001      123      996 2023-05-03 14:45:46.000000 egglog-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123      738 2023-05-03 14:45:46.000000 egglog-0.4.0/.readthedocs.yaml
--rw-r--r--   0     1001      123     1064 2023-05-03 14:45:46.000000 egglog-0.4.0/LICENSE
--rw-r--r--   0     1001      123     1102 2023-05-03 14:45:46.000000 egglog-0.4.0/README.md
--rw-r--r--   0     1001      123      372 2023-05-03 14:45:46.000000 egglog-0.4.0/conftest.py
--rw-r--r--   0     1001      123       57 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/.gitignore
--rw-r--r--   0     1001      123     1122 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/changelog.md
--rw-r--r--   0     1001      123     4205 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/conf.py
--rw-r--r--   0     1001      123     4529 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/explanation/compared_to_rust.md
--rw-r--r--   0     1001      123     1368 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/explanation/define_and_define.md
--rw-r--r--   0     1001      123     1511 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/explanation/optional_values.md
--rw-r--r--   0     1001      123      119 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/explanation.md
--rw-r--r--   0     1001      123      807 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/how-to-guides.md
--rw-r--r--   0     1001      123     1528 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/index.md
--rw-r--r--   0     1001      123      332 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/reference/bindings.md
--rw-r--r--   0     1001      123      434 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/reference/high-level.md
--rw-r--r--   0     1001      123       80 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/reference.md
--rw-r--r--   0     1001      123    17899 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/tutorials/getting-started.ipynb
--rw-r--r--   0     1001      123    14545 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/tutorials/screenshot-1.png
--rw-r--r--   0     1001      123    91888 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/tutorials/screenshot-2.png
--rw-r--r--   0     1001      123       56 2023-05-03 14:45:46.000000 egglog-0.4.0/docs/tutorials.md
--rw-r--r--   0     1001      123     1829 2023-05-03 14:45:46.000000 egglog-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123      126 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/__init__.py
--rw-r--r--   0     1001      123     7976 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/bindings.pyi
--rw-r--r--   0     1001      123     7129 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/builtins.py
--rw-r--r--   0     1001      123      168 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/config.py
--rw-r--r--   0     1001      123    21709 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/declarations.py
--rw-r--r--   0     1001      123    37417 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/egraph.py
--rw-r--r--   0     1001      123      232 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/README.rst
--rw-r--r--   0     1001      123        0 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/__init__.py
--rw-r--r--   0     1001      123      983 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/eqsat_basic.py
--rw-r--r--   0     1001      123     8632 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/lambda.py
--rw-r--r--   0     1001      123     5274 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/matrix.py
--rw-r--r--   0     1001      123     2093 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/examples/resolution.py
--rw-r--r--   0     1001      123     1140 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/monkeypatch.py
--rw-r--r--   0     1001      123        0 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/py.typed
--rw-r--r--   0     1001      123    11575 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/runtime.py
--rw-r--r--   0     1001      123     2841 2023-05-03 14:45:46.000000 egglog-0.4.0/python/egglog/type_constraint_solver.py
--rw-r--r--   0     1001      123     6047 2023-05-03 14:45:46.000000 egglog-0.4.0/python/tests/test_bindings.py
--rw-r--r--   0     1001      123     4383 2023-05-03 14:45:46.000000 egglog-0.4.0/python/tests/test_high_level.py
--rw-r--r--   0     1001      123     3289 2023-05-03 14:45:46.000000 egglog-0.4.0/python/tests/test_runtime.py
--rw-r--r--   0     1001      123     1209 2023-05-03 14:45:46.000000 egglog-0.4.0/python/tests/test_type_constraint_solver.py
--rw-r--r--   0     1001      123     1126 2023-05-03 14:45:46.000000 egglog-0.4.0/python/tests/test_typing.py
--rwxr-xr-x   0     1001      123      767 2023-05-03 14:46:20.000000 egglog-0.4.0/run-maturin-action.sh
--rw-r--r--   0     1001      123    18550 2023-05-03 14:45:46.000000 egglog-0.4.0/src/conversions.rs
--rw-r--r--   0     1001      123     2331 2023-05-03 14:45:46.000000 egglog-0.4.0/src/egraph.rs
--rw-r--r--   0     1001      123     1231 2023-05-03 14:45:46.000000 egglog-0.4.0/src/error.rs
--rw-r--r--   0     1001      123      462 2023-05-03 14:45:46.000000 egglog-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123     7739 2023-05-03 14:45:46.000000 egglog-0.4.0/src/utils.rs
--rw-r--r--   0     1001      123      116 2023-05-03 14:45:46.000000 egglog-0.4.0/stubtest_allow
--rw-r--r--   0     1001      123      418 2023-05-03 14:45:46.000000 egglog-0.4.0/test-data/unit/check-high-level.test
--rw-r--r--   0     1001      123    26515 2023-05-03 14:45:46.000000 egglog-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     2759 1970-01-01 00:00:00.000000 egglog-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 egglog-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123      180 2023-07-18 17:45:21.000000 egglog-0.5.1/.flake8
+-rw-r--r--   0     1001      123     3866 2023-07-18 17:45:21.000000 egglog-0.5.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      753 2023-07-18 17:45:21.000000 egglog-0.5.1/.gitignore
+-rw-r--r--   0     1001      123      996 2023-07-18 17:45:21.000000 egglog-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123      738 2023-07-18 17:45:21.000000 egglog-0.5.1/.readthedocs.yaml
+-rw-r--r--   0     1001      123     1064 2023-07-18 17:45:21.000000 egglog-0.5.1/LICENSE
+-rw-r--r--   0     1001      123     1117 2023-07-18 17:45:21.000000 egglog-0.5.1/README.md
+-rw-r--r--   0     1001      123      372 2023-07-18 17:45:21.000000 egglog-0.5.1/conftest.py
+-rw-r--r--   0     1001      123       71 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/.gitignore
+-rw-r--r--   0     1001      123     3039 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/changelog.md
+-rw-r--r--   0     1001      123     4661 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/conf.py
+-rw-r--r--   0     1001      123       13 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/.gitignore
+-rw-r--r--   0     1001      123    30290 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/big_graph.svg
+-rw-r--r--   0     1001      123     3181 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/compared_to_rust.md
+-rw-r--r--   0     1001      123     1368 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/define_and_define.md
+-rw-r--r--   0     1001      123     1511 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/optional_values.md
+-rw-r--r--   0     1001      123   390934 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation/pldi_2023_presentation.ipynb
+-rw-r--r--   0     1001      123      154 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/explanation.md
+-rw-r--r--   0     1001      123      807 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/how-to-guides.md
+-rw-r--r--   0     1001      123     1528 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/index.md
+-rw-r--r--   0     1001      123      332 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/reference/bindings.md
+-rw-r--r--   0     1001      123    17585 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/reference/egglog-translation.md
+-rw-r--r--   0     1001      123      434 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/reference/high-level.md
+-rw-r--r--   0     1001      123      109 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/reference.md
+-rw-r--r--   0     1001      123    17899 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/tutorials/getting-started.ipynb
+-rw-r--r--   0     1001      123    14545 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/tutorials/screenshot-1.png
+-rw-r--r--   0     1001      123    91888 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/tutorials/screenshot-2.png
+-rw-r--r--   0     1001      123       56 2023-07-18 17:45:21.000000 egglog-0.5.1/docs/tutorials.md
+-rw-r--r--   0     1001      123     1857 2023-07-18 17:45:21.000000 egglog-0.5.1/pyproject.toml
+-rw-r--r--   0     1001      123      143 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/__init__.py
+-rw-r--r--   0     1001      123     8188 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/bindings.pyi
+-rw-r--r--   0     1001      123     9451 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/builtins.py
+-rw-r--r--   0     1001      123      168 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/config.py
+-rw-r--r--   0     1001      123    32042 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/declarations.py
+-rw-r--r--   0     1001      123    36861 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/egraph.py
+-rw-r--r--   0     1001      123      232 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/README.rst
+-rw-r--r--   0     1001      123        0 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/__init__.py
+-rw-r--r--   0     1001      123      990 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/eqsat_basic.py
+-rw-r--r--   0     1001      123      505 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/fib.py
+-rw-r--r--   0     1001      123     8643 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/lambda.py
+-rw-r--r--   0     1001      123     5281 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/matrix.py
+-rw-r--r--   0     1001      123     4230 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/ndarrays.py
+-rw-r--r--   0     1001      123     2100 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/resolution.py
+-rw-r--r--   0     1001      123      723 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/examples/schedule_demo.py
+-rw-r--r--   0     1001      123     1168 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/ipython_magic.py
+-rw-r--r--   0     1001      123     1140 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/monkeypatch.py
+-rw-r--r--   0     1001      123        0 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/py.typed
+-rw-r--r--   0     1001      123    11975 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/runtime.py
+-rw-r--r--   0     1001      123     3153 2023-07-18 17:45:21.000000 egglog-0.5.1/python/egglog/type_constraint_solver.py
+-rw-r--r--   0     1001      123     6073 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_bindings.py
+-rw-r--r--   0     1001      123     5859 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_high_level.py
+-rw-r--r--   0     1001      123      864 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_modules.py
+-rw-r--r--   0     1001      123     3978 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_runtime.py
+-rw-r--r--   0     1001      123     1602 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_type_constraint_solver.py
+-rw-r--r--   0     1001      123     1126 2023-07-18 17:45:21.000000 egglog-0.5.1/python/tests/test_typing.py
+-rw-r--r--   0     1001      123    18489 2023-07-18 17:45:21.000000 egglog-0.5.1/src/conversions.rs
+-rw-r--r--   0     1001      123     2474 2023-07-18 17:45:21.000000 egglog-0.5.1/src/egraph.rs
+-rw-r--r--   0     1001      123     1221 2023-07-18 17:45:21.000000 egglog-0.5.1/src/error.rs
+-rw-r--r--   0     1001      123      460 2023-07-18 17:45:21.000000 egglog-0.5.1/src/lib.rs
+-rw-r--r--   0     1001      123     7739 2023-07-18 17:45:21.000000 egglog-0.5.1/src/utils.rs
+-rw-r--r--   0     1001      123      116 2023-07-18 17:45:21.000000 egglog-0.5.1/stubtest_allow
+-rw-r--r--   0     1001      123      418 2023-07-18 17:45:21.000000 egglog-0.5.1/test-data/unit/check-high-level.test
+-rw-r--r--   0     1001      123    36296 2023-07-18 17:45:21.000000 egglog-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 egglog-0.5.1/PKG-INFO
```

### Comparing `egglog-0.4.0/Cargo.toml` & `egglog-0.5.1/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [package]
 name = "egglog-python"
-version = "0.4.0"
+version = "0.5.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "egglog_python"
 crate-type = ["cdylib"]
 
 [dependencies]
 # Use unreleased version to depend on signature improvements https://github.com/PyO3/pyo3/pull/2702
 pyo3 = { version = "0.18.1", features = ["extension-module"] }
-egg-smol = { git = "https://github.com/egraphs-good/egglog", rev = "30feaaab88452ec4b6c5f7a199345298bac2dd0f" }
-# egg-smol = { path = "../egglog" }
+# egglog = { git = "https://github.com/egraphs-good/egglog", rev = "39b199d9bfce9cc47d0c54977279c5b04231e717" }
+egglog = { git = "https://github.com/saulshanabrook/egg-smol", rev = "353c4387640019bd2066991ee0488dc6d5c54168" }
+
+# egglog = { path = "../egg-smol" }
 pyo3-log = "0.8.1"
 log = "0.4.17"
 lalrpop-util = { version = "0.19.8", features = ["lexer"] }
 ordered-float = "3.4"
 
 [package.metadata.maturin]
 name = "egglog.bindings"
```

### Comparing `egglog-0.4.0/.github/workflows/CI.yml` & `egglog-0.5.1/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   push:
     branches:
       - main
       - master
     tags:
       - "*"
   pull_request:
+  workflow_dispatch:
 
 # Allow one concurrent deployment
 concurrency:
   group: ${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
@@ -82,73 +83,69 @@
             target/
           key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
       - run: pip install -e .[docs] pre-commit
       - run: pre-commit run --all-files docs
   linux:
     name: build linux
     runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [test]
     steps:
       - uses: actions/checkout@v3
-      - uses: PyO3/maturin-action@v1.31.0
+      - uses: PyO3/maturin-action@v1.40.1
         with:
           manylinux: auto
           command: build
           args: --release --sdist -o dist --find-interpreter
-          # Pin rust toolchain, so it won't install 1.65.0, otherwise get this error:
-          # Attempting to include the sdist output tarball dist/egglog-0.1.0.tar.gz into itself! Check 'cargo package --list' output.
-          # https://github.com/metadsl/egglog-python/actions/runs/3388178229/jobs/5629843303
-          rust-toolchain: "1.64.0"
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   windows:
     name: build windows
     runs-on: windows-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [test]
     steps:
       - uses: actions/checkout@v3
-      - uses: PyO3/maturin-action@v1.31.0
+      - uses: PyO3/maturin-action@v1.40.1
         with:
           command: build
           args: --release -o dist --find-interpreter
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   macos:
     name: build macos
     runs-on: macos-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    needs: [test]
     steps:
       - uses: actions/checkout@v3
-      - uses: PyO3/maturin-action@v1.31.0
+      - uses: PyO3/maturin-action@v1.40.1
         with:
           command: build
           args: --release -o dist --universal2 --find-interpreter
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    if: startsWith(github.ref, 'refs/tags/') || (github.event_name == 'workflow_dispatch')
     needs: [macos, windows, linux]
     steps:
       - uses: actions/download-artifact@v2
         with:
           name: wheels
       - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1.31.0
+        uses: PyO3/maturin-action@v1.40.1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --skip-existing *
```

### Comparing `egglog-0.4.0/.gitignore` & `egglog-0.5.1/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -72,7 +72,9 @@
 .python-version
 
 TODO
 *.code-workspace
 .dmypy.json
 *tmp*
 .envs
+
+.ipynb_checkpoints
```

### Comparing `egglog-0.4.0/.pre-commit-config.yaml` & `egglog-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/.readthedocs.yaml` & `egglog-0.5.1/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-20.04
   tools:
     python: "3.10"
     # You can also specify other tool versions:
     # nodejs: "16"
-    rust: "1.61"
+    rust: "1.64"
     # golang: "1.17"
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # If using Sphinx, optionally build your docs in additional formats such as PDF
```

### Comparing `egglog-0.4.0/LICENSE` & `egglog-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/README.md` & `egglog-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 # `egglog` Python wrapper
 
 [![Documentation Status](https://readthedocs.org/projects/egg-smol-python/badge/?version=latest)](https://egg-smol-python.readthedocs.io/en/latest/?badge=latest) [![Test](https://github.com/metadsl/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/metadsl/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 `egglog` is a Python package that provides bindings to the Rust library [`egglog`](https://github.com/egraphs-good/egglog/),
 allowing you to use e-graphs in Python for optimization, symbolic computation, and analysis.
 
-Please see the [documentation](https://egglog-python.readthedocs.io/en/latest/) for more information.
+Please see the [documentation](https://egg-smol-python.readthedocs.io/en/latest/?badge=latest) for more information.
```

### Comparing `egglog-0.4.0/docs/conf.py` & `egglog-0.5.1/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,34 @@
-# outline for a myst_nb project with sphinx
-# build with: sphinx-build -nW --keep-going -b html . ./_build/html
+import pathlib
+import subprocess
+
+##
+# Built presentation in sphinx
+##
+
+cwd = pathlib.Path(__file__).parent
+presentation_file = cwd / "explanation" / "pldi_2023_presentation.ipynb"
+output_dir = cwd / "presentations"
+
+subprocess.run(
+    [
+        "jupyter",
+        "nbconvert",
+        str(presentation_file),
+        "--to",
+        "slides",
+        "--output-dir",
+        str(output_dir),
+        "--TagRemovePreprocessor.remove_input_tags",
+        "remove-input",
+    ],
+    check=True,
+)
+
+html_extra_path = ["presentations/pldi_2023_presentation.slides.html"]
 
 # load extensions
 extensions = [
     "myst_nb",
     "sphinx.ext.autodoc",
     "sphinx_autodoc_typehints",
     "sphinx_gallery.gen_gallery",
```

### Comparing `egglog-0.4.0/docs/explanation/define_and_define.md` & `egglog-0.5.1/docs/explanation/define_and_define.md`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/explanation/optional_values.md` & `egglog-0.5.1/docs/explanation/optional_values.md`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/how-to-guides.md` & `egglog-0.5.1/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/index.md` & `egglog-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/tutorials/getting-started.ipynb` & `egglog-0.5.1/docs/tutorials/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/tutorials/screenshot-1.png` & `egglog-0.5.1/docs/tutorials/screenshot-1.png`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/docs/tutorials/screenshot-2.png` & `egglog-0.5.1/docs/tutorials/screenshot-2.png`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/pyproject.toml` & `egglog-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,40 +22,41 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Compilers",
     "Topic :: Software Development :: Interpreters",
     "Typing :: Typed",
 ]
-dependencies = ["typing-extensions", "black"]
+dependencies = ["typing-extensions", "black", "graphviz"]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "black", "mypy", "flake8", "isort"]
 
 test = ["pytest", "mypy"]
 
 docs = [
     "pydata-sphinx-theme",
     "myst-nb",
     "sphinx-autodoc-typehints",
     "sphinx-gallery",
     "matplotlib",
+    "nbconvert",
 ]
 
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 
 
 [tool.mypy]
-ignore_missing_imports = false
+ignore_missing_imports = true
 warn_redundant_casts = true
 check_untyped_defs = true
 strict_equality = true
 warn_unused_configs = true
 allow_redefinition = true
 enable_incomplete_feature = ["Unpack", "TypeVarTuple"]
```

### Comparing `egglog-0.4.0/python/egglog/bindings.pyi` & `egglog-0.5.1/python/egglog/bindings.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @final
 class EGraph:
     def __init__(self, fact_directory: str | Path | None = None, seminaive=True) -> None: ...
     def parse_program(self, __input: str, /) -> list[_Command]: ...
     def run_program(self, *commands: _Command) -> list[str]: ...
     def extract_report(self) -> Optional[ExtractReport]: ...
     def run_report(self) -> Optional[RunReport]: ...
+    def to_graphviz_string(self) -> str: ...
 
 @final
 class EggSmolError(Exception):
     context: str
 
 ##
 # Literals
@@ -92,14 +93,21 @@
 class Set:
     def __init__(self, lhs: str, args: list[_Expr], rhs: _Expr) -> None: ...
     lhs: str
     args: list[_Expr]
     rhs: _Expr
 
 @final
+class SetNoTrack:
+    def __init__(self, lhs: str, args: list[_Expr], rhs: _Expr) -> None: ...
+    lhs: str
+    args: list[_Expr]
+    rhs: _Expr
+
+@final
 class Delete:
     sym: str
     args: list[_Expr]
     def __init__(self, sym: str, args: list[_Expr]) -> None: ...
 
 @final
 class Union:
@@ -113,15 +121,15 @@
     msg: str
 
 @final
 class Expr_:
     def __init__(self, expr: _Expr) -> None: ...
     expr: _Expr
 
-_Action = Let | Set | Delete | Union | Panic | Expr_
+_Action = Let | Set | SetNoTrack | Delete | Union | Panic | Expr_
 
 ##
 # Other Structs
 ##
 
 @final
 class FunctionDecl:
@@ -203,14 +211,15 @@
     variants: list[_Expr]
 
     def __init__(self, cost: int, expr: _Expr, variants: list[_Expr]) -> None: ...
 
 ##
 # Schedules
 ##
+
 @final
 class Saturate:
     schedule: _Schedule
     def __init__(self, schedule: _Schedule) -> None: ...
 
 @final
 class Repeat:
```

### Comparing `egglog-0.4.0/python/egglog/builtins.py` & `egglog-0.5.1/python/egglog/builtins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Builtin sorts and function to egg.
 """
 
-
 from __future__ import annotations
 
 from typing import Generic, TypeVar, Union
 
 from .egraph import BUILTINS, BaseExpr, Unit
 
 __all__ = [
@@ -15,17 +14,19 @@
     "i64Like",
     "f64",
     "f64Like",
     "String",
     "StringLike",
     "Map",
     "Rational",
+    "Set",
+    "Vec",
+    "join",
 ]
 
-
 # The types which can be converted into an i64
 i64Like = Union[int, "i64"]
 
 
 @BUILTINS.class_(egg_sort="i64")
 class i64(BaseExpr):
     def __init__(self, value: int):
@@ -96,14 +97,18 @@
 
 
 @BUILTINS.class_(egg_sort="f64")
 class f64(BaseExpr):
     def __init__(self, value: float):
         ...
 
+    @BUILTINS.method(egg_fn="neg")
+    def __neg__(self) -> f64:  # type: ignore[empty-body]
+        ...
+
     @BUILTINS.method(egg_fn="+")
     def __add__(self, other: f64Like) -> f64:  # type: ignore[empty-body]
         ...
 
     @BUILTINS.method(egg_fn="-")
     def __sub__(self, other: f64Like) -> f64:  # type: ignore[empty-body]
         ...
@@ -141,72 +146,110 @@
         ...
 
     @BUILTINS.method(egg_fn="max")
     def max(self, other: f64Like) -> f64:  # type: ignore[empty-body]
         ...
 
 
+StringLike = Union[str, "String"]
+
+
 @BUILTINS.class_
 class String(BaseExpr):
     def __init__(self, value: str):
         ...
 
 
-StringLike = Union[str, String]
+@BUILTINS.function(egg_fn="+")
+def join(*strings: StringLike) -> String:  # type: ignore[empty-body]
+    ...
+
 
 T = TypeVar("T", bound=BaseExpr)
 V = TypeVar("V", bound=BaseExpr)
 
 
 @BUILTINS.class_(egg_sort="Map")
 class Map(BaseExpr, Generic[T, V]):
-    @BUILTINS.method(egg_fn="empty")
+    @BUILTINS.method(egg_fn="map-empty")
     @classmethod
     def empty(cls) -> Map[T, V]:  # type: ignore[empty-body]
         ...
 
-    @BUILTINS.method(egg_fn="insert")
+    @BUILTINS.method(egg_fn="map-insert")
     def insert(self, key: T, value: V) -> Map[T, V]:  # type: ignore[empty-body]
         ...
 
-    @BUILTINS.method(egg_fn="get")
+    @BUILTINS.method(egg_fn="map-get")
     def __getitem__(self, key: T) -> V:  # type: ignore[empty-body]
         ...
 
-    @BUILTINS.method(egg_fn="not-contains")
+    @BUILTINS.method(egg_fn="map-not-contains")
     def not_contains(self, key: T) -> Unit:  # type: ignore[empty-body]
         ...
 
-    @BUILTINS.method(egg_fn="contains")
+    @BUILTINS.method(egg_fn="map-contains")
     def contains(self, key: T) -> Unit:  # type: ignore[empty-body]
         ...
 
+    @BUILTINS.method(egg_fn="map-remove")
+    def remove(self, key: T) -> Map[T, V]:  # type: ignore[empty-body]
+        ...
+
+
+@BUILTINS.class_(egg_sort="Set")
+class Set(BaseExpr, Generic[T]):
+    @BUILTINS.method(egg_fn="set-of")
+    def __init__(self, *args: T) -> None:
+        ...
+
+    @BUILTINS.method(egg_fn="set-empty")
+    @classmethod
+    def empty(cls) -> Set[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="set-insert")
+    def insert(self, value: T) -> Set[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="set-not-contains")
+    def not_contains(self, value: T) -> Unit:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="set-contains")
+    def contains(self, value: T) -> Unit:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="set-remove")
+    def remove(self, value: T) -> Set[T]:  # type: ignore[empty-body]
+        ...
+
     @BUILTINS.method(egg_fn="set-union")
-    def __or__(self, __t: Map[T, V]) -> Map[T, V]:  # type: ignore[empty-body]
+    def __or__(self, other: Set[T]) -> Set[T]:  # type: ignore[empty-body]
         ...
 
     @BUILTINS.method(egg_fn="set-diff")
-    def __sub__(self, __t: Map[T, V]) -> Map[T, V]:  # type: ignore[empty-body]
+    def __sub__(self, other: Set[T]) -> Set[T]:  # type: ignore[empty-body]
         ...
 
     @BUILTINS.method(egg_fn="set-intersect")
-    def __and__(self, __t: Map[T, V]) -> Map[T, V]:  # type: ignore[empty-body]
-        ...
-
-    @BUILTINS.method(egg_fn="map-remove")
-    def remove(self, key: T) -> Map[T, V]:  # type: ignore[empty-body]
+    def __and__(self, other: Set[T]) -> Set[T]:  # type: ignore[empty-body]
         ...
 
 
 @BUILTINS.class_(egg_sort="Rational")
 class Rational(BaseExpr):
     @BUILTINS.method(egg_fn="rational")
     def __init__(self, num: i64Like, den: i64Like):
         ...
 
+    @BUILTINS.method(egg_fn="to-f64")
+    def to_f64(self) -> f64:  # type: ignore[empty-body]
+        ...
+
     @BUILTINS.method(egg_fn="+")
     def __add__(self, other: Rational) -> Rational:  # type: ignore[empty-body]
         ...
 
     @BUILTINS.method(egg_fn="-")
     def __sub__(self, other: Rational) -> Rational:  # type: ignore[empty-body]
         ...
@@ -258,7 +301,47 @@
     @BUILTINS.method(egg_fn="sqrt")
     def sqrt(self) -> Rational:  # type: ignore[empty-body]
         ...
 
     @BUILTINS.method(egg_fn="cbrt")
     def cbrt(self) -> Rational:  # type: ignore[empty-body]
         ...
+
+
+@BUILTINS.class_(egg_sort="Vec")
+class Vec(BaseExpr, Generic[T]):
+    @BUILTINS.method(egg_fn="vec-of")
+    def __init__(self, *args: T) -> None:
+        ...
+
+    @BUILTINS.method(egg_fn="vec-empty")
+    @classmethod
+    def empty(cls) -> Vec[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-append")
+    def append(self, *others: Vec[T]) -> Vec[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-push")
+    def push(self, value: T) -> Vec[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-pop")
+    def pop(self) -> Vec[T]:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-not-contains")
+    def not_contains(self, value: T) -> Unit:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-contains")
+    def contains(self, value: T) -> Unit:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-length")
+    def length(self) -> i64:  # type: ignore[empty-body]
+        ...
+
+    @BUILTINS.method(egg_fn="vec-get")
+    def __getitem__(self, index: i64Like) -> T:  # type: ignore[empty-body]
+        ...
```

### Comparing `egglog-0.4.0/python/egglog/declarations.py` & `egglog-0.5.1/python/egglog/declarations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 """
 Data only descriptions of the components of an egraph and the expressions.
 """
 
 from __future__ import annotations
 
+import itertools
+from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Iterable, Optional, Union, cast
+from typing import ClassVar, Iterable, Optional, Union
 
 from typing_extensions import assert_never
 
 from . import bindings
 
 __all__ = [
     "Declarations",
+    "ModuleDeclarations",
     "JustTypeRef",
     "ClassTypeVarRef",
     "TypeRefWithVars",
     "TypeOrVarRef",
     "FunctionRef",
     "MethodRef",
     "ClassMethodRef",
     "ClassVariableRef",
+    "FunctionCallableRef",
     "CallableRef",
     "ConstantRef",
-    "constant_function_decl",
     "FunctionDecl",
     "VarDecl",
     "LitType",
     "LitDecl",
     "CallDecl",
     "ExprDecl",
-    "tp_and_expr_decl_from_egg",
+    "TypedExprDecl",
     "ClassDecl",
-    "RewriteDecl",
-    "EqDecl",
-    "FactDecl",
-    "fact_decl_to_egg",
-    "RuleDecl",
-    "LetDecl",
-    "SetDecl",
-    "DeleteDecl",
-    "UnionDecl",
-    "PanicDecl",
-    "ActionDecl",
-    "action_decl_to_egg",
+    "Command",
+    "Action",
+    "ExprAction",
+    "Fact",
+    "Rewrite",
+    "BiRewrite",
+    "Eq",
+    "ExprFact",
+    "Rule",
+    "Let",
+    "Set",
+    "Delete",
+    "Union_",
+    "Panic",
+    "Action",
+    "Schedule",
+    "Sequence",
+    "Run",
 ]
 # Special methods which we might want to use as functions
 # Mapping to the operator they represent for pretty printing them
 # https://docs.python.org/3/reference/datamodel.html
 BINARY_METHODS = {
     "__lt__": "<",
     "__le__": "<=",
@@ -79,40 +88,27 @@
 }
 
 
 @dataclass
 class Declarations:
     _functions: dict[str, FunctionDecl] = field(default_factory=dict)
     _classes: dict[str, ClassDecl] = field(default_factory=dict)
-    _constants: dict[str, FunctionDecl] = field(default_factory=dict)
+    _constants: dict[str, JustTypeRef] = field(default_factory=dict)
 
     # Bidirectional mapping between egg function names and python callable references.
     # Note that there are possibly mutliple callable references for a single egg function name, like `+`
     # for both int and rational classes.
     _egg_fn_to_callable_refs: defaultdict[str, set[CallableRef]] = field(default_factory=lambda: defaultdict(set))
     _callable_ref_to_egg_fn: dict[CallableRef, str] = field(default_factory=dict)
 
     # Bidirectional mapping between egg sort names and python type references.
     _egg_sort_to_type_ref: dict[str, JustTypeRef] = field(default_factory=dict)
     _type_ref_to_egg_sort: dict[JustTypeRef, str] = field(default_factory=dict)
 
-    def _get_function_decl(self, ref: CallableRef) -> FunctionDecl:
-        if isinstance(ref, FunctionRef):
-            return self._functions[ref.name]
-        elif isinstance(ref, MethodRef):
-            return self._classes[ref.class_name].methods[ref.method_name]
-        elif isinstance(ref, ClassMethodRef):
-            return self._classes[ref.class_name].class_methods[ref.method_name]
-        elif isinstance(ref, ConstantRef):
-            return self._constants[ref.name]
-        elif isinstance(ref, ClassVariableRef):
-            return self._classes[ref.class_name].class_variables[ref.variable_name]
-        assert_never(ref)
-
-    def _set_function_decl(self, ref: CallableRef, decl: FunctionDecl) -> None:
+    def set_function_decl(self, ref: FunctionCallableRef, decl: FunctionDecl) -> None:
         """
         Sets a function declaration for the given callable reference.
         """
         if isinstance(ref, FunctionRef):
             if ref.name in self._functions:
                 raise ValueError(f"Function {ref.name} already registered")
             self._functions[ref.name] = decl
@@ -120,83 +116,194 @@
             if ref.method_name in self._classes[ref.class_name].methods:
                 raise ValueError(f"Method {ref.class_name}.{ref.method_name} already registered")
             self._classes[ref.class_name].methods[ref.method_name] = decl
         elif isinstance(ref, ClassMethodRef):
             if ref.method_name in self._classes[ref.class_name].class_methods:
                 raise ValueError(f"Class method {ref.class_name}.{ref.method_name} already registered")
             self._classes[ref.class_name].class_methods[ref.method_name] = decl
-        elif isinstance(ref, ConstantRef):
+        else:
+            assert_never(ref)
+
+    def set_constant_type(self, ref: ConstantCallableRef, tp: JustTypeRef) -> None:
+        if isinstance(ref, ConstantRef):
             if ref.name in self._constants:
                 raise ValueError(f"Constant {ref.name} already registered")
-            self._constants[ref.name] = decl
+            self._constants[ref.name] = tp
         elif isinstance(ref, ClassVariableRef):
             if ref.variable_name in self._classes[ref.class_name].class_variables:
                 raise ValueError(f"Class variable {ref.class_name}.{ref.variable_name} already registered")
-            self._classes[ref.class_name].class_variables[ref.variable_name] = decl
+            self._classes[ref.class_name].class_variables[ref.variable_name] = tp
         else:
             assert_never(ref)
 
+    def register_callable_ref(self, ref: CallableRef, egg_name: str) -> None:
+        """
+        Registers a callable reference with the given egg name. The callable's function needs to be registered
+        first.
+        """
+        if ref in self._callable_ref_to_egg_fn:
+            raise ValueError(f"Callable ref {ref} already registered")
+        self._callable_ref_to_egg_fn[ref] = egg_name
+        self._egg_fn_to_callable_refs[egg_name].add(ref)
+
+    def get_function_decl(self, ref: FunctionCallableRef) -> FunctionDecl:
+        if isinstance(ref, FunctionRef):
+            return self._functions[ref.name]
+        elif isinstance(ref, MethodRef):
+            return self._classes[ref.class_name].methods[ref.method_name]
+        elif isinstance(ref, ClassMethodRef):
+            return self._classes[ref.class_name].class_methods[ref.method_name]
+        assert_never(ref)
+
+    def get_constant_type(self, ref: ConstantCallableRef) -> JustTypeRef:
+        if isinstance(ref, ConstantRef):
+            return self._constants[ref.name]
+        elif isinstance(ref, ClassVariableRef):
+            return self._classes[ref.class_name].class_variables[ref.variable_name]
+        assert_never(ref)
+
+    def get_callable_refs(self, egg_name: str) -> Iterable[CallableRef]:
+        return self._egg_fn_to_callable_refs[egg_name]
+
+    def get_egg_fn(self, ref: CallableRef) -> str:
+        return self._callable_ref_to_egg_fn[ref]
+
+    def get_egg_sort(self, ref: JustTypeRef) -> str:
+        return self._type_ref_to_egg_sort[ref]
+
+
+@dataclass
+class ModuleDeclarations:
+    """
+    A set of working declerations for a module.
+    """
+
+    # The modules declarations we have, which we can edit
+    _decl: Declarations
+    # A list of other declarations we can use, but not edit
+    _included_decls: list[Declarations] = field(default_factory=list, repr=False)
+
+    @property
+    def all_decls(self) -> Iterable[Declarations]:
+        return itertools.chain([self._decl], self._included_decls)
+
+    def get_function_decl(self, ref: CallableRef) -> FunctionDecl:
+        if isinstance(ref, (ClassVariableRef, ConstantRef)):
+            for decls in self.all_decls:
+                try:
+                    return decls.get_constant_type(ref).to_constant_function_decl()
+                except KeyError:
+                    pass
+            raise KeyError(f"Constant {ref} not found")
+        elif isinstance(ref, (FunctionRef, MethodRef, ClassMethodRef)):
+            for decls in self.all_decls:
+                try:
+                    return decls.get_function_decl(ref)
+                except KeyError:
+                    pass
+            raise KeyError(f"Function {ref} not found")
+        else:
+            assert_never(ref)
+
+    def get_callable_refs(self, egg_name: str) -> Iterable[CallableRef]:
+        return itertools.chain.from_iterable(decls.get_callable_refs(egg_name) for decls in self.all_decls)
+
+    def get_egg_fn(self, ref: CallableRef) -> str:
+        for decls in self.all_decls:
+            try:
+                return decls.get_egg_fn(ref)
+            except KeyError:
+                pass
+        raise KeyError(f"Callable ref {ref} not found")
+
+    def get_egg_sort(self, ref: JustTypeRef) -> str:
+        for decls in self.all_decls:
+            try:
+                return decls.get_egg_sort(ref)
+            except KeyError:
+                pass
+        raise KeyError(f"Type {ref} not found")
+
+    def get_class_decl(self, name: str) -> ClassDecl:
+        for decls in self.all_decls:
+            try:
+                return decls._classes[name]
+            except KeyError:
+                pass
+        raise KeyError(f"Class {name} not found")
+
+    def get_registered_class_args(self, cls_name: str) -> tuple[JustTypeRef, ...]:
+        """
+        Given a class name, returns the first typevar regsisted with args of that class.
+        """
+        for decl in self.all_decls:
+            for tp in decl._type_ref_to_egg_sort.keys():
+                if tp.name == cls_name and tp.args:
+                    return tp.args
+        return ()
+
     def register_class(self, name: str, n_type_vars: int, egg_sort: Optional[str]) -> Iterable[bindings._Command]:
         # Register class first
-        if name in self._classes:
+        if name in self._decl._classes:
             raise ValueError(f"Class {name} already registered")
         decl = ClassDecl(n_type_vars=n_type_vars)
-        self._classes[name] = decl
-        return self._register_sort(JustTypeRef(name), egg_sort)
-
-    def _register_sort(self, ref: JustTypeRef, egg_name: Optional[str] = None) -> Iterable[bindings._Command]:
+        self._decl._classes[name] = decl
+        _egg_sort, cmds = self.register_sort(JustTypeRef(name), egg_sort)
+        return cmds
+
+    def register_sort(
+        self, ref: JustTypeRef, egg_name: Optional[str] = None
+    ) -> tuple[str, Iterable[bindings._Command]]:
         """
         Register a sort with the given name. If no name is given, one is generated.
 
         If this is a type called with generic args, register the generic args as well.
         """
-        if ref in self._type_ref_to_egg_sort:
-            if egg_name and self._type_ref_to_egg_sort[ref] != egg_name:
-                raise ValueError(f"Type {ref} is already registered with egg name {self._type_ref_to_egg_sort[ref]}")
-            return []
+        # If the sort is already registered, do nothing
+        try:
+            egg_sort = self.get_egg_sort(ref)
+        except KeyError:
+            pass
+        else:
+            return (egg_sort, [])
         egg_name = egg_name or ref.generate_egg_name()
-        if egg_name in self._egg_sort_to_type_ref:
+        if egg_name in self._decl._egg_sort_to_type_ref:
             raise ValueError(f"Sort {egg_name} is already registered.")
-        self._egg_sort_to_type_ref[egg_name] = ref
-        self._type_ref_to_egg_sort[ref] = egg_name
-        return ref.to_commands(self)
-
-    def register_callable(
-        self, ref: CallableRef, fn_decl: FunctionDecl, egg_name: Optional[str], generate_commands: bool = True
+        self._decl._egg_sort_to_type_ref[egg_name] = ref
+        self._decl._type_ref_to_egg_sort[ref] = egg_name
+        return egg_name, ref.to_commands(self)
+
+    def register_function_callable(
+        self,
+        ref: FunctionCallableRef,
+        fn_decl: FunctionDecl,
+        egg_name: Optional[str],
+        cost: Optional[int],
+        default: Optional[ExprDecl],
+        merge: Optional[ExprDecl],
+        merge_action: Iterable[Action],
     ) -> Iterable[bindings._Command]:
         """
         Registers a callable with the given egg name. The callable's function needs to be registered
         first.
         """
         egg_name = egg_name or ref.generate_egg_name()
-        self.register_callable_ref(ref, egg_name)
-        self._set_function_decl(ref, fn_decl)
-        return fn_decl.to_commands(self, egg_name) if generate_commands else []
+        self._decl.register_callable_ref(ref, egg_name)
+        self._decl.set_function_decl(ref, fn_decl)
+        return fn_decl.to_commands(self, egg_name, cost, default, merge, merge_action)
 
-    def register_callable_ref(self, ref: CallableRef, egg_name: str) -> None:
-        """
-        Registers a callable reference with the given egg name. The callable's function needs to be registered
-        first.
-        """
-        if ref in self._callable_ref_to_egg_fn:
-            raise ValueError(f"Callable ref {ref} already registered")
-        self._callable_ref_to_egg_fn[ref] = egg_name
-        self._egg_fn_to_callable_refs[egg_name].add(ref)
-
-    def get_egg_fn(self, ref: CallableRef) -> str:
-        return self._callable_ref_to_egg_fn[ref]
-
-
-def constant_function_decl(type_ref: JustTypeRef) -> FunctionDecl:
-    """
-    Create a function decleartion for a constant function. This is similar to how egglog compiles
-    the `constant` command.
-    """
-    # Divide high cost by 10 to not overflow the cost field.
-    return FunctionDecl(arg_types=(), return_type=type_ref.to_var(), cost=int(bindings.HIGH_COST / 10))
+    def register_constant_callable(
+        self, ref: ConstantCallableRef, type_ref: JustTypeRef, egg_name: Optional[str]
+    ) -> Iterable[bindings._Command]:
+        egg_function = ref.generate_egg_name()
+        self._decl.register_callable_ref(ref, egg_function)
+        self._decl.set_constant_type(ref, type_ref)
+        # Create a function decleartion for a constant function. This is similar to how egglog compiles
+        # the `declare` command.
+        return FunctionDecl((), type_ref.to_var()).to_commands(self, egg_name or ref.generate_egg_name())
 
 
 # Have two different types of type refs, one that can include vars recursively and one that cannot.
 # We only use the one with vars for classmethods and methods, and the other one for egg references as
 # well as runtime values.
 @dataclass(frozen=True)
 class JustTypeRef:
@@ -205,36 +312,45 @@
 
     def generate_egg_name(self) -> str:
         """
         Generates an egg sort name for this type reference by linearizing the type.
         """
         if not self.args:
             return self.name
-        args = "_".join(a.generate_egg_name() for a in self.args)
-        return f"{self.name}__{args}"
+        args = ", ".join(a.generate_egg_name() for a in self.args)
+        return f"{self.name}[{args}]"
 
-    def to_commands(self, decls: Declarations) -> Iterable[bindings._Command]:
+    def to_commands(self, mod_decls: ModuleDeclarations) -> Iterable[bindings._Command]:
         """
-        Register this type with the egg solver.
+        Returns commands to register this as a sort, as well as for any of its arguments.
         """
-        egg_name = decls._type_ref_to_egg_sort[self]
+        egg_name = mod_decls.get_egg_sort(self)
+        arg_sorts: list[bindings._Expr] = []
         for arg in self.args:
-            yield from decls._register_sort(arg)
-        arg_sorts = [cast("bindings._Expr", bindings.Var(decls._type_ref_to_egg_sort[a])) for a in self.args]
+            egg_sort, cmds = mod_decls.register_sort(arg)
+            arg_sorts.append(bindings.Var(egg_sort))
+            yield from cmds
         yield bindings.Sort(egg_name, (self.name, arg_sorts) if arg_sorts else None)
 
     def to_var(self) -> TypeRefWithVars:
         return TypeRefWithVars(self.name, tuple(a.to_var() for a in self.args))
 
     def pretty(self) -> str:
         if not self.args:
             return self.name
         args = ", ".join(a.pretty() for a in self.args)
         return f"{self.name}[{args}]"
 
+    def to_constant_function_decl(self) -> FunctionDecl:
+        """
+        Create a function declaration for a constant function. This is similar to how egglog compiles
+        the `constant` command.
+        """
+        return FunctionDecl(arg_types=(), return_type=self.to_var(), var_arg_type=None)
+
 
 @dataclass(frozen=True)
 class ClassTypeVarRef:
     """
     A class type variable represents one of the types of the class, if it is a generic
     class.
     """
@@ -267,27 +383,27 @@
 
 @dataclass(frozen=True)
 class MethodRef:
     class_name: str
     method_name: str
 
     def generate_egg_name(self) -> str:
-        return f"{self.class_name}__{self.method_name}"
+        return f"{self.class_name}.{self.method_name}"
 
 
 @dataclass(frozen=True)
 class ClassMethodRef:
     class_name: str
     method_name: str
 
     def to_egg(self, decls: Declarations) -> str:
-        return decls._callable_ref_to_egg_fn[self]
+        return decls.get_egg_fn(self)
 
     def generate_egg_name(self) -> str:
-        return f"{self.class_name}__{self.method_name}"
+        return f"{self.class_name}.{self.method_name}"
 
 
 @dataclass(frozen=True)
 class ConstantRef:
     name: str
 
     def generate_egg_name(self) -> str:
@@ -296,88 +412,96 @@
 
 @dataclass(frozen=True)
 class ClassVariableRef:
     class_name: str
     variable_name: str
 
     def generate_egg_name(self) -> str:
-        return f"{self.class_name}__{self.variable_name}"
+        return f"{self.class_name}.{self.variable_name}"
 
 
-CallableRef = Union[FunctionRef, MethodRef, ClassMethodRef, ConstantRef, ClassVariableRef]
+ConstantCallableRef = Union[ConstantRef, ClassVariableRef]
+FunctionCallableRef = Union[FunctionRef, MethodRef, ClassMethodRef]
+CallableRef = Union[ConstantCallableRef, FunctionCallableRef]
 
 
 @dataclass(frozen=True)
 class FunctionDecl:
     # TODO: Add arg name to arg so can call with keyword arg
     arg_types: tuple[TypeOrVarRef, ...]
     return_type: TypeOrVarRef
-    cost: Optional[int] = None
-    default: Optional[ExprDecl] = None
-    merge: Optional[ExprDecl] = None
-    merge_action: tuple[ActionDecl, ...] = ()
-
-    def to_commands(self, decls: Declarations, egg_name: str) -> Iterable[bindings._Command]:
-        just_arg_types = [a.to_just() for a in self.arg_types]
-        for a in just_arg_types:
-            yield from decls._register_sort(a)
-        just_return_type = self.return_type.to_just()
-        yield from decls._register_sort(just_return_type)
+    var_arg_type: Optional[TypeOrVarRef] = None
 
-        egg_fn_decl = bindings.FunctionDecl(
-            egg_name,
+    def to_commands(
+        self,
+        mod_decls: ModuleDeclarations,
+        egg_name: str,
+        cost: Optional[int] = None,
+        default: Optional[ExprDecl] = None,
+        merge: Optional[ExprDecl] = None,
+        merge_action: Iterable[Action] = (),
+    ) -> Iterable[bindings._Command]:
+        if self.var_arg_type is not None:
+            raise NotImplementedError("egglog does not support variable arguments yet.")
+        arg_sorts: list[str] = []
+        for a in self.arg_types:
             # Remove all vars from the type refs, raising an errory if we find one,
             # since we cannot create egg functions with vars
-            bindings.Schema(
-                [decls._type_ref_to_egg_sort[a] for a in just_arg_types],
-                decls._type_ref_to_egg_sort[just_return_type],
-            ),
-            self.default.to_egg(decls) if self.default else None,
-            self.merge.to_egg(decls) if self.merge else None,
-            [action_decl_to_egg(decls, a) for a in self.merge_action],
-            self.cost,
+            arg_sort, cmds = mod_decls.register_sort(a.to_just())
+            yield from cmds
+            arg_sorts.append(arg_sort)
+        return_sort, cmds = mod_decls.register_sort(self.return_type.to_just())
+        yield from cmds
+
+        egg_fn_decl = bindings.FunctionDecl(
+            egg_name,
+            bindings.Schema(arg_sorts, return_sort),
+            default.to_egg(mod_decls) if default else None,
+            merge.to_egg(mod_decls) if merge else None,
+            [a._to_egg_action(mod_decls) for a in merge_action],
+            cost,
         )
         yield bindings.Function(egg_fn_decl)
 
 
 @dataclass(frozen=True)
 class VarDecl:
     name: str
 
     @classmethod
-    def from_egg(cls, var: bindings.Var) -> tuple[JustTypeRef, LitDecl]:
+    def from_egg(cls, var: bindings.Var) -> TypedExprDecl:
         raise NotImplementedError("Cannot turn var into egg type because typing unknown.")
 
-    def to_egg(self, _decls: Declarations) -> bindings.Var:
+    def to_egg(self, _decls: ModuleDeclarations) -> bindings.Var:
         return bindings.Var(self.name)
 
     def pretty(self, **kwargs) -> str:
         return self.name
 
 
 LitType = Union[int, str, float, None]
 
 
 @dataclass(frozen=True)
 class LitDecl:
     value: LitType
 
     @classmethod
-    def from_egg(cls, lit: bindings.Lit) -> tuple[JustTypeRef, LitDecl]:
+    def from_egg(cls, lit: bindings.Lit) -> TypedExprDecl:
         if isinstance(lit.value, bindings.Int):
-            return JustTypeRef("i64"), cls(lit.value.value)
+            return TypedExprDecl(JustTypeRef("i64"), cls(lit.value.value))
         if isinstance(lit.value, bindings.String):
-            return JustTypeRef("String"), cls(lit.value.value)
+            return TypedExprDecl(JustTypeRef("String"), cls(lit.value.value))
         if isinstance(lit.value, bindings.F64):
-            return JustTypeRef("f64"), cls(lit.value.value)
+            return TypedExprDecl(JustTypeRef("f64"), cls(lit.value.value))
         elif isinstance(lit.value, bindings.Unit):
-            return JustTypeRef("unit"), cls(None)
+            return TypedExprDecl(JustTypeRef("Unit"), cls(None))
         assert_never(lit.value)
 
-    def to_egg(self, _decls: Declarations) -> bindings.Lit:
+    def to_egg(self, _decls: ModuleDeclarations) -> bindings.Lit:
         if self.value is None:
             return bindings.Lit(bindings.Unit())
         if isinstance(self.value, int):
             return bindings.Lit(bindings.Int(self.value))
         if isinstance(self.value, float):
             return bindings.Lit(bindings.F64(self.value))
         if isinstance(self.value, str):
@@ -387,63 +511,70 @@
     def pretty(self, wrap_lit=True, **kwargs) -> str:
         """
         Returns a string representation of the literal.
 
         :param wrap_lit: If True, wraps the literal in a call to the literal constructor.
         """
         if self.value is None:
-            return "unit()"
+            return "Unit()"
         if isinstance(self.value, int):
             return f"i64({self.value})" if wrap_lit else str(self.value)
         if isinstance(self.value, float):
             return f"f64({self.value})" if wrap_lit else str(self.value)
         if isinstance(self.value, str):
             return f"String({repr(self.value)})" if wrap_lit else repr(self.value)
         assert_never(self.value)
 
 
 @dataclass(frozen=True)
 class CallDecl:
     callable: CallableRef
-    args: tuple[ExprDecl, ...] = ()
+    args: tuple[TypedExprDecl, ...] = ()
     # type parameters that were bound to the callable, if it is a classmethod
+    # Used for pretty printing classmethod calls with type parameters
     bound_tp_params: Optional[tuple[JustTypeRef, ...]] = None
 
     def __post_init__(self):
         if self.bound_tp_params and not isinstance(self.callable, ClassMethodRef):
             raise ValueError("Cannot bind type parameters to a non-class method callable.")
 
     @classmethod
-    def from_egg(cls, decls: Declarations, call: bindings.Call) -> tuple[JustTypeRef, CallDecl]:
+    def from_egg(cls, mod_decls: ModuleDeclarations, call: bindings.Call) -> TypedExprDecl:
         from .type_constraint_solver import TypeConstraintSolver
 
-        results = [tp_and_expr_decl_from_egg(decls, a) for a in call.args]
-        arg_types = tuple(r[0] for r in results)
-        arg_decls = tuple(r[1] for r in results)
+        results = tuple(TypedExprDecl.from_egg(mod_decls, a) for a in call.args)
+        arg_types = tuple(r.tp for r in results)
 
         # Find the first callable ref that matches the call
-        for callable_ref in decls._egg_fn_to_callable_refs[call.name]:
-            tcs = TypeConstraintSolver()
-            fn_decl = decls._get_function_decl(callable_ref)
-            return_tp = tcs.infer_return_type(fn_decl.arg_types, fn_decl.return_type, arg_types)
-            return return_tp, cls(callable_ref, arg_decls)
+        for callable_ref in mod_decls.get_callable_refs(call.name):
+            # If this is a classmethod, we might need the type params that were bound for this type
+            # egglog currently only allows one instantiated type of any generic sort to be used in any program
+            # So we just lookup what args were registered for this sort
+            if isinstance(callable_ref, ClassMethodRef):
+                cls_args = mod_decls.get_registered_class_args(callable_ref.class_name)
+                tcs = TypeConstraintSolver.from_type_parameters(cls_args)
+            else:
+                tcs = TypeConstraintSolver()
+            fn_decl = mod_decls.get_function_decl(callable_ref)
+            return_tp = tcs.infer_return_type(fn_decl.arg_types, fn_decl.return_type, fn_decl.var_arg_type, arg_types)
+            return TypedExprDecl(return_tp, cls(callable_ref, tuple(results)))
         raise ValueError(f"Could not find callable ref for call {call}")
 
-    def to_egg(self, decls: Declarations) -> bindings.Call:
+    def to_egg(self, mod_decls: ModuleDeclarations) -> bindings.Call:
         """Convert a Call to an egg Call."""
-        egg_fn = decls._callable_ref_to_egg_fn[self.callable]
-        return bindings.Call(egg_fn, [a.to_egg(decls) for a in self.args])
+        egg_fn = mod_decls.get_egg_fn(self.callable)
+        return bindings.Call(egg_fn, [a.to_egg(mod_decls) for a in self.args])
 
     def pretty(self, parens=True, **kwargs) -> str:
         """
         Pretty print the call.
 
         :param parens: If true, wrap the call in parens if it is a binary or unary method call.
         """
-        ref, args = self.callable, list(self.args)
+        ref, args = self.callable, [a.expr for a in self.args]
         if isinstance(ref, FunctionRef):
             fn_str = ref.name
         elif isinstance(ref, ClassMethodRef):
             tp_ref = JustTypeRef(ref.class_name, self.bound_tp_params or ())
             if ref.method_name == "__init__":
                 fn_str = tp_ref.pretty()
             else:
@@ -473,144 +604,331 @@
 
 
 def test_expr_pretty():
     assert VarDecl("x").pretty() == "x"
     assert LitDecl(42).pretty() == "i64(42)"
     assert LitDecl("foo").pretty() == 'String("foo")'
     assert LitDecl(None).pretty() == "unit()"
-    assert CallDecl(FunctionRef("foo"), (VarDecl("x"),)).pretty() == "foo(x)"
-    assert CallDecl(FunctionRef("foo"), (VarDecl("x"), VarDecl("y"), VarDecl("z"))).pretty() == "foo(x, y, z)"
-    assert CallDecl(MethodRef("foo", "__add__"), (VarDecl("x"), VarDecl("y"))).pretty() == "x + y"
-    assert CallDecl(MethodRef("foo", "__getitem__"), (VarDecl("x"), VarDecl("y"))).pretty() == "x[y]"
-    assert CallDecl(ClassMethodRef("foo", "__init__"), (VarDecl("x"), VarDecl("y"))).pretty() == "foo(x, y)"
-    assert CallDecl(ClassMethodRef("foo", "bar"), (VarDecl("x"), VarDecl("y"))).pretty() == "foo.bar(x, y)"
-    assert CallDecl(MethodRef("foo", "__call__"), (VarDecl("x"), VarDecl("y"))).pretty() == "x(y)"
+
+    def v(x: str) -> TypedExprDecl:
+        return TypedExprDecl(JustTypeRef(""), VarDecl(x))
+
+    assert CallDecl(FunctionRef("foo"), (v("x"),)).pretty() == "foo(x)"
+    assert CallDecl(FunctionRef("foo"), (v("x"), v("y"), v("z"))).pretty() == "foo(x, y, z)"
+    assert CallDecl(MethodRef("foo", "__add__"), (v("x"), v("y"))).pretty() == "x + y"
+    assert CallDecl(MethodRef("foo", "__getitem__"), (v("x"), v("y"))).pretty() == "x[y]"
+    assert CallDecl(ClassMethodRef("foo", "__init__"), (v("x"), v("y"))).pretty() == "foo(x, y)"
+    assert CallDecl(ClassMethodRef("foo", "bar"), (v("x"), v("y"))).pretty() == "foo.bar(x, y)"
+    assert CallDecl(MethodRef("foo", "__call__"), (v("x"), v("y"))).pretty() == "x(y)"
     assert (
         CallDecl(
             ClassMethodRef("Map", "__init__"),
             (),
-            (JustTypeRef("i64"), JustTypeRef("unit")),
+            (JustTypeRef("i64"), JustTypeRef("Unit")),
         ).pretty()
-        == "Map[i64, unit]()"
+        == "Map[i64, Unit]()"
     )
 
 
 ExprDecl = Union[VarDecl, LitDecl, CallDecl]
 
 
-def tp_and_expr_decl_from_egg(decls: Declarations, expr: bindings._Expr) -> tuple[JustTypeRef, ExprDecl]:
-    if isinstance(expr, bindings.Var):
-        return VarDecl.from_egg(expr)
-    if isinstance(expr, bindings.Lit):
-        return LitDecl.from_egg(expr)
-    if isinstance(expr, bindings.Call):
-        return CallDecl.from_egg(decls, expr)
-    assert_never(expr)
+@dataclass(frozen=True)
+class TypedExprDecl:
+    tp: JustTypeRef
+    expr: ExprDecl
+
+    @classmethod
+    def from_egg(cls, mod_decls: ModuleDeclarations, expr: bindings._Expr) -> TypedExprDecl:
+        if isinstance(expr, bindings.Var):
+            return VarDecl.from_egg(expr)
+        if isinstance(expr, bindings.Lit):
+            return LitDecl.from_egg(expr)
+        if isinstance(expr, bindings.Call):
+            return CallDecl.from_egg(mod_decls, expr)
+        assert_never(expr)
+
+    def to_egg(self, decls: ModuleDeclarations) -> bindings._Expr:
+        return self.expr.to_egg(decls)
 
 
 @dataclass
 class ClassDecl:
     methods: dict[str, FunctionDecl] = field(default_factory=dict)
     class_methods: dict[str, FunctionDecl] = field(default_factory=dict)
-    class_variables: dict[str, FunctionDecl] = field(default_factory=dict)
+    class_variables: dict[str, JustTypeRef] = field(default_factory=dict)
     n_type_vars: int = 0
 
 
+class Command(ABC):
+    """
+    A command that can be executed in the egg interpreter.
+
+    We only use this for commands which return no result and don't create new Python objects.
+
+    Anything that can be passed to the `register` function in a Module is a Command.
+    """
+
+    @abstractmethod
+    def _to_egg_command(self, mod_decls: ModuleDeclarations) -> bindings._Command:
+        raise NotImplementedError
+
+    @abstractmethod
+    def __str__(self) -> str:
+        raise NotImplementedError
+
+
 @dataclass(frozen=True)
-class RewriteDecl:
-    lhs: ExprDecl
-    rhs: ExprDecl
-    conditions: tuple[FactDecl, ...]
+class Rewrite(Command):
+    _ruleset: str
+    _lhs: ExprDecl
+    _rhs: ExprDecl
+    _conditions: tuple[Fact, ...]
+    _fn_name: ClassVar[str] = "rewrite"
+
+    def __str__(self) -> str:
+        args_str = ", ".join(map(str, [self._rhs.pretty(), *self._conditions]))
+        return f"{self._fn_name}({self._lhs.pretty()}).to({args_str})"
 
-    def to_egg(self, decls: Declarations) -> bindings.Rewrite:
+    def _to_egg_command(self, mod_decls: ModuleDeclarations) -> bindings._Command:
+        return bindings.RewriteCommand(self._ruleset, self._to_egg_rewrite(mod_decls))
+
+    def _to_egg_rewrite(self, mod_decls: ModuleDeclarations) -> bindings.Rewrite:
         return bindings.Rewrite(
-            self.lhs.to_egg(decls),
-            self.rhs.to_egg(decls),
-            [fact_decl_to_egg(decls, c) for c in self.conditions],
+            self._lhs.to_egg(mod_decls),
+            self._rhs.to_egg(mod_decls),
+            [c._to_egg_fact(mod_decls) for c in self._conditions],
         )
 
 
 @dataclass(frozen=True)
-class EqDecl:
-    exprs: tuple[ExprDecl, ...]
+class BiRewrite(Rewrite):
+    _fn_name: ClassVar[str] = "birewrite"
+
+    def _to_egg_command(self, mod_decls: ModuleDeclarations) -> bindings._Command:
+        return bindings.BiRewriteCommand(self._ruleset, self._to_egg_rewrite(mod_decls))
 
-    def to_egg(self, decls: Declarations) -> bindings.Eq:
-        return bindings.Eq([e.to_egg(decls) for e in self.exprs])
 
+class Fact(ABC):
+    """
+    An e-graph fact, either an equality or a unit expression.
+    """
+
+    @abstractmethod
+    def _to_egg_fact(self, mod_decls: ModuleDeclarations) -> bindings._Fact:
+        raise NotImplementedError
 
-FactDecl = Union[ExprDecl, EqDecl]
 
+@dataclass(frozen=True)
+class Eq(Fact):
+    _exprs: tuple[ExprDecl, ...]
+
+    def __str__(self) -> str:
+        first, *rest = (e.pretty() for e in self._exprs)
+        args_str = ", ".join(rest)
+        return f"eq({first}).to({args_str})"
 
-def fact_decl_to_egg(decls: Declarations, fact: FactDecl) -> bindings._Fact:
-    if isinstance(fact, EqDecl):
-        return fact.to_egg(decls)
-    return bindings.Fact(fact.to_egg(decls))
+    def _to_egg_fact(self, mod_decls: ModuleDeclarations) -> bindings.Eq:
+        return bindings.Eq([e.to_egg(mod_decls) for e in self._exprs])
 
 
 @dataclass(frozen=True)
-class RuleDecl:
-    head: tuple[ActionDecl, ...]
-    body: tuple[FactDecl, ...]
+class ExprFact(Fact):
+    _expr: ExprDecl
 
-    def to_egg(self, decls: Declarations) -> bindings.Rule:
-        return bindings.Rule(
-            [action_decl_to_egg(decls, a) for a in self.head],
-            [fact_decl_to_egg(decls, f) for f in self.body],
-        )
+    def __str__(self) -> str:
+        return self._expr.pretty()
+
+    def _to_egg_fact(self, mod_decls: ModuleDeclarations) -> bindings.Fact:
+        return bindings.Fact(self._expr.to_egg(mod_decls))
 
 
 @dataclass(frozen=True)
-class LetDecl:
+class Rule(Command):
+    head: tuple[Action, ...]
+    body: tuple[Fact, ...]
     name: str
-    value: ExprDecl
+    ruleset: str
+
+    def __str__(self) -> str:
+        head_str = ", ".join(map(str, self.head))
+        body_str = ", ".join(map(str, self.body))
+        return f"rule({head_str}).then({body_str})"
+
+    def _to_egg_command(self, mod_decls: ModuleDeclarations) -> bindings.RuleCommand:
+        return bindings.RuleCommand(
+            self.name,
+            self.ruleset,
+            bindings.Rule(
+                [a._to_egg_action(mod_decls) for a in self.head],
+                [f._to_egg_fact(mod_decls) for f in self.body],
+            ),
+        )
+
+
+class Action(Command, ABC):
+    @abstractmethod
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings._Action:
+        raise NotImplementedError
+
+    def _to_egg_command(self, mod_decls: ModuleDeclarations) -> bindings._Command:
+        return bindings.ActionCommand(self._to_egg_action(mod_decls))
+
 
-    def to_egg(self, decls: Declarations) -> bindings.Let:
-        return bindings.Let(self.name, self.value.to_egg(decls))
+@dataclass(frozen=True)
+class Let(Action):
+    _name: str
+    _value: ExprDecl
+
+    def __str__(self) -> str:
+        return f"let({self._name}, {self._value.pretty()})"
+
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings.Let:
+        return bindings.Let(self._name, self._value.to_egg(mod_decls))
 
 
 @dataclass(frozen=True)
-class SetDecl:
-    call: CallDecl
-    rhs: ExprDecl
+class Set(Action):
+    _call: CallDecl
+    _rhs: ExprDecl
 
-    def to_egg(self, decls: Declarations) -> bindings.Set:
+    def __str__(self) -> str:
+        return f"set({self._call.pretty()}).to({self._rhs.pretty()})"
+
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings.Set:
         return bindings.Set(
-            decls._callable_ref_to_egg_fn[self.call.callable],
-            [a.to_egg(decls) for a in self.call.args],
-            self.rhs.to_egg(decls),
+            mod_decls.get_egg_fn(self._call.callable),
+            [a.to_egg(mod_decls) for a in self._call.args],
+            self._rhs.to_egg(mod_decls),
         )
 
 
 @dataclass(frozen=True)
-class DeleteDecl:
-    call: CallDecl
+class ExprAction(Action):
+    _expr: ExprDecl
+
+    def __str__(self) -> str:
+        return self._expr.pretty()
+
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings.Expr_:
+        return bindings.Expr_(self._expr.to_egg(mod_decls))
+
+
+@dataclass(frozen=True)
+class Delete(Action):
+    _call: CallDecl
+
+    def __str__(self) -> str:
+        return f"delete({self._call.pretty()})"
 
-    def to_egg(self, decls: Declarations) -> bindings.Delete:
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings.Delete:
         return bindings.Delete(
-            decls._callable_ref_to_egg_fn[self.call.callable], [a.to_egg(decls) for a in self.call.args]
+            mod_decls.get_egg_fn(self._call.callable), [a.to_egg(mod_decls) for a in self._call.args]
         )
 
 
 @dataclass(frozen=True)
-class UnionDecl:
-    lhs: ExprDecl
-    rhs: ExprDecl
+class Union_(Action):
+    _lhs: ExprDecl
+    _rhs: ExprDecl
 
-    def to_egg(self, decls: Declarations) -> bindings.Union:
-        return bindings.Union(self.lhs.to_egg(decls), self.rhs.to_egg(decls))
+    def __str__(self) -> str:
+        return f"union({self._lhs.pretty()}).with_({self._rhs.pretty()})"
+
+    def _to_egg_action(self, mod_decls: ModuleDeclarations) -> bindings.Union:
+        return bindings.Union(self._lhs.to_egg(mod_decls), self._rhs.to_egg(mod_decls))
 
 
 @dataclass(frozen=True)
-class PanicDecl:
+class Panic(Action):
     message: str
 
-    def to_egg(self, _decls: Declarations) -> bindings.Panic:
+    def __str__(self) -> str:
+        return f"panic({self.message})"
+
+    def _to_egg_action(self, _decls: ModuleDeclarations) -> bindings.Panic:
         return bindings.Panic(self.message)
 
 
-ActionDecl = Union[LetDecl, SetDecl, DeleteDecl, UnionDecl, PanicDecl, ExprDecl]
+# def action_decl_to_egg(decls: Declarations, action: ActionDecl) -> bindings._Action:
+#     if isinstance(action, (CallDecl, LitDecl, VarDecl)):
+#         return bindings.Expr_(action.to_egg(decls))
+#     return action.to_egg(decls)
+
+
+class Schedule(ABC):
+    def __mul__(self, length: int) -> Schedule:
+        """
+        Repeat the schedule a number of times.
+        """
+        return Repeat(length, self)
+
+    def saturate(self) -> Schedule:
+        """
+        Run the schedule until the e-graph is saturated.
+        """
+        return Saturate(self)
+
+    @abstractmethod
+    def __str__(self) -> str:
+        raise NotImplementedError
+
+    @abstractmethod
+    def _to_egg_schedule(self, mod_decls: ModuleDeclarations) -> bindings._Schedule:
+        raise NotImplementedError
+
+
+@dataclass
+class Run(Schedule):
+    """Configuration of a run"""
+
+    limit: int
+    ruleset: str
+    until: tuple[Fact, ...]
+
+    def __str__(self) -> str:
+        args_str = ", ".join(map(str, [self.ruleset, self.limit, *self.until]))
+        return f"run({args_str})"
+
+    def _to_egg_schedule(self, mod_decls: ModuleDeclarations) -> bindings._Schedule:
+        return bindings.Run(self._to_egg_config(mod_decls))
+
+    def _to_egg_config(self, mod_decls: ModuleDeclarations) -> bindings.RunConfig:
+        return bindings.RunConfig(
+            self.ruleset,
+            self.limit,
+            [fact._to_egg_fact(mod_decls) for fact in self.until] if self.until else None,
+        )
+
+
+@dataclass
+class Saturate(Schedule):
+    schedule: Schedule
+
+    def __str__(self) -> str:
+        return f"{self.schedule}.saturate()"
+
+    def _to_egg_schedule(self, mod_decls: ModuleDeclarations) -> bindings._Schedule:
+        return bindings.Saturate(self.schedule._to_egg_schedule(mod_decls))
+
+
+@dataclass
+class Repeat(Schedule):
+    length: int
+    schedule: Schedule
+
+    def __str__(self) -> str:
+        return f"{self.schedule} * {self.length}"
+
+    def _to_egg_schedule(self, mod_decls: ModuleDeclarations) -> bindings._Schedule:
+        return bindings.Repeat(self.length, self.schedule._to_egg_schedule(mod_decls))
+
+
+@dataclass
+class Sequence(Schedule):
+    schedules: tuple[Schedule, ...]
 
+    def __str__(self) -> str:
+        return f"sequence({', '.join(map(str, self.schedules))})"
 
-def action_decl_to_egg(decls: Declarations, action: ActionDecl) -> bindings._Action:
-    if isinstance(action, (CallDecl, LitDecl, VarDecl)):
-        return bindings.Expr_(action.to_egg(decls))
-    return action.to_egg(decls)
+    def _to_egg_schedule(self, mod_decls: ModuleDeclarations) -> bindings._Schedule:
+        return bindings.Sequence([schedule._to_egg_schedule(mod_decls) for schedule in self.schedules])
```

### Comparing `egglog-0.4.0/python/egglog/egraph.py` & `egglog-0.5.1/python/egglog/egraph.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
 from copy import deepcopy
-from dataclasses import dataclass, field
+from dataclasses import InitVar, dataclass, field
 from inspect import Parameter, currentframe, signature
 from types import FunctionType
 from typing import _GenericAlias  # type: ignore[attr-defined]
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -18,36 +19,32 @@
     TypeVar,
     Union,
     cast,
     get_type_hints,
     overload,
 )
 
-from typing_extensions import (
-    ParamSpec,
-    TypeVarTuple,
-    Unpack,
-    assert_never,
-    get_args,
-    get_origin,
-)
+import graphviz
+from egglog.declarations import Declarations
+from typing_extensions import ParamSpec, get_args, get_origin
 
 from . import bindings
 from .declarations import *
 from .monkeypatch import monkeypatch_forward_ref
 from .runtime import *
 from .runtime import _resolve_callable, class_to_ref
 
 if TYPE_CHECKING:
     from .builtins import String
 
 monkeypatch_forward_ref()
 
 __all__ = [
     "EGraph",
+    "Module",
     "BUILTINS",
     "BaseExpr",
     "Unit",
     "rewrite",
     "eq",
     "panic",
     "let",
@@ -56,251 +53,77 @@
     "set_",
     "rule",
     "var",
     "vars_",
     "Fact",
     "expr_parts",
     "Schedule",
-    "config",
-    "sequence",
+    "run",
+    "seq",
 ]
 
 T = TypeVar("T")
-TS = TypeVarTuple("TS")
 P = ParamSpec("P")
 TYPE = TypeVar("TYPE", bound="type[BaseExpr]")
 CALLABLE = TypeVar("CALLABLE", bound=Callable)
 EXPR = TypeVar("EXPR", bound="BaseExpr")
-
+E1 = TypeVar("E1", bound="BaseExpr")
+E2 = TypeVar("E2", bound="BaseExpr")
+E3 = TypeVar("E3", bound="BaseExpr")
+E4 = TypeVar("E4", bound="BaseExpr")
 # Attributes which are sometimes added to classes by the interpreter or the dataclass decorator, or by ipython.
 # We ignore these when inspecting the class.
 
 IGNORED_ATTRIBUTES = {
     "__module__",
     "__doc__",
     "__dict__",
     "__weakref__",
     "__orig_bases__",
     "__annotations__",
     "__hash__",
 }
 
 
-@dataclass
-class EGraph:
-    """
-    An expression graph.
-    """
-
-    _egraph: bindings.EGraph | None = field(repr=False)
-    _decls: Declarations = field(repr=False)
-    # The current declarations which have been pushed to the stack
-    _decl_stack: list[Declarations] = field(default_factory=list, repr=False)
-    _BUILTIN_DECLS: ClassVar[Declarations | None] = None
-
-    def __init__(self, *, _for_builtins: bool = False):
-        """
-        Creates a new e-graph.
-        """
-        # If this is the e-graph to register declerations for our builtins, don't actually create a runtime e-graph
-        if _for_builtins:
-            self._egraph = None
-            self._decls = Declarations()
-            # Set the global builtins to use these declerations
-            EGraph._BUILTIN_DECLS = self._decls
-        # Otherwise, we are creating a normal e-graph and use the builtin declerations as the base
-        else:
-            self._egraph = bindings.EGraph()
-            if not EGraph._BUILTIN_DECLS:
-                raise RuntimeError("Builtin values not registered yet")
-            self._decls = deepcopy(EGraph._BUILTIN_DECLS)
-        self._decl_stack = []
-
-    def _run_program(self, commands: Iterable[bindings._Command]) -> None:
-        if self._egraph:
-            self._egraph.run_program(*commands)
-
-    def _get_egraph(self) -> bindings.EGraph:
-        if not self._egraph:
-            raise RuntimeError("Cannot get the e-graph")
-        return self._egraph
-
-    def simplify(self, expr: EXPR, limit: int, *until: Fact) -> EXPR:
-        """
-        Simplifies the given expression.
-        """
-        return self._simplify(expr, limit, None, until)
-
-    def _simplify(self, expr: EXPR, limit: int, ruleset: Optional[Ruleset], until: tuple[Fact, ...]) -> EXPR:
-        tp, decl = expr_parts(expr)
-        egg_expr = decl.to_egg(self._decls)
-        self._run_program([bindings.Simplify(egg_expr, Config(limit, ruleset, until)._to_egg_config(self._decls))])
-        extract_report = self._get_egraph().extract_report()
-        if not extract_report:
-            raise ValueError("No extract report saved")
-        new_tp, new_decl = tp_and_expr_decl_from_egg(self._decls, extract_report.expr)
-        return cast(EXPR, RuntimeExpr(self._decls, new_tp, new_decl))
-
-    def relation(self, name: str, *tps: Unpack[TS], egg_fn: Optional[str] = None) -> Callable[[Unpack[TS]], Unit]:
-        """
-        Defines a relation, which is the same as a function which returns unit.
-        """
-        arg_types = tuple(self._resolve_type_annotation(cast(object, tp), [], None) for tp in tps)
-        fn_decl = FunctionDecl(arg_types, TypeRefWithVars("unit"))
-        commands = self._decls.register_callable(FunctionRef(name), fn_decl, egg_fn)
-        self._run_program(commands)
-        return cast(Callable[[Unpack[TS]], Unit], RuntimeFunction(self._decls, name))
-
-    def include(self, path: str) -> None:
-        """
-        Include a file of rules.
-        """
-        raise NotImplementedError(
-            "Not implemented yet, because we don't have a way of registering the types with Python"
-        )
-
-    def input(self, fn: Callable[..., String], path: str) -> None:
-        """
-        Loads a CSV file and sets it as *input, output of the function.
-        """
-        fn_name = self._decls.get_egg_fn(_resolve_callable(fn))
-        self._run_program([bindings.Input(fn_name, path)])
-
-    def output(self) -> None:
-        raise NotImplementedError("Not imeplemented yet, because there are no examples in the egglog repo")
-
-    def calc(self) -> None:
-        raise NotImplementedError("Not implemented yet")
+_BUILTIN_DECLS: Declarations | None = None
 
-    @overload
-    def run(self, limit: int, /, *until: Fact) -> bindings.RunReport:
-        ...
 
-    @overload
-    def run(self, schedule: Schedule, /) -> bindings.RunReport:
-        ...
-
-    def run(self, limit_or_schedule: int | Schedule, /, *until: Fact) -> bindings.RunReport:
-        """
-        Run the egraph until the given limit or until the given facts are true.
-        """
-        if isinstance(limit_or_schedule, int):
-            limit_or_schedule = config(limit_or_schedule, None, *until)
-        return self._run_schedule(limit_or_schedule)
-
-    def _run_schedule(self, schedule: Schedule) -> bindings.RunReport:
-        self._run_program([bindings.RunScheduleCommand(schedule._to_egg(self._decls))])
-        run_report = self._get_egraph().run_report()
-        if not run_report:
-            raise ValueError("No run report saved")
-        return run_report
-
-    def check(self, *facts: Fact) -> None:
-        """
-        Check if a fact is true in the egraph.
-        """
-        self._run_program([self._facts_to_check(facts)])
-
-    def check_fail(self, *facts) -> None:
-        """
-        Checks that one of the facts is not true
-        """
-        self._run_program([bindings.Fail(self._facts_to_check(facts))])
-
-    def _facts_to_check(self, facts: Iterable[Fact]) -> bindings.Check:
-        egg_facts = [fact_decl_to_egg(self._decls, _fact_to_decl(f)) for f in facts]
-        return bindings.Check(egg_facts)
-
-    def extract(self, expr: EXPR) -> EXPR:
-        """
-        Extract the lowest cost expression from the egraph.
-        """
-        tp, decl = expr_parts(expr)
-        egg_expr = decl.to_egg(self._decls)
-        extract_report = self._run_extract(egg_expr, 0)
-        new_tp, new_decl = tp_and_expr_decl_from_egg(self._decls, extract_report.expr)
-        if new_tp != tp:
-            raise RuntimeError(f"Type mismatch: {tp} != {new_tp}")
-        return cast(EXPR, RuntimeExpr(self._decls, tp, new_decl))
-
-    def extract_multiple(self, expr: EXPR, n: int) -> list[EXPR]:
-        """
-        Extract multiple expressions from the egraph.
-        """
-        tp, decl = expr_parts(expr)
-        egg_expr = decl.to_egg(self._decls)
-        extract_report = self._run_extract(egg_expr, n + 1)
-        new_decls = [tp_and_expr_decl_from_egg(self._decls, egg_expr)[1] for egg_expr in extract_report.variants]
-        return [cast(EXPR, RuntimeExpr(self._decls, tp, new_decl)) for new_decl in new_decls]
-
-    def _run_extract(self, expr: bindings._Expr, n: int) -> bindings.ExtractReport:
-        self._run_program([bindings.Extract(n, expr)])
-        extract_report = self._get_egraph().extract_report()
-        if not extract_report:
-            raise ValueError("No extract report saved")
-        return extract_report
-
-    def constant(self, name: str, tp: type[EXPR], egg_name: Optional[str] = None) -> EXPR:
-        """
-        Defines a named constant of a certain type.
-
-        This is the same as defining a nullary function with a high cost.
-        """
-        ref = ConstantRef(name)
-        type_ref, commands = self._register_constant(ref, tp, egg_name, None)
-        self._run_program(commands)
-        return cast(EXPR, RuntimeExpr(self._decls, type_ref, CallDecl(ref)))
-
-    def _register_constant(
-        self,
-        ref: ConstantRef | ClassVariableRef,
-        tp: object,
-        egg_name: Optional[str],
-        cls_type_and_name: Optional[tuple[type | RuntimeClass, str]],
-    ) -> tuple[JustTypeRef, Iterable[bindings._Command]]:
-        """
-        Register a constant, returning its typeref.
-        """
-        type_ref = self._resolve_type_annotation(tp, [], cls_type_and_name).to_just()
-        fn_decl = constant_function_decl(type_ref)
-        return type_ref, self._decls.register_callable(ref, fn_decl, egg_name)
-
-    def define(self, name: str, expr: EXPR) -> EXPR:
-        """
-        Define a new expression in the egraph and return a reference to it.
-        """
-        # Don't support cost and maybe will be removed in favor of let
-        # https://github.com/egraphs-good/egglog/issues/128#issuecomment-1523760578
-        tp, decl = expr_parts(expr)
-        self._run_program([bindings.Define(name, decl.to_egg(self._decls), None)])
-        return cast(EXPR, RuntimeExpr(self._decls, tp, VarDecl(name)))
+@dataclass
+class _BaseModule(ABC):
+    """
+    Base Module which provides methods to register sorts, expressions, actions etc.
 
-    def push(self) -> None:
-        """
-        Push the current state of the egraph, so that it can be popped later and reverted back.
-        """
-        self._run_program([bindings.Push(1)])
-        self._decl_stack.append(self._decls)
-        self._decls = deepcopy(self._decls)
+    Inherited by:
+    - EGraph: Holds a live EGraph instance
+    - Builtins: Stores a list of the builtins which have already been pre-regsietered
+    - Module: Stores a list of commands and additional declerations
+    """
 
-    def pop(self) -> None:
-        """
-        Pop the current state of the egraph, reverting back to the previous state.
-        """
-        self._run_program([bindings.Pop(1)])
-        self._decls = self._decl_stack.pop()
+    # Any modules you want to depend on
+    deps: InitVar[list[Module]] = []
+    # All dependencies flattened
+    _flatted_deps: list[Module] = field(init=False, default_factory=list)
+    _mod_decls: ModuleDeclarations = field(init=False)
+
+    def __post_init__(self, modules: list[Module] = []) -> None:
+        included_decls = [_BUILTIN_DECLS] if _BUILTIN_DECLS else []
+        # Traverse all the included modules to flatten all their dependencies and add to the included declerations
+        for mod in modules:
+            for child_mod in [*mod._flatted_deps, mod]:
+                if child_mod not in self._flatted_deps:
+                    self._flatted_deps.append(child_mod)
+                    included_decls.append(child_mod._mod_decls._decl)
+        self._mod_decls = ModuleDeclarations(Declarations(), included_decls)
 
-    def __enter__(self):
+    @abstractmethod
+    def _process_commands(self, cmds: Iterable[bindings._Command]) -> None:
         """
-        Copy the egraph state, so that it can be reverted back to the original state at the end.
+        Process the commands generated by this module.
         """
-        self.push()
-
-    def __exit__(self, exc_type, exc, exc_tb):
-        self.pop()
+        raise NotImplementedError
 
     @overload
     def class_(self, *, egg_sort: str) -> Callable[[TYPE], TYPE]:
         ...
 
     @overload
     def class_(self, cls: TYPE, /) -> TYPE:
@@ -333,27 +156,25 @@
         """
         cls_name = cls.__name__
         # Get all the methods from the class
         cls_dict: dict[str, Any] = {k: v for k, v in cls.__dict__.items() if k not in IGNORED_ATTRIBUTES}
         parameters: list[TypeVar] = cls_dict.pop("__parameters__", [])
 
         n_type_vars = len(parameters)
-        commands = list(self._decls.register_class(cls_name, n_type_vars, egg_sort))
+        self._process_commands(self._mod_decls.register_class(cls_name, n_type_vars, egg_sort))
         # The type ref of self is paramterized by the type vars
         slf_type_ref = TypeRefWithVars(cls_name, tuple(ClassTypeVarRef(i) for i in range(n_type_vars)))
 
         # First register any class vars as constants
         hint_globals = hint_globals.copy()
         hint_globals[cls_name] = cls
         for k, v in get_type_hints(cls, globalns=hint_globals, localns=hint_locals).items():
             if v.__origin__ == ClassVar:
                 (inner_tp,) = v.__args__
-                commands.extend(
-                    self._register_constant(ClassVariableRef(cls_name, k), inner_tp, None, (cls, cls_name))[1]
-                )
+                self._register_constant(ClassVariableRef(cls_name, k), inner_tp, None, (cls, cls_name))
             else:
                 raise NotImplementedError("The only supported annotations on class attributes are class vars")
 
         # Then register each of its methods
         for method_name, method in cls_dict.items():
             is_init = method_name == "__init__"
             # Don't register the init methods for literals, since those don't use the type checking mechanisms
@@ -372,105 +193,106 @@
             if isinstance(fn, classmethod):
                 fn = fn.__func__
                 is_classmethod = True
             else:
                 # We count __init__ as a classmethod since it is called on the class
                 is_classmethod = is_init
 
-            fn_decl = self._generate_function_decl(
+            ref: ClassMethodRef | MethodRef = (
+                ClassMethodRef(cls_name, method_name) if is_classmethod else MethodRef(cls_name, method_name)
+            )
+            self._register_function(
+                ref,
+                egg_fn,
                 fn,
                 hint_locals,
                 default,
                 cost,
                 merge,
                 on_merge,
                 "cls" if is_classmethod and not is_init else slf_type_ref,
                 parameters,
                 is_init,
                 # If this is an i64, use the runtime class for the alias so that i64Like is resolved properly
                 # Otherwise, this might be a Map in which case pass in the original cls so that we
                 # can do Map[T, V] on it, which is not allowed on the runtime class
-                cls_type_and_name=(RuntimeClass(self._decls, "i64") if cls_name == "i64" else cls, cls_name),
-            )
-            ref: ClassMethodRef | MethodRef = (
-                ClassMethodRef(cls_name, method_name) if is_classmethod else MethodRef(cls_name, method_name)
-            )
-            commands.extend(
-                self._decls.register_callable(ref, fn_decl, egg_fn, generate_commands=self._egraph is not None)
+                cls_type_and_name=(
+                    RuntimeClass(self._mod_decls, cls_name) if cls_name in {"i64", "String"} else cls,
+                    cls_name,
+                ),
             )
 
-        self._run_program(commands)
         # Register != as a method so we can print it as a string
-        self._decls.register_callable_ref(MethodRef(cls_name, "__ne__"), "!=")
-        return RuntimeClass(self._decls, cls_name)
+        self._mod_decls._decl.register_callable_ref(MethodRef(cls_name, "__ne__"), "!=")
+        return RuntimeClass(self._mod_decls, cls_name)
 
     # We seperate the function and method overloads to make it simpler to know if we are modifying a function or method,
     # So that we can add the functions eagerly to the registry and wait on the methods till we process the class.
 
     # We have to seperate method/function overloads for those that use the T params and those that don't
     # Otherwise, if you say just pass in `cost` then the T param is inferred as `Nothing` and
     # It will break the typing.
     @overload
     def method(  # type: ignore
         self,
         *,
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         merge: Optional[Callable[[Any, Any], Any]] = None,
-        on_merge: Optional[Callable[[Any, Any], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[Any, Any], Iterable[ActionLike]]] = None,
     ) -> Callable[[CALLABLE], CALLABLE]:
         ...
 
     @overload
     def method(
         self,
         *,
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         default: Optional[EXPR] = None,
         merge: Optional[Callable[[EXPR, EXPR], EXPR]] = None,
-        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[ActionLike]]] = None,
     ) -> Callable[[Callable[P, EXPR]], Callable[P, EXPR]]:
         ...
 
     def method(
         self,
         *,
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         default: Optional[EXPR] = None,
         merge: Optional[Callable[[EXPR, EXPR], EXPR]] = None,
-        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[ActionLike]]] = None,
     ) -> Callable[[Callable[P, EXPR]], Callable[P, EXPR]]:
         return lambda fn: _WrappedMethod(egg_fn, cost, default, merge, on_merge, fn)
 
     @overload
     def function(self, fn: CALLABLE, /) -> CALLABLE:
         ...
 
     @overload
     def function(  # type: ignore
         self,
         *,
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         merge: Optional[Callable[[Any, Any], Any]] = None,
-        on_merge: Optional[Callable[[Any, Any], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[Any, Any], Iterable[ActionLike]]] = None,
     ) -> Callable[[CALLABLE], CALLABLE]:
         ...
 
     @overload
     def function(
         self,
         *,
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         default: Optional[EXPR] = None,
         merge: Optional[Callable[[EXPR, EXPR], EXPR]] = None,
-        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[EXPR, EXPR], Iterable[ActionLike]]] = None,
     ) -> Callable[[Callable[P, EXPR]], Callable[P, EXPR]]:
         ...
 
     def function(self, *args, **kwargs) -> Any:
         """
         Registers a function.
         """
@@ -487,43 +309,43 @@
         self,
         fn: Callable[..., RuntimeExpr],
         hint_locals: dict[str, Any],
         egg_fn: Optional[str] = None,
         cost: Optional[int] = None,
         default: Optional[RuntimeExpr] = None,
         merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], RuntimeExpr]] = None,
-        on_merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], Iterable[Action]]] = None,
+        on_merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], Iterable[ActionLike]]] = None,
     ) -> RuntimeFunction:
         """
         Uncurried version of function decorator
         """
         name = fn.__name__
         # Save function decleartion
-        fn_decl = self._generate_function_decl(fn, hint_locals, default, cost, merge, on_merge)
-        commands = self._decls.register_callable(FunctionRef(name), fn_decl, egg_fn)
-        self._run_program(commands)
+        self._register_function(FunctionRef(name), egg_fn, fn, hint_locals, default, cost, merge, on_merge)
         # Return a runtime function which will act like the decleration
-        return RuntimeFunction(self._decls, name)
+        return RuntimeFunction(self._mod_decls, name)
 
-    def _generate_function_decl(
+    def _register_function(
         self,
+        ref: FunctionCallableRef,
+        egg_name: Optional[str],
         fn: Any,
         # Pass in the locals, retrieved from the frame when wrapping,
         # so that we support classes and function defined inside of other functions (which won't show up in the globals)
         hint_locals: dict[str, Any],
         default: Optional[RuntimeExpr],
         cost: Optional[int],
         merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], RuntimeExpr]],
-        on_merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], Iterable[Action]]],
+        on_merge: Optional[Callable[[RuntimeExpr, RuntimeExpr], Iterable[ActionLike]]],
         # The first arg is either cls, for a classmethod, a self type, or none for a function
         first_arg: Literal["cls"] | TypeOrVarRef | None = None,
         cls_typevars: list[TypeVar] = [],
         is_init: bool = False,
         cls_type_and_name: Optional[tuple[type | RuntimeClass, str]] = None,
-    ) -> FunctionDecl:
+    ) -> None:
         if not isinstance(fn, FunctionType):
             raise NotImplementedError(f"Can only generate function decls for functions not {fn}  {type(fn)}")
 
         hint_globals = fn.__globals__.copy()
 
         if cls_type_and_name:
             hint_globals[cls_type_and_name[1]] = cls_type_and_name[0]
@@ -539,54 +361,60 @@
         params = list(signature(fn).parameters.values())
         # Remove first arg if this is a classmethod or a method, since it won't have an annotation
         if first_arg is not None:
             first, *params = params
             if first.annotation != Parameter.empty:
                 raise ValueError(f"First arg of a method must not have an annotation, not {first.annotation}")
 
+        # Check that all the params are positional or keyword, and that there is only one var arg at the end
+        found_var_arg = False
         for param in params:
-            if param.kind != Parameter.POSITIONAL_OR_KEYWORD:
+            if found_var_arg:
+                raise ValueError("Can only have a single var arg at the end")
+            kind = param.kind
+            if kind == Parameter.VAR_POSITIONAL:
+                found_var_arg = True
+            elif kind != Parameter.POSITIONAL_OR_KEYWORD:
                 raise ValueError(f"Can only register functions with positional or keyword args, not {param.kind}")
 
+        if found_var_arg:
+            var_arg_param, *params = params
+            var_arg_type = self._resolve_type_annotation(hints[var_arg_param.name], cls_typevars, cls_type_and_name)
+        else:
+            var_arg_type = None
         arg_types = tuple(self._resolve_type_annotation(hints[t.name], cls_typevars, cls_type_and_name) for t in params)
         # If the first arg is a self, and this not an __init__ fn, add this as a typeref
         if isinstance(first_arg, (ClassTypeVarRef, TypeRefWithVars)) and not is_init:
             arg_types = (first_arg,) + arg_types
 
-        default_decl = None if default is None else default.__egg_expr__
+        default_decl = None if default is None else default.__egg_typed_expr__.expr
         merge_decl = (
             None
             if merge is None
             else merge(
-                RuntimeExpr(self._decls, return_type.to_just(), VarDecl("old")),
-                RuntimeExpr(self._decls, return_type.to_just(), VarDecl("new")),
-            ).__egg_expr__
+                RuntimeExpr(self._mod_decls, TypedExprDecl(return_type.to_just(), VarDecl("old"))),
+                RuntimeExpr(self._mod_decls, TypedExprDecl(return_type.to_just(), VarDecl("new"))),
+            ).__egg_typed_expr__.expr
         )
         merge_action = (
-            ()
+            []
             if on_merge is None
-            else tuple(
-                map(
-                    _action_to_decl,
-                    on_merge(
-                        RuntimeExpr(self._decls, return_type.to_just(), VarDecl("old")),
-                        RuntimeExpr(self._decls, return_type.to_just(), VarDecl("new")),
-                    ),
+            else _action_likes(
+                on_merge(
+                    RuntimeExpr(self._mod_decls, TypedExprDecl(return_type.to_just(), VarDecl("old"))),
+                    RuntimeExpr(self._mod_decls, TypedExprDecl(return_type.to_just(), VarDecl("new"))),
                 )
             )
         )
-        decl = FunctionDecl(
-            return_type=return_type,
-            arg_types=arg_types,
-            cost=cost,
-            default=default_decl,
-            merge=merge_decl,
-            merge_action=merge_action,
+        fn_decl = FunctionDecl(return_type=return_type, var_arg_type=var_arg_type, arg_types=arg_types)
+        self._process_commands(
+            self._mod_decls.register_function_callable(
+                ref, fn_decl, egg_name, cost, default_decl, merge_decl, merge_action
+            )
         )
-        return decl
 
     def _resolve_type_annotation(
         self,
         tp: object,
         cls_typevars: list[TypeVar],
         cls_type_and_name: Optional[tuple[type | RuntimeClass, str]],
     ) -> TypeOrVarRef:
@@ -622,58 +450,322 @@
                 ),
             )
 
         if isinstance(tp, (RuntimeClass, RuntimeParamaterizedClass)):
             return class_to_ref(tp).to_var()
         raise TypeError(f"Unexpected type annotation {tp}")
 
-    def register(self, *values: Rewrite | Birewrite | Rule | Action) -> None:
+    def register(self, command_or_generator: CommandLike | CommandGenerator, *commands: CommandLike) -> None:
         """
         Registers any number of rewrites or rules.
         """
-        self._run_program(_value_to_command(self._decls, v, ruleset="") for v in values)
+        if isinstance(command_or_generator, FunctionType):
+            assert not commands
+            commands = tuple(_command_generator(command_or_generator))
+        else:
+            commands = (cast(CommandLike, command_or_generator), *commands)
+        self._process_commands(_command_like(command)._to_egg_command(self._mod_decls) for command in commands)
 
     def ruleset(self, name: str) -> Ruleset:
-        self._run_program([bindings.AddRuleset(name)])
-        return Ruleset(self, name)
+        self._process_commands([bindings.AddRuleset(name)])
+        return Ruleset(name)
+
+    # Overload to support aritys 0-4 until variadic generic support map, so we can map from type to value
+    @overload
+    def relation(
+        self, name: str, tp1: type[E1], tp2: type[E2], tp3: type[E3], tp4: type[E4], /
+    ) -> Callable[[E1, E2, E3, E4], Unit]:
+        ...
+
+    @overload
+    def relation(self, name: str, tp1: type[E1], tp2: type[E2], tp3: type[E3], /) -> Callable[[E1, E2, E3], Unit]:
+        ...
+
+    @overload
+    def relation(self, name: str, tp1: type[E1], tp2: type[E2], /) -> Callable[[E1, E2], Unit]:
+        ...
+
+    @overload
+    def relation(self, name: str, tp1: type[T], /, *, egg_fn: Optional[str] = None) -> Callable[[T], Unit]:
+        ...
+
+    @overload
+    def relation(self, name: str, /, *, egg_fn: Optional[str] = None) -> Callable[[], Unit]:
+        ...
+
+    def relation(self, name: str, /, *tps: type, egg_fn: Optional[str] = None) -> Callable[..., Unit]:
+        """
+        Defines a relation, which is the same as a function which returns unit.
+        """
+        arg_types = tuple(self._resolve_type_annotation(cast(object, tp), [], None) for tp in tps)
+        fn_decl = FunctionDecl(arg_types, TypeRefWithVars("Unit"))
+        commands = self._mod_decls.register_function_callable(
+            FunctionRef(name), fn_decl, egg_fn, cost=None, default=None, merge=None, merge_action=[]
+        )
+        self._process_commands(commands)
+        return cast(Callable[..., Unit], RuntimeFunction(self._mod_decls, name))
+
+    def input(self, fn: Callable[..., String], path: str) -> None:
+        """
+        Loads a CSV file and sets it as *input, output of the function.
+        """
+        fn_name = self._mod_decls.get_egg_fn(_resolve_callable(fn))
+        self._process_commands([bindings.Input(fn_name, path)])
+
+    def constant(self, name: str, tp: type[EXPR], egg_name: Optional[str] = None) -> EXPR:
+        """
+        Defines a named constant of a certain type.
+
+        This is the same as defining a nullary function with a high cost.
+        """
+        ref = ConstantRef(name)
+        type_ref = self._register_constant(ref, tp, egg_name, None)
+        return cast(EXPR, RuntimeExpr(self._mod_decls, TypedExprDecl(type_ref, CallDecl(ref))))
+
+    def _register_constant(
+        self,
+        ref: ConstantRef | ClassVariableRef,
+        tp: object,
+        egg_name: Optional[str],
+        cls_type_and_name: Optional[tuple[type | RuntimeClass, str]],
+    ) -> JustTypeRef:
+        """
+        Register a constant, returning its typeref().
+        """
+        type_ref = self._resolve_type_annotation(tp, [], cls_type_and_name).to_just()
+        self._process_commands(self._mod_decls.register_constant_callable(ref, type_ref, egg_name))
+        return type_ref
+
+    def define(self, name: str, expr: EXPR) -> EXPR:
+        """
+        Define a new expression in the egraph and return a reference to it.
+        """
+        # Don't support cost and maybe will be removed in favor of let
+        # https://github.com/egraphs-good/egglog/issues/128#issuecomment-1523760578
+        typed_expr = expr_parts(expr)
+        self._process_commands([bindings.Define(name, typed_expr.to_egg(self._mod_decls), None)])
+        return cast(EXPR, RuntimeExpr(self._mod_decls, TypedExprDecl(typed_expr.tp, VarDecl(name))))
+
+
+@dataclass
+class _Builtins(_BaseModule):
+    def __post_init__(self, modules: list[Module] = []) -> None:
+        """
+        Register these declarations as builtins, so others can use them.
+        """
+        assert not modules
+        super().__post_init__(modules)
+        global _BUILTIN_DECLS
+        if _BUILTIN_DECLS is not None:
+            raise RuntimeError("Builtins already initialized")
+        _BUILTIN_DECLS = self._mod_decls._decl
+
+    def _process_commands(self, cmds: Iterable[bindings._Command]) -> None:
+        """
+        Commands which would have been used to create the builtins are discarded, since they are already registered.
+        """
+        pass
+
+
+@dataclass
+class Module(_BaseModule):
+    _cmds: list[bindings._Command] = field(default_factory=list, repr=False)
+
+    def _process_commands(self, cmds: Iterable[bindings._Command]) -> None:
+        self._cmds.extend(cmds)
+
+
+@dataclass
+class EGraph(_BaseModule):
+    """
+    Represents an EGraph instance at runtime
+    """
 
+    _egraph: bindings.EGraph = field(repr=False, default_factory=bindings.EGraph)
+    # The current declarations which have been pushed to the stack
+    _decl_stack: list[Declarations] = field(default_factory=list, repr=False)
+
+    def __post_init__(self, modules: list[Module] = []) -> None:
+        super().__post_init__(modules)
+        for m in self._flatted_deps:
+            self._process_commands(m._cmds)
+
+    def _process_commands(self, commands: Iterable[bindings._Command]) -> None:
+        self._egraph.run_program(*commands)
+
+    def _repr_mimebundle_(self, *args, **kwargs):
+        """
+        Returns the graphviz representation of the e-graph.
+        """
+
+        return self.graphviz._repr_mimebundle_(*args, **kwargs)
+
+    @property
+    def graphviz(self) -> graphviz.Source:
+        return graphviz.Source(self._egraph.to_graphviz_string())
+
+    def _repr_html_(self) -> str:
+        """
+        Add a _repr_html_ to be an SVG to work with sphinx gallery
+        ala https://github.com/xflr6/graphviz/pull/121
+        until this PR is merged and released
+        https://github.com/sphinx-gallery/sphinx-gallery/pull/1138
+        """
+        return self.graphviz.pipe(format="svg").decode()
+
+    def display(self):
+        """
+        Displays the e-graph in the notebook.
+        """
+        from IPython.display import display
+
+        display(self)
+
+    def simplify(self, expr: EXPR, limit: int, *until: Fact, ruleset: Optional[Ruleset] = None) -> EXPR:
+        """
+        Simplifies the given expression.
+        """
+        typed_expr = expr_parts(expr)
+        egg_expr = typed_expr.to_egg(self._mod_decls)
+        self._process_commands(
+            [bindings.Simplify(egg_expr, Run(limit, _ruleset_name(ruleset), until)._to_egg_config(self._mod_decls))]
+        )
+        extract_report = self._egraph.extract_report()
+        if not extract_report:
+            raise ValueError("No extract report saved")
+        new_typed_expr = TypedExprDecl.from_egg(self._mod_decls, extract_report.expr)
+        return cast(EXPR, RuntimeExpr(self._mod_decls, new_typed_expr))
+
+    def include(self, path: str) -> None:
+        """
+        Include a file of rules.
+        """
+        raise NotImplementedError(
+            "Not implemented yet, because we don't have a way of registering the types with Python"
+        )
+
+    def output(self) -> None:
+        raise NotImplementedError("Not imeplemented yet, because there are no examples in the egglog repo")
+
+    @overload
+    def run(self, limit: int, /, *until: Fact, ruleset: Optional[Ruleset] = None) -> bindings.RunReport:
+        ...
+
+    @overload
+    def run(self, schedule: Schedule, /) -> bindings.RunReport:
+        ...
 
-def _value_to_command(
-    decls: Declarations, value: Rewrite | Birewrite | Rule | Action, ruleset: str
-) -> bindings._Command:
-    if isinstance(value, Rewrite):
-        return bindings.RewriteCommand(ruleset, value._to_decl().to_egg(decls))
-    if isinstance(value, Birewrite):
-        return bindings.BiRewriteCommand(ruleset, value._to_decl().to_egg(decls))
-    if isinstance(value, Rule):
-        return bindings.RuleCommand(value.name or "", ruleset, value._to_decl().to_egg(decls))
-    return bindings.ActionCommand(action_decl_to_egg(decls, _action_to_decl(value)))
+    def run(
+        self, limit_or_schedule: int | Schedule, /, *until: Fact, ruleset: Optional[Ruleset] = None
+    ) -> bindings.RunReport:
+        """
+        Run the egraph until the given limit or until the given facts are true.
+        """
+        if isinstance(limit_or_schedule, int):
+            limit_or_schedule = run(ruleset, limit_or_schedule, *until)
+        return self._run_schedule(limit_or_schedule)
+
+    def _run_schedule(self, schedule: Schedule) -> bindings.RunReport:
+        self._process_commands([bindings.RunScheduleCommand(schedule._to_egg_schedule(self._mod_decls))])
+        run_report = self._egraph.run_report()
+        if not run_report:
+            raise ValueError("No run report saved")
+        return run_report
+
+    def check(self, *facts: FactLike) -> None:
+        """
+        Check if a fact is true in the egraph.
+        """
+        self._process_commands([self._facts_to_check(facts)])
+
+    def check_fail(self, *facts: FactLike) -> None:
+        """
+        Checks that one of the facts is not true
+        """
+        self._process_commands([bindings.Fail(self._facts_to_check(facts))])
+
+    def _facts_to_check(self, facts: Iterable[FactLike]) -> bindings.Check:
+        egg_facts = [f._to_egg_fact(self._mod_decls) for f in _fact_likes(facts)]
+        return bindings.Check(egg_facts)
+
+    def extract(self, expr: EXPR) -> EXPR:
+        """
+        Extract the lowest cost expression from the egraph.
+        """
+        typed_expr = expr_parts(expr)
+        egg_expr = typed_expr.to_egg(self._mod_decls)
+        extract_report = self._run_extract(egg_expr, 0)
+        new_typed_expr = TypedExprDecl.from_egg(self._mod_decls, extract_report.expr)
+        if new_typed_expr.tp != typed_expr.tp:
+            raise RuntimeError(f"Type mismatch: {new_typed_expr.tp} != {typed_expr.tp}")
+        return cast(EXPR, RuntimeExpr(self._mod_decls, new_typed_expr))
+
+    def extract_multiple(self, expr: EXPR, n: int) -> list[EXPR]:
+        """
+        Extract multiple expressions from the egraph.
+        """
+        typed_expr = expr_parts(expr)
+        egg_expr = typed_expr.to_egg(self._mod_decls)
+        extract_report = self._run_extract(egg_expr, n)
+        new_exprs = [TypedExprDecl.from_egg(self._mod_decls, egg_expr) for egg_expr in extract_report.variants]
+        return [cast(EXPR, RuntimeExpr(self._mod_decls, expr)) for expr in new_exprs]
+
+    def _run_extract(self, expr: bindings._Expr, n: int) -> bindings.ExtractReport:
+        self._process_commands([bindings.Extract(n, expr)])
+        extract_report = self._egraph.extract_report()
+        if not extract_report:
+            raise ValueError("No extract report saved")
+        return extract_report
+
+    def push(self) -> None:
+        """
+        Push the current state of the egraph, so that it can be popped later and reverted back.
+        """
+        self._process_commands([bindings.Push(1)])
+        self._decl_stack.append(self._mod_decls._decl)
+        self._decls = deepcopy(self._mod_decls._decl)
+
+    def pop(self) -> None:
+        """
+        Pop the current state of the egraph, reverting back to the previous state.
+        """
+        self._process_commands([bindings.Pop(1)])
+        self._mod_decls._decl = self._decl_stack.pop()
+
+    def __enter__(self):
+        """
+        Copy the egraph state, so that it can be reverted back to the original state at the end.
+        """
+        self.push()
+
+    def __exit__(self, exc_type, exc, exc_tb):
+        self.pop()
 
 
 @dataclass(frozen=True)
 class _WrappedMethod(Generic[P, EXPR]):
     """
-    Used to wrap a method and store some extra options on it before processing it.
+    Used to wrap a method and store some extra options on it before processing it when processing the class.
     """
 
     egg_fn: Optional[str]
     cost: Optional[int]
     default: Optional[EXPR]
     merge: Optional[Callable[[EXPR, EXPR], EXPR]]
-    on_merge: Optional[Callable[[EXPR, EXPR], Iterable[Action]]]
+    on_merge: Optional[Callable[[EXPR, EXPR], Iterable[ActionLike]]]
     fn: Callable[P, EXPR]
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> EXPR:
         raise NotImplementedError("We should never call a wrapped method. Did you forget to wrap the class?")
 
 
 class _BaseExprMetaclass(type):
     """
     Metaclass of BaseExpr, used to override isistance checks, so that runtime expressions are instances
-    of BaseExpr at runtime, so this matches the intuition.
+    of BaseExpr at runtime.
     """
 
     def __instancecheck__(self, instance: object) -> bool:
         return isinstance(instance, RuntimeExpr)
 
 
 class BaseExpr(metaclass=_BaseExprMetaclass):
@@ -695,423 +787,255 @@
         """
         Equality is currently not supported. We only add this method so that
         if you try to use it MyPy will warn you.
         """
         ...
 
 
-BUILTINS = EGraph(_for_builtins=True)
+BUILTINS = _Builtins()
 
 
 @BUILTINS.class_(egg_sort="Unit")
 class Unit(BaseExpr):
     """
     The unit type. This is also used to reprsent if a value exists, if it is resolved or not.
     """
 
     def __init__(self) -> None:
         ...
 
 
 @dataclass(frozen=True)
 class Ruleset:
-    _egraph: EGraph = field(repr=False)
     name: str
 
-    def register(self, *values: Rewrite | Birewrite | Rule) -> None:
-        """
-        Registers any number of rewrites or rules.
-        """
-        self._egraph._run_program(_value_to_command(self._egraph._decls, v, ruleset=self.name) for v in values)
-
-    def run(self, limit: int, *until: Fact) -> bindings.RunReport:
-        """
-        Run the e-graph with this ruleset.
-        """
-        return self._egraph._run_schedule(config(limit, self, *until))
 
-    def simplify(self, expr: EXPR, limit: int, *until: Fact) -> EXPR:
-        """
-        Simplify the given expression with this ruleset.
-        """
-        return self._egraph._simplify(expr, limit, self, until)
+def _ruleset_name(ruleset: Optional[Ruleset]) -> str:
+    return ruleset.name if ruleset else ""
 
 
 # We use these builders so that when creating these structures we can type check
 # if the arguments are the same type of expression
 
 
-def rewrite(lhs: EXPR) -> _RewriteBuilder[EXPR]:
+def rewrite(lhs: EXPR, ruleset: Optional[Ruleset] = None) -> _RewriteBuilder[EXPR]:
     """Rewrite the given expression to a new expression."""
-    return _RewriteBuilder(lhs=lhs)
+    return _RewriteBuilder(lhs, ruleset)
 
 
-def birewrite(lhs: EXPR) -> _BirewriteBuilder[EXPR]:
+def birewrite(lhs: EXPR, ruleset: Optional[Ruleset] = None) -> _BirewriteBuilder[EXPR]:
     """Rewrite the given expression to a new expression and vice versa."""
-    return _BirewriteBuilder(lhs=lhs)
+    return _BirewriteBuilder(lhs, ruleset)
 
 
 def eq(expr: EXPR) -> _EqBuilder[EXPR]:
     """Check if the given expression is equal to the given value."""
     return _EqBuilder(expr)
 
 
-def panic(message: str) -> Panic:
+def panic(message: str) -> Action:
     """Raise an error with the given message."""
     return Panic(message)
 
 
-def let(name: str, expr: BaseExpr) -> Let:
+def let(name: str, expr: BaseExpr) -> Action:
     """Create a let binding."""
-    return Let(name, expr)
+    return Let(name, expr_parts(expr).expr)
+
 
+def expr_action(expr: BaseExpr) -> Action:
+    typed_expr = expr_parts(expr)
+    return ExprAction(typed_expr.expr)
 
-def delete(expr: BaseExpr) -> Delete:
+
+def delete(expr: BaseExpr) -> Action:
     """Create a delete expression."""
-    return Delete(expr)
+    decl = expr_parts(expr).expr
+    if not isinstance(decl, CallDecl):
+        raise ValueError(f"Can only delete calls not {decl}")
+    return Delete(decl)
+
+
+def expr_fact(expr: BaseExpr) -> Fact:
+    return ExprFact(expr_parts(expr).expr)
 
 
 def union(lhs: EXPR) -> _UnionBuilder[EXPR]:
     """Create a union of the given expression."""
     return _UnionBuilder(lhs=lhs)
 
 
 def set_(lhs: EXPR) -> _SetBuilder[EXPR]:
     """Create a set of the given expression."""
     return _SetBuilder(lhs=lhs)
 
 
-def rule(*facts: Fact, name: Optional[str] = None) -> _RuleBuilder:
+def rule(*facts: FactLike, ruleset: Optional[Ruleset] = None, name: Optional[str] = None) -> _RuleBuilder:
     """Create a rule with the given facts."""
-    return _RuleBuilder(facts=facts, name=name)
+    return _RuleBuilder(facts=_fact_likes(facts), name=name, ruleset=ruleset)
 
 
 def var(name: str, bound: type[EXPR]) -> EXPR:
     """Create a new variable with the given name and type."""
     return cast(EXPR, _var(name, bound))
 
 
 def _var(name: str, bound: Any) -> RuntimeExpr:
     """Create a new variable with the given name and type."""
     if not isinstance(bound, (RuntimeClass, RuntimeParamaterizedClass)):
         raise TypeError(f"Unexpected type {type(bound)}")
-    return RuntimeExpr(bound.__egg_decls__, class_to_ref(bound), VarDecl(name))
+    return RuntimeExpr(bound.__egg_decls__, TypedExprDecl(class_to_ref(bound), VarDecl(name)))
 
 
 def vars_(names: str, bound: type[EXPR]) -> Iterable[EXPR]:
     """Create variables with the given names and type."""
     for name in names.split(" "):
         yield var(name, bound)
 
 
 @dataclass
 class _RewriteBuilder(Generic[EXPR]):
     lhs: EXPR
+    ruleset: Optional[Ruleset]
 
-    def to(self, rhs: EXPR, *conditions: Fact) -> Rewrite:
-        return Rewrite(lhs=self.lhs, rhs=rhs, conditions=list(conditions))
+    def to(self, rhs: EXPR, *conditions: FactLike) -> Command:
+        return Rewrite(
+            _ruleset_name(self.ruleset),
+            expr_parts(self.lhs).expr,
+            expr_parts(rhs).expr,
+            _fact_likes(conditions),
+        )
 
     def __str__(self) -> str:
         return f"rewrite({self.lhs})"
 
 
 @dataclass
 class _BirewriteBuilder(Generic[EXPR]):
     lhs: EXPR
+    ruleset: Optional[Ruleset]
 
-    def to(self, rhs: EXPR, *conditions: Fact) -> Birewrite:
-        return Birewrite(lhs=self.lhs, rhs=rhs, conditions=list(conditions))
+    def to(self, rhs: EXPR, *conditions: FactLike) -> Command:
+        return BiRewrite(
+            _ruleset_name(self.ruleset),
+            expr_parts(self.lhs).expr,
+            expr_parts(rhs).expr,
+            _fact_likes(conditions),
+        )
 
     def __str__(self) -> str:
         return f"birewrite({self.lhs})"
 
 
 @dataclass
 class _EqBuilder(Generic[EXPR]):
-    expr: BaseExpr
+    expr: EXPR
 
-    def to(self, *exprs: EXPR) -> Eq:
-        return Eq([self.expr, *exprs])
+    def to(self, *exprs: EXPR) -> Fact:
+        return Eq(tuple(expr_parts(e).expr for e in (self.expr, *exprs)))
 
     def __str__(self) -> str:
         return f"eq({self.expr})"
 
 
 @dataclass
 class _SetBuilder(Generic[EXPR]):
     lhs: BaseExpr
 
-    def to(self, rhs: EXPR) -> Set:
-        return Set(lhs=self.lhs, rhs=rhs)
+    def to(self, rhs: EXPR) -> Action:
+        lhs = expr_parts(self.lhs).expr
+        if not isinstance(lhs, CallDecl):
+            raise ValueError(f"Can only create a call with a call for the lhs, got {lhs}")
+        return Set(lhs, expr_parts(rhs).expr)
 
     def __str__(self) -> str:
         return f"set_({self.lhs})"
 
 
 @dataclass
 class _UnionBuilder(Generic[EXPR]):
     lhs: BaseExpr
 
-    def with_(self, rhs: EXPR) -> Union_:
-        return Union_(lhs=self.lhs, rhs=rhs)
+    def with_(self, rhs: EXPR) -> Action:
+        return Union_(expr_parts(self.lhs).expr, expr_parts(rhs).expr)
 
     def __str__(self) -> str:
         return f"union({self.lhs})"
 
 
 @dataclass
 class _RuleBuilder:
     facts: tuple[Fact, ...]
     name: Optional[str]
+    ruleset: Optional[Ruleset]
 
-    def then(self, *actions: Action) -> Rule:
-        return Rule(actions, self.facts, self.name)
+    def then(self, *actions: ActionLike) -> Command:
+        return Rule(_action_likes(actions), self.facts, self.name or "", _ruleset_name(self.ruleset))
 
 
-def expr_parts(expr: BaseExpr) -> tuple[JustTypeRef, ExprDecl]:
+def expr_parts(expr: BaseExpr) -> TypedExprDecl:
     """
     Returns the underlying type and decleration of the expression. Useful for testing structural equality or debugging.
-
-    :rtype: tuple[object, object]
     """
     assert isinstance(expr, RuntimeExpr)
-    return expr.__egg_parts__
-
-
-@dataclass
-class Rewrite:
-    lhs: BaseExpr
-    rhs: BaseExpr
-    conditions: list[Fact]
-
-    def __str__(self) -> str:
-        args_str = ", ".join(map(str, [self.rhs, *self.conditions]))
-        return f"rewrite({self.lhs}).to({args_str})"
-
-    def _to_decl(self) -> RewriteDecl:
-        return RewriteDecl(
-            expr_parts(self.lhs)[1],
-            expr_parts(self.rhs)[1],
-            tuple(_fact_to_decl(fact) for fact in self.conditions),
-        )
-
-
-@dataclass
-class Birewrite:
-    lhs: BaseExpr
-    rhs: BaseExpr
-    conditions: list[Fact]
-
-    def __str__(self) -> str:
-        args_str = ", ".join(map(str, [self.rhs, *self.conditions]))
-        return f"birewrite({self.lhs}).to({args_str})"
-
-    def _to_decl(self) -> RewriteDecl:
-        return RewriteDecl(
-            expr_parts(self.lhs)[1],
-            expr_parts(self.rhs)[1],
-            tuple(_fact_to_decl(fact) for fact in self.conditions),
-        )
-
-
-@dataclass
-class Eq:
-    exprs: list[BaseExpr]
-
-    def __str__(self) -> str:
-        first, *rest = self.exprs
-        args_str = ", ".join(map(str, rest))
-        return f"eq({first}).to({args_str})"
-
-    def _to_decl(self) -> EqDecl:
-        return EqDecl(tuple(expr_parts(expr)[1] for expr in self.exprs))
-
-
-Fact = Union[Unit, Eq]
-
-
-def _fact_to_decl(fact: Fact) -> FactDecl:
-    if isinstance(fact, Eq):
-        return fact._to_decl()
-    elif isinstance(fact, BaseExpr):
-        return expr_parts(fact)[1]
-    assert_never(fact)
+    return expr.__egg_typed_expr__
 
 
-@dataclass
-class Delete:
-    expr: BaseExpr
-
-    def __str__(self) -> str:
-        return f"delete({self.expr})"
-
-    def _to_decl(self) -> DeleteDecl:
-        decl = expr_parts(self.expr)[1]
-        if not isinstance(decl, CallDecl):
-            raise ValueError(f"Can only delete calls not {decl}")
-        return DeleteDecl(decl)
-
-
-@dataclass
-class Panic:
-    message: str
-
-    def __str__(self) -> str:
-        return f"panic({self.message})"
-
-    def _to_decl(self) -> PanicDecl:
-        return PanicDecl(self.message)
-
-
-@dataclass
-class Union_:
-    lhs: BaseExpr
-    rhs: BaseExpr
-
-    def __str__(self) -> str:
-        return f"union({self.lhs}).with_({self.rhs})"
-
-    def _to_decl(self) -> UnionDecl:
-        return UnionDecl(expr_parts(self.lhs)[1], expr_parts(self.rhs)[1])
-
-
-@dataclass
-class Set:
-    lhs: BaseExpr
-    rhs: BaseExpr
-
-    def __str__(self) -> str:
-        return f"set_({self.lhs}).to({self.rhs})"
-
-    def _to_decl(self) -> SetDecl:
-        lhs = expr_parts(self.lhs)[1]
-        if not isinstance(lhs, CallDecl):
-            raise ValueError(f"Can only create a call with a call for the lhs, got {lhs}")
-        return SetDecl(lhs, expr_parts(self.rhs)[1])
-
-
-@dataclass
-class Let:
-    name: str
-    value: BaseExpr
-
-    def __str__(self) -> str:
-        return f"let({self.name}, {self.value})"
-
-    def _to_decl(self) -> LetDecl:
-        return LetDecl(self.name, expr_parts(self.value)[1])
-
-
-Action = Union[Let, Set, Delete, Union_, Panic, "BaseExpr"]
-
-
-def _action_to_decl(action: Action) -> ActionDecl:
-    if isinstance(action, BaseExpr):
-        return expr_parts(action)[1]
-    return action._to_decl()
-
-
-@dataclass
-class Rule:
-    header: tuple[Action, ...]
-    body: tuple[Fact, ...]
-    name: Optional[str]
-
-    def _to_decl(self) -> RuleDecl:
-        return RuleDecl(
-            tuple(_action_to_decl(action) for action in self.header),
-            tuple(_fact_to_decl(fact) for fact in self.body),
-        )
-
-
-def config(limit: int, ruleset: Optional[Ruleset] = None, *until: Fact) -> Config:
+def run(ruleset: Optional[Ruleset] = None, limit: int = 1, *until: Fact) -> Run:
     """
     Create a run configuration.
     """
-    return Config(limit, ruleset, tuple(until))
+    return Run(limit, _ruleset_name(ruleset), tuple(until))
 
 
-def sequence(*schedules: Schedule) -> Schedule:
+def seq(*schedules: Schedule) -> Schedule:
     """
     Run a sequence of schedules.
     """
     return Sequence(tuple(schedules))
 
 
-class _BaseSchedule:
-    def __mul__(self, length: int) -> Schedule:
-        """
-        Repeat the schedule a number of times.
-        """
-        if not isinstance(self, (Config, Repeat, Saturate, Sequence)):
-            raise TypeError(f"Cannot multiply {type(self)}")
-        return Repeat(length, self)
+CommandLike = Union[Command, BaseExpr]
 
-    def saturate(self) -> Schedule:
-        """
-        Run the schedule until the e-graph is saturated.
-        """
-        if not isinstance(self, (Config, Repeat, Saturate, Sequence)):
-            raise TypeError(f"Cannot saturate {type(self)}")
-        return Saturate(self)
 
+def _command_like(command_like: CommandLike) -> Command:
+    if isinstance(command_like, BaseExpr):
+        return expr_action(command_like)
+    return command_like
 
-@dataclass
-class Config(_BaseSchedule):
-    """Configuration of a run"""
 
-    limit: int
-    ruleset: Optional[Ruleset]
-    until: tuple[Fact, ...] = field(default_factory=tuple)
+CommandGenerator = Callable[..., Iterable[Command]]
 
-    def __str__(self) -> str:
-        args_str = ", ".join(map(str, [self.limit, self.ruleset, *self.until]))
-        return f"config({args_str})"
 
-    def _to_egg(self, decls: Declarations) -> bindings._Schedule:
-        return bindings.Run(self._to_egg_config(decls))
-
-    def _to_egg_config(self, decls: Declarations) -> bindings.RunConfig:
-        return bindings.RunConfig(
-            self.ruleset.name if self.ruleset else "",
-            self.limit,
-            [fact_decl_to_egg(decls, _fact_to_decl(fact)) for fact in self.until] if self.until else None,
-        )
-
-
-@dataclass
-class Saturate(_BaseSchedule):
-    schedule: Schedule
+def _command_generator(gen: CommandGenerator) -> Iterable[Command]:
+    """
+    Calls the function with variables of the type and name of the arguments.
+    """
+    hints = get_type_hints(gen)
+    args = (_var(p.name, hints[p.name]) for p in signature(gen).parameters.values())
+    return gen(*args)
 
-    def __str__(self) -> str:
-        return f"{self.schedule}.saturate()"
 
-    def _to_egg(self, declerations: Declarations) -> bindings._Schedule:
-        return bindings.Saturate(self.schedule._to_egg(declerations))
+ActionLike = Union[Action, BaseExpr]
 
 
-@dataclass
-class Repeat(_BaseSchedule):
-    length: int
-    schedule: Schedule
+def _action_likes(action_likes: Iterable[ActionLike]) -> tuple[Action, ...]:
+    return tuple(map(_action_like, action_likes))
 
-    def __str__(self) -> str:
-        return f"{self.schedule} * {self.length}"
 
-    def _to_egg(self, declerations: Declarations) -> bindings._Schedule:
-        return bindings.Repeat(self.length, self.schedule._to_egg(declerations))
+def _action_like(action_like: ActionLike) -> Action:
+    if isinstance(action_like, BaseExpr):
+        return expr_action(action_like)
+    return action_like
 
 
-@dataclass
-class Sequence(_BaseSchedule):
-    schedules: tuple[Schedule, ...]
+FactLike = Union[Fact, Unit]
 
-    def __str__(self) -> str:
-        return f"sequence({', '.join(map(str, self.schedules))})"
 
-    def _to_egg(self, declerations: Declarations) -> bindings._Schedule:
-        return bindings.Sequence([schedule._to_egg(declerations) for schedule in self.schedules])
+def _fact_likes(fact_likes: Iterable[FactLike]) -> tuple[Fact, ...]:
+    return tuple(map(_fact_like, fact_likes))
 
 
-# Define Schedule union instead of using BaseSchedule b/c Python doesn't suppot
-# closed types
-Schedule = Union[Config, Repeat, Saturate, Sequence]
+def _fact_like(fact_like: FactLike) -> Fact:
+    if isinstance(fact_like, BaseExpr):
+        return expr_fact(fact_like)
+    return fact_like
```

### Comparing `egglog-0.4.0/python/egglog/examples/eqsat_basic.py` & `egglog-0.5.1/python/egglog/examples/eqsat_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,7 +36,8 @@
     rewrite(a + b).to(b + a),
     rewrite(a * (b + c)).to((a * b) + (a * c)),
     rewrite(Num(i) + Num(j)).to(Num(i + j)),
     rewrite(Num(i) * Num(j)).to(Num(i * j)),
 )
 egraph.run(10)
 egraph.check(eq(expr1).to(expr2))
+egraph
```

### Comparing `egglog-0.4.0/python/egglog/examples/lambda.py` & `egglog-0.5.1/python/egglog/examples/lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 @egraph.function
 def if_(c: Term, t: Term, f: Term) -> Term:
     ...
 
 
-StringSet = Map[Var, i64]
+StringSet = Set[Var]
 
 
 @egraph.function(merge=lambda old, new: old & new)
 def freer(t: Term) -> StringSet:
     ...
 
 
@@ -91,15 +91,15 @@
 (t, t1, t2, t3, t4) = vars_("t t1 t2 t3 t4", Term)
 (x, y) = vars_("x y", Var)
 fv, fv1, fv2, fv3 = vars_("fv fv1 fv2 fv3", StringSet)
 i1, i2 = vars_("i1 i2", i64)
 egraph.register(
     # freer
     rule(eq(t).to(Term.val(v))).then(set_(freer(t)).to(StringSet.empty())),
-    rule(eq(t).to(Term.var(x))).then(set_(freer(t)).to(StringSet.empty().insert(x, i64(1)))),
+    rule(eq(t).to(Term.var(x))).then(set_(freer(t)).to(StringSet.empty().insert(x))),
     rule(eq(t).to(t1 + t2), eq(freer(t1)).to(fv1), eq(freer(t2)).to(fv2)).then(set_(freer(t)).to(fv1 | fv2)),
     rule(eq(t).to(t1 == t2), eq(freer(t1)).to(fv1), eq(freer(t2)).to(fv2)).then(set_(freer(t)).to(fv1 | fv2)),
     rule(eq(t).to(t1(t2)), eq(freer(t1)).to(fv1), eq(freer(t2)).to(fv2)).then(set_(freer(t)).to(fv1 | fv2)),
     rule(eq(t).to(lam(x, t1)), eq(freer(t1)).to(fv)).then(set_(freer(t)).to(fv.remove(x))),
     rule(eq(t).to(let_(x, t1, t2)), eq(freer(t1)).to(fv1), eq(freer(t2)).to(fv2)).then(
         set_(freer(t)).to(fv1.remove(x) | fv2)
     ),
@@ -173,17 +173,19 @@
 
 
 def assert_simplifies(left: BaseExpr, right: BaseExpr) -> None:
     """
     Simplify and print
     """
     with egraph:
-        res = egraph.simplify(left, 30)
-    print(f"{left} ➡  {res}")
-    assert expr_parts(res) == expr_parts(right), f"{res} != {right}"
+        egraph.register(left)
+        egraph.run(30)
+        res = egraph.extract(left)
+        print(f"{left} ➡  {res}")
+        egraph.check(eq(left).to(right))
 
 
 assert_simplifies((Term.val(Val(1))).eval(), Val(1))
 assert_simplifies((Term.val(Val(1)) + Term.val(Val(2))).eval(), Val(3))
 
 
 # lambda under
```

### Comparing `egglog-0.4.0/python/egglog/examples/matrix.py` & `egglog-0.5.1/python/egglog/examples/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,7 +177,8 @@
 egraph.check(eq(ex1).to(simple_ex1))
 
 ex2 = egraph.define("ex2", kron(Matrix.identity(p), C) @ kron(A, Matrix.identity(m)))
 
 egraph.run(10)
 # Verify it is not simplified
 egraph.check_fail(eq(ex2).to(kron(A, C)))
+egraph
```

### Comparing `egglog-0.4.0/python/egglog/examples/resolution.py` & `egglog-0.5.1/python/egglog/examples/resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,7 +77,8 @@
     union(p1).with_(F),
     set_(~p0 | (~p1 | (p2 | F))).to(T),
 )
 egraph.run(10)
 egraph.check(T != F)
 egraph.check(eq(p0).to(F))
 egraph.check(eq(p2).to(F))
+egraph
```

### Comparing `egglog-0.4.0/python/egglog/monkeypatch.py` & `egglog-0.5.1/python/egglog/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/python/egglog/runtime.py` & `egglog-0.5.1/python/egglog/runtime.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 This module holds a number of types which are only used at runtime to emulate Python objects.
 
 Users will not import anything from this module, and statically they won't know these are the types they are using.
 
 But at runtime they will be exposed.
 
-Note that all their internal fields are prefixed with __egg_ to avoid name collisions with user code.
+Note that all their internal fields are prefixed with __egg_ to avoid name collisions with user code, but will end in __
+so they are not mangled by Python and can be accessed by the user.
 """
 
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Collection, Iterable, Optional, Union
 
 import black
 from typing_extensions import assert_never
 
-from . import config as configuration  # noqa: F401
+from . import config  # noqa: F401
 from .declarations import *
 from .declarations import BINARY_METHODS, UNARY_METHODS
 from .type_constraint_solver import *
 
 __all__ = [
     "LIT_CLASS_NAMES",
     "RuntimeClass",
@@ -30,76 +31,80 @@
     "RuntimeFunction",
     "ArgType",
 ]
 
 
 BLACK_MODE = black.Mode(line_length=120)  # type: ignore
 
-UNIT_CLASS_NAME = "unit"
+UNIT_CLASS_NAME = "Unit"
 UNARY_LIT_CLASS_NAMES = {"i64", "f64", "String"}
 LIT_CLASS_NAMES = UNARY_LIT_CLASS_NAMES | {UNIT_CLASS_NAME}
 
 
 @dataclass
 class RuntimeClass:
-    __egg_decls__: Declarations
+    __egg_decls__: ModuleDeclarations
     __egg_name__: str
 
     def __call__(self, *args: ArgType) -> RuntimeExpr:
         """
         Create an instance of this kind by calling the __init__ classmethod
         """
         # If this is a literal type, initializing it with a literal should return a literal
         if self.__egg_name__ in UNARY_LIT_CLASS_NAMES:
             assert len(args) == 1
             assert isinstance(args[0], (int, float, str))
-            return RuntimeExpr(self.__egg_decls__, JustTypeRef(self.__egg_name__), LitDecl(args[0]))
+            return RuntimeExpr(self.__egg_decls__, TypedExprDecl(JustTypeRef(self.__egg_name__), LitDecl(args[0])))
         if self.__egg_name__ == UNIT_CLASS_NAME:
             assert len(args) == 0
-            return RuntimeExpr(self.__egg_decls__, JustTypeRef(self.__egg_name__), LitDecl(None))
+            return RuntimeExpr(self.__egg_decls__, TypedExprDecl(JustTypeRef(self.__egg_name__), LitDecl(None)))
 
         return RuntimeClassMethod(self.__egg_decls__, self.__egg_name__, "__init__")(*args)
 
     def __dir__(self) -> list[str]:
-        cls_decl = self.__egg_decls__._classes[self.__egg_name__]
+        cls_decl = self.__egg_decls__.get_class_decl(self.__egg_name__)
         possible_methods = list(cls_decl.class_methods) + list(cls_decl.class_variables)
         if "__init__" in possible_methods:
             possible_methods.remove("__init__")
             possible_methods.append("__call__")
         return possible_methods
 
-    def __getitem__(self, args: tuple[RuntimeTypeArgType, ...]) -> RuntimeParamaterizedClass:
+    def __getitem__(self, args: tuple[RuntimeTypeArgType, ...] | RuntimeTypeArgType) -> RuntimeParamaterizedClass:
+        if not isinstance(args, tuple):
+            args = (args,)
         tp = JustTypeRef(self.__egg_name__, tuple(class_to_ref(arg) for arg in args))
         return RuntimeParamaterizedClass(self.__egg_decls__, tp)
 
     def __getattr__(self, name: str) -> RuntimeClassMethod | RuntimeExpr:
-        cls_decl = self.__egg_decls__._classes[self.__egg_name__]
+        cls_decl = self.__egg_decls__.get_class_decl(self.__egg_name__)
         # if this is a class variable, return an expr for it, otherwise, assume it's a method
         if name in cls_decl.class_variables:
-            return_tp = cls_decl.class_variables[name].return_type.to_just()
-            return RuntimeExpr(self.__egg_decls__, return_tp, CallDecl(ClassVariableRef(self.__egg_name__, name)))
+            return_tp = cls_decl.class_variables[name]
+            return RuntimeExpr(
+                self.__egg_decls__, TypedExprDecl(return_tp, CallDecl(ClassVariableRef(self.__egg_name__, name)))
+            )
         return RuntimeClassMethod(self.__egg_decls__, self.__egg_name__, name)
 
     def __str__(self) -> str:
         return self.__egg_name__
 
     # Make hashable so can go in Union
     def __hash__(self) -> int:
         return hash((id(self.__egg_decls__), self.__egg_name__))
 
 
 @dataclass
 class RuntimeParamaterizedClass:
-    __egg_decls__: Declarations
+    __egg_decls__: ModuleDeclarations
     # Note that this will never be a typevar because we don't use RuntimeParamaterizedClass for maps on their own methods
     # which is the only time we define function which take typevars
     __egg_tp__: JustTypeRef
 
     def __post_init__(self):
-        desired_args = self.__egg_decls__._classes[self.__egg_tp__.name].n_type_vars
+        desired_args = self.__egg_decls__.get_class_decl(self.__egg_tp__.name).n_type_vars
         if len(self.__egg_tp__.args) != desired_args:
             raise ValueError(f"Expected {desired_args} type args, got {len(self.__egg_tp__.args)}")
 
     def __call__(self, *args: ArgType) -> RuntimeExpr:
         return RuntimeClassMethod(self.__egg_decls__, class_to_ref(self), "__init__")(*args)
 
     def __getattr__(self, name: str) -> RuntimeClassMethod:
@@ -119,197 +124,181 @@
     if isinstance(cls, RuntimeParamaterizedClass):
         return cls.__egg_tp__
     assert_never(cls)
 
 
 @dataclass
 class RuntimeFunction:
-    __egg_decls__: Declarations
+    __egg_decls__: ModuleDeclarations
     __egg_name__: str
+    __egg_fn_ref__: FunctionRef = field(init=False)
+    __egg_fn_decl__: FunctionDecl = field(init=False)
 
     def __post_init__(self):
-        if self.__egg_name__ not in self.__egg_decls__._functions:
-            raise ValueError(f"Function {self.__egg_name__} does not exist")
+        self.__egg_fn_ref__ = FunctionRef(self.__egg_name__)
+        self.__egg_fn_decl__ = self.__egg_decls__.get_function_decl(self.__egg_fn_ref__)
 
     def __call__(self, *args: ArgType) -> RuntimeExpr:
-        return _call(
-            self.__egg_decls__,
-            FunctionRef(self.__egg_name__),
-            self.__egg_decls__._functions[self.__egg_name__],
-            args,
-        )
+        return _call(self.__egg_decls__, self.__egg_fn_ref__, self.__egg_fn_decl__, args)
 
     def __str__(self) -> str:
         return self.__egg_name__
 
 
 def _call(
-    decls: Declarations,
+    decls: ModuleDeclarations,
     callable_ref: CallableRef,
     # Not included if this is the != method
     fn_decl: Optional[FunctionDecl],
     args: Collection[ArgType],
     bound_params: Optional[tuple[JustTypeRef, ...]] = None,
 ) -> RuntimeExpr:
     upcasted_args = [_resolve_literal(decls, arg) for arg in args]
 
-    arg_types = [arg.__egg_tp__ for arg in upcasted_args]
+    arg_types = [arg.__egg_typed_expr__.tp for arg in upcasted_args]
 
     if bound_params is not None:
         tcs = TypeConstraintSolver.from_type_parameters(bound_params)
     else:
         tcs = TypeConstraintSolver()
 
     if fn_decl is not None:
-        return_tp = tcs.infer_return_type(fn_decl.arg_types, fn_decl.return_type, arg_types)
+        return_tp = tcs.infer_return_type(fn_decl.arg_types, fn_decl.return_type, fn_decl.var_arg_type, arg_types)
     else:
-        return_tp = JustTypeRef("unit")
+        return_tp = JustTypeRef("Unit")
 
-    arg_decls = tuple(arg.__egg_expr__ for arg in upcasted_args)
+    arg_decls = tuple(arg.__egg_typed_expr__ for arg in upcasted_args)
     expr_decl = CallDecl(callable_ref, arg_decls, bound_params)
-    return RuntimeExpr(decls, return_tp, expr_decl)
+    return RuntimeExpr(decls, TypedExprDecl(return_tp, expr_decl))
 
 
 @dataclass
 class RuntimeClassMethod:
-    __egg_decls__: Declarations
+    __egg_decls__: ModuleDeclarations
     # Either a string if it isn't bound or a tp if it s
     __egg_tp__: JustTypeRef | str
     __egg_method_name__: str
+    __egg_callable_ref__: ClassMethodRef = field(init=False)
+    __egg_fn_decl__: FunctionDecl = field(init=False)
 
     def __post_init__(self):
-        if self.__egg_method_name__ not in self.__egg_decls__._classes[self.class_name].class_methods:
+        self.__egg_callable_ref__ = ClassMethodRef(self.class_name, self.__egg_method_name__)
+        try:
+            self.__egg_fn_decl__ = self.__egg_decls__.get_function_decl(self.__egg_callable_ref__)
+        except KeyError:
             raise AttributeError(f"Class {self.class_name} does not have method {self.__egg_method_name__}")
 
     def __call__(self, *args: ArgType) -> RuntimeExpr:
-        fn_decl = self.__egg_decls__._classes[self.class_name].class_methods[self.__egg_method_name__]
         bound_params = self.__egg_tp__.args if isinstance(self.__egg_tp__, JustTypeRef) else None
-        return _call(
-            self.__egg_decls__,
-            ClassMethodRef(self.class_name, self.__egg_method_name__),
-            fn_decl,
-            args,
-            bound_params,
-        )
+        return _call(self.__egg_decls__, self.__egg_callable_ref__, self.__egg_fn_decl__, args, bound_params)
 
     def __str__(self) -> str:
         return f"{self.class_name}.{self.__egg_method_name__}"
 
     @property
     def class_name(self) -> str:
         if isinstance(self.__egg_tp__, str):
             return self.__egg_tp__
         return self.__egg_tp__.name
 
 
 @dataclass
 class RuntimeMethod:
-    __egg_decls__: Declarations
-    __egg_tp__: JustTypeRef
+    __egg_decls__: ModuleDeclarations
+    __egg_typed_expr__: TypedExprDecl
     __egg_method_name__: str
-    __egg_slf_arg__: ExprDecl
+    __egg_callable_ref__: MethodRef = field(init=False)
+    __egg_fn_decl__: Optional[FunctionDecl] = field(init=False)
 
     def __post_init__(self):
-        if (
-            self.__egg_method_name__ not in self.__egg_decls__._classes[self.class_name].methods
-            # Special case for __ne__ which does not have a normal function defintion since
-            # it relies of type parameters
-            and self.__egg_method_name__ != "__ne__"
-        ):
-            raise AttributeError(f"Class {self.class_name} does not have method {self.__egg_method_name__}")
+        self.__egg_callable_ref__ = MethodRef(self.class_name, self.__egg_method_name__)
+        # Special case for __ne__ which does not have a normal function defintion since
+        # it relies of type parameters
+        if self.__egg_method_name__ == "__ne__":
+            self.__egg_fn_decl__ = None
+        else:
+            try:
+                self.__egg_fn_decl__ = self.__egg_decls__.get_function_decl(self.__egg_callable_ref__)
+            except KeyError:
+                raise AttributeError(f"Class {self.class_name} does not have method {self.__egg_method_name__}")
 
     def __call__(self, *args: ArgType) -> RuntimeExpr:
-        fn_decl = (
-            self.__egg_decls__._classes[self.class_name].methods[self.__egg_method_name__]
-            if self.__egg_method_name__ != "__ne__"
-            else None
-        )
-
-        first_arg = RuntimeExpr(self.__egg_decls__, self.__egg_tp__, self.__egg_slf_arg__)
+        first_arg = RuntimeExpr(self.__egg_decls__, self.__egg_typed_expr__)
         args = (first_arg, *args)
-
-        return _call(
-            self.__egg_decls__,
-            MethodRef(self.class_name, self.__egg_method_name__),
-            fn_decl,
-            args,
-        )
+        return _call(self.__egg_decls__, self.__egg_callable_ref__, self.__egg_fn_decl__, args)
 
     @property
     def class_name(self) -> str:
-        return self.__egg_tp__.name
+        return self.__egg_typed_expr__.tp.name
 
 
 @dataclass
 class RuntimeExpr:
-    __egg_decls__: Declarations
-    __egg_tp__: JustTypeRef
-    __egg_expr__: ExprDecl
-
-    @property
-    def __egg_parts__(self) -> tuple[JustTypeRef, ExprDecl]:
-        return self.__egg_tp__, self.__egg_expr__
+    __egg_decls__: ModuleDeclarations
+    __egg_typed_expr__: TypedExprDecl
 
     def __getattr__(self, name: str) -> RuntimeMethod:
-        return RuntimeMethod(self.__egg_decls__, self.__egg_tp__, name, self.__egg_expr__)
+        return RuntimeMethod(self.__egg_decls__, self.__egg_typed_expr__, name)
 
     def __repr__(self) -> str:
         """
         The repr of the expr is the pretty printed version of the expr.
         """
         return str(self)
 
     def __str__(self) -> str:
-        pretty_expr = self.__egg_expr__.pretty(parens=False)
-        if configuration.SHOW_TYPES:
-            s = f"_: {self.__egg_tp__.pretty()} = {pretty_expr}"
+        pretty_expr = self.__egg_typed_expr__.expr.pretty(parens=False)
+        if config.SHOW_TYPES:
+            s = f"_: {self.__egg_typed_expr__.tp.pretty()} = {pretty_expr}"
             return black.format_str(s, mode=black.FileMode()).strip()
         else:
             return black.format_str(pretty_expr, mode=black.FileMode(line_length=180)).strip()
 
     def __dir__(self) -> Iterable[str]:
-        return list(self.__egg_decls__._classes[self.__egg_tp__.name].methods)
+        return list(self.__egg_decls__.get_class_decl(self.__egg_typed_expr__.tp.name).methods)
 
     # Have __eq__ take no NoReturn (aka Never https://docs.python.org/3/library/typing.html#typing.Never) because
     # we don't wany any type that MyPy thinks is an expr to be used with __eq__.
     # That's because we want to reserve __eq__ for domain specific equality checks, overloading this method.
     # To check if two exprs are equal, use the expr_eq method.
     def __eq__(self, other: NoReturn) -> Expr:  # type: ignore
-        raise NotImplementedError("Compare the __parts__ attribute instead")
+        raise NotImplementedError(
+            "Do not use == on RuntimeExpr. Compare the __egg_typed_expr__ attribute instead for structural equality."
+        )
 
 
 # Define each of the special methods, since we have already declared them for pretty printing
 for name in list(BINARY_METHODS) + list(UNARY_METHODS) + ["__getitem__", "__call__"]:
 
     def _special_method(self: RuntimeExpr, *args: ArgType, __name: str = name) -> RuntimeExpr:
-        return RuntimeMethod(self.__egg_decls__, self.__egg_tp__, __name, self.__egg_expr__)(*args)
+        return RuntimeMethod(self.__egg_decls__, self.__egg_typed_expr__, __name)(*args)
 
     setattr(RuntimeExpr, name, _special_method)
 
 
 # Args can either be expressions or literals which are automatically promoted
 ArgType = Union[RuntimeExpr, int, str, float]
 
 
-def _resolve_literal(decls: Declarations, arg: ArgType) -> RuntimeExpr:
+def _resolve_literal(decls: ModuleDeclarations, arg: ArgType) -> RuntimeExpr:
     if isinstance(arg, int):
-        return RuntimeExpr(decls, JustTypeRef("i64"), LitDecl(arg))
+        return RuntimeExpr(decls, TypedExprDecl(JustTypeRef("i64"), LitDecl(arg)))
     elif isinstance(arg, float):
-        return RuntimeExpr(decls, JustTypeRef("f64"), LitDecl(arg))
+        return RuntimeExpr(decls, TypedExprDecl(JustTypeRef("f64"), LitDecl(arg)))
     elif isinstance(arg, str):
-        return RuntimeExpr(decls, JustTypeRef("String"), LitDecl(arg))
+        return RuntimeExpr(decls, TypedExprDecl(JustTypeRef("String"), LitDecl(arg)))
     return arg
 
 
 def _resolve_callable(callable: object) -> CallableRef:
     """
     Resolves a runtime callable into a ref
     """
     if isinstance(callable, RuntimeFunction):
         return FunctionRef(callable.__egg_name__)
     if isinstance(callable, RuntimeClassMethod):
         return ClassMethodRef(callable.class_name, callable.__egg_method_name__)
     if isinstance(callable, RuntimeMethod):
-        return MethodRef(callable.__egg_tp__.name, callable.__egg_method_name__)
+        return MethodRef(callable.__egg_typed_expr__.tp.name, callable.__egg_method_name__)
     if isinstance(callable, RuntimeClass):
         return ClassMethodRef(callable.__egg_name__, "__init__")
     raise NotImplementedError(f"Cannot turn {callable} into a callable ref")
```

### Comparing `egglog-0.4.0/python/egglog/type_constraint_solver.py` & `egglog-0.5.1/python/egglog/type_constraint_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Collection
+from itertools import chain, repeat
+from typing import Collection, Optional
 
 from .declarations import *
 
 __all__ = ["TypeConstraintSolver", "TypeConstraintError"]
 
 
 class TypeConstraintError(RuntimeError):
@@ -34,32 +35,36 @@
             cs._cls_typevar_index_to_type[i] = tp
         return cs
 
     def infer_return_type(
         self,
         fn_args: Collection[TypeOrVarRef],
         fn_return: TypeOrVarRef,
+        fn_var_args: Optional[TypeOrVarRef],
         args: Collection[JustTypeRef],
     ) -> JustTypeRef:
         # Infer the type of each type variable based on the actual types of the arguments
-        self._infer_typevars_zip(fn_args, args)
+        self._infer_typevars_zip(fn_args, fn_var_args, args)
         # Substitute the type variables with their inferred types
         return self._subtitute_typevars(fn_return)
 
-    def _infer_typevars_zip(self, fn_args: Collection[TypeOrVarRef], args: Collection[JustTypeRef]) -> None:
-        if len(fn_args) != len(args):
+    def _infer_typevars_zip(
+        self, fn_args: Collection[TypeOrVarRef], fn_var_args: Optional[TypeOrVarRef], args: Collection[JustTypeRef]
+    ) -> None:
+        if len(fn_args) != len(args) if fn_var_args is None else len(fn_args) > len(args):
             raise TypeConstraintError(f"Expected {len(fn_args)} args, got {len(args)}")
-        for fn_arg, arg in zip(fn_args, args):
+        all_fn_args = fn_args if fn_var_args is None else chain(fn_args, repeat(fn_var_args))
+        for fn_arg, arg in zip(all_fn_args, args):
             self._infer_typevars(fn_arg, arg)
 
     def _infer_typevars(self, fn_arg: TypeOrVarRef, arg: JustTypeRef) -> None:
         if isinstance(fn_arg, TypeRefWithVars):
             if fn_arg.name != arg.name:
                 raise TypeConstraintError(f"Expected {fn_arg.name}, got {arg.name}")
-            self._infer_typevars_zip(fn_arg.args, arg.args)
+            self._infer_typevars_zip(fn_arg.args, None, arg.args)
         elif fn_arg.index not in self._cls_typevar_index_to_type:
             self._cls_typevar_index_to_type[fn_arg.index] = arg
         elif self._cls_typevar_index_to_type[fn_arg.index] != arg:
             raise TypeConstraintError(f"Expected {fn_arg}, got {arg}")
 
     def _subtitute_typevars(self, tp: TypeOrVarRef) -> JustTypeRef:
         if isinstance(tp, ClassTypeVarRef):
```

### Comparing `egglog-0.4.0/python/tests/test_bindings.py` & `egglog-0.5.1/python/tests/test_bindings.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     metadata_process = subprocess.run(
         ["cargo", "metadata", "--format-version", "1", "-q"],
         capture_output=True,
         check=True,
     )
     metadata = json.loads(metadata_process.stdout)
-    (egglog_package,) = [package for package in metadata["packages"] if package["name"] == "egg-smol"]
+    (egglog_package,) = [package for package in metadata["packages"] if package["name"] == "egglog"]
     return pathlib.Path(egglog_package["manifest_path"]).parent
 
 
 EGG_SMOL_FOLDER = get_egglog_folder()
 
 SLOW_TESTS = ["repro-unsound"]
 
@@ -140,25 +140,25 @@
         # From map example
         egraph = EGraph()
         egraph.run_program(
             Sort(
                 "MyMap",
                 ("Map", [Var("i64"), Var("String")]),
             ),
-            Define("my_map1", Call("insert", [Call("empty", []), Lit(Int(1)), Lit(String("one"))]), None),
-            Define("my_map2", Call("insert", [Var("my_map1"), Lit(Int(2)), Lit(String("two"))]), None),
-            Check([Eq([Lit(String("one")), Call("get", [Var("my_map1"), Lit(Int(1))])])]),
+            Define("my_map1", Call("map-insert", [Call("map-empty", []), Lit(Int(1)), Lit(String("one"))]), None),
+            Define("my_map2", Call("map-insert", [Var("my_map1"), Lit(Int(2)), Lit(String("two"))]), None),
+            Check([Eq([Lit(String("one")), Call("map-get", [Var("my_map1"), Lit(Int(1))])])]),
             Extract(0, Var("my_map2")),
         )
         assert egraph.extract_report() == ExtractReport(
             0,
             Call(
-                "insert",
+                "map-insert",
                 [
-                    Call("insert", [Call("empty", []), Lit(Int(2)), Lit(String("two"))]),
+                    Call("map-insert", [Call("map-empty", []), Lit(Int(2)), Lit(String("two"))]),
                     Lit(Int(1)),
                     Lit(String("one")),
                 ],
             ),
             [],
         )
```

### Comparing `egglog-0.4.0/python/tests/test_high_level.py` & `egglog-0.5.1/python/tests/test_high_level.py`

 * *Files 18% similar despite different names*

```diff
@@ -157,21 +157,81 @@
 
         def __init__(self, v: i64) -> None:
             pass
 
     assert expr_parts(egraph.simplify(Numeric.ONE, 10)) == expr_parts(Numeric.ONE)
 
     egraph.register(union(Numeric.ONE).with_(Numeric(i64(1))))
-
-    assert expr_parts(egraph.simplify(Numeric.ONE, 10)) == expr_parts(Numeric(i64(1)))
+    egraph.run(10)
+    egraph.check(eq(Numeric.ONE).to(Numeric(i64(1))))
 
 
 def test_extract_constant_twice():
     # Sometimes extrcting a constant twice will give an error
     egraph = EGraph()
 
     @egraph.class_
     class Numeric(BaseExpr):
         ONE: ClassVar[Numeric]
 
     egraph.extract(Numeric.ONE)
     egraph.extract(Numeric.ONE)
+
+
+def test_relation():
+    egraph = EGraph()
+
+    test_relation = egraph.relation("test_relation", i64, i64)
+    egraph.register(test_relation(i64(1), i64(1)))
+
+
+def test_variable_args():
+    egraph = EGraph()
+    # Create dummy function with type so its registered
+    egraph.relation("_", Set[i64])
+
+    egraph.check(Set(i64(1), i64(2)).contains(i64(1)))
+
+
+@pytest.mark.xfail(reason="We have to manually register sorts before using them")
+def test_generic_sort():
+    egraph = EGraph()
+    egraph.check(Set(i64(1), i64(2)).contains(i64(1)))
+
+
+def test_modules() -> None:
+    m = Module()
+
+    @m.class_
+    class Numeric(BaseExpr):
+        ONE: ClassVar[Numeric]
+
+    m2 = Module()
+
+    @m2.class_
+    class OtherNumeric(BaseExpr):
+        @m2.method(cost=10)
+        def __init__(self, v: i64Like) -> None:
+            ...
+
+    egraph = EGraph(deps=[m, m2])
+
+    @egraph.function
+    def from_numeric(n: Numeric) -> OtherNumeric:  # type: ignore[empty-body]
+        ...
+
+    egraph.register(rewrite(OtherNumeric(1)).to(from_numeric(Numeric.ONE)))
+    assert expr_parts(egraph.simplify(OtherNumeric(i64(1)), 10)) == expr_parts(from_numeric(Numeric.ONE))
+
+
+def test_f64_negation() -> None:
+    egraph = EGraph()
+    # expr1 = -2.0
+    expr1 = egraph.define("expr1", -f64(2.0))
+
+    # expr2 = 2.0
+    expr2 = egraph.define("expr2", f64(2.0))
+
+    # expr3 = -(-2.0)
+    expr3 = egraph.define("expr3", -(-f64(2.0)))
+    egraph.check(eq(expr1).to(-expr2))
+    egraph.check(eq(expr3).to(expr2))
```

### Comparing `egglog-0.4.0/python/tests/test_runtime.py` & `egglog-0.5.1/python/tests/test_runtime.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,116 +2,138 @@
 
 from egglog.declarations import *
 from egglog.runtime import *
 from egglog.type_constraint_solver import *
 
 
 def test_type_str():
-    decls = Declarations(
-        _classes={
-            "i64": ClassDecl(),
-            "Map": ClassDecl(n_type_vars=2),
-        }
+    decls = ModuleDeclarations(
+        Declarations(
+            _classes={
+                "i64": ClassDecl(),
+                "Map": ClassDecl(n_type_vars=2),
+            }
+        )
     )
     i64 = RuntimeClass(decls, "i64")
     Map = RuntimeClass(decls, "Map")
     assert str(i64) == "i64"
     assert str(Map[i64, i64]) == "Map[i64, i64]"
 
 
 def test_function_call():
-    decls = Declarations(
-        _classes={
-            "i64": ClassDecl(),
-        },
-        _functions={
-            "one": FunctionDecl(
-                (),
-                TypeRefWithVars("i64"),
-            ),
-        },
+    decls = ModuleDeclarations(
+        Declarations(
+            _classes={
+                "i64": ClassDecl(),
+            },
+            _functions={
+                "one": FunctionDecl(
+                    (),
+                    TypeRefWithVars("i64"),
+                ),
+            },
+        )
     )
     one = RuntimeFunction(decls, "one")
-    assert one().__egg_parts__ == RuntimeExpr(decls, JustTypeRef("i64"), CallDecl(FunctionRef("one"))).__egg_parts__
+    assert (
+        one().__egg_typed_expr__
+        == RuntimeExpr(decls, TypedExprDecl(JustTypeRef("i64"), CallDecl(FunctionRef("one")))).__egg_typed_expr__
+    )
 
 
 def test_classmethod_call():
     from pytest import raises
 
     K, V = ClassTypeVarRef(0), ClassTypeVarRef(1)
-    decls = Declarations(
-        _classes={
-            "i64": ClassDecl(),
-            "unit": ClassDecl(),
-            "Map": ClassDecl(
-                n_type_vars=2,
-                class_methods={
-                    "create": FunctionDecl(
-                        (),
-                        TypeRefWithVars("Map", (K, V)),
-                    )
-                },
-            ),
-        }
+    decls = ModuleDeclarations(
+        Declarations(
+            _classes={
+                "i64": ClassDecl(),
+                "unit": ClassDecl(),
+                "Map": ClassDecl(
+                    n_type_vars=2,
+                    class_methods={
+                        "create": FunctionDecl(
+                            (),
+                            TypeRefWithVars("Map", (K, V)),
+                        )
+                    },
+                ),
+            }
+        )
     )
     Map = RuntimeClass(decls, "Map")
     with raises(TypeConstraintError):
         Map.create()  # type: ignore
     i64 = RuntimeClass(decls, "i64")
     unit = RuntimeClass(decls, "unit")
     assert (
-        Map[i64, unit].create().__egg_parts__
+        Map[i64, unit].create().__egg_typed_expr__
         == RuntimeExpr(
             decls,
-            JustTypeRef("Map", (JustTypeRef("i64"), JustTypeRef("unit"))),
-            CallDecl(
-                ClassMethodRef("Map", "create"),
-                (),
-                (JustTypeRef("i64"), JustTypeRef("unit")),
+            TypedExprDecl(
+                JustTypeRef("Map", (JustTypeRef("i64"), JustTypeRef("unit"))),
+                CallDecl(
+                    ClassMethodRef("Map", "create"),
+                    (),
+                    (JustTypeRef("i64"), JustTypeRef("unit")),
+                ),
             ),
-        ).__egg_parts__
+        ).__egg_typed_expr__
     )
 
 
 def test_expr_special():
-    decls = Declarations(
-        _classes={
-            "i64": ClassDecl(
-                methods={
-                    "__add__": FunctionDecl(
-                        (TypeRefWithVars("i64"), TypeRefWithVars("i64")),
-                        TypeRefWithVars("i64"),
-                    )
-                },
-                class_methods={
-                    "__init__": FunctionDecl(
-                        (TypeRefWithVars("i64"),),
-                        TypeRefWithVars("i64"),
-                    )
-                },
-            ),
-        },
+    decls = ModuleDeclarations(
+        Declarations(
+            _classes={
+                "i64": ClassDecl(
+                    methods={
+                        "__add__": FunctionDecl(
+                            (TypeRefWithVars("i64"), TypeRefWithVars("i64")),
+                            TypeRefWithVars("i64"),
+                        )
+                    },
+                    class_methods={
+                        "__init__": FunctionDecl(
+                            (TypeRefWithVars("i64"),),
+                            TypeRefWithVars("i64"),
+                        )
+                    },
+                ),
+            },
+        )
     )
     i64 = RuntimeClass(decls, "i64")
     one = i64(1)  # type: ignore
     res = one + one  # type: ignore
     expected_res = RuntimeExpr(
         decls,
-        JustTypeRef("i64"),
-        CallDecl(MethodRef("i64", "__add__"), (LitDecl(1), LitDecl(1))),
+        TypedExprDecl(
+            JustTypeRef("i64"),
+            CallDecl(
+                MethodRef("i64", "__add__"),
+                (TypedExprDecl(JustTypeRef("i64"), LitDecl(1)), TypedExprDecl(JustTypeRef("i64"), LitDecl(1))),
+            ),
+        ),
     )
-    assert res.__egg_parts__ == expected_res.__egg_parts__
+    assert res.__egg_typed_expr__ == expected_res.__egg_typed_expr__
 
 
 def test_class_variable():
-    decls = Declarations(
-        _classes={
-            "i64": ClassDecl(class_variables={"one": FunctionDecl((), TypeRefWithVars("i64"))}),
-        },
+    decls = ModuleDeclarations(
+        Declarations(
+            _classes={
+                "i64": ClassDecl(class_variables={"one": JustTypeRef("i64")}),
+            },
+        )
     )
     i64 = RuntimeClass(decls, "i64")
     one = i64.one
     assert isinstance(one, RuntimeExpr)
     assert (
-        one.__egg_parts__
-        == RuntimeExpr(decls, JustTypeRef("i64"), CallDecl(ClassVariableRef("i64", "one"))).__egg_parts__
+        one.__egg_typed_expr__
+        == RuntimeExpr(
+            decls, TypedExprDecl(JustTypeRef("i64"), CallDecl(ClassVariableRef("i64", "one")))
+        ).__egg_typed_expr__
     )
```

### Comparing `egglog-0.4.0/python/tests/test_typing.py` & `egglog-0.5.1/python/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/src/egraph.rs` & `egglog-0.5.1/src/egraph.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 // Wrapper around EGraph type
 
-use std::path::PathBuf;
-
 use crate::conversions::*;
 use crate::error::EggResult;
+
 use log::info;
 use pyo3::prelude::*;
+use std::path::PathBuf;
 
 /// EGraph()
 /// --
 ///
 /// Create an empty EGraph.
 #[pyclass(
     unsendable,
     text_signature = "(*, fact_directory=None, seminaive=True)"
 )]
 pub struct EGraph {
-    egraph: egg_smol::EGraph,
+    egraph: egglog::EGraph,
 }
 
 #[pymethods]
 impl EGraph {
     #[new]
     #[pyo3(signature = (*, fact_directory=None, seminaive=true))]
     fn new(fact_directory: Option<PathBuf>, seminaive: bool) -> Self {
-        let mut egraph = egg_smol::EGraph::default();
-        egraph.fact_directory = fact_directory.clone();
+        let mut egraph = egglog::EGraph::default();
+        egraph.fact_directory = fact_directory;
         egraph.seminaive = seminaive;
         Self { egraph }
     }
 
     /// Parse a program into a list of commands.
     #[pyo3(signature = (input, /))]
     fn parse_program(&mut self, input: &str) -> EggResult<Vec<Command>> {
@@ -39,36 +39,42 @@
     }
 
     /// Run a series of commands on the EGraph.
     /// Returns a list of strings representing the output.
     /// An EggSmolError is raised if there is problem parsing or executing.
     #[pyo3(signature=(*commands))]
     fn run_program(&mut self, commands: Vec<Command>) -> EggResult<Vec<String>> {
-        let commands: Vec<egg_smol::ast::Command> =
-            commands.into_iter().map(|x| x.into()).collect();
+        let commands: Vec<egglog::ast::Command> = commands.into_iter().map(|x| x.into()).collect();
         info!("Running commands {:?}", commands);
         let res = self.egraph.run_program(commands)?;
         Ok(res)
     }
 
     /// Gets the last expressions extracted from the EGraph, if the last command
     /// was a Simplify or Extract command.
     #[pyo3(signature = ())]
     fn extract_report(&mut self) -> Option<ExtractReport> {
         info!("Getting last extract report");
-        match self.egraph.get_extract_report() {
-            Some(report) => Some(report.into()),
-            None => None,
-        }
+        self.egraph
+            .get_extract_report()
+            .as_ref()
+            .map(|report| report.into())
     }
 
     /// Gets the last run report from the EGraph, if the last command
     /// was a run or simplify command.
     #[pyo3(signature = ())]
     fn run_report(&mut self) -> Option<RunReport> {
         info!("Getting last run report");
-        match self.egraph.get_run_report() {
-            Some(report) => Some(report.into()),
-            None => None,
-        }
+        self.egraph
+            .get_run_report()
+            .as_ref()
+            .map(|report| report.into())
+    }
+
+    /// Returns the EGraph as graphviz string.
+    #[pyo3(signature = ())]
+    fn to_graphviz_string(&self) -> String {
+        info!("Getting graphviz");
+        self.egraph.to_graphviz_string()
     }
 }
```

### Comparing `egglog-0.4.0/src/error.rs` & `egglog-0.5.1/src/error.rs`

 * *Files 14% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 impl EggSmolError {
     #[new]
     fn new(context: String) -> Self {
         EggSmolError { context }
     }
 }
 
-// Wrap the egg_smol::Error so we can automatically convert from it to the PyErr
+// Wrap the egglog::Error so we can automatically convert from it to the PyErr
 // and so return it from each function automatically
 // https://pyo3.rs/latest/function/error_handling.html#foreign-rust-error-types
 // TODO: Create classes for each of these errors
-pub struct WrappedError(egg_smol::Error);
+pub struct WrappedError(egglog::Error);
 
 // Convert from the WrappedError to the PyErr by creating a new Python error
 impl From<WrappedError> for PyErr {
     fn from(error: WrappedError) -> Self {
         PyErr::new::<EggSmolError, _>(error.0.to_string())
     }
 }
 
-// Convert from an egg_smol::Error to a WrappedError
-impl From<egg_smol::Error> for WrappedError {
-    fn from(other: egg_smol::Error) -> Self {
+// Convert from an egglog::Error to a WrappedError
+impl From<egglog::Error> for WrappedError {
+    fn from(other: egglog::Error) -> Self {
         Self(other)
     }
 }
 
 // Use similar to PyResult, wraps a result type and can be converted to PyResult
 pub type EggResult<T> = Result<T, WrappedError>;
```

### Comparing `egglog-0.4.0/src/utils.rs` & `egglog-0.5.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `egglog-0.4.0/Cargo.lock` & `egglog-0.5.1/Cargo.lock`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,88 @@
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "ahash"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf6ccdb167abbf410dcb915cabd428929d7f6a04980b54a11f26a39f1c7f7107"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+
+[[package]]
+name = "anstream"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys",
+]
+
+[[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "ascii-canvas"
@@ -45,25 +100,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8824ecca2e851cec16968d54a01dd372ef8f95b244fb84b84e70128be347c3c6"
 dependencies = [
  "term",
 ]
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bit-set"
@@ -83,75 +127,135 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
+name = "bumpalo"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
 name = "cc"
-version = "1.0.77"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9f73505338f7d905b19d18738976aae232eb46b8efc15554ffc56deb5d9ebe4"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.0.28"
+version = "4.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f94eecf2f2d0e0220737d9e6d8530da1e903b97dde58ebaf749262e85ce133c9"
+checksum = "8f644d0dac522c8b05ddc39aaaccc5b136d5dc4ff216610c5641e3be5becf56c"
 dependencies = [
- "bitflags",
+ "clap_builder",
  "clap_derive",
- "clap_lex",
- "is-terminal",
  "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af410122b9778e024f9e0fb35682cc09cc3f85cad5e8d3ba8f47a9702df6e73d"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "clap_lex",
  "strsim",
- "termcolor",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.0.21"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0177313f9f02afc995627906bbd8967e2be069f5261954222dac78290c2b9014"
+checksum = "54a9bb5758fc5dfe728d1019941681eccaf0cf8a4189b692a0ee2f2ecf90a050"
 dependencies = [
  "heck",
- "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.0"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
+name = "cpufeatures"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d4198f73e42b4936b35b5bb248d81d2b595ecb170da0bac7655c54eedfa8da8"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
- "os_str_bytes",
+ "libc",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
 name = "dirs-next"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b98cf8ebf19c3d1b223e151f99a4f9f0690dca41414773390fc824184ac833e1"
 dependencies = [
  "cfg-if",
  "dirs-sys-next",
@@ -165,26 +269,42 @@
 dependencies = [
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
-name = "egg-smol"
+name = "dot-generator"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0aaac7ada45f71873ebce336491d1c1bc4a7c8042c7cea978168ad59e805b871"
+dependencies = [
+ "dot-structures",
+]
+
+[[package]]
+name = "dot-structures"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "545da7d6df7f8fd0de7106669a7d0bfa3dbcfa24d81da46906ad658188b2ff7c"
+
+[[package]]
+name = "egglog"
 version = "0.1.0"
-source = "git+https://github.com/egraphs-good/egglog?rev=30feaaab88452ec4b6c5f7a199345298bac2dd0f#30feaaab88452ec4b6c5f7a199345298bac2dd0f"
+source = "git+https://github.com/saulshanabrook/egg-smol?rev=353c4387640019bd2066991ee0488dc6d5c54168#353c4387640019bd2066991ee0488dc6d5c54168"
 dependencies = [
  "clap",
  "env_logger",
- "glob",
- "hashbrown 0.13.1",
- "indexmap",
+ "getrandom",
+ "graphviz-rust",
+ "hashbrown 0.14.0",
+ "indexmap 2.0.0",
  "instant",
  "lalrpop",
- "lalrpop-util",
+ "lalrpop-util 0.20.0",
  "lazy_static",
  "log",
  "num-integer",
  "num-rational",
  "num-traits",
  "ordered-float",
  "regex",
@@ -193,35 +313,35 @@
  "symbol_table",
  "symbolic_expressions",
  "thiserror",
 ]
 
 [[package]]
 name = "egglog-python"
-version = "0.4.0"
+version = "0.5.1"
 dependencies = [
- "egg-smol",
- "lalrpop-util",
+ "egglog",
+ "lalrpop-util 0.19.12",
  "log",
  "ordered-float",
  "pyo3",
  "pyo3-log",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "ena"
-version = "0.14.0"
+version = "0.14.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7402b94a93c24e742487327a7cd839dc9d36fec9de9fb25b09f2dae459f36c3"
+checksum = "c533630cf40e9caa44bd91aadc88a75d75a4c3a12b4cfde353cbed41daa1e1f1"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.10.0"
@@ -232,229 +352,308 @@
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
+name = "fastrand"
+version = "1.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
+dependencies = [
+ "instant",
+]
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi",
+ "wasm-bindgen",
 ]
 
 [[package]]
-name = "glob"
-version = "0.3.1"
+name = "graphviz-rust"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+checksum = "56e6ed437c021ff97f2517bfd9c629b5bbbb71b123ba5556e01df359e3f6bc18"
+dependencies = [
+ "dot-generator",
+ "dot-structures",
+ "into-attr",
+ "into-attr-derive",
+ "pest",
+ "pest_derive",
+ "rand",
+ "tempfile",
+]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash 0.7.6",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.13.1"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33ff8ae62cd3a9102e5637afc8452c55acf3844001bd5374e0b0bd7b6616c038"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
 dependencies = [
- "ahash 0.8.2",
+ "ahash 0.8.3",
+ "allocator-api2",
 ]
 
 [[package]]
 name = "heck"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
-
-[[package]]
-name = "hermit-abi"
-version = "0.1.19"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
 name = "indoc"
-version = "1.0.7"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adab1eaa3408fb7f0c777a73e7465fd5656136fc93b670eb6df3c88c2c1344e3"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "into-attr"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6ec0dd848c05d2695dd73818984fb156ac8cbcbfdf4e474243590bfcc2468e9"
+dependencies = [
+ "dot-structures",
+]
+
+[[package]]
+name = "into-attr-derive"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8fbf3ed04003b36d48d9acb5ee7d66eaf1efa8318bc26571c6b86db7b05f12a"
+dependencies = [
+ "dot-generator",
+ "dot-structures",
+ "into-attr",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "io-lifetimes"
-version = "1.0.3"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46112a93252b123d31a119a8d1a1ac19deac4fac6e0e8b0df58f0d4e5870e63c"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
+ "hermit-abi",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.1"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927609f78c2913a6f6ac3c27a4fe87f43e2a35367c0c4b0f8265e8f49a104330"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.2.6",
- "io-lifetimes",
- "rustix",
+ "hermit-abi",
+ "rustix 0.38.4",
  "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "js-sys"
+version = "0.3.64"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "lalrpop"
-version = "0.19.8"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30455341b0e18f276fa64540aff54deafb54c589de6aca68659c63dd2d5d823"
+checksum = "da4081d44f4611b66c6dd725e6de3169f9f63905421e8626fcb86b6a898998b8"
 dependencies = [
  "ascii-canvas",
- "atty",
  "bit-set",
  "diff",
  "ena",
+ "is-terminal",
  "itertools",
- "lalrpop-util",
+ "lalrpop-util 0.20.0",
  "petgraph",
  "pico-args",
  "regex",
  "regex-syntax",
  "string_cache",
  "term",
  "tiny-keccak",
  "unicode-xid",
 ]
 
 [[package]]
 name = "lalrpop-util"
-version = "0.19.8"
+version = "0.19.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf796c978e9b4d983414f4caedc9273aa33ee214c5b887bd55fde84c85d2dc4"
+checksum = "d3c48237b9604c5a4702de6b824e02006c3214327564636aef27c1028a8fa0ed"
+dependencies = [
+ "regex",
+]
+
+[[package]]
+name = "lalrpop-util"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f35c735096c0293d313e8f2a641627472b83d01b937177fe76e5e2708d31e0d"
 dependencies = [
  "regex",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.137"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc7fcc620a3bff7cdd7a365be3376c97191aeaccc2a603e600951e452615bf89"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.3"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f9f08d8963a6c613f4b1a78f4f4a4dbfadf8e6545b2d72861731e4858b8b47f"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -513,315 +712,385 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "ordered-float"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13a384337e997e6860ffbaa83708b2ef329fd8c54cb67a5f64d421e0f943254f"
+checksum = "2fc2dbde8f8a79f2102cc474ceb0ad68e3b80b85289ea62389b60e66777e4213"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
-name = "parking_lot"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
-dependencies = [
- "instant",
- "lock_api",
- "parking_lot_core 0.8.6",
-]
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.5",
+ "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.6"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "smallvec",
- "winapi",
+ "windows-targets",
 ]
 
 [[package]]
-name = "parking_lot_core"
-version = "0.9.5"
+name = "pest"
+version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "0d2d1d55045829d65aad9d389139882ad623b33b904e7c9f1b10c5b8927298e5"
 dependencies = [
- "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-sys",
+ "thiserror",
+ "ucd-trie",
+]
+
+[[package]]
+name = "pest_derive"
+version = "2.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f94bca7e7a599d89dea5dfa309e217e7906c3c007fb9c3299c40b10d6a315d3"
+dependencies = [
+ "pest",
+ "pest_generator",
+]
+
+[[package]]
+name = "pest_generator"
+version = "2.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "99d490fe7e8556575ff6911e45567ab95e71617f43781e5c05490dc8d75c965c"
+dependencies = [
+ "pest",
+ "pest_meta",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
+name = "pest_meta"
+version = "2.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2674c66ebb4b4d9036012091b537aae5878970d6999f81a265034d85b136b341"
+dependencies = [
+ "once_cell",
+ "pest",
+ "sha2",
 ]
 
 [[package]]
 name = "petgraph"
-version = "0.6.2"
+version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6d5014253a1331579ce62aa67443b4a658c5e7dd03d4bc6d302b94474888143"
+checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
- "indexmap",
+ "indexmap 1.9.3",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6796ad771acdc0123d2a88dc428b5e38ef24456743ddb1744ed628f9815c096"
 dependencies = [
  "siphasher",
 ]
 
 [[package]]
 name = "pico-args"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db8bcd96cb740d03149cbad5518db9fd87126a10ab519c011893b1754134c468"
+checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
 
 [[package]]
-name = "precomputed-hash"
-version = "0.1.1"
+name = "ppv-lite86"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "proc-macro-error"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
-dependencies = [
- "proc-macro-error-attr",
- "proc-macro2",
- "quote",
- "syn",
- "version_check",
-]
-
-[[package]]
-name = "proc-macro-error-attr"
-version = "1.0.4"
+name = "precomputed-hash"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
-dependencies = [
- "proc-macro2",
- "quote",
- "version_check",
-]
+checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.47"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ea3d908b0e36316caf9e9e2c4625cdde190a7e6f440d794667ed17a1855e725"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
- "parking_lot 0.11.2",
+ "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
+checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.21"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe448f377a7d6961e30f5955f9b8d106c3f5e449d493ee1b125c1d43c2b5179"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags 1.3.2",
 ]
 
 [[package]]
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
-version = "1.7.0"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.36.4"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb93e85278e08bb5788653183213d3a60fc242b10cb9be96586f5a73dcb67c23"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
+ "linux-raw-sys 0.3.8",
+ "windows-sys",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys 0.4.3",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.9"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97477e48b4cf8603ad5f7aaf897467cf42ab4218a38ef76fb14c2d6773a6d6a8"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
+
+[[package]]
+name = "sha2"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+dependencies = [
+ "cfg-if",
+ "cpufeatures",
+ "digest",
+]
 
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "string_cache"
-version = "0.8.4"
+version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213494b7a2b503146286049378ce02b482200519accc31872ee8be91fa820a08"
+checksum = "f91138e76242f575eb1d3b38b4f1362f10d3a43f47d182a5b359af488a02293b"
 dependencies = [
  "new_debug_unreachable",
  "once_cell",
- "parking_lot 0.12.1",
+ "parking_lot",
  "phf_shared",
  "precomputed-hash",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
@@ -840,109 +1109,206 @@
 [[package]]
 name = "symbolic_expressions"
 version = "5.0.3"
 source = "git+https://github.com/oflatt/symbolic-expressions?rev=4c0ea5ca008f972450b2af72387e64d2c1c6a791#4c0ea5ca008f972450b2af72387e64d2c1c6a791"
 
 [[package]]
 name = "syn"
-version = "1.0.104"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ae548ec36cf198c0ef7710d3c230987c2d6d7bd98ad6edc0274462724c585ce"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+
+[[package]]
+name = "tempfile"
+version = "3.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "fastrand",
+ "redox_syscall 0.3.5",
+ "rustix 0.37.23",
+ "windows-sys",
+]
 
 [[package]]
 name = "term"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c59df8ac95d96ff9bede18eb7300b0fda5e5d8d90960e76f8e14ae765eedbf1f"
 dependencies = [
  "dirs-next",
  "rustversion",
  "winapi",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.1.3"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
+checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.37"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10deb33631e3c9018b9baf9dcbbc4f737320d2b576bac10f6aefa048fa407e3e"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.37"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "982d17546b47146b28f7c22e3d08465f6b8903d0ea13c1660d9d84a6e7adcdbb"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
+name = "typenum"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+
+[[package]]
+name = "ucd-trie"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed646292ffc8188ef8ea4d1e0e0150fb15a5c2e12ad9b8fc191ae7a8a7f3c4b9"
+
+[[package]]
 name = "unicode-ident"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ceab39d59e4c9499d4e5a8ee0e2735b891bb7308ac83dfb4e80cad195c9f6f3"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58ee9362deb4a96cef4d437d1ad49cffc9b9e92d202b6995674e928ce684f112"
+checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+
+[[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -967,61 +1333,70 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `egglog-0.4.0/PKG-INFO` & `egglog-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egglog
-Version: 0.4.0
+Version: 0.5.1
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,19 +15,21 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions
 Requires-Dist: black
+Requires-Dist: graphviz
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: myst-nb; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-gallery; extra == 'docs'
 Requires-Dist: matplotlib; extra == 'docs'
+Requires-Dist: nbconvert; extra == 'docs'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
@@ -43,9 +45,9 @@
 # `egglog` Python wrapper
 
 [![Documentation Status](https://readthedocs.org/projects/egg-smol-python/badge/?version=latest)](https://egg-smol-python.readthedocs.io/en/latest/?badge=latest) [![Test](https://github.com/metadsl/egglog-python/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/metadsl/egglog-python/actions/workflows/CI.yml) [![PyPi Package](https://img.shields.io/pypi/v/egglog.svg)](https://pypi.org/project/egglog/) [![License](https://img.shields.io/pypi/l/egglog.svg)](https://pypi.org/project/egglog/) [![Python Versions](https://img.shields.io/pypi/pyversions/egglog.svg)](https://pypi.org/project/egglog/) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 `egglog` is a Python package that provides bindings to the Rust library [`egglog`](https://github.com/egraphs-good/egglog/),
 allowing you to use e-graphs in Python for optimization, symbolic computation, and analysis.
 
-Please see the [documentation](https://egglog-python.readthedocs.io/en/latest/) for more information.
+Please see the [documentation](https://egg-smol-python.readthedocs.io/en/latest/?badge=latest) for more information.
```

