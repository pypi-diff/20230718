# Comparing `tmp/pyees-1.4.1.tar.gz` & `tmp/pyees-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.1.tar", last modified: Mon Jul 17 07:26:26 2023, max compression
+gzip compressed data, was "pyees-1.4.2.tar", last modified: Tue Jul 18 11:18:32 2023, max compression
```

## Comparing `pyees-1.4.1.tar` & `pyees-1.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.625005 pyees-1.4.1/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-17 07:26:26.640630 pyees-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.328119 pyees-1.4.1/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.1/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.1/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.1/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.1/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.1/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.1/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.1/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.1/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.1/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.1/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.1/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.1/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.1/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.4.1/pyees/testUnit.py
--rw-rw-rw-   0        0        0    84033 2023-07-17 07:24:33.000000 pyees-1.4.1/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.1/pyees/unit.py
--rw-rw-rw-   0        0        0    33943 2023-07-17 07:25:31.000000 pyees-1.4.1/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:26:26.562502 pyees-1.4.1/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-17 07:26:24.000000 pyees-1.4.1/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-17 07:26:26.656255 pyees-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-17 07:26:19.000000 pyees-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:18:32.047046 pyees-1.4.2/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-18 11:18:32.062670 pyees-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 11:18:31.812663 pyees-1.4.2/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.2/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.2/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.2/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.2/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.2/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.2/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.2/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.2/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.2/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.2/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.2/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.2/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.2/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.4.2/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84460 2023-07-18 11:17:21.000000 pyees-1.4.2/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.2/pyees/unit.py
+-rw-rw-rw-   0        0        0    36013 2023-07-18 11:17:32.000000 pyees-1.4.2/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:18:32.015794 pyees-1.4.2/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-18 11:18:29.000000 pyees-1.4.2/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 11:18:32.109547 pyees-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-18 11:18:23.000000 pyees-1.4.2/setup.py
```

### Comparing `pyees-1.4.1/LICENSE.txt` & `pyees-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/PKG-INFO` & `pyees-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.1
+Version: 1.4.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.1/README.md` & `pyees-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/fit.py` & `pyees-1.4.2/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/profileFit.py` & `pyees-1.4.2/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/profilePyees.py` & `pyees-1.4.2/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/prop.py` & `pyees-1.4.2/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/sheet.py` & `pyees-1.4.2/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/solve.py` & `pyees-1.4.2/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/stackOverflowODR.py` & `pyees-1.4.2/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testFit.py` & `pyees-1.4.2/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testProp.py` & `pyees-1.4.2/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testPyees.py` & `pyees-1.4.2/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testSheet.py` & `pyees-1.4.2/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testSolve.py` & `pyees-1.4.2/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testUnit.py` & `pyees-1.4.2/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/testVariable.py` & `pyees-1.4.2/pyees/testVariable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1322,14 +1322,22 @@
         self.assertEqual(time[0].unit, 'min')
         self.assertEqual(time[1].unit, 'min')
         self.assertEqual(time[2].unit, 'min')
         self.assertEqual(time[0].uncert, 0.1/60)
         self.assertEqual(time[1].uncert, 0.2/60)
         self.assertEqual(time[2].uncert, 0.3/60)
 
+
+        t1 = variable([1,2,3], 'min')
+        t1[1].convert('s')
+        dt = variable(10, 'min')
+        with self.assertRaises(Exception) as context:
+            t1 + dt
+        self.assertTrue("Some of the scalarvariables in [1, 120, 3] [min] did not have the unit [min] as they should. This could happen if the user has converted a scalarVaraible instead of the arrayVaraible." in str(context.exception))
+        
     def testCompare(self):
         a = variable(1, 'm')
         b = variable([2, 3, 4], 'm')
         np.testing.assert_equal(a < b, [True, True, True])
         np.testing.assert_equal(a <= b, [True, True, True])
         np.testing.assert_equal(a > b, [False, False, False])
         np.testing.assert_equal(a >= b, [False, False, False])
