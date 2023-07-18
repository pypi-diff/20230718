# Comparing `tmp/PH-units-1.4.1.tar.gz` & `tmp/PH-units-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.4.1.tar", last modified: Sun Jul 16 23:08:33 2023, max compression
+gzip compressed data, was "dist/PH-units-1.5.0.tar", last modified: Tue Jul 18 12:43:24 2023, max compression
```

## Comparing `PH-units-1.4.1.tar` & `PH-units-1.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-07-16 23:07:10.000000 PH-units-1.4.1/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-07-16 23:07:10.000000 PH-units-1.4.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-07-16 23:07:10.000000 PH-units-1.4.1/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-16 23:08:33.000000 PH-units-1.4.1/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      781 2023-07-16 23:08:33.000000 PH-units-1.4.1/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-16 23:08:33.000000 PH-units-1.4.1/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-16 23:08:33.000000 PH-units-1.4.1/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-16 23:08:33.000000 PH-units-1.4.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-07-16 23:07:10.000000 PH-units-1.4.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-07-16 23:07:10.000000 PH-units-1.4.1/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5224 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/parser.py
--rw-r--r--   0 runner     (501) staff       (20)     7430 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_type.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-16 23:08:33.000000 PH-units-1.4.1/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2999 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      605 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     1220 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/density.py
--rw-r--r--   0 runner     (501) staff       (20)      763 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/emissions_factors.py
--rw-r--r--   0 runner     (501) staff       (20)     6566 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2681 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)      584 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/moisture_vapor_resistance.py
--rw-r--r--   0 runner     (501) staff       (20)     2474 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1408 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)     1030 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)     1188 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     2354 2023-07-16 23:07:10.000000 PH-units-1.4.1/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-07-16 23:07:10.000000 PH-units-1.4.1/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-07-16 23:08:33.000000 PH-units-1.4.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-16 23:07:10.000000 PH-units-1.4.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-07-18 12:42:01.000000 PH-units-1.5.0/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-07-18 12:42:01.000000 PH-units-1.5.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-07-18 12:42:01.000000 PH-units-1.5.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-18 12:43:24.000000 PH-units-1.5.0/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      781 2023-07-18 12:43:24.000000 PH-units-1.5.0/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-18 12:43:24.000000 PH-units-1.5.0/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-07-18 12:43:24.000000 PH-units-1.5.0/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-07-18 12:43:24.000000 PH-units-1.5.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-07-18 12:42:01.000000 PH-units-1.5.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-07-18 12:42:01.000000 PH-units-1.5.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5224 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/parser.py
+-rw-r--r--   0 runner     (501) staff       (20)     8491 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_type.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-18 12:43:24.000000 PH-units-1.5.0/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2999 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      605 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/density.py
+-rw-r--r--   0 runner     (501) staff       (20)      763 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/emissions_factors.py
+-rw-r--r--   0 runner     (501) staff       (20)     6566 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2681 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)      584 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/moisture_vapor_resistance.py
+-rw-r--r--   0 runner     (501) staff       (20)     2474 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1408 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)     1030 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)     1188 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2023-07-18 12:42:01.000000 PH-units-1.5.0/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-07-18 12:42:01.000000 PH-units-1.5.0/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-07-18 12:43:24.000000 PH-units-1.5.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-07-18 12:42:01.000000 PH-units-1.5.0/setup.py
```

### Comparing `PH-units-1.4.1/.github/workflows/ci.yaml` & `PH-units-1.5.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/LICENSE` & `PH-units-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/PH_units.egg-info/PKG-INFO` & `PH-units-1.5.0/PH_units.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.4.1
+Version: 1.5.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.4.1/PH_units.egg-info/SOURCES.txt` & `PH-units-1.5.0/PH_units.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/PKG-INFO` & `PH-units-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.4.1
+Version: 1.5.0
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.4.1/README.md` & `PH-units-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/converter.py` & `PH-units-1.5.0/ph_units/converter.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/parser.py` & `PH-units-1.5.0/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_type.py` & `PH-units-1.5.0/ph_units/unit_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -151,25 +151,46 @@
             raise TypeError(
                 "Error: Cannot multiply '{}' by '{}'.".format(type(other), self.__class__.__name__)
             )
         if isinstance(other, Unit):
             if self.unit != other.unit:
                 # -- If either unit is a [%] type, should still be able to multiply them together
                 if self.unit in ["%", "-"] or other.unit in ["%", "-"]:
