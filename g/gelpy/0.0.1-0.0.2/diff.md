# Comparing `tmp/gelpy-0.0.1-py3-none-any.whl.zip` & `tmp/gelpy-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 34169 bytes, number of entries: 13
+Zip file size: 34053 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       28 b- defN 20-Feb-02 00:00 gelpy/__init__.py
 -rw-r--r--  2.0 unx     1808 b- defN 20-Feb-02 00:00 gelpy/background_BackgroundHandler.py
 -rw-r--r--  2.0 unx    10223 b- defN 20-Feb-02 00:00 gelpy/background_ransac_fit_models.py
 -rw-r--r--  2.0 unx    12084 b- defN 20-Feb-02 00:00 gelpy/image_handling.py
 -rw-r--r--  2.0 unx     9685 b- defN 20-Feb-02 00:00 gelpy/line_profile_handling.py
 -rw-r--r--  2.0 unx    14519 b- defN 20-Feb-02 00:00 gelpy/package_api.py
 -rw-r--r--  2.0 unx    10221 b- defN 20-Feb-02 00:00 gelpy/profile_fit_handling.py
 -rw-r--r--  2.0 unx    13720 b- defN 20-Feb-02 00:00 gelpy/profile_fitting_models.py
 -rw-r--r--  2.0 unx      159 b- defN 20-Feb-02 00:00 gelpy/utility_functions.py
-?rw-r--r--  2.0 unx     4697 b- defN 20-Feb-02 00:00 gelpy-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 gelpy-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 gelpy-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1061 b- defN 20-Feb-02 00:00 gelpy-0.0.1.dist-info/RECORD
-13 files, 113441 bytes uncompressed, 32413 bytes compressed:  71.4%
+?rw-r--r--  2.0 unx     4440 b- defN 20-Feb-02 00:00 gelpy-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 gelpy-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 gelpy-0.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1061 b- defN 20-Feb-02 00:00 gelpy-0.0.2.dist-info/RECORD
+13 files, 113184 bytes uncompressed, 32297 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: gelpy/profile_fitting_models.py
 Comment: 
 
 Filename: gelpy/utility_functions.py
 Comment: 
 
-Filename: gelpy-0.0.1.dist-info/METADATA
+Filename: gelpy-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gelpy-0.0.1.dist-info/WHEEL
+Filename: gelpy-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gelpy-0.0.1.dist-info/licenses/LICENSE
+Filename: gelpy-0.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: gelpy-0.0.1.dist-info/RECORD
+Filename: gelpy-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gelpy-0.0.1.dist-info/METADATA` & `gelpy-0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: gelpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small python package used for gel electrophoresis visualization, fitting and analysis
 Project-URL: homepage, https://github.com/ckarfusehr/GelPy
 Project-URL: bug-tracker, https://github.com/ckarfusehr/GelPy/issues
 Author-email: Christoph Karfusehr <c.karfusehr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: ipykernel>=6.19.2
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: numpy>=1.24.3
 Requires-Dist: pandas>=2.0.2
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: scikit-learn>=1.2.2
 Requires-Dist: scipy>=1.10.1
@@ -38,24 +38,17 @@
 - Save all generated images
 - Save the gel object, including all the plots, lane profiles, and fits, as a Python object. You can then send this object as one file to your collaborator, who can load it back into Python and continue where you left off.
 
 Another benefit of using this package over, for example, Fiji for data extraction is that all lane profiles, fitting parameters, and the original image are directly available in Python and do not have to be saved and imported again for further custom analysis
 
 ## Installation
 
-### pip
+Install via pip:
 
-```
-conda create -n <your_environment_name>
-conda install python
-pip installl gelpy
-
-```
-
-(`conda install python`is only needed if your system wide python installation is older than 3.8. This is because `conda create -n <env_name>` gives you an empty environment without Python in it):
+`pip installl gelpy`
 
 
 ## How to use gelpy
 
 I recommend checking out the example Jupyter notebook in the "Example" folder. I hope to add proper documentation soon. Also, please note that the docstring was generated with GPT and may potentially contain errors in its current state.
 
 ## How to contribute by coding
```

## Comparing `gelpy-0.0.1.dist-info/licenses/LICENSE` & `gelpy-0.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `gelpy-0.0.1.dist-info/RECORD` & `gelpy-0.0.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 gelpy/background_ransac_fit_models.py,sha256=xENbkIK1YJNpF3w7JwJykh96Pyi4lB0yqgKS7X7WRA8,10223
 gelpy/image_handling.py,sha256=ifpRqFycNuJzUInFxKAQlaai-CofcfYMjl3B-MHH3i8,12084
 gelpy/line_profile_handling.py,sha256=3h9MPxU5-UCTIslI8O23gx9A7zuHXESn4xjSD5bw4Co,9685
 gelpy/package_api.py,sha256=gnFpX1y5U4gP0mT4Fuda0XexfduJddbnhgIhDRkNIZA,14519
 gelpy/profile_fit_handling.py,sha256=UCirGr00Q7KT4Y5p_sgmyoDnZQYFMC7L4Q6Op5zkpTM,10221
 gelpy/profile_fitting_models.py,sha256=1ZdklyhMMhhyG0bv3hD8QvHYlnaAClQct2u-VX4-zNI,13720
 gelpy/utility_functions.py,sha256=pUuXbETu9zp9OTgc6kle7-4oJrUQPRoefGe-Svepnz0,159
-gelpy-0.0.1.dist-info/METADATA,sha256=w-Q9bZOkMoC9kLTIaSXlrE6UwYgIxQcr4kFS08LM6CA,4697
-gelpy-0.0.1.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-gelpy-0.0.1.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-gelpy-0.0.1.dist-info/RECORD,,
+gelpy-0.0.2.dist-info/METADATA,sha256=Nd9jRmcAaV6esGoyq52qgUCIN-iKh4jlMvAbRjSVrao,4440
+gelpy-0.0.2.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+gelpy-0.0.2.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+gelpy-0.0.2.dist-info/RECORD,,
```

