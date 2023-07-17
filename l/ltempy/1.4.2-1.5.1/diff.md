# Comparing `tmp/ltempy-1.4.2.tar.gz` & `tmp/ltempy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltempy-1.4.2.tar", last modified: Thu Feb 16 07:23:09 2023, max compression
+gzip compressed data, was "ltempy-1.5.1.tar", last modified: Mon Jul 17 23:06:17 2023, max compression
```

## Comparing `ltempy-1.4.2.tar` & `ltempy-1.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-02-16 07:23:09.350344 ltempy-1.4.2/
--rw-r--r--   0 wsp        (501) staff       (20)    35130 2021-04-27 19:53:57.000000 ltempy-1.4.2/LICENSE
--rw-r--r--   0 wsp        (501) staff       (20)     1859 2023-02-16 07:23:09.350389 ltempy-1.4.2/PKG-INFO
--rw-r--r--   0 wsp        (501) staff       (20)     1237 2021-11-27 07:25:12.000000 ltempy-1.4.2/README.md
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-02-16 07:23:09.347820 ltempy-1.4.2/ltempy/
--rw-r--r--   0 wsp        (501) staff       (20)     1500 2021-11-27 06:48:39.000000 ltempy-1.4.2/ltempy/__init__.py
--rw-r--r--   0 wsp        (501) staff       (20)     7198 2022-07-13 22:03:41.000000 ltempy-1.4.2/ltempy/_utils.py
--rw-r--r--   0 wsp        (501) staff       (20)     6808 2022-08-23 19:04:50.000000 ltempy-1.4.2/ltempy/colors.py
--rw-r--r--   0 wsp        (501) staff       (20)     3290 2021-11-27 07:22:51.000000 ltempy-1.4.2/ltempy/constants.py
--rw-r--r--   0 wsp        (501) staff       (20)    16486 2023-02-15 20:50:38.000000 ltempy-1.4.2/ltempy/plot.py
--rw-r--r--   0 wsp        (501) staff       (20)    16772 2022-08-18 07:59:14.000000 ltempy-1.4.2/ltempy/process.py
--rw-r--r--   0 wsp        (501) staff       (20)    26357 2023-02-16 07:21:37.000000 ltempy-1.4.2/ltempy/simulate.py
--rw-r--r--   0 wsp        (501) staff       (20)     8976 2022-07-13 23:03:33.000000 ltempy-1.4.2/ltempy/sitie.py
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-02-16 07:23:09.348504 ltempy-1.4.2/ltempy.egg-info/
--rw-r--r--   0 wsp        (501) staff       (20)     1859 2023-02-16 07:23:09.000000 ltempy-1.4.2/ltempy.egg-info/PKG-INFO
--rw-r--r--   0 wsp        (501) staff       (20)      478 2023-02-16 07:23:09.000000 ltempy-1.4.2/ltempy.egg-info/SOURCES.txt
--rw-r--r--   0 wsp        (501) staff       (20)        1 2023-02-16 07:23:09.000000 ltempy-1.4.2/ltempy.egg-info/dependency_links.txt
--rw-r--r--   0 wsp        (501) staff       (20)       17 2023-02-16 07:23:09.000000 ltempy-1.4.2/ltempy.egg-info/requires.txt
--rw-r--r--   0 wsp        (501) staff       (20)        7 2023-02-16 07:23:09.000000 ltempy-1.4.2/ltempy.egg-info/top_level.txt
--rw-r--r--   0 wsp        (501) staff       (20)      104 2021-04-27 19:35:04.000000 ltempy-1.4.2/pyproject.toml
--rw-r--r--   0 wsp        (501) staff       (20)      716 2023-02-16 07:23:09.350614 ltempy-1.4.2/setup.cfg
--rw-r--r--   0 wsp        (501) staff       (20)      796 2023-02-16 07:21:51.000000 ltempy-1.4.2/setup.py
-drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-02-16 07:23:09.350113 ltempy-1.4.2/tests/
--rw-r--r--   0 wsp        (501) staff       (20)      389 2021-11-27 06:48:55.000000 ltempy-1.4.2/tests/test_colors.py
--rw-r--r--   0 wsp        (501) staff       (20)      185 2021-11-27 06:49:24.000000 ltempy-1.4.2/tests/test_constants.py
--rw-r--r--   0 wsp        (501) staff       (20)     1171 2022-07-10 04:18:39.000000 ltempy-1.4.2/tests/test_ndap_x_and_y.py
--rw-r--r--   0 wsp        (501) staff       (20)     2348 2022-08-18 07:48:54.000000 ltempy-1.4.2/tests/test_process.py
--rw-r--r--   0 wsp        (501) staff       (20)     2790 2022-12-07 21:47:27.000000 ltempy-1.4.2/tests/test_simulate.py
--rw-r--r--   0 wsp        (501) staff       (20)      471 2022-07-10 04:19:53.000000 ltempy-1.4.2/tests/test_sitie.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-07-17 23:06:17.862327 ltempy-1.5.1/
+-rw-r--r--   0 wsp        (501) staff       (20)    35130 2021-04-27 19:53:57.000000 ltempy-1.5.1/LICENSE
+-rw-r--r--   0 wsp        (501) staff       (20)     1859 2023-07-17 23:06:17.862433 ltempy-1.5.1/PKG-INFO
+-rw-r--r--   0 wsp        (501) staff       (20)     1237 2021-11-27 07:25:12.000000 ltempy-1.5.1/README.md
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-07-17 23:06:17.858789 ltempy-1.5.1/ltempy/
+-rw-r--r--   0 wsp        (501) staff       (20)     1500 2021-11-27 06:48:39.000000 ltempy-1.5.1/ltempy/__init__.py
+-rw-r--r--   0 wsp        (501) staff       (20)     7401 2023-07-17 22:44:55.000000 ltempy-1.5.1/ltempy/_utils.py
+-rw-r--r--   0 wsp        (501) staff       (20)     6808 2022-08-23 19:04:50.000000 ltempy-1.5.1/ltempy/colors.py
+-rw-r--r--   0 wsp        (501) staff       (20)     3475 2023-07-17 22:32:18.000000 ltempy-1.5.1/ltempy/constants.py
+-rw-r--r--   0 wsp        (501) staff       (20)    16486 2023-02-15 20:50:38.000000 ltempy-1.5.1/ltempy/plot.py
+-rw-r--r--   0 wsp        (501) staff       (20)    16772 2023-07-15 00:26:40.000000 ltempy-1.5.1/ltempy/process.py
+-rw-r--r--   0 wsp        (501) staff       (20)    26551 2023-07-17 22:46:43.000000 ltempy-1.5.1/ltempy/simulate.py
+-rw-r--r--   0 wsp        (501) staff       (20)     8976 2023-03-02 08:48:12.000000 ltempy-1.5.1/ltempy/sitie.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-07-17 23:06:17.859917 ltempy-1.5.1/ltempy.egg-info/
+-rw-r--r--   0 wsp        (501) staff       (20)     1859 2023-07-17 23:06:17.000000 ltempy-1.5.1/ltempy.egg-info/PKG-INFO
+-rw-r--r--   0 wsp        (501) staff       (20)      478 2023-07-17 23:06:17.000000 ltempy-1.5.1/ltempy.egg-info/SOURCES.txt
+-rw-r--r--   0 wsp        (501) staff       (20)        1 2023-07-17 23:06:17.000000 ltempy-1.5.1/ltempy.egg-info/dependency_links.txt
+-rw-r--r--   0 wsp        (501) staff       (20)       17 2023-07-17 23:06:17.000000 ltempy-1.5.1/ltempy.egg-info/requires.txt
+-rw-r--r--   0 wsp        (501) staff       (20)        7 2023-07-17 23:06:17.000000 ltempy-1.5.1/ltempy.egg-info/top_level.txt
+-rw-r--r--   0 wsp        (501) staff       (20)      104 2021-04-27 19:35:04.000000 ltempy-1.5.1/pyproject.toml
+-rw-r--r--   0 wsp        (501) staff       (20)      716 2023-07-17 23:06:17.862842 ltempy-1.5.1/setup.cfg
+-rw-r--r--   0 wsp        (501) staff       (20)      796 2023-07-17 23:04:21.000000 ltempy-1.5.1/setup.py
+drwxr-xr-x   0 wsp        (501) staff       (20)        0 2023-07-17 23:06:17.862031 ltempy-1.5.1/tests/
+-rw-r--r--   0 wsp        (501) staff       (20)      389 2021-11-27 06:48:55.000000 ltempy-1.5.1/tests/test_colors.py
+-rw-r--r--   0 wsp        (501) staff       (20)      185 2021-11-27 06:49:24.000000 ltempy-1.5.1/tests/test_constants.py
+-rw-r--r--   0 wsp        (501) staff       (20)     1171 2022-07-10 04:18:39.000000 ltempy-1.5.1/tests/test_ndap_x_and_y.py
+-rw-r--r--   0 wsp        (501) staff       (20)     2348 2022-08-18 07:48:54.000000 ltempy-1.5.1/tests/test_process.py
+-rw-r--r--   0 wsp        (501) staff       (20)     2790 2022-12-07 21:47:27.000000 ltempy-1.5.1/tests/test_simulate.py
+-rw-r--r--   0 wsp        (501) staff       (20)      471 2022-07-10 04:19:53.000000 ltempy-1.5.1/tests/test_sitie.py
```

### Comparing `ltempy-1.4.2/LICENSE` & `ltempy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/PKG-INFO` & `ltempy-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltempy
-Version: 1.4.2
+Version: 1.5.1
 Summary: Utilities for Lorentz TEM data analysis and simulation.
 Home-page: https://github.com/McMorranLab/ltempy
 Author: William S. Parker
 Author-email: will.parker0@gmail.com
 Project-URL: Documentation, https://mcmorranlab.github.io/ltempy/
 Project-URL: Bug Tracker, https://github.com/McMorranLab/ltempy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ltempy-1.4.2/README.md` & `ltempy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy/__init__.py` & `ltempy-1.5.1/ltempy/__init__.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy/_utils.py` & `ltempy-1.5.1/ltempy/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     Gp = G(p, sig, z_hat, thickness * s_mag)
     sig_x_z = np.cross(sig, z_hat, axisa=0, axisb=0, axisc=0)
     p_x_p_M = np.cross(p, np.cross(p, M, axisa=0, axisb=0,
                        axisc=0), axis=0, axisb=0, axisc=0)
     weights = 2 * _.e / _.hbar / _.c * 1j * thickness / s_mag * \
         Gp * np.einsum('i...,i...->...', sig_x_z, p_x_p_M)
     weights[:, 0, 0, :] = 0
