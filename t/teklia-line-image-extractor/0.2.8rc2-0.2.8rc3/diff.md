# Comparing `tmp/teklia-line-image-extractor-0.2.8rc2.tar.gz` & `tmp/teklia-line-image-extractor-0.2.8rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teklia-line-image-extractor-0.2.8rc2.tar", last modified: Thu Apr 13 09:27:19 2023, max compression
+gzip compressed data, was "teklia-line-image-extractor-0.2.8rc3.tar", last modified: Tue Jul 18 17:04:42 2023, max compression
```

## Comparing `teklia-line-image-extractor-0.2.8rc2.tar` & `teklia-line-image-extractor-0.2.8rc3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2308 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1500 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.351626 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     7197 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/line_image_extractor/main.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1444 2023-04-13 09:27:06.000000 teklia-line-image-extractor-0.2.8rc2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:27:19.355626 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2308 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      503 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-13 09:27:19.000000 teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:04:42.334267 teklia-line-image-extractor-0.2.8rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-18 17:04:42.334267 teklia-line-image-extractor-0.2.8rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-18 17:04:34.000000 teklia-line-image-extractor-0.2.8rc3/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:04:42.334267 teklia-line-image-extractor-0.2.8rc3/line_image_extractor/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/line_image_extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/line_image_extractor/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7197 2023-07-18 17:03:32.000000 teklia-line-image-extractor-0.2.8rc3/line_image_extractor/image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/line_image_extractor/main.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 17:04:42.334267 teklia-line-image-extractor-0.2.8rc3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1444 2023-07-12 17:01:10.000000 teklia-line-image-extractor-0.2.8rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 17:04:42.334267 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-18 17:04:42.000000 teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/top_level.txt
```

### Comparing `teklia-line-image-extractor-0.2.8rc2/LICENSE` & `teklia-line-image-extractor-0.2.8rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc2/PKG-INFO` & `teklia-line-image-extractor-0.2.8rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.8rc2
+Version: 0.2.8rc3
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.com/teklia/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `teklia-line-image-extractor-0.2.8rc2/README.md` & `teklia-line-image-extractor-0.2.8rc3/README.md`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/extractor.py` & `teklia-line-image-extractor-0.2.8rc3/line_image_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/image_utils.py` & `teklia-line-image-extractor-0.2.8rc3/line_image_extractor/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     return bg + poly_img
 
 
 def extract_min_area_rect_image(img: np.ndarray, polygon: np.ndarray) -> np.ndarray:
     min_area_rect = cv2.minAreaRect(polygon)
     # convert minimum area rect to polygon
     box = cv2.boxPoints(min_area_rect)
-    box = np.int0(box)
+    box = np.intp(box)
     bbox = polygon_to_bbox(box)
 
     # get min area rect image
     box_img = extract_polygon_image(img, polygon=box, bbox=bbox)
     return box_img
```

### Comparing `teklia-line-image-extractor-0.2.8rc2/line_image_extractor/main.py` & `teklia-line-image-extractor-0.2.8rc3/line_image_extractor/main.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc2/setup.py` & `teklia-line-image-extractor-0.2.8rc3/setup.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.8rc2/teklia_line_image_extractor.egg-info/PKG-INFO` & `teklia-line-image-extractor-0.2.8rc3/teklia_line_image_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.8rc2
+Version: 0.2.8rc3
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.com/teklia/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

