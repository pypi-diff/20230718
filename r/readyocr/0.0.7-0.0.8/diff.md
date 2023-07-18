# Comparing `tmp/readyocr-0.0.7.tar.gz` & `tmp/readyocr-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readyocr-0.0.7.tar", last modified: Fri Jul  7 08:54:15 2023, max compression
+gzip compressed data, was "readyocr-0.0.8.tar", last modified: Tue Jul 18 03:54:12 2023, max compression
```

## Comparing `readyocr-0.0.7.tar` & `readyocr-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.638320 readyocr-0.0.7/
--rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.7/LICENSE
--rw-r--r--   0 annguyen   (501) staff       (20)     4976 2023-07-07 08:54:15.638163 readyocr-0.0.7/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     3220 2023-07-07 08:52:15.000000 readyocr-0.0.7/README.md
--rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-07 08:54:01.000000 readyocr-0.0.7/pyproject.toml
--rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-07 08:54:15.638372 readyocr-0.0.7/setup.cfg
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.632150 readyocr-0.0.7/src/
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.633249 readyocr-0.0.7/src/readyocr/
--rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.7/src/readyocr/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.7/src/readyocr/__main__.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.636899 readyocr-0.0.7/src/readyocr/entities/
--rw-r--r--   0 annguyen   (501) staff       (20)      673 2023-07-07 07:27:48.000000 readyocr-0.0.7/src/readyocr/entities/__init__.py
--rw-r--r--   0 annguyen   (501) staff       (20)     6096 2023-07-04 09:06:20.000000 readyocr-0.0.7/src/readyocr/entities/bbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.7/src/readyocr/entities/block.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1707 2023-07-04 10:52:14.000000 readyocr-0.0.7/src/readyocr/entities/cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3092 2023-07-06 09:13:13.000000 readyocr-0.0.7/src/readyocr/entities/document.py
--rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.7/src/readyocr/entities/entity_list.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-06 09:24:44.000000 readyocr-0.0.7/src/readyocr/entities/entity_tag.py
--rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.7/src/readyocr/entities/key.py
--rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.7/src/readyocr/entities/line.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1800 2023-07-04 14:14:05.000000 readyocr-0.0.7/src/readyocr/entities/merged_cell.py
--rw-r--r--   0 annguyen   (501) staff       (20)     3184 2023-07-06 09:12:12.000000 readyocr-0.0.7/src/readyocr/entities/page.py
--rw-r--r--   0 annguyen   (501) staff       (20)     4740 2023-07-06 09:12:08.000000 readyocr-0.0.7/src/readyocr/entities/page_entity.py
--rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.7/src/readyocr/entities/paragraph.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1071 2023-07-04 10:51:14.000000 readyocr-0.0.7/src/readyocr/entities/table.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1702 2023-07-04 07:38:31.000000 readyocr-0.0.7/src/readyocr/entities/textbox.py
--rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.7/src/readyocr/entities/value.py
--rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.7/src/readyocr/entities/word.py
--rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.7/src/readyocr/exceptions.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.637437 readyocr-0.0.7/src/readyocr/parsers/
--rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.7/src/readyocr/parsers/google_document_ai_parser.py
--rw-r--r--   0 annguyen   (501) staff       (20)     7385 2023-07-07 07:50:05.000000 readyocr-0.0.7/src/readyocr/parsers/textract_parser.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.637928 readyocr-0.0.7/src/readyocr/utils/
--rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.7/src/readyocr/utils/geometry_utils.py
--rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.7/src/readyocr/utils/languages.py
--rw-r--r--   0 annguyen   (501) staff       (20)     4165 2023-07-07 08:41:10.000000 readyocr-0.0.7/src/readyocr/utils/visualize.py
-drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-07 08:54:15.633987 readyocr-0.0.7/src/readyocr.egg-info/
--rw-r--r--   0 annguyen   (501) staff       (20)     4976 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/PKG-INFO
--rw-r--r--   0 annguyen   (501) staff       (20)     1034 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/SOURCES.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/dependency_links.txt
--rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/requires.txt
--rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-07 08:54:15.000000 readyocr-0.0.7/src/readyocr.egg-info/top_level.txt
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.729426 readyocr-0.0.8/
+-rw-r--r--   0 annguyen   (501) staff       (20)     1054 2023-07-05 10:49:26.000000 readyocr-0.0.8/LICENSE
+-rw-r--r--   0 annguyen   (501) staff       (20)     5273 2023-07-18 03:54:12.729266 readyocr-0.0.8/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     3517 2023-07-18 03:52:51.000000 readyocr-0.0.8/README.md
+-rw-r--r--   0 annguyen   (501) staff       (20)      954 2023-07-18 03:53:05.000000 readyocr-0.0.8/pyproject.toml
+-rw-r--r--   0 annguyen   (501) staff       (20)       38 2023-07-18 03:54:12.729479 readyocr-0.0.8/setup.cfg
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.717564 readyocr-0.0.8/src/
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.719091 readyocr-0.0.8/src/readyocr/
+-rw-r--r--   0 annguyen   (501) staff       (20)        0 2023-07-06 03:56:02.000000 readyocr-0.0.8/src/readyocr/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)       85 2023-07-06 03:55:00.000000 readyocr-0.0.8/src/readyocr/__main__.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.726919 readyocr-0.0.8/src/readyocr/entities/
+-rw-r--r--   0 annguyen   (501) staff       (20)      673 2023-07-07 07:27:48.000000 readyocr-0.0.8/src/readyocr/entities/__init__.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     6272 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/bbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      939 2023-07-05 06:44:00.000000 readyocr-0.0.8/src/readyocr/entities/block.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2010 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3299 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/document.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2900 2023-07-06 09:24:46.000000 readyocr-0.0.8/src/readyocr/entities/entity_list.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1044 2023-07-07 09:42:13.000000 readyocr-0.0.8/src/readyocr/entities/entity_tag.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      702 2023-07-04 07:38:27.000000 readyocr-0.0.8/src/readyocr/entities/key.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      707 2023-07-04 07:38:28.000000 readyocr-0.0.8/src/readyocr/entities/line.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2098 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/merged_cell.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     3314 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/page.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     5142 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/page_entity.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      963 2023-07-05 06:43:29.000000 readyocr-0.0.8/src/readyocr/entities/paragraph.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1241 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/table.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     2211 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/entities/textbox.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      712 2023-07-04 07:38:31.000000 readyocr-0.0.8/src/readyocr/entities/value.py
+-rw-r--r--   0 annguyen   (501) staff       (20)      933 2023-07-04 14:04:18.000000 readyocr-0.0.8/src/readyocr/entities/word.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     1121 2023-06-29 07:18:54.000000 readyocr-0.0.8/src/readyocr/exceptions.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.727877 readyocr-0.0.8/src/readyocr/parsers/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5782 2023-07-07 04:10:18.000000 readyocr-0.0.8/src/readyocr/parsers/google_document_ai_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7781 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/parsers/readyocr_parser.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     7360 2023-07-18 03:36:31.000000 readyocr-0.0.8/src/readyocr/parsers/textract_parser.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.728818 readyocr-0.0.8/src/readyocr/utils/
+-rw-r--r--   0 annguyen   (501) staff       (20)      233 2023-06-29 04:14:42.000000 readyocr-0.0.8/src/readyocr/utils/geometry_utils.py
+-rw-r--r--   0 annguyen   (501) staff       (20)    15686 2023-06-30 09:13:14.000000 readyocr-0.0.8/src/readyocr/utils/languages.py
+-rw-r--r--   0 annguyen   (501) staff       (20)     4165 2023-07-07 08:41:10.000000 readyocr-0.0.8/src/readyocr/utils/visualize.py
+drwxr-xr-x   0 annguyen   (501) staff       (20)        0 2023-07-18 03:54:12.720116 readyocr-0.0.8/src/readyocr.egg-info/
+-rw-r--r--   0 annguyen   (501) staff       (20)     5273 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/PKG-INFO
+-rw-r--r--   0 annguyen   (501) staff       (20)     1074 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/SOURCES.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        1 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/dependency_links.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)      176 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/requires.txt
+-rw-r--r--   0 annguyen   (501) staff       (20)        9 2023-07-18 03:54:12.000000 readyocr-0.0.8/src/readyocr.egg-info/top_level.txt
```

### Comparing `readyocr-0.0.7/LICENSE` & `readyocr-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/PKG-INFO` & `readyocr-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.7
+Version: 0.0.8
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -114,14 +114,26 @@
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    dict_resp = document.export_json()
+
+    #TODO: finish load function, please refer to Textract Package
+    same_document = load(dict_resp)
+    ```
+
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.7/README.md` & `readyocr-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,26 @@
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    dict_resp = document.export_json()
+
+    #TODO: finish load function, please refer to Textract Package
+    same_document = load(dict_resp)
+    ```
+
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.7/pyproject.toml` & `readyocr-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "readyocr"
-version = "0.0.7"
+version = "0.0.8"
 description = "A nice package OCR for Amazon Textract and Google Document AI"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
   { name="Sy An", email="syan.vn@gmail.com" },
 ]
 classifiers = [
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/__init__.py` & `readyocr-0.0.8/src/readyocr/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/bbox.py` & `readyocr-0.0.8/src/readyocr/entities/bbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,7 +150,15 @@
         :return: Returns denormalized co-ordinates x, y and dimensions width, height as numpy array.
         :rtype: numpy.array
         """
         return np.array([self.x, self.y, self.width, self.height])
 
     def __repr__(self):
         return f"BoundingBox(x: {self.x}, y: {self.y}, width: {self.width}, height: {self.height})"
+    
+    def export_json(self):
+        return {
+            "x": self.x,
+            "y": self.y,
+            "width": self.width,
+            "height": self.height
+        }
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/block.py` & `readyocr-0.0.8/src/readyocr/entities/block.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/cell.py` & `readyocr-0.0.8/src/readyocr/entities/cell.py`

 * *Files 18% similar despite different names*

```diff
@@ -59,8 +59,19 @@
     def col_index(self, col_index: int):
         """
         Sets the column index of the cell
 
         :param col_index: Column index of the cell
         :type col_index: int
         """
-        self._col_index = int(col_index)
+        self._col_index = int(col_index)
+
+    def export_json(self):
+        """
+        :return: Returns the json representation of the cell
+        :rtype: dict
+        """
+        response = super().export_json()
+        response["rowIndex"] = self.row_index
+        response["columnIndex"] = self.col_index
+        
+        return response
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/document.py` & `readyocr-0.0.8/src/readyocr/entities/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,8 +85,17 @@
         return EntityList(descendants)
     
     def __repr__(self):
         return os.linesep.join([
             "This document holds the following data:",
             f"Pages - {len(self.pages)}",
             f"Descendants - {len(self.descendants)}"
-        ])
+        ])
+    
+    def export_json(self):
+        return {
+            "document": {
+                "pages": [
+                    page.export_json() for page in self._pages
+                ]
+            }
+        }
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/entity_list.py` & `readyocr-0.0.8/src/readyocr/entities/entity_list.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/entity_tag.py` & `readyocr-0.0.8/src/readyocr/entities/entity_tag.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/key.py` & `readyocr-0.0.8/src/readyocr/entities/key.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/line.py` & `readyocr-0.0.8/src/readyocr/entities/line.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/merged_cell.py` & `readyocr-0.0.8/src/readyocr/entities/merged_cell.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,8 +61,19 @@
     def col_span(self, col_span: int):
         """
         Sets the column span of the MergedCell
 
         :param col_span: Column span of the MergedCell
         :type col_span: int
         """
-        self._col_span = int(col_span)
+        self._col_span = int(col_span)
+
+    def export_json(self):
+        """
+        :return: Returns the json representation of the merged cell
+        :rtype: dict
+        """
+        response = super().export_json()
+        response["rowSpan"] = self.row_span
+        response["columnSpan"] = self.col_span
+
+        return response
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/page.py` & `readyocr-0.0.8/src/readyocr/entities/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import os
-import string
-import logging
-from typing import List, Tuple
-from copy import deepcopy
-from collections import defaultdict
-
 from readyocr.entities.bbox import SpatialObject
 from readyocr.entities.entity_list import EntityList
-from readyocr.utils.geometry_utils import sort_by_position
 from readyocr.entities.page_entity import PageEntity
 
 
 class Page(SpatialObject):
     """ 
     Creates a new document, ideally representing a single item in the dataset.
     
@@ -104,7 +97,18 @@
         return EntityList(parents)
     
     def __repr__(self):
         return os.linesep.join([
             f"Page(id: {self.id}, width: {self.width}, height: {self.height}, page_num: {self.page_num})",
             f"Children - {len(self.children)}"
         ])
+    
+    def export_json(self):
+        return {
+            "id": self.id,
+            "pageNumber": self.page_num,
+            "dimension": {
+                "width": self.width,
+                "height": self.height
+            },
+            "entities": [x.export_json() for x in self.descendants]
+        }
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/page_entity.py` & `readyocr-0.0.8/src/readyocr/entities/page_entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Dict
 from typing_extensions import Self
 
 from readyocr.entities.bbox import BoundingBox
 from readyocr.entities.entity_list import EntityList
 from readyocr.entities.entity_tag import EntityTag
 
+
 class PageEntity(ABC):
     """
     :param id: Unique identifier for the document entity.
 
     :param ABC: Abstract Base Class for all Document entities.
     :type ABC: ABC
     """
@@ -170,7 +171,20 @@
     def __eq__(self, other):
         if isinstance(other, PageEntity):
             return self.id == other.id
         return NotImplemented
     
     def __hash__(self):
         return hash(self.id)
+
+    def export_json(self):
+        """
+        Exports the entity as a JSON object.
+        """
+        return {
+            "id": self.id,
+            "class": self.__class__.__name__,
+            "boundingBox": self.bbox.export_json(),
+            "metadata": self.metadata,
+            "tags": [tag for tag in self.tags],
+            "childrendIds": [child.id for child in self.children]
+        }
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/paragraph.py` & `readyocr-0.0.8/src/readyocr/entities/paragraph.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/table.py` & `readyocr-0.0.8/src/readyocr/entities/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,8 +37,17 @@
     def title(self, title: str):
         """
         Sets the title of the Table
 
         :param title: title of the Table
         :type title: str
         """
-        self._title = title
+        self._title = title
+
+    def add(self, child: PageEntity):
+        """
+        _summary_
+
+        :return: _description_
+        :rtype: _type_
+        """
+        self._children.add(child)
```

### Comparing `readyocr-0.0.7/src/readyocr/entities/value.py` & `readyocr-0.0.8/src/readyocr/entities/value.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/entities/word.py` & `readyocr-0.0.8/src/readyocr/entities/word.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/exceptions.py` & `readyocr-0.0.8/src/readyocr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/parsers/google_document_ai_parser.py` & `readyocr-0.0.8/src/readyocr/parsers/google_document_ai_parser.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/parsers/textract_parser.py` & `readyocr-0.0.8/src/readyocr/parsers/textract_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from textractor.parsers.response_parser import parse
 
 from readyocr.entities import BoundingBox, Word, Line, Table, Cell, MergedCell, Key, Value, Page, Document
 
-def load(textract_json: dict) -> Document:
+def load(response: dict) -> Document:
     """
     Convert textract json to readyocr document
 
-    :param textract_json: json response from textract
-    :type textract_json: dict
+    :param response: json response from textract
+    :type response: dict
     :return: readyocr document
     :rtype: Document
     """
-    t_doc = parse(textract_json)
+    t_doc = parse(response)
     document = Document(num_pages=len(t_doc.pages))
 
     for t_page in t_doc.pages:
         page = Page(
             id=t_page.id,
-            width=t_page.width,
-            height=t_page.height,
+            width=None,
+            height=None,
             page_num=t_page.page_num
         )
 
         # Extract t_line t_word from textract and add to readyocr page
         for t_line in t_page.lines:
             line = Line(
                 id=t_line.id,
@@ -62,15 +62,15 @@
                     y=t_key.y,
                     width=t_key.width,
                     height=t_key.height,
                 ),
                 text='key',
                 confidence=t_key.confidence
             )
