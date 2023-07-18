# Comparing `tmp/RangeSlider-2023.7.1.tar.gz` & `tmp/RangeSlider-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RangeSlider-2023.7.1.tar", last modified: Tue Jul 18 13:24:27 2023, max compression
+gzip compressed data, was "RangeSlider-2023.7.2.tar", last modified: Tue Jul 18 14:07:46 2023, max compression
```

## Comparing `RangeSlider-2023.7.1.tar` & `RangeSlider-2023.7.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    12625 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    11734 2023-07-17 18:35:22.000000 RangeSlider-2023.7.1/README.md
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/RangeSlider/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    36567 2023-07-17 18:40:49.000000 RangeSlider-2023.7.1/RangeSlider/RangeSlider.py
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       64 2022-12-25 11:45:33.000000 RangeSlider-2023.7.1/RangeSlider/__init__.py
-drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/RangeSlider.egg-info/
--rw-rw-r--   0 harsh     (1000) harsh     (1000)    12625 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/PKG-INFO
--rw-rw-r--   0 harsh     (1000) harsh     (1000)      209 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/SOURCES.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/dependency_links.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       12 2023-07-18 13:24:27.000000 RangeSlider-2023.7.1/RangeSlider.egg-info/top_level.txt
--rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-07-18 13:24:27.690401 RangeSlider-2023.7.1/setup.cfg
--rw-rw-r--   0 harsh     (1000) harsh     (1000)     2034 2023-07-18 13:23:43.000000 RangeSlider-2023.7.1/setup.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 14:07:46.510510 RangeSlider-2023.7.2/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    13720 2023-07-18 14:07:46.510510 RangeSlider-2023.7.2/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    12837 2023-07-18 14:06:03.000000 RangeSlider-2023.7.2/README.md
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 14:07:46.510510 RangeSlider-2023.7.2/RangeSlider/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    36567 2023-07-18 14:00:29.000000 RangeSlider-2023.7.2/RangeSlider/RangeSlider.py
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       64 2022-12-25 11:45:33.000000 RangeSlider-2023.7.2/RangeSlider/__init__.py
+drwxrwxr-x   0 harsh     (1000) harsh     (1000)        0 2023-07-18 14:07:46.510510 RangeSlider-2023.7.2/RangeSlider.egg-info/
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)    13720 2023-07-18 14:07:46.000000 RangeSlider-2023.7.2/RangeSlider.egg-info/PKG-INFO
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)      209 2023-07-18 14:07:46.000000 RangeSlider-2023.7.2/RangeSlider.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)        1 2023-07-18 14:07:46.000000 RangeSlider-2023.7.2/RangeSlider.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       12 2023-07-18 14:07:46.000000 RangeSlider-2023.7.2/RangeSlider.egg-info/top_level.txt
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)       38 2023-07-18 14:07:46.510510 RangeSlider-2023.7.2/setup.cfg
+-rw-rw-r--   0 harsh     (1000) harsh     (1000)     2034 2023-07-18 14:07:16.000000 RangeSlider-2023.7.2/setup.py
```

### Comparing `RangeSlider-2023.7.1/PKG-INFO` & `RangeSlider-2023.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: RangeSlider
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Python tkinter widget for range selection in slider widget structure with two handles
 Home-page: https://github.com/harshvinay752/RangeSlider
 Author: Harsh Agarwal
 Author-email: harshvinay752@gmail.com
 License: MIT
