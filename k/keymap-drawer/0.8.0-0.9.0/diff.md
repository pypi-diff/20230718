# Comparing `tmp/keymap_drawer-0.8.0-py3-none-any.whl.zip` & `tmp/keymap_drawer-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 48686 bytes, number of entries: 30
+Zip file size: 48955 bytes, number of entries: 30
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 keymap_drawer/__init__.py
 -rw-r--r--  2.0 unx     6741 b- defN 80-Jan-01 00:00 keymap_drawer/__main__.py
 -rw-r--r--  2.0 unx     9464 b- defN 80-Jan-01 00:00 keymap_drawer/config.py
 -rw-r--r--  2.0 unx    13787 b- defN 80-Jan-01 00:00 keymap_drawer/draw.py
 -rw-r--r--  2.0 unx     5784 b- defN 80-Jan-01 00:00 keymap_drawer/dts.py
 -rw-r--r--  2.0 unx     5798 b- defN 80-Jan-01 00:00 keymap_drawer/glyph.py
 -rw-r--r--  2.0 unx     9388 b- defN 80-Jan-01 00:00 keymap_drawer/keymap.py
--rw-r--r--  2.0 unx    15866 b- defN 80-Jan-01 00:00 keymap_drawer/parse.py
+-rw-r--r--  2.0 unx    17235 b- defN 80-Jan-01 00:00 keymap_drawer/parse.py
 -rw-r--r--  2.0 unx    12301 b- defN 80-Jan-01 00:00 keymap_drawer/physical_layout.py
--rw-r--r--  2.0 unx     4183 b- defN 80-Jan-01 00:00 resources/qmk_layouts/adv360.json
+-rw-r--r--  2.0 unx     3571 b- defN 80-Jan-01 00:00 resources/qmk_layouts/adv360.json
 -rw-r--r--  2.0 unx     2114 b- defN 80-Jan-01 00:00 resources/qmk_layouts/berylline.json
 -rw-r--r--  2.0 unx     2267 b- defN 80-Jan-01 00:00 resources/qmk_layouts/chocofi.json
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 resources/qmk_layouts/clog.json
 -rw-r--r--  2.0 unx     3502 b- defN 80-Jan-01 00:00 resources/qmk_layouts/corne_rotated.json
 -rw-r--r--  2.0 unx     3684 b- defN 80-Jan-01 00:00 resources/qmk_layouts/fingerpunch@ffkb.json
 -rw-r--r--  2.0 unx     2153 b- defN 80-Jan-01 00:00 resources/qmk_layouts/fingerpunch@luakeeb.json
 -rw-r--r--  2.0 unx     3353 b- defN 80-Jan-01 00:00 resources/qmk_layouts/glove80.json
@@ -20,13 +20,13 @@
 -rw-r--r--  2.0 unx     2537 b- defN 80-Jan-01 00:00 resources/qmk_layouts/klotz.json
 -rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 resources/qmk_layouts/osprey.json
 -rw-r--r--  2.0 unx     2466 b- defN 80-Jan-01 00:00 resources/qmk_layouts/paroxysm.json
 -rw-r--r--  2.0 unx     3728 b- defN 80-Jan-01 00:00 resources/qmk_layouts/revxlp.json
 -rw-r--r--  2.0 unx     2838 b- defN 80-Jan-01 00:00 resources/qmk_layouts/rufous.json
 -rw-r--r--  2.0 unx     2803 b- defN 80-Jan-01 00:00 resources/qmk_layouts/totem.json
 -rw-r--r--  2.0 unx     6244 b- defN 80-Jan-01 00:00 resources/zmk_keyboard_layouts.yaml
--rw-r--r--  2.0 unx    26110 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2619 b- defN 16-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/RECORD
-30 files, 165145 bytes uncompressed, 44452 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx    26110 b- defN 80-Jan-01 00:00 keymap_drawer-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 keymap_drawer-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 keymap_drawer-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 keymap_drawer-0.9.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2619 b- defN 16-Jan-01 00:00 keymap_drawer-0.9.0.dist-info/RECORD
+30 files, 165902 bytes uncompressed, 44721 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -69,23 +69,23 @@
 
 Filename: resources/qmk_layouts/totem.json
 Comment: 
 
 Filename: resources/zmk_keyboard_layouts.yaml
 Comment: 
 
