# Comparing `tmp/strsim_2-1.0.1.tar.gz` & `tmp/strsim_2-1.1.0.tar.gz`

## Comparing `strsim_2-1.0.1.tar` & `strsim_2-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 strsim_2-1.0.1/Cargo.toml
--rw-r--r--   0     1001      123     3271 2023-06-20 22:21:30.000000 strsim_2-1.0.1/.github/workflows/build.sh
--rw-r--r--   0     1001      123     3060 2023-06-20 22:21:30.000000 strsim_2-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     2641 2023-06-20 22:21:30.000000 strsim_2-1.0.1/.github/workflows/pydiscovery.py
--rw-r--r--   0     1001      123      575 2023-06-20 22:21:30.000000 strsim_2-1.0.1/.gitignore
--rw-r--r--   0     1001      123     1064 2023-06-20 22:21:30.000000 strsim_2-1.0.1/LICENSE
--rw-r--r--   0     1001      123       54 2023-06-20 22:21:30.000000 strsim_2-1.0.1/README.md
--rw-r--r--   0     1001      123       10 2023-06-20 22:22:11.000000 strsim_2-1.0.1/dist/strsim_2-1.0.1.tar.gz
--rw-r--r--   0     1001      123      709 2023-06-20 22:21:30.000000 strsim_2-1.0.1/pyproject.toml
--rw-r--r--   0     1001      123     1301 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/error.rs
--rw-r--r--   0     1001      123      275 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/helper.rs
--rw-r--r--   0     1001      123     4752 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/hybrid_jaccard.rs
--rw-r--r--   0     1001      123     2533 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/jaro.rs
--rw-r--r--   0     1001      123     2154 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/jaro_winkler.rs
--rw-r--r--   0     1001      123     6878 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/levenshtein.rs
--rw-r--r--   0     1001      123     5145 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/lib.rs
--rw-r--r--   0     1001      123     3779 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/monge_elkan.rs
--rw-r--r--   0     1001      123     2840 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/python.rs
--rw-r--r--   0     1001      123     6454 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/tokenizers.rs
--rw-r--r--   0     1001      123      115 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/wrapped_strsim/mod.rs
--rw-r--r--   0     1001      123     2502 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/wrapped_strsim/seq_strsim.rs
--rw-r--r--   0     1001      123     2554 2023-06-20 22:21:30.000000 strsim_2-1.0.1/src/wrapped_strsim/set_strsim.rs
--rw-r--r--   0     1001      123      161 2023-06-20 22:21:30.000000 strsim_2-1.0.1/strsim/__init__.py
--rw-r--r--   0     1001      123      798 2023-06-20 22:21:30.000000 strsim_2-1.0.1/strsim/__init__.pyi
--rw-r--r--   0     1001      123        0 2023-06-20 22:21:30.000000 strsim_2-1.0.1/strsim/py.typed
--rw-r--r--   0     1001      123        0 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/__init__.py
--rw-r--r--   0     1001      123      929 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/common/mod.rs
--rw-r--r--   0     1001      123      967 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/hybrid_jaccard.rs
--rw-r--r--   0     1001      123      977 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/jaro.rs
--rw-r--r--   0     1001      123     1527 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/jaro_winkler.rs
--rw-r--r--   0     1001      123     1781 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/levenshtein.rs
--rw-r--r--   0     1001      123     1167 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/monge_elkan.rs
--rw-r--r--   0     1001      123      554 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/resources/rltk_check.py
--rw-r--r--   0     1001      123    10981 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/resources/strsim_check.ipynb
--rw-r--r--   0     1001      123     1944 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/resources/test_linear_sum_assignment.ipynb
--rw-r--r--   0     1001      123      896 2023-06-20 22:21:30.000000 strsim_2-1.0.1/tests/test_python.py
--rw-r--r--   0     1001      123    11819 2023-06-20 22:21:34.000000 strsim_2-1.0.1/Cargo.lock
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 strsim_2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 strsim_2-1.1.0/Cargo.toml
+-rw-r--r--   0     1001      123     3271 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/build.sh
+-rw-r--r--   0     1001      123     3060 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     2641 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.github/workflows/pydiscovery.py
+-rw-r--r--   0     1001      123      575 2023-07-18 17:29:19.000000 strsim_2-1.1.0/.gitignore
+-rw-r--r--   0     1001      123     1064 2023-07-18 17:29:19.000000 strsim_2-1.1.0/LICENSE
+-rw-r--r--   0     1001      123       54 2023-07-18 17:29:19.000000 strsim_2-1.1.0/README.md
+-rw-r--r--   0     1001      123       10 2023-07-18 17:29:54.000000 strsim_2-1.1.0/dist/strsim_2-1.1.0.tar.gz
+-rw-r--r--   0     1001      123      709 2023-07-18 17:29:19.000000 strsim_2-1.1.0/pyproject.toml
+-rw-r--r--   0     1001      123     1301 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/error.rs
+-rw-r--r--   0     1001      123      275 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/helper.rs
+-rw-r--r--   0     1001      123     4752 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/hybrid_jaccard.rs
+-rw-r--r--   0     1001      123     2533 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/jaro.rs
+-rw-r--r--   0     1001      123     2154 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/jaro_winkler.rs
+-rw-r--r--   0     1001      123     6878 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/levenshtein.rs
+-rw-r--r--   0     1001      123     5145 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/lib.rs
+-rw-r--r--   0     1001      123     3779 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/monge_elkan.rs
+-rw-r--r--   0     1001      123     2840 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/python.rs
+-rw-r--r--   0     1001      123     6454 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/tokenizers.rs
+-rw-r--r--   0     1001      123      115 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/mod.rs
+-rw-r--r--   0     1001      123     2502 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/seq_strsim.rs
+-rw-r--r--   0     1001      123     2554 2023-07-18 17:29:19.000000 strsim_2-1.1.0/src/wrapped_strsim/set_strsim.rs
+-rw-r--r--   0     1001      123      161 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/__init__.py
+-rw-r--r--   0     1001      123      798 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/__init__.pyi
+-rw-r--r--   0     1001      123        0 2023-07-18 17:29:19.000000 strsim_2-1.1.0/strsim/py.typed
+-rw-r--r--   0     1001      123        0 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/__init__.py
+-rw-r--r--   0     1001      123      929 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/common/mod.rs
+-rw-r--r--   0     1001      123      967 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/hybrid_jaccard.rs
+-rw-r--r--   0     1001      123      977 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/jaro.rs
+-rw-r--r--   0     1001      123     1527 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/jaro_winkler.rs
+-rw-r--r--   0     1001      123     1781 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/levenshtein.rs
+-rw-r--r--   0     1001      123     1167 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/monge_elkan.rs
+-rw-r--r--   0     1001      123      554 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/rltk_check.py
+-rw-r--r--   0     1001      123    10981 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/strsim_check.ipynb
+-rw-r--r--   0     1001      123     1944 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/resources/test_linear_sum_assignment.ipynb
+-rw-r--r--   0     1001      123      896 2023-07-18 17:29:19.000000 strsim_2-1.1.0/tests/test_python.py
+-rw-r--r--   0     1001      123    11543 2023-07-18 17:29:21.000000 strsim_2-1.1.0/Cargo.lock
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 strsim_2-1.1.0/PKG-INFO
```

### Comparing `strsim_2-1.0.1/Cargo.toml` & `strsim_2-1.1.0/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "yass-2"
-version = "1.0.1"
+version = "1.1.0"
 edition = "2021"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/strsim"
 repository = "https://github.com/binh-vu/strsim"
 license-file = "LICENSE"
 description = "Yet another string similarity library"
 keywords = ["string-similarity", "strsim", "levenshtein", "jaro-winkler"]