+    ### adjusting for "missing" constants in Eq (2) of Mansuripur
+    weights = weights * _.mu0 / 4 / np.pi
+    ### adjusting for "extra" factor of c in Eq (12) of Mansuripur
+    weights = weights * _.c
     return(weights)
 
 
 def laplacian_2d(data, dx, dy):
     # 2-dimensional laplacian, implemented via Fourier transform
     QX = np.fft.fftfreq(data.shape[1], dx)
     QY = np.fft.fftfreq(data.shape[0], dy)
```

### Comparing `ltempy-1.4.2/ltempy/colors.py` & `ltempy-1.5.1/ltempy/colors.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy/constants.py` & `ltempy-1.5.1/ltempy/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,60 +34,61 @@
 `constants.hbar`) will be affected, as both \(e\) (the electron charge) and \(\hbar\) (the reduced Planck constant),
 have different numerical values when km is the base unit.
 """
 
 __all__ = ['s','m','kg','A','K','mol','cd','c','hbar','e','pi','set_units']
 
 def set_units(second=1, meter=1, kilogram=1, Ampere=1, Kelvin=1, mole=1, candela=1):
-	"""Sets the units across the ltempy module.
+    """Sets the units across the ltempy module.
 
-	For example, `set_units(meter = 1e3)` sets the millimeter as the base unit for length.
+    For example, `set_units(meter = 1e3)` sets the millimeter as the base unit for length.
 
-	**Parameters**
+    **Parameters**
 
-	* **second** : _number, optional_ <br />
-	The SI base unit for time. <br />
-	Default is `second = 1`.
-
-	* **meter** : _number, optional_ <br />
-	The SI base unit for length. <br />
-	Default is `meter = 1`.
-
-	* **kilogram** : _number, optional_ <br />
-	The SI base unit for mass. <br />
-	Default is `kilogram = 1`.
-
-	* **Ampere** : _number, optional_ <br />
-	The SI base unit for current. <br />
-	Default is `Ampere = 1`.
-
-	* **Kelvin** : _number, optional_ <br />
-	The SI base unit for temperature. <br />
-	Default is `Kelvin = 1`.
-
-	* **mole** : _number, optional_ <br />
-	The SI base unit for amount of substance. <br />
-	Default is `mole = 1`.
-
-	* **candela** : _number, optional_ <br />
-	The SI base unit for luminous intensity. <br />
-	Default is `candela = 1`.
-	"""
-	global s,m,kg,A,K,mol,cd
-	s,m,kg,A,K,mol,cd = second, meter, kilogram, Ampere, Kelvin, mole, candela
-	set_consts(s, m, kg, A, K, mol, cd)
+    * **second** : _number, optional_ <br />
+    The SI base unit for time. <br />
+    Default is `second = 1`.
+
+    * **meter** : _number, optional_ <br />
+    The SI base unit for length. <br />
+    Default is `meter = 1`.
+
+    * **kilogram** : _number, optional_ <br />
+    The SI base unit for mass. <br />
+    Default is `kilogram = 1`.
+
+    * **Ampere** : _number, optional_ <br />
+    The SI base unit for current. <br />
+    Default is `Ampere = 1`.
+
+    * **Kelvin** : _number, optional_ <br />
+    The SI base unit for temperature. <br />
+    Default is `Kelvin = 1`.
+
+    * **mole** : _number, optional_ <br />
+    The SI base unit for amount of substance. <br />
+    Default is `mole = 1`.
+
+    * **candela** : _number, optional_ <br />
+    The SI base unit for luminous intensity. <br />
+    Default is `candela = 1`.
+    """
+    global s,m,kg,A,K,mol,cd
+    s,m,kg,A,K,mol,cd = second, meter, kilogram, Ampere, Kelvin, mole, candela
+    set_consts(s, m, kg, A, K, mol, cd)
 
 def set_consts(s, m, kg, A, K, mol, cd):
-	"""Utility function for `set_units()`."""
-	global c, hbar, e, pi
-	F = s**4 * A**2 / m**2 / kg
-	J = kg * m**2 / s**2
-	C = A * s
-	W = kg * m**2 / s**3
-	eV = 1.602176634e-19 * J
-
-	c       = 299792458.0   			* m / s
-	hbar    = 1.0545718176461565e-34	* J * s
-	e       = 1.602176634e-19			* C
-	pi      = 3.141592653589793
+    """Utility function for `set_units()`."""
+    global c, hbar, e, pi, mu0
+    F = s**4 * A**2 / m**2 / kg
+    J = kg * m**2 / s**2
+    C = A * s
+    W = kg * m**2 / s**3
+    eV = 1.602176634e-19 * J
+
+    c       = 299792458.0   			* m / s
+    hbar    = 1.0545718176461565e-34	* J * s
+    e       = 1.602176634e-19			* C
+    pi      = 3.141592653589793
+    mu0     = 1.25663706212e-6          * kg * m / s**2 / A**2
 
 set_units()
```

### Comparing `ltempy-1.4.2/ltempy/plot.py` & `ltempy-1.5.1/ltempy/plot.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy/process.py` & `ltempy-1.5.1/ltempy/process.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy/simulate.py` & `ltempy-1.5.1/ltempy/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,16 @@
     dzA_mn[:,0,0,selz_p] = 0
     dzA_mn[:,0,0,selz_z] = -4 * _.pi * np.cross(z_hat[:,0,0,:], M[:,0,0,:], axisa=0, axisb=0, axisc=0)
     B_mn = np.zeros((3, mx.shape[0], mx.shape[1], z.shape[-1]), dtype=complex)
     B_mn[0] = dyA_mn[2] - dzA_mn[1]
     B_mn[1] = dzA_mn[0] - dxA_mn[2]
     B_mn[2] = dxA_mn[1] - dyA_mn[0]
     B = B_mn.shape[1] * B_mn.shape[2] * np.fft.ifft2(B_mn, axes=(1,2))
+    ### adjusting for "missing" constants in Eq (2) of Mansuripur
+    B = B * _.mu0 / 4 / np.pi 
     return(np.squeeze(B.real))
 
 def A_from_mag(mx, my, mz, dx = 1, dy = 1, z = 0, thickness = 60e-9):
     r"""Calculate the magnetic vector potential of a specified 2-d magnetic configuration.
 
     This is an implementation of [1], Eqn (11), which gives the Fourier components of
     the magnetic vector potential.