-Filename: keymap_drawer-0.8.0.dist-info/METADATA
+Filename: keymap_drawer-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: keymap_drawer-0.8.0.dist-info/WHEEL
+Filename: keymap_drawer-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: keymap_drawer-0.8.0.dist-info/LICENSE
+Filename: keymap_drawer-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: keymap_drawer-0.8.0.dist-info/entry_points.txt
+Filename: keymap_drawer-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: keymap_drawer-0.8.0.dist-info/RECORD
+Filename: keymap_drawer-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keymap_drawer/parse.py

```diff
@@ -13,60 +13,74 @@
 from .config import ParseConfig
 from .dts import DeviceTree
 
 
 ZMK_LAYOUTS_PATH = Path(__file__).parent.parent / "resources" / "zmk_keyboard_layouts.yaml"
 
 
-class KeymapParser(ABC):
+class KeymapParser(ABC):  # pylint: disable=too-many-instance-attributes
     """Abstract base class for parsing firmware keymap representations."""
 
     def __init__(
         self,
         config: ParseConfig,
         columns: int | None,
         base_keymap: KeymapData | None = None,
         layer_names: list[str] | None = None,
     ):
         self.cfg = config
         self.columns = columns if columns is not None else 0
         self.layer_names: list[str] | None = layer_names
         self.base_keymap = base_keymap
-        self.layer_activated_from: dict[int, set[int]] = {}
+        self.layer_activated_from: dict[int, set[int]] = {}  # layer to key positions
+        self.conditional_layers: dict[int, list[int]] = {}  # then-layer to if-layers mapping
         self.trans_key = LayoutKey.from_key_spec(self.cfg.trans_legend)
         self.raw_binding_map = self.cfg.raw_binding_map.copy()
 
-    def update_layer_activated_from(self, from_layer: int | None, to_layer: int, key_positions: Sequence[int]) -> None:
+    def update_layer_activated_from(
+        self, from_layers: Sequence[int], to_layer: int, key_positions: Sequence[int]
+    ) -> None:
         """
         Update the data structure that keeps track of what keys were held (i.e. momentary layer keys)
         in order to activate a given layer. Also considers what keys were already being held in order
-        to activate the `from_layer` that the `to_layer` is being activated from.
+        to activate the `from_layers` that the `to_layer` is being activated from.
+
+        `from_layers` can be empty (e.g. for combos) or have multiple elements (for conditional layers).
 
         In order to properly keep track of multiple layer activation sequences, this method needs
         to be called in the order of increasing `to_layer` indices. It also ignores activating lower
         layer indices from higher layers and only considers the first discovered keys.
         """
         # ignore reverse order activations and if we already have a way to get to this layer
-        if (from_layer is not None and from_layer >= to_layer) or to_layer in self.layer_activated_from:
+        if (from_layers and any(layer >= to_layer for layer in from_layers)) or to_layer in self.layer_activated_from:
             return
+
         self.layer_activated_from[to_layer] = set(key_positions)  # came here through these key(s)
+
         # also consider how the layer we are coming from got activated
-        if from_layer is not None:
+        for from_layer in from_layers:
             self.layer_activated_from[to_layer] |= self.layer_activated_from.get(from_layer, set())
 
     def add_held_keys(self, layers: dict[str, list[LayoutKey]]) -> dict[str, list[LayoutKey]]:
         """Add "held" specifiers to keys that we previously determined were held to activate a given layer."""
         assert self.layer_names is not None
+
+        # handle conditional layers
+        for then_layer, if_layers in sorted(self.conditional_layers.items()):
+            self.update_layer_activated_from(if_layers, then_layer, [])
+
+        # assign held keys
         for layer_index, activating_keys in self.layer_activated_from.items():
             for key_idx in activating_keys:
                 key = layers[self.layer_names[layer_index]][key_idx]
                 if key == self.trans_key:  # clear legend if it is a transparent key
                     layers[self.layer_names[layer_index]][key_idx] = LayoutKey(type="held")
                 else:
                     key.type = "held"
+
         return layers
 
     def _parse(self, in_str: str, file_name: str | None = None) -> tuple[dict, KeymapData]:
         raise NotImplementedError
 
     def parse(self, in_buf: TextIOWrapper) -> dict:
         """Wrapper to call parser on a file handle and do post-processing after firmware-specific parsing."""
@@ -109,33 +123,33 @@
 
         key_str = self._prefix_re.sub("", key_str)
 
         if m := self._trans_re.fullmatch(key_str):  # transparent
             return self.trans_key
         if m := self._mo_re.fullmatch(key_str):  # momentary layer
             to_layer = int(m.group(1).strip())
-            self.update_layer_activated_from(current_layer, to_layer, key_positions)
+            self.update_layer_activated_from([current_layer], to_layer, key_positions)
             return LayoutKey(tap=self.layer_names[to_layer])
         if m := self._mts_re.fullmatch(key_str):  # short mod-tap syntax
             tap_key = mapped(m.group(2).strip())
             return LayoutKey(tap=tap_key.tap, hold=m.group(1), shifted=tap_key.shifted)
         if m := self._mtl_re.fullmatch(key_str):  # long mod-tap syntax
             tap_key = mapped(m.group(2).strip())
             return LayoutKey(tap=tap_key.tap, hold=m.group(1).strip(), shifted=tap_key.shifted)
         if m := self._lt_re.fullmatch(key_str):  # layer-tap
             to_layer = int(m.group(1).strip())
-            self.update_layer_activated_from(current_layer, to_layer, key_positions)
+            self.update_layer_activated_from([current_layer], to_layer, key_positions)
             tap_key = mapped(m.group(2).strip())
             return LayoutKey(tap=tap_key.tap, hold=self.layer_names[to_layer], shifted=tap_key.shifted)
         if m := self._osm_re.fullmatch(key_str):  # one-shot mod
             tap_key = mapped(m.group(1).strip())
             return LayoutKey(tap=tap_key.tap, hold=self.cfg.sticky_label, shifted=tap_key.shifted)
         if m := self._osl_re.fullmatch(key_str):  # one-shot layer
             to_layer = int(m.group(1).strip())
-            self.update_layer_activated_from(current_layer, to_layer, key_positions)
+            self.update_layer_activated_from([current_layer], to_layer, key_positions)
             return LayoutKey(tap=self.layer_names[to_layer], hold=self.cfg.sticky_label)
         return mapped(key_str)
 
     def _parse(self, in_str: str, file_name: str | None = None) -> tuple[dict, KeymapData]:
         """
         Parse a JSON keymap with its file content and path (unused), then return the layout spec and KeymapData
         to be dumped to YAML.
@@ -180,15 +194,15 @@
         config: ParseConfig,
         columns: int | None,
         base_keymap: KeymapData | None = None,
         layer_names: list[str] | None = None,
     ):
         super().__init__(config, columns, base_keymap, layer_names)
         self.hold_taps = {"&mt": ["&kp", "&kp"], "&lt": ["&mo", "&kp"]}
-        self.mod_morphs: dict[str, list[str]] = {}
+        self.mod_morphs = {"&gresc": ["&kp ESC", "&kp GRAVE"]}
         self.sticky_keys = {"&sk": ["&kp"], "&sl": ["&mo"]}
 
     def _update_raw_binding_map(self, dts: DeviceTree) -> None:
         raw_keys = list(self.raw_binding_map.keys())
         prep_keys = dts.preprocess_extra_data("\n".join(raw_keys)).splitlines()
         assert len(raw_keys) == len(
             prep_keys
@@ -232,15 +246,17 @@
             case [ref, par] if ref in self.sticky_keys:
                 l_key = self._str_to_key(f"{self.sticky_keys[ref][0]} {par}", current_layer, key_positions)
                 return LayoutKey(tap=l_key.tap, hold=self.cfg.sticky_label, shifted=l_key.shifted)
             case [("&out" | "&bt" | "&ext_power" | "&rgb_ug"), *pars]:
                 return LayoutKey(tap=" ".join(pars).replace("_", " ").replace(" SEL ", " "))
             case [("&mo" | "&to" | "&tog") as behavior, par]:
                 if behavior in ("&mo",):
-                    self.update_layer_activated_from(current_layer, int(par), key_positions)
+                    self.update_layer_activated_from(
+                        [current_layer] if current_layer is not None else [], int(par), key_positions
+                    )
                 return LayoutKey(tap=self.layer_names[int(par)])
             case [ref, hold_par, tap_par] if ref in self.hold_taps:
                 hold_key = self._str_to_key(f"{self.hold_taps[ref][0]} {hold_par}", current_layer, key_positions)
                 tap_key = self._str_to_key(f"{self.hold_taps[ref][1]} {tap_par}", current_layer, key_positions)
                 return LayoutKey(tap=tap_key.tap, hold=hold_key.tap, shifted=tap_key.shifted)
             case [ref] | [ref, "0"]:
                 return LayoutKey(tap=ref)
@@ -257,14 +273,24 @@
                 out[f"&{node.label}"] = bindings[:n_bindings]
             return out
 
         self.hold_taps |= get_behavior_bindings("zmk,behavior-hold-tap", 2)
         self.mod_morphs |= get_behavior_bindings("zmk,behavior-mod-morph", 2)
         self.sticky_keys |= get_behavior_bindings("zmk,behavior-sticky-key", 1)
 
+    def _update_conditional_layers(self, dts: DeviceTree) -> None:
+        cl_parents = dts.get_compatible_nodes("zmk,conditional-layers")
+        cl_nodes = [node for parent in cl_parents for node in parent.children]
+        for node in cl_nodes:
+            if not (then_layer_val := node.get_array("then-layer")):
+                raise RuntimeError(f'Could not parse `then-layer` for conditional layer node "{node.name}"')
+            if not (if_layers := node.get_array("if-layers")):
+                raise RuntimeError(f'Could not parse `if-layers` for conditional layer node "{node.name}"')
+            self.conditional_layers[int(then_layer_val[0])] = [int(val) for val in if_layers]
+
     def _get_layers(self, dts: DeviceTree) -> dict[str, list[LayoutKey]]:
         if not (layer_parents := dts.get_compatible_nodes("zmk,keymap")):
             raise RuntimeError('Could not find any keymap nodes with "zmk,keymap" compatible property')
 
         layer_nodes = [node for parent in layer_parents for node in parent.children]
         if self.layer_names is None:
             self.layer_names = [
@@ -318,14 +344,15 @@
         """
         dts = DeviceTree(in_str, file_name, self.cfg.preprocess)
 
         if self.cfg.preprocess and self.raw_binding_map:
             self._update_raw_binding_map(dts)
 
         self._update_behaviors(dts)
+        self._update_conditional_layers(dts)
         layers = self._get_layers(dts)
         combos = self._get_combos(dts)
         layers = self.add_held_keys(layers)
 
         keymap_data = KeymapData(layers=layers, combos=combos, layout=None, config=None)
 
         if not file_name:
```