@@ -15,15 +15,15 @@
 
 [dependencies]
 anyhow = "1.0.71"
 derive_more = "0.99.17"
 hashbrown = "0.13.2"
 itertools = "0.10.5"
 lsap = "1.0.2"
-pyo3 = { version = "0.18.3", features = ["anyhow", "multiple-pymethods"] }
+pyo3 = { version = "0.19.1", features = ["anyhow", "multiple-pymethods"] }
 thiserror = "1.0.40"
 
 
 [dev-dependencies]
 approx = "0.5.1"
 maplit = "1.0.2"
```

### Comparing `strsim_2-1.0.1/.github/workflows/build.sh` & `strsim_2-1.1.0/.github/workflows/build.sh`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/.github/workflows/ci.yml` & `strsim_2-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/.github/workflows/pydiscovery.py` & `strsim_2-1.1.0/.github/workflows/pydiscovery.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/.gitignore` & `strsim_2-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/LICENSE` & `strsim_2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/pyproject.toml` & `strsim_2-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "strsim-2"
-version = "1.0.1"
+version = "1.1.0"
 description = "Yet another string similarity library (implemented in Rust)"
 readme = "README.md"
 authors = [
     { name = "Binh Vu", email = "binh@toan2.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `strsim_2-1.0.1/src/error.rs` & `strsim_2-1.1.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/hybrid_jaccard.rs` & `strsim_2-1.1.0/src/hybrid_jaccard.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/jaro.rs` & `strsim_2-1.1.0/src/jaro.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/jaro_winkler.rs` & `strsim_2-1.1.0/src/jaro_winkler.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/levenshtein.rs` & `strsim_2-1.1.0/src/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/lib.rs` & `strsim_2-1.1.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/monge_elkan.rs` & `strsim_2-1.1.0/src/monge_elkan.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/python.rs` & `strsim_2-1.1.0/src/python.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/tokenizers.rs` & `strsim_2-1.1.0/src/tokenizers.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/wrapped_strsim/seq_strsim.rs` & `strsim_2-1.1.0/src/wrapped_strsim/seq_strsim.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/src/wrapped_strsim/set_strsim.rs` & `strsim_2-1.1.0/src/wrapped_strsim/set_strsim.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/strsim/__init__.pyi` & `strsim_2-1.1.0/strsim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/common/mod.rs` & `strsim_2-1.1.0/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/hybrid_jaccard.rs` & `strsim_2-1.1.0/tests/hybrid_jaccard.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/jaro.rs` & `strsim_2-1.1.0/tests/jaro.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/jaro_winkler.rs` & `strsim_2-1.1.0/tests/jaro_winkler.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/levenshtein.rs` & `strsim_2-1.1.0/tests/levenshtein.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/monge_elkan.rs` & `strsim_2-1.1.0/tests/monge_elkan.rs`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/resources/rltk_check.py` & `strsim_2-1.1.0/tests/resources/rltk_check.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/resources/strsim_check.ipynb` & `strsim_2-1.1.0/tests/resources/strsim_check.ipynb`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/resources/test_linear_sum_assignment.ipynb` & `strsim_2-1.1.0/tests/resources/test_linear_sum_assignment.ipynb`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/tests/test_python.py` & `strsim_2-1.1.0/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `strsim_2-1.0.1/Cargo.lock` & `strsim_2-1.1.0/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,17 @@
  "cfg-if",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -68,25 +68,14 @@
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
-name = "ghost"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash",
 ]
@@ -95,35 +84,32 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0539b5de9241582ce6bd6b0ba7399313560151e58c9aaf8b74b711b1bdce644"
-dependencies = [
- "ghost",
-]
+checksum = "25b1d6b4b9fb75fc419bdef998b689df5080a32931cb3395b86202046b56a9ea"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -144,17 +130,17 @@
 name = "maplit"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e2e65a1a2e43cfcb47a895c4c8b10d1f4a61097f9f254f183aee60cad9c651d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.15"
@@ -191,26 +177,26 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
@@ -219,60 +205,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -289,83 +275,83 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.8"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -373,17 +359,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
@@ -430,15 +416,15 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "yass-2"
-version = "1.0.1"
+version = "1.1.0"
 dependencies = [
  "anyhow",
  "approx",
  "derive_more",
  "hashbrown",
  "itertools",
  "lsap",
```

### Comparing `strsim_2-1.0.1/PKG-INFO` & `strsim_2-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strsim-2
-Version: 1.0.1
+Version: 1.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 License-File: LICENSE
 Summary: Yet another string similarity library (implemented in Rust)
```