@@ -240,14 +242,16 @@
     sigp = sig + 1j * z_hat
     sigm = sig - 1j * z_hat
 
     A_mn = A_mn_components(
                 mx.shape[0], mx.shape[1], z.shape[-1], selz_m, selz_z,
                 selz_p, s_mag, z, sigm, sigp, sig, M, thickness, z_hat)
     A = A_mn.shape[1] * A_mn.shape[2] * np.fft.ifft2(A_mn, axes=(1,2))
+    ### adjusting for "missing" constants in Eq (2) of Mansuripur
+    A = A * _.mu0 / 4 / np.pi 
     return(np.squeeze(A.real))
 
 def ind_from_mag(mx, my, mz, dx=1, dy=1, thickness=60e-9, p = np.array([0,0,1])):
     """Calculate the integrated perpendicular magnetic field of a magnetized sample.
 
     This is shorthand for `ind_from_phase(ab_phase(*args))`. This method is used rather than `B_from_mag`
     because the integral over z can be done analytically.
```

### Comparing `ltempy-1.4.2/ltempy/sitie.py` & `ltempy-1.5.1/ltempy/sitie.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/ltempy.egg-info/PKG-INFO` & `ltempy-1.5.1/ltempy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltempy
-Version: 1.4.2
+Version: 1.5.1
 Summary: Utilities for Lorentz TEM data analysis and simulation.
 Home-page: https://github.com/McMorranLab/ltempy
 Author: William S. Parker
 Author-email: will.parker0@gmail.com
 Project-URL: Documentation, https://mcmorranlab.github.io/ltempy/
 Project-URL: Bug Tracker, https://github.com/McMorranLab/ltempy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ltempy-1.4.2/setup.cfg` & `ltempy-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ltempy
-version = 1.4.2
+version = 1.5.1
 author = William S. Parker
 author_email = will.parker0@gmail.com
 description = Utilities for Lorentz TEM data analysis and simulation.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/McMorranLab/ltempy
 project_urls =
```

### Comparing `ltempy-1.4.2/setup.py` & `ltempy-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'ltempy',
 	packages = find_packages(),
-	version = '1.4.2',
+	version = '1.5.1',
 	author = 'William S. Parker',
 	author_email = 'will.parker0@gmail.com',
 	description = 'Utilities for Lorentz TEM data analysis and simulation.',
 	url = 'https://github.com/McMorranLab/ltempy',
 	project_urls={
 		"Documentation" : "https://mcmorranlab.github.io/ltempy/",
 		"Bug Tracker": "https://github.com/McMorranLab/ltempy/issues",
```

### Comparing `ltempy-1.4.2/tests/test_ndap_x_and_y.py` & `ltempy-1.5.1/tests/test_ndap_x_and_y.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/tests/test_process.py` & `ltempy-1.5.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `ltempy-1.4.2/tests/test_simulate.py` & `ltempy-1.5.1/tests/test_simulate.py`

 * *Files identical despite different names*

