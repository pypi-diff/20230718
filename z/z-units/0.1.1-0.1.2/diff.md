# Comparing `tmp/z_units-0.1.1.tar.gz` & `tmp/z_units-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z_units-0.1.1.tar", last modified: Tue Jun 20 15:41:23 2023, max compression
+gzip compressed data, was "z_units-0.1.2.tar", last modified: Tue Jul 18 14:22:12 2023, max compression
```

## Comparing `z_units-0.1.1.tar` & `z_units-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.1/LICENSE
--rw-r--r--   0        0        0      739 2023-06-20 15:09:52.178275 z_units-0.1.1/README.md
--rw-r--r--   0        0        0      482 2023-06-20 15:41:23.750115 z_units-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-06-13 15:10:39.946194 z_units-0.1.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1339 2023-06-20 15:32:51.630557 z_units-0.1.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-06-20 15:32:51.630557 z_units-0.1.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    18855 2023-05-27 13:51:23.872491 z_units-0.1.1/tests/test_quantity.py
--rw-r--r--   0        0        0      369 2023-06-14 16:10:41.774469 z_units-0.1.1/tests/test_unit.py
--rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.1/z_units/__init__.py
--rw-r--r--   0        0        0     1099 2023-06-20 15:09:52.182275 z_units-0.1.1/z_units/config.py
--rw-r--r--   0        0        0       93 2023-05-27 13:51:23.872491 z_units-0.1.1/z_units/constant.py
--rw-r--r--   0        0        0     4785 2023-05-30 13:53:30.266379 z_units-0.1.1/z_units/quantity.py
--rw-r--r--   0        0        0    21352 2023-06-14 16:13:18.996833 z_units-0.1.1/z_units/unit.py
--rw-r--r--   0        0        0     9232 2023-06-02 15:07:02.749962 z_units-0.1.1/z_units/unit_registry.py
--rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.1/z_units/util.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 z_units-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1524 2023-07-18 14:19:21.237992 z_units-0.1.2/README.md
+-rw-r--r--   0        0        0      482 2023-07-18 14:22:12.751657 z_units-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-07-02 15:02:03.569818 z_units-0.1.2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1339 2023-07-03 15:10:37.598530 z_units-0.1.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-07-03 15:10:37.598530 z_units-0.1.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    19021 2023-07-02 15:02:03.269821 z_units-0.1.2/tests/test_quantity.py
+-rw-r--r--   0        0        0      476 2023-06-27 16:02:52.925927 z_units-0.1.2/tests/test_unit.py
+-rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.2/z_units/__init__.py
+-rw-r--r--   0        0        0     1096 2023-07-02 15:02:03.271815 z_units-0.1.2/z_units/config.py
+-rw-r--r--   0        0        0       91 2023-07-02 15:02:03.264838 z_units-0.1.2/z_units/constant.py
+-rw-r--r--   0        0        0     5132 2023-07-10 15:01:56.710109 z_units-0.1.2/z_units/quantity.py
+-rw-r--r--   0        0        0    23140 2023-07-03 15:10:37.389231 z_units-0.1.2/z_units/unit.py
+-rw-r--r--   0        0        0     9232 2023-06-02 15:07:02.749962 z_units-0.1.2/z_units/unit_registry.py
+-rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.2/z_units/util.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 z_units-0.1.2/PKG-INFO
```

### Comparing `z_units-0.1.1/LICENSE` & `z_units-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `z_units-0.1.1/tests/.pytest_cache/v/cache/nodeids` & `z_units-0.1.2/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `z_units-0.1.1/tests/test_quantity.py` & `z_units-0.1.2/tests/test_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,31 @@
 from z_units.config import set_local_atmospheric_pressure, set_standard_temperature
 
 
 def test_length():
     x = q.Length(1)
     assert x.unit.symbol == 'm'
     assert x.unit == x.base_unit
+    assert f'{x:U}' == '1 m'
+    assert f'{x:Uq}' == '1 m'
+    assert f'{x:Up}' == '1 m'
     assert isclose(x.to('km').value, 1e-3, rel_tol=1e-4)
     assert isclose(x.to('dm').value, 1e1, rel_tol=1e-4)
     assert isclose(x.to('cm').value, 1e2, rel_tol=1e-4)
     assert isclose(x.to('mm').value, 1e3, rel_tol=1e-4)
     assert isclose(x.to('um').value, 1e6, rel_tol=1e-4)
     assert isclose(x.to('ft').value, 3.28084, rel_tol=1e-4)
     assert isclose(x.to('in').value, 39.37008, rel_tol=1e-4)
 
 
 def test_area():
     x = q.Area(1)
     assert x.unit.symbol == 'm2'
+    assert f'{x:U}' == '1 m2'
+    assert f'{x:Up}' == '1 m**2'
     assert x.unit == x.base_unit
     assert isclose(x.to('km2').value, 1e-6, rel_tol=1e-4)
     assert isclose(x.to('dm2').value, 1e2, rel_tol=1e-4)
     assert isclose(x.to('cm2').value, 1e4, rel_tol=1e-4)
     assert isclose(x.to('mm2').value, 1e6, rel_tol=1e-4)
     assert isclose(x.to('um2').value, 1e12, rel_tol=1e-4)
     assert isclose(x.to('ft2').value, 10.7639, rel_tol=1e-4)
@@ -142,15 +147,15 @@
     assert x.unit == x.base_unit
     assert isclose(x.to('K').value, 1, rel_tol=1e-4)
     assert isclose(x.to('R').value, 1.8, rel_tol=1e-4)
     assert isclose(x.to('F').value, 1.8, rel_tol=1e-4)
 
 
 def test_pressure():
