# Comparing `tmp/bolt11-1.0.2.tar.gz` & `tmp/bolt11-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt11-1.0.2.tar", max compression
+gzip compressed data, was "bolt11-1.0.3.tar", max compression
```

## Comparing `bolt11-1.0.2.tar` & `bolt11-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1112 2023-07-11 07:15:44.389912 bolt11-1.0.2/LICENSE
--rwxr-xr-x   0        0        0     3119 2023-07-11 07:15:44.389912 bolt11-1.0.2/README.md
--rw-r--r--   0        0        0      353 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/__init__.py
--rw-r--r--   0        0        0     1127 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/bit_utils.py
--rw-r--r--   0        0        0      599 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/cli.py
--rw-r--r--   0        0        0      243 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/compat.py
--rw-r--r--   0        0        0     3932 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/decode.py
--rw-r--r--   0        0        0     2926 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/encode.py
--rw-r--r--   0        0        0     2850 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/fallback.py
--rw-r--r--   0        0        0     3486 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/features.py
--rw-r--r--   0        0        0     1768 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/routehint.py
--rw-r--r--   0        0        0     2322 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/models/signature.py
--rw-r--r--   0        0        0       26 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/py.typed
--rw-r--r--   0        0        0     3962 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/types.py
--rw-r--r--   0        0        0     1947 2023-07-11 07:15:44.389912 bolt11-1.0.2/bolt11/utils.py
--rw-r--r--   0        0        0     1545 2023-07-11 07:15:44.389912 bolt11-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1112 2023-07-18 07:08:24.507071 bolt11-1.0.3/LICENSE
+-rwxr-xr-x   0        0        0     3119 2023-07-18 07:08:24.507071 bolt11-1.0.3/README.md
+-rw-r--r--   0        0        0      353 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/__init__.py
+-rw-r--r--   0        0        0     1127 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/bit_utils.py
+-rw-r--r--   0        0        0      599 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/compat.py
+-rw-r--r--   0        0        0     3932 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/decode.py
+-rw-r--r--   0        0        0     2926 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/encode.py
+-rw-r--r--   0        0        0     2850 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     3226 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/features.py
+-rw-r--r--   0        0        0     1768 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2322 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/models/signature.py
+-rw-r--r--   0        0        0       26 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/py.typed
+-rw-r--r--   0        0        0     3962 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/types.py
+-rw-r--r--   0        0        0     1947 2023-07-18 07:08:24.507071 bolt11-1.0.3/bolt11/utils.py
+-rw-r--r--   0        0        0     1545 2023-07-18 07:08:24.507071 bolt11-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3924 1970-01-01 00:00:00.000000 bolt11-1.0.3/PKG-INFO
```

### Comparing `bolt11-1.0.2/LICENSE` & `bolt11-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/README.md` & `bolt11-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/bit_utils.py` & `bolt11-1.0.3/bolt11/bit_utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/cli.py` & `bolt11-1.0.3/bolt11/cli.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/decode.py` & `bolt11-1.0.3/bolt11/decode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/encode.py` & `bolt11-1.0.3/bolt11/encode.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/models/fallback.py` & `bolt11-1.0.3/bolt11/models/fallback.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/models/features.py` & `bolt11-1.0.3/bolt11/models/features.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from math import floor
-from typing import Dict, NamedTuple, Optional
+from typing import Dict, NamedTuple, Optional, Union
 
 from bitstring import BitArray, Bits
 
 
 class FeatureState(Enum):
     required = 0
     supported = 1
@@ -25,69 +25,50 @@
     option_anchors_zero_fee_htlc_tx = 11
     option_route_blinding = 13
     option_shutdown_anysegwit = 14
     option_channel_type = 15
     option_scid_alias = 16
     option_payment_metadata = 17
     option_zeroconf_chanids = 18
