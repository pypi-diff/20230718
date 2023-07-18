# Comparing `tmp/streamlit-cropperjs-0.0.5.tar.gz` & `tmp/streamlit-cropperjs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-cropperjs-0.0.5.tar", last modified: Sun Jul 16 09:12:16 2023, max compression
+gzip compressed data, was "streamlit-cropperjs-0.0.6.tar", last modified: Tue Jul 18 11:13:37 2023, max compression
```

## Comparing `streamlit-cropperjs-0.0.5.tar` & `streamlit-cropperjs-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.222062 streamlit-cropperjs-0.0.5/
--rw-rw-rw-   0        0        0     1048 2023-07-15 10:05:27.000000 streamlit-cropperjs-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       55 2023-07-16 08:33:37.000000 streamlit-cropperjs-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2023-07-16 09:12:16.221060 streamlit-cropperjs-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      503 2023-07-15 10:18:48.000000 streamlit-cropperjs-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 09:12:16.223060 streamlit-cropperjs-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-16 09:12:03.000000 streamlit-cropperjs-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.194061 streamlit-cropperjs-0.0.5/streamlit_cropperjs/
--rw-rw-rw-   0        0        0     4000 2023-07-16 08:39:37.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.181959 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.213059 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/
--rw-rw-rw-   0        0        0      221 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   197413 2023-07-16 07:35:31.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0      471 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.188048 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.218061 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/
--rw-rw-rw-   0        0        0   291787 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js
--rw-rw-rw-   0        0        0      881 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1223369 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.map
-drwxrwxrwx   0        0        0        0 2023-07-16 09:12:16.209060 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/
--rw-rw-rw-   0        0        0      827 2023-07-16 09:12:16.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2023-07-16 09:12:16.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:12:16.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 09:12:16.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 09:12:16.000000 streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.916234 streamlit-cropperjs-0.0.6/
+-rw-rw-rw-   0        0        0     1048 2023-07-15 10:05:27.000000 streamlit-cropperjs-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       55 2023-07-16 08:33:37.000000 streamlit-cropperjs-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1338 2023-07-18 11:13:37.915235 streamlit-cropperjs-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2023-07-16 09:17:05.000000 streamlit-cropperjs-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:13:37.917234 streamlit-cropperjs-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-07-18 11:09:50.000000 streamlit-cropperjs-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.887235 streamlit-cropperjs-0.0.6/streamlit_cropperjs/
+-rw-rw-rw-   0        0        0     4001 2023-07-18 11:06:18.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.880442 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.908235 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/
+-rw-rw-rw-   0        0        0      221 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   197413 2023-07-16 07:35:31.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0      471 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.881442 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.913235 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   291787 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js
+-rw-rw-rw-   0        0        0      881 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1223369 2023-07-16 07:35:30.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.map
+drwxrwxrwx   0        0        0        0 2023-07-18 11:13:37.903237 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/
+-rw-rw-rw-   0        0        0     1338 2023-07-18 11:13:37.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2023-07-18 11:13:37.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:13:37.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 11:13:37.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 11:13:37.000000 streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/top_level.txt
```

### Comparing `streamlit-cropperjs-0.0.5/LICENSE` & `streamlit-cropperjs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.5/PKG-INFO` & `streamlit-cropperjs-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-Metadata-Version: 2.1
-Name: streamlit-cropperjs
-Version: 0.0.5
-Summary: A streamlit module integrating cropperjs
-Home-page: https://github.com/erjieyong/streamlit-cropperjs
-Author: erjieyong
-Author-email: erjieyong@gmail.com
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# streamlit-cropperjs
-
-Integrating the amazing [cropperjs](https://github.com/fengyuanchen/cropperjs) with streamlit. 
-
-This streamlit module is primarily built with mobile usage in mind.
-
-## Features
-- Crop and return image data
-- Supports touch (mobile)
-- Supports cropping on demand with a button
-
-## Future Development
-- Support for all cropperjs options
-- Support for cropperjs v2
-
-## References
-[https://github.com/fengyuanchen/cropperjs](https://github.com/fengyuanchen/cropperjs)
+# Streamlit-cropperjs
+
+Integrating the amazing [cropperjs](https://github.com/fengyuanchen/cropperjs) with streamlit. 
+
+This streamlit module is primarily built with mobile usage in mind.
+
+![](https://github.com/erjieyong/streamlit-cropperjs/blob/main/streamlit-cropperjs-demo.gif)
+## Installation
+`pip install streamlit-cropperjs`
+
+## Example
+```
+import streamlit as st
+
+from streamlit_cropperjs import st_cropperjs
+
+pic = st.file_uploader("Upload a picture", key="uploaded_pic")
+if pic:
+    pic = pic.read()
+    cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
+    if cropped_pic:
+        st.image(cropped_pic, output_format="PNG")
+```
+
+## Features
+- Crop and return image data
+- Supports touch (mobile)
+- Supports cropping on demand with a button (customised button text)
+
+## Future Development
+- Support for all cropperjs options
+- Support for cropperjs v2
+
+## References
+[https://github.com/fengyuanchen/cropperjs](https://github.com/fengyuanchen/cropperjs)
```

### Comparing `streamlit-cropperjs-0.0.5/setup.py` & `streamlit-cropperjs-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-cropperjs",
-    version="0.0.5",
+    version="0.0.6",
     author="erjieyong",
     author_email="erjieyong@gmail.com",
     description="A streamlit module integrating cropperjs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erjieyong/streamlit-cropperjs",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs/__init__.py` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,13 +80,13 @@
 
 
 # Add some test code to play with the component while it's in development.
 # During development, we can run this just as we would any other Streamlit
 # app: `$ streamlit run st_cropperjs/__init__.py`
 if not _RELEASE:
     st.subheader("Streamlit-Cropperjs")
-    pic = st.camera_input("Upload a picture", key="uploaded_pic")
+    pic = st.file_uploader("Upload a picture", key="uploaded_pic")
     if pic:
         pic = pic.read()
         cropped_pic = st_cropperjs(pic=pic, btn_text="Detect!", key="foo")
         if cropped_pic:
             st.image(cropped_pic, output_format="PNG")
```

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/bootstrap.min.css` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.LICENSE.txt` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.map` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs/frontend/build/static/js/main.6951a196.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-cropperjs-0.0.5/streamlit_cropperjs.egg-info/SOURCES.txt` & `streamlit-cropperjs-0.0.6/streamlit_cropperjs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