-    x = q.Pressure(100)
+    x = q.Pressure(100, 'kPa')
     assert x.value == 100
     assert x.unit.symbol == 'kPa'
     assert isclose(x.to('Pa').value, 100e3)
     assert isclose(x.to('MPa').value, 100e-3)
     assert isclose(x.to('bar').value, 100e-2)
     assert isclose(x.to('mbar').value, 1000)
     assert isclose(x.to('kgf/cm2').value, 1.019716, rel_tol=1e-4)
@@ -168,15 +173,15 @@
     assert isclose(x.to('psig').value, -0.19218, rel_tol=1e-4)
     assert isclose(x.to('lbf/ft2_g').value, -27.673, rel_tol=1e-4)
     assert isclose(x.to('torr_g').value, -9.9385, rel_tol=1e-4)
     assert isclose(x.to('mmHg_0C_g').value, -9.9385, rel_tol=1e-4)
     assert isclose(x.to('inHg_32F_g').value, -0.39127, rel_tol=1e-4)
     assert isclose(x.to('inHg_60F_g').value, -0.39237, rel_tol=1e-4)
     assert isclose(q.Pressure(1, 'MPag').to('psi').value, 159.73368651, rel_tol=1e-4)
-    set_local_atmospheric_pressure(50)
+    set_local_atmospheric_pressure(50e3)
     assert isclose(x.to('kPag').value, 50)
 
 
 def test_volume_flow():
     v = q.VolumeFlow(1)
     assert v.unit.symbol == 'm3/s'
     assert v.base_unit.symbol == v.unit.symbol
```

### Comparing `z_units-0.1.1/z_units/config.py` & `z_units-0.1.2/z_units/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 def get_standard_temperature():
     return _config['standard_temperature']
 
 
 def set_local_atmospheric_pressure(pressure):
     """
     Set local atmospheric pressure for gauge pressure conversion,
-    default value is 101.325 kPa
-    :param pressure: number in 'kPa'
+    default value is 101325 Pa
+    :param pressure: number in 'Pa'
     :return:
     """
     if isinstance(pressure, (int, float)):
         value = pressure
     else:
         raise ValueError(f"{pressure} is not a number.")
     _config['local_atmospheric_pressure'] = value
```

### Comparing `z_units-0.1.1/z_units/quantity.py` & `z_units-0.1.2/z_units/quantity.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,23 @@
         if isinstance(self.value, float):
             return f"<{self.__class__.__name__}({self.value:.9}, '{self.unit.symbol}')>"
         return f"<{self.__class__.__name__}({self.value}, '{self.unit.symbol}')>"
 
     def __str__(self):
         return f'{self.value}'
 
+    def __format__(self, format_spec=''):
+        if (pos := format_spec.find('u')) > -1:
+            unit = format(self.unit, format_spec[pos + 1:])
+            format_spec = format_spec[0:pos]
+            if unit:
+                return ' '.join([format(self.value, format_spec), unit])
+
+        return format(self.value, format_spec)
+
     @property
     def unit(self) -> Unit:
         return self._unit
 
 
 class Length(Quantity):
     def get_unit_registry(self):
```

### Comparing `z_units-0.1.1/z_units/unit_registry.py` & `z_units-0.1.2/z_units/unit_registry.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.1/z_units/util.py` & `z_units-0.1.2/z_units/util.py`

 * *Files identical despite different names*

### Comparing `z_units-0.1.1/PKG-INFO` & `z_units-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: z-units
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple unit converter for chemical engineering
 Author-Email: zenius <zenius@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zxzenius/z-units
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # z-units
 
-A simple unit converter for chemical engineering
+A simple unit-converter for chemical engineers
 
-## install
+## Feature
+
+* Gauge pressure (MPag, kPag, psig, ...) can be used
+* Friendly to HYSYS user
+
+## Install
 
 ```shell
 pip install z-units
 ```
 
 ## Usage
 
@@ -27,19 +32,60 @@
 # to base unit
 f.to_base()
 # convert
 f.to('kmol/s')
 # list available units
 print(f.units)
 # get value
-unit, value = f.unit, f.value
+value, unit = f.value, f.unit
 # gauge pressure
 p = q.Pressure(5, 'bar').to('MPag')
-# change local atmospheric pressure (default: 101.325 kPa)
+# change local atmospheric pressure (default: 101325 Pa)
 from z_units import config
-config.set_local_atmospheric_pressure(50)
+config.set_local_atmospheric_pressure(50e3)
 q.Pressure(100, 'kPa').to('kPag')
 # change standard temperature (default: 20 degC)
 # affect standard cubic meter "Sm**3"
 config.set_standard_temperature(15)
 q.Substance(100, 'Nm3').to('Sm3')
-```
+# formatting
+# with unit in styles, format spec starts with "u"
+format(q.MolarEntropy(100), 'u')
+# '100 kJ/kmol-C' (quick-style)
+format(q.MolarEntropy(100), 'up')
+# '100 kJ/(kmol*C)' (expression-style)
+```
+
+## Predefined Quantities
+
+* Length
+* Area
+* Volume
+* Time
+* Mass
+* Force
+* Substance
+* Energy
+* Velocity
+* Temperature
+* DeltaTemperature
+* Pressure
+* VolumeFlow
+* MassDensity
+* HeatFlow
+* MolarFlow
+* MassFlow
+* MolarDensity
+* MolarHeatCapacity
+* MolarEntropy
+* MolarHeat
+* ThermalConductivity
+* Viscosity
+* SurfaceTension
+* MassHeatCapacity
+* MassEntropy
+* MassHeat
+* StandardGasFlow
+* KinematicViscosity
+* MolarVolume
+* Fraction
+* Dimensionless
```