-    extra_1 = 19
-    extra_2 = 20
-    extra_3 = 21
-    extra_4 = 22
-    extra_5 = 23
-    extra_6 = 24
-    extra_7 = 25
-    extra_8 = 26
-    extra_9 = 27
-    extra_10 = 28
-    extra_11 = 29
-    extra_12 = 30
-    extra_13 = 31
-    extra_14 = 32
-    extra_15 = 33
-    extra_16 = 34
-    extra_17 = 35
-    extra_18 = 36
-    extra_19 = 37
-    extra_20 = 38
-    extra_21 = 39
-    extra_22 = 40
-    extra_23 = 41
-    extra_24 = 42
-    extra_25 = 43
-    extra_26 = 44
-    extra_27 = 45
-    extra_28 = 46
-    extra_29 = 47
-    extra_30 = 48
-    extra_31 = 49
+
+
+class FeatureExtra:
+    def __init__(self, index: int):
+        self.feature_index = index
+
+    @property
+    def value(self) -> int:
+        return self.feature_index + len(Feature)
+
+    @property
+    def name(self) -> str:
+        return f"extra_{self.feature_index - len(Feature)}"
 
 
 class Features(NamedTuple):
     data: Bits
-    feature_list: Dict[Feature, FeatureState]
+    feature_list: Dict[Union[Feature, FeatureExtra], FeatureState]
 
     @classmethod
     def from_bitstring(cls, data: Bits) -> "Features":
         length = data.length
-        feature_list: Dict[Feature, FeatureState] = {}
+        feature_list: Dict[Union[Feature, FeatureExtra], FeatureState] = {}
         for i in range(0, length):
             feature_index = floor(i / 2)
-            if floor(i / 2) > len(Feature):
-                raise ValueError(f"Feature index ({i}) out of range, word_length: {length}")
             si = i + 1
             cut = data[-si : -si + 1] if i > 0 else data[-si:]
             if bool(cut):
-                feature = Feature(floor(i / 2))
-                if feature not in feature_list:
-                    feature_list[Feature(feature_index)] = FeatureState.supported if i % 2 else FeatureState.required
+                feature: Union[Feature, FeatureExtra] = (
+                    Feature(feature_index) if feature_index < len(Feature) else FeatureExtra(feature_index)
+                )
+                feature_list[feature] = FeatureState.supported if i % 2 else FeatureState.required
         return cls(data, feature_list)
 
     @classmethod
-    def from_feature_list(cls, feature_list: Dict[Feature, FeatureState]) -> "Features":
+    def from_feature_list(cls, feature_list: Dict[Union[Feature, FeatureExtra], FeatureState]) -> "Features":
         length = max([feature.value + 1 for feature in feature_list]) * 2
         data = BitArray(length=length)
         for feature, feature_state in feature_list.items():
             if feature_state == FeatureState.required:
                 data.invert(feature.value * 2)  # type: ignore
             elif feature_state == FeatureState.supported:
                 data.invert(feature.value * 2 + 1)  # type: ignore
```

### Comparing `bolt11-1.0.2/bolt11/models/routehint.py` & `bolt11-1.0.3/bolt11/models/routehint.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/models/signature.py` & `bolt11-1.0.3/bolt11/models/signature.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/types.py` & `bolt11-1.0.3/bolt11/types.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/bolt11/utils.py` & `bolt11-1.0.3/bolt11/utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-1.0.2/pyproject.toml` & `bolt11-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt11"
-version = "1.0.2"
+version = "1.0.3"
 description = "A library for encoding and decoding BOLT11 payment requests."
 repository = "https://github.com/lnbits/bolt11"
 authors = [
     "eillarra <eneko@illarra.com>",
     "Alan Bits <alan@lnbits.com>"
 ]
 license = "MIT"
@@ -27,15 +27,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 isort = "^5.12.0"
-pyright = "^1.1.293"
+pyright = "^1.1.317"
 pylint = "^2.17.2"
 pre-commit = "^3.3.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bolt11-1.0.2/PKG-INFO` & `bolt11-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt11
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library for encoding and decoding BOLT11 payment requests.
 Home-page: https://github.com/lnbits/bolt11
 License: MIT
 Author: eillarra
 Author-email: eneko@illarra.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