## resources/qmk_layouts/adv360.json

### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'layouts'": "{'LAYOUT': {'layout': {delete: [61, 60, 58, 57, 55, 54, 38, 37]}}}"}*

```diff
@@ -158,30 +158,14 @@
                     "r": 15,
                     "rx": 5.25,
                     "ry": 4,
                     "x": 7.75,
                     "y": 4
                 },
                 {
-                    "h": 0,
-                    "r": 15,
-                    "rx": 5.25,
-                    "ry": 4,
-                    "x": 6.75,
-                    "y": 5
-                },
-                {
-                    "h": 0,
-                    "r": -15,
-                    "rx": 12.75,
-                    "ry": 4,
-                    "x": 10.25,
-                    "y": 5
-                },
-                {
                     "r": -15,
                     "rx": 12.75,
                     "ry": 4,
                     "x": 9.25,
                     "y": 4
                 },
                 {
@@ -242,76 +226,28 @@
                     "y": 3
                 },
                 {
                     "x": 5.25,
                     "y": 3
                 },
                 {
-                    "h": 0,
-                    "r": 15,
-                    "rx": 5.25,
-                    "ry": 4,
-                    "x": 5.75,
-                    "y": 5
-                },
-                {
-                    "h": 0,
-                    "r": 15,
-                    "rx": 5.25,
-                    "ry": 4,
-                    "x": 6.75,
-                    "y": 5
-                },
-                {
                     "r": 15,
                     "rx": 5.25,
                     "ry": 4,
                     "x": 7.75,
                     "y": 5
                 },
                 {
-                    "h": 0,
-                    "r": 15,
-                    "rx": 5.25,
-                    "ry": 4,
-                    "x": 6.75,
-                    "y": 5
-                },
-                {
-                    "h": 0,
-                    "r": -15,
-                    "rx": 12.75,
-                    "ry": 4,
-                    "x": 10.25,
-                    "y": 5
-                },
-                {
                     "r": -15,
                     "rx": 12.75,
                     "ry": 4,
                     "x": 9.25,
                     "y": 5
                 },
                 {
-                    "h": 0,
-                    "r": -15,
-                    "rx": 12.75,
-                    "ry": 4,
-                    "x": 10.25,
-                    "y": 5
-                },
-                {
-                    "h": 0,
-                    "r": -15,
-                    "rx": 12.75,
-                    "ry": 4,
-                    "x": 11.25,
-                    "y": 5
-                },
-                {
                     "x": 11.75,
                     "y": 3
                 },
                 {
                     "x": 12.75,
                     "y": 3
                 },
```