```

### Comparing `pyees-1.4.1/pyees/unit.py` & `pyees-1.4.2/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.1/pyees/variable.py` & `pyees-1.4.2/pyees/variable.py`

 * *Files 5% similar despite different names*

```diff
@@ -306,16 +306,18 @@
         
         ## if the output unit is 'K' and one of the inputs is a temperature and the other is a tempreature difference
         ## then return the output in the same unit as the temperature
         ## this has no affect if the inputs are in 'K' and 'DeltaK'
         ## but the output is converted to 'C' if the inputs are in 'C' and 'DeltaK' 
         SIBaseUnits = [self._unitObject.unitDictSI, other._unitObject.unitDictSI]
         if outputUnit.unitDict == {'K':{None:1}} and {'DELTAK':{None:1}} in SIBaseUnits and {'K':{None:1}} in SIBaseUnits:
-            var.convert(str([selfUnit, otherUnit][SIBaseUnits.index({'K':{None:1}})])) 
-            
+            var.convert(str([selfUnit, otherUnit][SIBaseUnits.index({'K':{None:1}})]))     
+            for elem in var:
+                elem._unitObject = var._unitObject
+        
         return var
 
     def __radd__(self, other):
         return self + other
 
     def __sub__(self, other):
         if not isinstance(other, scalarVariable):
@@ -355,15 +357,16 @@
 
         SIBaseUnits = [self._unitObject.unitDictSI, other._unitObject.unitDictSI]
         if outputUnit.unitDictSI == {'K':{None:1}} and SIBaseUnits[0] == {'K':{None:1}} and SIBaseUnits[1] == {'K':{None:1}}:
             if list(self._unitObject.unitDict.keys())[0] == list(other._unitObject.unitDict.keys())[0]:
                 var._unitObject = unit('DELTA' + list(self._unitObject.unitDict.keys())[0])
             else:
                 var._unitObject = unit('DELTAK')
-            
+            for elem in var:
+                elem._unitObject = var._unitObject
         return var
 
     def __rsub__(self, other):
         return - self + other
 
     def __mul__(self, other):
     
@@ -673,15 +676,56 @@
             if not value is None:
                 for v, u in zip(value, uncert):
                     self.scalarVariables.append(scalarVariable(v, self._unitObject, u, nDigits))
         else:
             self.scalarVariables = scalarVariables
             self._unitObject = self.scalarVariables[0]._unitObject
             self.nDigits = self.scalarVariables[0].nDigits
-            
+
+    def __checkUnitOfScalarVariables(self):
+        for var in self.scalarVariables:
+            if var._unitObject != self._unitObject:
+                raise ValueError(f'Some of the scalarvariables in {self} did not have the unit [{self.unit}] as they should. This could happen if the user has converted a scalarVaraible instead of the arrayVaraible.')
+        
+    def __add__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__add__(self, other)
+
+    def __sub__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__sub__(self, other)
+
+    def __mul__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__mul__(self, other)
+
+    def __rmul__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__rmul__(self, other)
+
+    def __pow__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__pow__(self, other)
+
+    def __rpow__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__rpow__(self, other)
+    
+    def __truediv__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__truediv__(self, other)
+
+    def __rtruediv__(self, other):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__rtruediv__(self, other)
+    
+    def __neg__(self):
+        self.__checkUnitOfScalarVariables()
+        return scalarVariable.__neg__(self)
+
     def _calculateUncertanty(self):
         for elem in self.scalarVariables:
             elem._calculateUncertanty()
     
     def addCovariance(self, var, grad: np.ndarray, unitStr: str):
         for elem, varElem, gradElem in zip(self.scalarVariables, var, grad):
             elem.addCovariance(varElem, gradElem, unitStr)
@@ -947,13 +991,29 @@
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 if __name__ == "__main__":
-    time = variable([601.15],'s')
-    time.convert('min')
+
+    t_in = variable(50, 'C', 1.2)
+    t_out = variable([10, 15, 20, 25, 30, 35, 40], 'C', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
+    
+    dt = t_in - t_out
+    print(dt)
+    for elem in dt:
+        print(elem)
+
+    
+    t_in = variable(50, 'C', 1.2)
+    dt = variable([10, 15, 20, 25, 30, 35, 40], 'DELTAC', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
+    
+    t_out = t_in + dt
+    print(t_out)
+    for elem in t_out:
+        print(elem)
+        
+        
+    
     
-    print(time)
-    print(time[0])
```

### Comparing `pyees-1.4.1/pyees.egg-info/PKG-INFO` & `pyees-1.4.2/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.1
+Version: 1.4.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.1/setup.py` & `pyees-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.1',
+    version='1.4.2',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