-                    # --find then non-precent unt
+                    # --find then non-percent unt
                     unit_type = self.unit if self.unit != "%" else other.unit
                     return Unit(self.value * other.value, unit_type)
                 else:
                     raise TypeError(
                         "Error: Cannot multiply '{}' by '{}'.".format(self.unit, other.unit)
                     )
             else:
                 return Unit(self.value * other.value, self.unit)
         return Unit(self.value * other, self.unit)
 
+    def __truediv__(self, other):
+        # type: (Union[Unit, int, float]) -> Unit
+        if not isinstance(other, (Unit, float, int)):
+            raise TypeError(
+                "Error: Cannot divide '{}' by '{}'.".format(type(other), self.__class__.__name__)
+            )
+        if isinstance(other, Unit):
+            if self.unit != other.unit:
+                # -- If either unit is a [%] type, should still be able to multiply them together
+                if self.unit in ["%", "-"] or other.unit in ["%", "-"]:
+                    # --find then non-percent unt
+                    unit_type = self.unit if self.unit != "%" else other.unit
+                    return Unit(self.value / other.value, unit_type)
+                else:
+                    raise TypeError(
+                        "Error: Cannot divide '{}' by '{}'.".format(self.unit, other.unit)
+                    )
+            else:
+                return Unit(self.value / other.value, "-")
+        return Unit(self.value / other, self.unit)
+
     def __bool__(self):
         # type: () -> bool
         return True
 
     def __nonzero__(self):
         # type: () -> bool
         return True
@@ -179,31 +200,31 @@
         return iter([self])
 
     def __len__(self):
         # type: () -> int
         return 1
 
     def __eq__(self, other):
-        # type: (Unit) -> bool
+        # type: (Any) -> bool
         if not isinstance(other, Unit):
-            return False
+            return self.value == other
         return self.value == other.value and self.unit == other.unit
 
     def __le__(self, other):
-        # type: (Unit) -> bool
+        # type: (Any) -> bool
         if not isinstance(other, Unit):
-            return False
+            return self.value <= other
         if not self.unit == other.unit:
             raise TypeError("Cannot compare '{}' to '{}'.".format(self.unit, other.unit))
         return self.value <= other.value
 
     def __lt__(self, other):
-        # type: (Unit) -> bool
+        # type: (Any) -> bool
         if not isinstance(other, Unit):
-            return False
+            return self.value < other
         if not self.unit == other.unit:
             raise TypeError("Cannot compare '{}' to '{}'.".format(self.unit, other.unit))
         return self.value < other.value
 
     def __setattr__(self, name, value):
         # type: (str, Any) -> None
         if self._frozen and hasattr(self, name):
```

### Comparing `PH-units-1.4.1/ph_units/unit_types/__init__.py` & `PH-units-1.5.0/ph_units/unit_types/__init__.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/area.py` & `PH-units-1.5.0/ph_units/unit_types/area.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/density.py` & `PH-units-1.5.0/ph_units/unit_types/density.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/emissions_factors.py` & `PH-units-1.5.0/ph_units/unit_types/emissions_factors.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/energy.py` & `PH-units-1.5.0/ph_units/unit_types/energy.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/envelope.py` & `PH-units-1.5.0/ph_units/unit_types/envelope.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/length.py` & `PH-units-1.5.0/ph_units/unit_types/length.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/moisture_vapor_resistance.py` & `PH-units-1.5.0/ph_units/unit_types/moisture_vapor_resistance.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/power.py` & `PH-units-1.5.0/ph_units/unit_types/power.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/speed.py` & `PH-units-1.5.0/ph_units/unit_types/speed.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/temperature.py` & `PH-units-1.5.0/ph_units/unit_types/temperature.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/volume.py` & `PH-units-1.5.0/ph_units/unit_types/volume.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/ph_units/unit_types/volume_flow.py` & `PH-units-1.5.0/ph_units/unit_types/volume_flow.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.4.1/setup.cfg` & `PH-units-1.5.0/setup.cfg`

 * *Files identical despite different names*

