# Comparing `tmp/graph_cordinates-0.0.3.tar.gz` & `tmp/graph_cordinates-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_cordinates-0.0.3.tar", last modified: Sat Jul 15 14:04:26 2023, max compression
+gzip compressed data, was "graph_cordinates-0.0.4.tar", last modified: Tue Jul 18 08:56:54 2023, max compression
```

## Comparing `graph_cordinates-0.0.3.tar` & `graph_cordinates-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/
--rw-rw-rw-   0        0        0     1348 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.346145 graph_cordinates-0.0.3/graph_cordinates/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.3/graph_cordinates/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.3/graph_cordinates/graph_cordinates.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/graph_cordinates.egg-info/
--rw-rw-rw-   0        0        0     1348 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1740 2023-07-15 14:03:59.000000 graph_cordinates-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:56:54.680544 graph_cordinates-0.0.4/
+-rw-rw-rw-   0        0        0     1465 2023-07-18 08:56:54.680544 graph_cordinates-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 08:56:54.647250 graph_cordinates-0.0.4/graph_cordinates/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.4/graph_cordinates/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.4/graph_cordinates/graph_cordinates.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:56:54.679273 graph_cordinates-0.0.4/graph_cordinates.egg-info/
+-rw-rw-rw-   0        0        0     1465 2023-07-18 08:56:54.000000 graph_cordinates-0.0.4/graph_cordinates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-18 08:56:54.000000 graph_cordinates-0.0.4/graph_cordinates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:56:54.000000 graph_cordinates-0.0.4/graph_cordinates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-18 08:56:54.000000 graph_cordinates-0.0.4/graph_cordinates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:56:54.680544 graph_cordinates-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1792 2023-07-18 08:55:12.000000 graph_cordinates-0.0.4/setup.py
```

### Comparing `graph_cordinates-0.0.3/PKG-INFO` & `graph_cordinates-0.0.4/graph_cordinates.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: graph_cordinates
-Version: 0.0.3
+Name: graph-cordinates
+Version: 0.0.4
 Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array 
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
-Keywords: stock price,Python,Cordinates,Image,2D Curve
+Keywords: stock_price,Python,Cordinates,Image,2D Curve
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
  
+See the logic and an example implementation on my github
+
+https://github.com/kumarUjjawal3621/mypython_lib 
+
+
 How to use: 
 
 1. import graph_cordinates.graph_cordinates as gc 
 
 2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) 
 
 3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image 
@@ -35,7 +40,8 @@
 
    0: When the graph's background color is relatively darker than the curve
 
    1: Otherwise)  
 
 
 Caution- Try to pass the Image by erasing the axes
+
```

### Comparing `graph_cordinates-0.0.3/graph_cordinates/graph_cordinates.py` & `graph_cordinates-0.0.4/graph_cordinates/graph_cordinates.py`

 * *Files identical despite different names*

### Comparing `graph_cordinates-0.0.3/graph_cordinates.egg-info/PKG-INFO` & `graph_cordinates-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
-Name: graph-cordinates
-Version: 0.0.3
+Name: graph_cordinates
+Version: 0.0.4
 Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array 
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
-Keywords: stock price,Python,Cordinates,Image,2D Curve
+Keywords: stock_price,Python,Cordinates,Image,2D Curve
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
  
+See the logic and an example implementation on my github
+
+https://github.com/kumarUjjawal3621/mypython_lib 
+
+
 How to use: 
 
 1. import graph_cordinates.graph_cordinates as gc 
 
 2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) 
 
 3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image 
@@ -35,7 +40,8 @@
 
    0: When the graph's background color is relatively darker than the curve
 
    1: Otherwise)  
 
 
 Caution- Try to pass the Image by erasing the axes
+
```

### Comparing `graph_cordinates-0.0.3/setup.py` & `graph_cordinates-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
-DESCRIPTION = 'From Image of a curve/graph, extract and store the cordinates pairs in a 2D array \n Github link (https://github.com/kumarUjjawal3621/mypython_lib)'
+VERSION = '0.0.4'
+DESCRIPTION = 'From Image of a curve/graph, extract and store the cordinates pairs in a 2D array '
 LONG_DESCRIPTION = """ 
+See the logic and an example implementation on my github\n
+https://github.com/kumarUjjawal3621/mypython_lib \n
+
 How to use: \n
 1. import graph_cordinates.graph_cordinates as gc \n
 2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) \n
 3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image \n
     
 How to pass arguments- \n
 1. image_path == path to a graph image \n
 2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]\n
 3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]\n
 4. background_value == 0 or 1 \n
    0: When the graph's background color is relatively darker than the curve\n
    1: Otherwise)  \n
 
 Caution- Try to pass the Image by erasing the axes
+
 """
 # Setting up
 
 setup(
     name="graph_cordinates",
     version=VERSION,
     author="Ujjawal Kumar (India)",
     author_email="<kumarujjawal3621@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['stock price','Python', 'Cordinates', 'Image', '2D Curve'],
+    keywords=['stock_price','Python', 'Cordinates', 'Image', '2D Curve'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