## Comparing `keymap_drawer-0.8.0.dist-info/METADATA` & `keymap_drawer-0.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keymap-drawer
-Version: 0.8.0
+Version: 0.9.0
 Summary: A module and CLI tool to help parse and draw keyboard layouts.
 Home-page: https://github.com/caksoylar/keymap-drawer
 License: MIT
 Author: Cem Aksoylar
 Author-email: caksoylar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `keymap_drawer-0.8.0.dist-info/LICENSE` & `keymap_drawer-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keymap_drawer-0.8.0.dist-info/RECORD` & `keymap_drawer-0.9.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 keymap_drawer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keymap_drawer/__main__.py,sha256=k-j2SVcBBfoJ-zRW8rrDuH0nr2GzEhScadabb0HnREM,6741
 keymap_drawer/config.py,sha256=XvhCymSdfeWj7Vt2WePigyeIyPKnODFYqqpArRxzsYw,9464
 keymap_drawer/draw.py,sha256=xPMt0meDsywAjA1V4GfwsBhDj-KRmOJunBjPX-FdsOY,13787
 keymap_drawer/dts.py,sha256=bBrkdwDxfNYcag5ppyp5KoemZ1SJjMsFqsLbDs5I0zo,5784
 keymap_drawer/glyph.py,sha256=bLDtb_Zcl6fHMCxJ6JGcgogcXhb-U84fkEHDckDvR1s,5798
 keymap_drawer/keymap.py,sha256=saEQG30NgVftS7cax60aHmx9i1WHiEm4RZdm1p0yGSk,9388
-keymap_drawer/parse.py,sha256=wGWeY9D3YVYZWh_dOjZY9-jeFi7h9T2GuRDejIKTh74,15866
+keymap_drawer/parse.py,sha256=Lw6UefT1T18mcPRNZIuTlqEmsbdXCmHgxwdy3mY0wRU,17235
 keymap_drawer/physical_layout.py,sha256=xKtFg3p9DjVBURHdA0KpU6vPKFr3gkxmaDc0cjoo1v0,12301
-resources/qmk_layouts/adv360.json,sha256=MM5xOXcn9-O4hzei6RPJoFhLbqz86fEqczdqGU6N2uE,4183
+resources/qmk_layouts/adv360.json,sha256=ye0KHz_y1hWjbV1WRw405igP94U-VFOQbDrfd-3vcko,3571
 resources/qmk_layouts/berylline.json,sha256=lsTJzCcQ78TeYUYoBa67fAb4cm6_phrwL9eHphw4qq4,2114
 resources/qmk_layouts/chocofi.json,sha256=Lsayi_fcsljEGGmQwmI_KLUf7snLy_qEqSSVbFcpEkQ,2267
 resources/qmk_layouts/clog.json,sha256=wzkTRyevr0OkZoFNJkWRQ8APpKQ3S5cBiuwdxSnTRt8,2437
 resources/qmk_layouts/corne_rotated.json,sha256=8hTZZSuP4C2p9ywDtnW4o8ThNC9Zw0ue9qwGX1aaOXk,3502
 resources/qmk_layouts/fingerpunch@ffkb.json,sha256=toAtmnP65nnEGE-alZUGShf5E-l58vvl3nipRBBh9hQ,3684
 resources/qmk_layouts/fingerpunch@luakeeb.json,sha256=-kfdKkkZKYZgaippjtyGY1fDDsq_is0j4fJwabY2jVg,2153
 resources/qmk_layouts/glove80.json,sha256=nVaOqX5UofUcPIstYu29pT1vPyqyNpV8cXcX4e0b8Dk,3353
@@ -19,12 +19,12 @@
 resources/qmk_layouts/klotz.json,sha256=jV-tpL1FixKxk78_EnW4UvfricUYsFfFbWf-j1SeY7Y,2537
 resources/qmk_layouts/osprey.json,sha256=_2qw3uVKeuZNybUEhWpcy0U831lldj1LfH6szXeh_j4,1783
 resources/qmk_layouts/paroxysm.json,sha256=y17689V0dqnDhmDgxlzw1kPnNaQub-GHgrsa4-kEV_8,2466
 resources/qmk_layouts/revxlp.json,sha256=FRFgeD6PAQAwDg1gVEZPJl7-tPdTFv7HSQ7Pc-62hgI,3728
 resources/qmk_layouts/rufous.json,sha256=6VtvTikJtgEYx0xfkSTT9_KaLdW5TfmoFoaz0uf5GYQ,2838
 resources/qmk_layouts/totem.json,sha256=HXKwNwjT9lByzFhqlAFhxhhp_SYerOsTasJwUppCh4U,2803
 resources/zmk_keyboard_layouts.yaml,sha256=jC_CzZWmyIXWAIxSER877imSqI0u_0trMzxBLQDIsL0,6244
-keymap_drawer-0.8.0.dist-info/METADATA,sha256=3rFGcmy7cEIaY9grVDm8lNsZ05eb75rxAA7Ld1dT7ko,26110
-keymap_drawer-0.8.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-keymap_drawer-0.8.0.dist-info/LICENSE,sha256=ym_5D56d6k2MroMU8y9ZDt1ZUI4H7PYgbfa87rNFCaM,1069
-keymap_drawer-0.8.0.dist-info/entry_points.txt,sha256=kog7wHfRs-vFQWhh8V3H-Ra4UPbW1nINE9VHJZ1aK2w,54
-keymap_drawer-0.8.0.dist-info/RECORD,,
+keymap_drawer-0.9.0.dist-info/METADATA,sha256=5o6lkdtRgtWq6HPEBgLE_AvLRoJhmaGcljOXaPEpDhw,26110
+keymap_drawer-0.9.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+keymap_drawer-0.9.0.dist-info/LICENSE,sha256=ym_5D56d6k2MroMU8y9ZDt1ZUI4H7PYgbfa87rNFCaM,1069
+keymap_drawer-0.9.0.dist-info/entry_points.txt,sha256=kog7wHfRs-vFQWhh8V3H-Ra4UPbW1nINE9VHJZ1aK2w,54
+keymap_drawer-0.9.0.dist-info/RECORD,,
```

