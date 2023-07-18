# Comparing `tmp/trad-0.1.0.tar.gz` & `tmp/trad-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trad-0.1.0.tar", max compression
+gzip compressed data, was "trad-0.1.1.tar", max compression
```

## Comparing `trad-0.1.0.tar` & `trad-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-06-21 19:21:38.903040 trad-0.1.0/LICENSE
--rw-r--r--   0        0        0      513 2023-06-21 19:21:38.903040 trad-0.1.0/README.rst
--rw-r--r--   0        0        0      640 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/__init__.py
--rw-r--r--   0        0        0      848 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/helper.py
--rw-r--r--   0        0        0      909 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/plasma.py
--rw-r--r--   0        0        0     2197 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/specradiance.py
--rw-r--r--   0        0        0     4044 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/sync.py
--rw-r--r--   0        0        0     1745 2023-06-21 19:21:38.903040 trad-0.1.0/mod/trad/units.py
--rw-r--r--   0        0        0      580 2023-06-21 19:21:38.903040 trad-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 trad-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-18 05:02:34.792009 trad-0.1.1/LICENSE
+-rw-r--r--   0        0        0      513 2023-07-18 05:02:34.792009 trad-0.1.1/README.rst
+-rw-r--r--   0        0        0      640 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/__init__.py
+-rw-r--r--   0        0        0      848 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/helper.py
+-rw-r--r--   0        0        0     1041 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/plasma.py
+-rw-r--r--   0        0        0     2204 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/specradiance.py
+-rw-r--r--   0        0        0     4123 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/sync.py
+-rw-r--r--   0        0        0     1745 2023-07-18 05:02:34.796009 trad-0.1.1/mod/trad/units.py
+-rw-r--r--   0        0        0      580 2023-07-18 05:02:34.796009 trad-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 trad-0.1.1/PKG-INFO
```

### Comparing `trad-0.1.0/LICENSE` & `trad-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trad-0.1.0/README.rst` & `trad-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `trad-0.1.0/mod/trad/__init__.py` & `trad-0.1.1/mod/trad/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Composable Radiative Transfer"""
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

### Comparing `trad-0.1.0/mod/trad/helper.py` & `trad-0.1.1/mod/trad/helper.py`

 * *Files identical despite different names*

### Comparing `trad-0.1.0/mod/trad/specradiance.py` & `trad-0.1.1/mod/trad/specradiance.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 """
 
 
 from astropy import constants as c, units as u
 from phun    import phun
 
-from .units  import *
 from .helper import *
 
 
 @phun({
     'si' : (u.W      ) / u.sr / (u.m *u.m ) / u.Hz,
     'cgs': (u.erg/u.s) / u.sr / (u.cm*u.cm) / u.Hz,
 })
@@ -60,8 +59,12 @@
     with :math:`h`, :math:`c`, and :math:`k_\mathrm{B}` being the
     Planck's constant, speed of light, and Boltzmann constant,
     respectively.
 
     """
     a = float((2 * c.h * u_nu**3) / (c.c**2 * u.sr) / u_res)**(1/3)
     x = float((c.h * u_nu) / (c.k_B * u_T))
-    return lambda nu, T: (a*nu)**3 / (backend.exp(x*nu/T) - 1)
+
+    def pure(nu, T):
+        return (a*nu)**3 / (backend.exp(x*nu/T) - 1)
+
+    return pure
```

### Comparing `trad-0.1.0/mod/trad/sync.py` & `trad-0.1.1/mod/trad/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 """
 
 
 from astropy import constants as c, units as u
 from scipy.special import kn # jax does not support kn
 from phun import phun
 
-from .plasma       import Te, gyrofrequency
+from .plasma       import u_T_me, gyrofrequency
 from .specradiance import blackbody
 
 
 @phun({
     'si' : (u.W      ) / u.sr / u.m**3  / u.Hz,
     'cgs': (u.erg/u.s) / u.sr / u.cm**3 / u.Hz,
 })
-def emissivity(u_nu, u_ne, u_Thetae, u_B, u_theta, u_res='si', backend=None):
+def emissivity(u_nu, u_ne, u_Te, u_B, u_theta, u_res='si', backend=None):
     r"""Synchrotron emissivity
 
     An approximation of the synchrotron emissivity at given
     frequency               :math:`\nu`,
     electron number density :math:`n_e`,
     electron temperature    :math:`T_e`,
     magnetic field strength :math:`B`, and
@@ -88,31 +88,38 @@
     """
     pi   = backend.pi
     sqrt = backend.sqrt
     exp  = backend.exp
     sin  = backend.sin
     nuc  = gyrofrequency(u_B)
 
+    r = float(u_theta.to(u.rad))
+    t = float(u_T_me.to(u_Te))
+
+    s = float((2/9) / t**2)
     A = float(sqrt(2) * (pi/3) * (c.cgs.e.gauss**2/c.c/u.sr) * u_ne * nuc.unit / u_res)
     x = float(1 * u_nu / nuc.unit)
 
-    def jnu_pure(nu, ne, Thetae, B, theta):
-        nus = (2/9) * nuc(B) * Thetae*Thetae * sin(theta)
+    def pure(nu, ne, Te, B, theta):
+        nus = s * Te**2 * nuc(B) * sin(theta * r)
         X = x * nu / nus
         Y = (X**(1/2) + 2**(11/12) * X**(1/6))**2 * exp(-X**(1/3))
-        K = kn(2, 1/Thetae)
+        K = kn(2, t/Te)
         return A * (ne*nus) * (Y/K)
 
-    return jnu_pure
+    return pure
 
 
 @phun({
     'si' : 1/u.m,
     'cgs': 1/u.cm,
 })
-def absorptivity(u_nu, u_ne, u_Thetae, u_B, u_theta, u_res='si', backend=None):
+def absorptivity(u_nu, u_ne, u_Te, u_B, u_theta, u_res='si', backend=None):
     r"""Synchrotron absorptivity"""
 
-    Bnu = blackbody(u_nu, Te)
-    jnu = emissivity(u_nu, u_ne, u_Thetae, u_B, u_theta)
+    Bnu = blackbody(u_nu, u_Te)
+    jnu = emissivity(u_nu, u_ne, u_Te, u_B, u_theta)
+
+    def pure(nu, ne, Te, B, theta):
+        return jnu(nu, ne, Te, B, theta) / Bnu(nu, Te)
 
-    return lambda nu, ne, Thetae, B, theta: jnu(nu, ne, Thetae, B, theta) / Bnu(nu, Thetae)
+    return pure
```

### Comparing `trad-0.1.0/mod/trad/units.py` & `trad-0.1.1/mod/trad/units.py`

 * *Files identical despite different names*

### Comparing `trad-0.1.0/pyproject.toml` & `trad-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trad"
-version = "0.1.0"
+version = "0.1.1"
 description = "Composable Radiative Transfer"
 authors = ["Chi-kwan Chan <chanc@arizona.edu>"]
 readme = "README.rst"
 packages = [{include="trad", from="mod"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `trad-0.1.0/PKG-INFO` & `trad-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trad
-Version: 0.1.0
+Version: 0.1.1
 Summary: Composable Radiative Transfer
 Author: Chi-kwan Chan
 Author-email: chanc@arizona.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

