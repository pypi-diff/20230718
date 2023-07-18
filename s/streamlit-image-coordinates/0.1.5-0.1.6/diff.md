# Comparing `tmp/streamlit-image-coordinates-0.1.5.tar.gz` & `tmp/streamlit-image-coordinates-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-image-coordinates-0.1.5.tar", last modified: Tue Jun 13 14:47:53 2023, max compression
+gzip compressed data, was "streamlit-image-coordinates-0.1.6.tar", last modified: Tue Jul 18 14:45:16 2023, max compression
```

## Comparing `streamlit-image-coordinates-0.1.5.tar` & `streamlit-image-coordinates-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:29.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:53.399477 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 14:47:53.000000 streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:16.833133 streamlit-image-coordinates-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 14:45:16.833133 streamlit-image-coordinates-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:45:16.833133 streamlit-image-coordinates-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:16.829133 streamlit-image-coordinates-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:16.829133 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:16.833133 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:04.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:45:16.833133 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-18 14:45:16.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 14:45:16.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:45:16.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 14:45:16.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 14:45:16.000000 streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/top_level.txt
```

### Comparing `streamlit-image-coordinates-0.1.5/LICENSE` & `streamlit-image-coordinates-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.5/PKG-INFO` & `streamlit-image-coordinates-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.5
+Version: 0.1.6
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.5/README.md` & `streamlit-image-coordinates-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.5/setup.py` & `streamlit-image-coordinates-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-image-coordinates",
-    version="0.1.5",
+    version="0.1.6",
     author="Zachary Blackwood",
     author_email="zachary@streamlit.io",
     description=(
         "Streamlit component that displays an image and returns the coordinates when "
         "you click on it"
     ),
     long_description=long_description,
```

### Comparing `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/__init__.py` & `streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/main.js` & `streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -45,15 +45,15 @@
             } else if (!width) {
                 width = height * img.naturalWidth / img.naturalHeight
             }
 
             img.width = width
             img.height = height
 
-            Streamlit.setFrameHeight(height)
+            Streamlit.setFrameHeight(height + 10)
 
             // When image is clicked, send the coordinates to Python through sendValue
             if (!img.onclick) {
                 img.onclick = clickListener
             }
         }
     }
```

### Comparing `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js` & `streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/PKG-INFO` & `streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-image-coordinates
-Version: 0.1.5
+Version: 0.1.6
 Summary: Streamlit component that displays an image and returns the coordinates when you click on it
 Home-page: https://github.com/blackary/streamlit-image-coordinates/
 Author: Zachary Blackwood
 Author-email: zachary@streamlit.io
 License: MIT License
 Keywords: python streamlit images component
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `streamlit-image-coordinates-0.1.5/src/streamlit_image_coordinates.egg-info/SOURCES.txt` & `streamlit-image-coordinates-0.1.6/src/streamlit_image_coordinates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