-
+            
             # add word to key
             for t_word in t_key.words:
                 word = Word(
                     id=t_word.id,
                     bbox=BoundingBox(
                         x=t_word.x,
                         y=t_word.y,
```

### Comparing `readyocr-0.0.7/src/readyocr/utils/languages.py` & `readyocr-0.0.8/src/readyocr/utils/languages.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr/utils/visualize.py` & `readyocr-0.0.8/src/readyocr/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `readyocr-0.0.7/src/readyocr.egg-info/PKG-INFO` & `readyocr-0.0.8/src/readyocr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readyocr
-Version: 0.0.7
+Version: 0.0.8
 Summary: A nice package OCR for Amazon Textract and Google Document AI
 Author-email: Sy An <syan.vn@gmail.com>
 License: Copyright 2023 Sy An
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -114,14 +114,26 @@
             textbox=item,
             padding=1,
         )
     ```
 
     ![Textract Textbox Output Visualize](https://raw.githubusercontent.com/syanng/readyocr/main/images/visualize_textbox.png)
 
+* ReadyOCR support export json object and also load from same json object
+
+    ```
+    from readyocr.parsers.readyocr_parser import load
+
+    ...
+    dict_resp = document.export_json()
+
+    #TODO: finish load function, please refer to Textract Package
+    same_document = load(dict_resp)
+    ```
+
 ### Examples
 
 Please find all the available [examples](examples/) for better understanding ReadyOCR.
 
 ### License
 
 ReadyOCR is released under the MIT license. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `readyocr-0.0.7/src/readyocr.egg-info/SOURCES.txt` & `readyocr-0.0.8/src/readyocr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 src/readyocr/entities/page_entity.py
 src/readyocr/entities/paragraph.py
 src/readyocr/entities/table.py
 src/readyocr/entities/textbox.py
 src/readyocr/entities/value.py
 src/readyocr/entities/word.py
 src/readyocr/parsers/google_document_ai_parser.py
+src/readyocr/parsers/readyocr_parser.py
 src/readyocr/parsers/textract_parser.py
 src/readyocr/utils/geometry_utils.py
 src/readyocr/utils/languages.py
 src/readyocr/utils/visualize.py
```