-Download-URL: https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.1.tar.gz
+Download-URL: https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.2.tar.gz
 Keywords: Python,tkinter,range,slider,two handle,selector,widget
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,21 +19,28 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
-# RangeSlider 2023.07.1
+[![PyPi](https://img.shields.io/pypi/v/RangeSlider)](https://pypi.org/project/RangeSlider/)
+[![Downloads](https://img.shields.io/pypi/dm/RangeSlider)](https://pypi.org/project/RangeSlider)
+
+# RangeSlider 2023.07.2
 
 Range selection widget for Python Tkinter GUI developement in slider widget structure with two handles.
 <!--    
 ***Add-on files***
 + An ipython notebook is provided to illustrate the basic usage of tool. -->
 
+***Updates and Fixes in v2023.07.2 w.r.t v2023.07.1***
++ Updated: Documentation, included padX and padY in widget calls to avoid confusion with errors. However, the values needs to be updated in case of non-suitability depending on system and used font size, handle size etc.
++ Added: Sample ipython notebook containing code. (Visit: https://github.com/harshvinay752/RangeSlider/blob/1a068138c63ca61ccc734e71c27201e7a851c65a/sample.ipynb)
+
 ***Updates and Fixes in v2023.07.1 w.r.t v2022.12.1***
 + Fixed: Error in updation of UI in absence of step markers.
 + Fixed: Error in initialisation of handle values. (Closing the issue: https://github.com/harshvinay752/RangeSlider/issues/7#issue-1806570927)
 + Added: Complimentary check for correct [step_size] parameter in case of usage of step markers.
 + Fixed: Updated example code in documentation.
 
 ***Updates and Fixes in v2022.12.1 w.r.t. v2021.7.4***
@@ -54,15 +61,15 @@
 + Ability to bind a tkinter variable, making it easier to check for slider movement
 + Custom font and position for value text
 + Customizable value precision
 + Custom suffix option
 + Many others...
 
 # Preview
-[![](/image.PNG)](https://raw.githubusercontent.com/harshvinay752/RangeSlider/main/image.PNG)
+[preview.png] image file in repository.
 
 ## Usage
 
 ***Importing required sliders***
 
 For horizontal RangeSlider:
 ```
@@ -84,20 +91,22 @@
 from tkinter.ttk import *
 import tkinter as tk
  
 root = tk.Tk()
  
 hLeft = tk.DoubleVar(value = 0.2)  #left handle variable initialised to value 0.2
 hRight = tk.DoubleVar(value = 0.85)  #right handle variable initialised to value 0.85
-hSlider = RangeSliderH( root , [hLeft, hRight] )   #horizontal slider
+hSlider = RangeSliderH( root , [hLeft, hRight] , padX = 12)   #horizontal slider, [padX] value might be needed to be different depending on system, font and handle size. Usually [padX] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 hSlider.pack()   # or grid or place method could be used
 
 vBottom = tk.DoubleVar(value = 0)   #bottom handle variable
 vTop = tk.DoubleVar(value = 1)   #top handle variable
-vSlider = RangeSliderV( root, [vBottom, vTop] )    #vertical slider
+vSlider = RangeSliderV( root, [vBottom, vTop] , padY = 12)    #vertical slider, [padY] value might be needed to be different depending on system, font and handle size. Usually [padY] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 vSlider.pack()  # or grid or place method could be used
 
 root.mainloop()
 ```
 
 ***Getting current value***
 ```
@@ -226,8 +235,7 @@
 # Words of Developer
 
 This is the second version of this library. It is one of its kind widget for tkinter. When I was developing a tool for my college project I found that at the time no inbuilt or external tool is available for tkinter allowing range selection. However, range selection is a high demand tool specially for applications dealing with data visualizations. I would appreciate any developer from any community who wants to contribute to this project.
 
 I thank RWitak and Sebastian for contributing to this project.
 
 
-
```

### Comparing `RangeSlider-2023.7.1/README.md` & `RangeSlider-2023.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
-# RangeSlider 2023.07.1
+[![PyPi](https://img.shields.io/pypi/v/RangeSlider)](https://pypi.org/project/RangeSlider/)
+[![Downloads](https://img.shields.io/pypi/dm/RangeSlider)](https://pypi.org/project/RangeSlider)
+
+# RangeSlider 2023.07.2
 
 Range selection widget for Python Tkinter GUI developement in slider widget structure with two handles.
 <!--    
 ***Add-on files***
 + An ipython notebook is provided to illustrate the basic usage of tool. -->
 
+***Updates and Fixes in v2023.07.2 w.r.t v2023.07.1***
++ Updated: Documentation, included padX and padY in widget calls to avoid confusion with errors. However, the values needs to be updated in case of non-suitability depending on system and used font size, handle size etc.
++ Added: Sample ipython notebook containing code. (Visit: https://github.com/harshvinay752/RangeSlider/blob/1a068138c63ca61ccc734e71c27201e7a851c65a/sample.ipynb)
+
 ***Updates and Fixes in v2023.07.1 w.r.t v2022.12.1***
 + Fixed: Error in updation of UI in absence of step markers.
 + Fixed: Error in initialisation of handle values. (Closing the issue: https://github.com/harshvinay752/RangeSlider/issues/7#issue-1806570927)
 + Added: Complimentary check for correct [step_size] parameter in case of usage of step markers.
 + Fixed: Updated example code in documentation.
 
 ***Updates and Fixes in v2022.12.1 w.r.t. v2021.7.4***
@@ -29,15 +36,15 @@
 + Ability to bind a tkinter variable, making it easier to check for slider movement
 + Custom font and position for value text
 + Customizable value precision
 + Custom suffix option
 + Many others...
 
 # Preview
-[![](/image.PNG)](https://raw.githubusercontent.com/harshvinay752/RangeSlider/main/image.PNG)
+[preview.png] image file in repository.
 
 ## Usage
 
 ***Importing required sliders***
 
 For horizontal RangeSlider:
 ```
@@ -59,20 +66,22 @@
 from tkinter.ttk import *
 import tkinter as tk
  
 root = tk.Tk()
  
 hLeft = tk.DoubleVar(value = 0.2)  #left handle variable initialised to value 0.2
 hRight = tk.DoubleVar(value = 0.85)  #right handle variable initialised to value 0.85
-hSlider = RangeSliderH( root , [hLeft, hRight] )   #horizontal slider
+hSlider = RangeSliderH( root , [hLeft, hRight] , padX = 12)   #horizontal slider, [padX] value might be needed to be different depending on system, font and handle size. Usually [padX] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 hSlider.pack()   # or grid or place method could be used
 
 vBottom = tk.DoubleVar(value = 0)   #bottom handle variable
 vTop = tk.DoubleVar(value = 1)   #top handle variable
-vSlider = RangeSliderV( root, [vBottom, vTop] )    #vertical slider
+vSlider = RangeSliderV( root, [vBottom, vTop] , padY = 12)    #vertical slider, [padY] value might be needed to be different depending on system, font and handle size. Usually [padY] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 vSlider.pack()  # or grid or place method could be used
 
 root.mainloop()
 ```
 
 ***Getting current value***
 ```
@@ -199,8 +208,7 @@
 
 
 # Words of Developer
 
 This is the second version of this library. It is one of its kind widget for tkinter. When I was developing a tool for my college project I found that at the time no inbuilt or external tool is available for tkinter allowing range selection. However, range selection is a high demand tool specially for applications dealing with data visualizations. I would appreciate any developer from any community who wants to contribute to this project.
 
 I thank RWitak and Sebastian for contributing to this project.
-
```

### Comparing `RangeSlider-2023.7.1/RangeSlider/RangeSlider.py` & `RangeSlider-2023.7.2/RangeSlider/RangeSlider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from tkinter import *
 from tkinter.ttk import *
 
-# v2023.07.1
+# v2023.07.2
 
 class RangeSliderH(Frame):
     LINE_COLOR = "#476b6b"
     LINE_S_COLOR="#0a50ff"
     LINE_WIDTH = 3
     BAR_COLOR_INNER = "#5c8a8a"
     BAR_COLOR_OUTTER = "#c2d6d6"
```

### Comparing `RangeSlider-2023.7.1/RangeSlider.egg-info/PKG-INFO` & `RangeSlider-2023.7.2/RangeSlider.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: RangeSlider
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Python tkinter widget for range selection in slider widget structure with two handles
 Home-page: https://github.com/harshvinay752/RangeSlider
 Author: Harsh Agarwal
 Author-email: harshvinay752@gmail.com
 License: MIT
-Download-URL: https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.1.tar.gz
+Download-URL: https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.2.tar.gz
 Keywords: Python,tkinter,range,slider,two handle,selector,widget
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,21 +19,28 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
-# RangeSlider 2023.07.1
+[![PyPi](https://img.shields.io/pypi/v/RangeSlider)](https://pypi.org/project/RangeSlider/)
+[![Downloads](https://img.shields.io/pypi/dm/RangeSlider)](https://pypi.org/project/RangeSlider)
+
+# RangeSlider 2023.07.2
 
 Range selection widget for Python Tkinter GUI developement in slider widget structure with two handles.
 <!--    
 ***Add-on files***
 + An ipython notebook is provided to illustrate the basic usage of tool. -->
 
+***Updates and Fixes in v2023.07.2 w.r.t v2023.07.1***
++ Updated: Documentation, included padX and padY in widget calls to avoid confusion with errors. However, the values needs to be updated in case of non-suitability depending on system and used font size, handle size etc.
++ Added: Sample ipython notebook containing code. (Visit: https://github.com/harshvinay752/RangeSlider/blob/1a068138c63ca61ccc734e71c27201e7a851c65a/sample.ipynb)
+
 ***Updates and Fixes in v2023.07.1 w.r.t v2022.12.1***
 + Fixed: Error in updation of UI in absence of step markers.
 + Fixed: Error in initialisation of handle values. (Closing the issue: https://github.com/harshvinay752/RangeSlider/issues/7#issue-1806570927)
 + Added: Complimentary check for correct [step_size] parameter in case of usage of step markers.
 + Fixed: Updated example code in documentation.
 
 ***Updates and Fixes in v2022.12.1 w.r.t. v2021.7.4***
@@ -54,15 +61,15 @@
 + Ability to bind a tkinter variable, making it easier to check for slider movement
 + Custom font and position for value text
 + Customizable value precision
 + Custom suffix option
 + Many others...
 
 # Preview
-[![](/image.PNG)](https://raw.githubusercontent.com/harshvinay752/RangeSlider/main/image.PNG)
+[preview.png] image file in repository.
 
 ## Usage
 
 ***Importing required sliders***
 
 For horizontal RangeSlider:
 ```
@@ -84,20 +91,22 @@
 from tkinter.ttk import *
 import tkinter as tk
  
 root = tk.Tk()
  
 hLeft = tk.DoubleVar(value = 0.2)  #left handle variable initialised to value 0.2
 hRight = tk.DoubleVar(value = 0.85)  #right handle variable initialised to value 0.85
-hSlider = RangeSliderH( root , [hLeft, hRight] )   #horizontal slider
+hSlider = RangeSliderH( root , [hLeft, hRight] , padX = 12)   #horizontal slider, [padX] value might be needed to be different depending on system, font and handle size. Usually [padX] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 hSlider.pack()   # or grid or place method could be used
 
 vBottom = tk.DoubleVar(value = 0)   #bottom handle variable
 vTop = tk.DoubleVar(value = 1)   #top handle variable
-vSlider = RangeSliderV( root, [vBottom, vTop] )    #vertical slider
+vSlider = RangeSliderV( root, [vBottom, vTop] , padY = 12)    #vertical slider, [padY] value might be needed to be different depending on system, font and handle size. Usually [padY] = 12 serves,
+                                                              #otherwise a recommended value will be shown through an error message
 vSlider.pack()  # or grid or place method could be used
 
 root.mainloop()
 ```
 
 ***Getting current value***
 ```
@@ -226,8 +235,7 @@
 # Words of Developer
 
 This is the second version of this library. It is one of its kind widget for tkinter. When I was developing a tool for my college project I found that at the time no inbuilt or external tool is available for tkinter allowing range selection. However, range selection is a high demand tool specially for applications dealing with data visualizations. I would appreciate any developer from any community who wants to contribute to this project.
 
 I thank RWitak and Sebastian for contributing to this project.
 
 
-
```

### Comparing `RangeSlider-2023.7.1/setup.py` & `RangeSlider-2023.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 with open("README.md",'r') as fh:
     long_description=fh.read()
 
 setup(
   name = 'RangeSlider',         # How you named your package folder (MyLib)
   packages = ['RangeSlider'],   # Chose the same as "name"
-  version = '2023.07.1',      # Start with a small number and increase it with every change you make
+  version = '2023.07.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python tkinter widget for range selection in slider widget structure with two handles',   # Give a short description about your library
   author = 'Harsh Agarwal',                   # Type in your name
   author_email = 'harshvinay752@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/harshvinay752/RangeSlider',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.1.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/harshvinay752/RangeSlider/archive/refs/tags/2023.07.2.tar.gz',    # I explain this later on
   keywords = ['Python','tkinter','range','slider','two handle','selector','widget'],   # Keywords that define your package best
   install_requires=[],
   long_description=long_description,
   long_description_content_type="text/markdown",
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

