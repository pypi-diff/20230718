# Comparing `tmp/PyPDFForm-1.2.9.tar.gz` & `tmp/PyPDFForm-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.9.tar", last modified: Sun Jun 11 04:10:16 2023, max compression
+gzip compressed data, was "PyPDFForm-1.3.0.tar", last modified: Mon Jul 17 22:01:49 2023, max compression
```

## Comparing `PyPDFForm-1.2.9.tar` & `PyPDFForm-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.078910 PyPDFForm-1.2.9/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.082911 PyPDFForm-1.2.9/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/font_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.082911 PyPDFForm-1.2.9/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 04:10:16.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:49.460981 PyPDFForm-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-17 22:01:49.460981 PyPDFForm-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:49.456981 PyPDFForm-1.3.0/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:49.460981 PyPDFForm-1.3.0/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/font_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:49.460981 PyPDFForm-1.3.0/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:01:49.456981 PyPDFForm-1.3.0/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-17 22:01:49.000000 PyPDFForm-1.3.0/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-17 22:01:49.000000 PyPDFForm-1.3.0/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:01:49.000000 PyPDFForm-1.3.0/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-17 22:01:49.000000 PyPDFForm-1.3.0/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 22:01:49.000000 PyPDFForm-1.3.0/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:01:49.460981 PyPDFForm-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-17 22:01:34.000000 PyPDFForm-1.3.0/setup.py
```

### Comparing `PyPDFForm-1.2.9/LICENSE` & `PyPDFForm-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PKG-INFO` & `PyPDFForm-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.9
+Version: 1.3.0
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
-    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"></a>
     <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.9 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.3.0 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
 chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
                     //static.pepy.tech/personalized-badge/
-pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
              [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/constants.py` & `PyPDFForm-1.3.0/PyPDFForm/core/constants.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/filler.py` & `PyPDFForm-1.3.0/PyPDFForm/core/filler.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,52 +27,42 @@
     radio_button_tracker = {}
 
     for page, _elements in template.get_elements_by_page(template_pdf).items():
         texts_to_draw[page] = []
         text_watermarks.append(b"")
         for _element in _elements:
             key = template.get_element_key(_element)
+            needs_to_be_drawn = False
 
-            if isinstance(elements[key], Checkbox):
-                if elements[key].value:
-                    font_size = font_size_core.checkbox_radio_font_size(_element)
-                    _to_draw = utils.checkbox_radio_to_draw(elements[key], font_size)
-                    x, y = template.get_draw_checkbox_radio_coordinates(
-                        _element, _to_draw
-                    )
-                    texts_to_draw[page].append(
-                        [
-                            _to_draw,
-                            x,
-                            y,
-                        ]
-                    )
-            elif isinstance(elements[key], Radio):
-                if key not in radio_button_tracker:
-                    radio_button_tracker[key] = 0
-                radio_button_tracker[key] += 1
-
-                if elements[key].value == radio_button_tracker[key] - 1:
-                    font_size = font_size_core.checkbox_radio_font_size(_element)
-                    _to_draw = utils.checkbox_radio_to_draw(elements[key], font_size)
-                    x, y = template.get_draw_checkbox_radio_coordinates(
-                        _element, _to_draw
-                    )
-                    texts_to_draw[page].append(
-                        [
-                            _to_draw,
-                            x,
-                            y,
-                        ]
-                    )
+            if isinstance(elements[key], (Checkbox, Radio)):
+                font_size = font_size_core.checkbox_radio_font_size(_element)
+                _to_draw = utils.checkbox_radio_to_draw(elements[key], font_size)
+                x, y = template.get_draw_checkbox_radio_coordinates(_element, _to_draw)
+                if isinstance(elements[key], Checkbox) and elements[key].value:
+                    needs_to_be_drawn = True
+                elif isinstance(elements[key], Radio):
+                    if key not in radio_button_tracker:
+                        radio_button_tracker[key] = 0
+                    radio_button_tracker[key] += 1
+                    if elements[key].value == radio_button_tracker[key] - 1:
+                        needs_to_be_drawn = True
             else:
+                elements[
+                    key
+                ].text_line_x_coordinates = template.get_text_line_x_coordinates(
+                    _element, elements[key]
+                )
                 x, y = template.get_draw_text_coordinates(_element, elements[key])
+                _to_draw = elements[key]
+                needs_to_be_drawn = True
+
+            if needs_to_be_drawn:
                 texts_to_draw[page].append(
                     [
-                        elements[key],
+                        _to_draw,
                         x,
                         y,
                     ]
                 )
 
     for page, texts in texts_to_draw.items():
         _watermarks = watermark_core.create_watermarks_and_draw(
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/font.py` & `PyPDFForm-1.3.0/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/font_size.py` & `PyPDFForm-1.3.0/PyPDFForm/core/font_size.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,19 @@
 # -*- coding: utf-8 -*-
 """Contains helpers for calculating font sizes."""
 
 from math import sqrt
-from typing import Dict, Union
+from typing import Union
 
 import pdfrw
 
-from ..middleware.constants import ELEMENT_TYPES, GLOBAL_FONT_SIZE
-from ..middleware.text import Text
+from ..middleware.constants import GLOBAL_FONT_SIZE
 from . import constants, template
 
 
-def update_text_field_font_sizes(
-    template_stream: bytes,
-    elements: Dict[str, ELEMENT_TYPES],
-) -> None:
-    """Updates text fields' font sizes."""
-
-    template_pdf = pdfrw.PdfReader(fdata=template_stream)
-
-    for _, _elements in template.get_elements_by_page(template_pdf).items():
-        for _element in _elements:
-            key = template.get_element_key(_element)
-
-            if isinstance(elements[key], Text) and elements[key].font_size is None:
-                elements[key].font_size = template.get_text_field_font_size(
-                    _element
-                ) or text_field_font_size(_element)
-
-
 def text_field_font_size(element: pdfrw.PdfDict) -> Union[float, int]:
     """
     Calculates the font size it should be drawn with
     given a text field element.
     """
 
     if template.is_text_multiline(element):
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/image.py` & `PyPDFForm-1.3.0/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/patterns.py` & `PyPDFForm-1.3.0/PyPDFForm/core/patterns.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/template.py` & `PyPDFForm-1.3.0/PyPDFForm/core/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,25 @@
 # -*- coding: utf-8 -*-
 """Contains helpers for template."""
 
+from copy import deepcopy
 from typing import Dict, List, Tuple, Union
 
 import pdfrw
 from reportlab.pdfbase.pdfmetrics import stringWidth
 
 from ..middleware.constants import ELEMENT_TYPES
 from ..middleware.text import Text
-from . import constants, utils
+from . import constants
 from .patterns import (DROPDOWN_CHOICE_PATTERNS, ELEMENT_ALIGNMENT_PATTERNS,
                        ELEMENT_KEY_PATTERNS, ELEMENT_TYPE_PATTERNS,
                        TEXT_FIELD_APPEARANCE_PATTERNS,
                        TEXT_FIELD_FLAG_PATTERNS)
 
 
-def remove_all_elements(pdf: bytes) -> bytes:
-    """Removes all elements from a pdfrw parsed PDF form."""
-
-    pdf = pdfrw.PdfReader(fdata=pdf)
-
-    for page in pdf.pages:
-        elements = page[constants.ANNOTATION_KEY]
-        if elements:
-            for j in reversed(range(len(elements))):
-                elements.pop(j)
-
-    return utils.generate_stream(pdf)
-
-
 def get_elements_by_page(
     pdf: Union[bytes, pdfrw.PdfReader]
 ) -> Dict[int, List[pdfrw.PdfDict]]:
     """Iterates through a PDF and returns all elements found grouped by page."""
 
     if isinstance(pdf, bytes):
         pdf = pdfrw.PdfReader(fdata=pdf)
@@ -267,14 +254,18 @@
     element_value = element_middleware.value or ""
     length = (
         min(len(element_value), element_middleware.max_length)
         if element_middleware.max_length is not None
         else len(element_value)
     )
     element_value = element_value[:length]
+
+    if element_middleware.text_wrap_length is not None:
+        element_value = element_value[: element_middleware.text_wrap_length]
+
     character_paddings = (
         element_middleware.character_paddings[:length]
         if element_middleware.character_paddings is not None
         else element_middleware.character_paddings
     )
 
     alignment = get_element_alignment(element) or 0
@@ -330,7 +321,34 @@
                     element_middleware.font,
                     element_middleware.font_size,
                 )
                 / 2
             )
 
     return x, y
+
+
+def get_text_line_x_coordinates(
+    element: pdfrw.PdfDict, element_middleware: Text
+) -> Union[List[float], None]:
+    """
+    Returns the x coordinates to draw lines
+    of the text at given a PDF form paragraph element.
+    """
+
+    if (
+        element_middleware.text_wrap_length is not None
+        and element_middleware.text_lines is not None
+        and len(element_middleware.text_lines)
+        and isinstance(element_middleware.value, str)
+        and len(element_middleware.value) > element_middleware.text_wrap_length
+    ):
+        result = []
+        _ele = deepcopy(element_middleware)
+        for each in element_middleware.text_lines:
+            _ele.value = each
+            _ele.text_wrap_length = None
+            result.append(get_draw_text_coordinates(element, _ele)[0])
+
+        return result
+
+    return None
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/core/watermark.py` & `PyPDFForm-1.3.0/PyPDFForm/core/watermark.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,41 +40,48 @@
     canv.setFillColorRGB(
         element.font_color[0], element.font_color[1], element.font_color[2]
     )
 
     if element.comb is True:
         for i, char in enumerate(text_to_draw):
             canv.drawString(
-                coordinate_x + element.character_paddings[i] + element.text_x_offset,
-                coordinate_y + element.text_y_offset,
+                coordinate_x + element.character_paddings[i],
+                coordinate_y,
                 char,
             )
-    elif len(text_to_draw) < element.text_wrap_length:
+    elif (
+        element.text_wrap_length is None or len(text_to_draw) < element.text_wrap_length
+    ):
         canv.drawString(
-            coordinate_x + element.text_x_offset,
-            coordinate_y + element.text_y_offset,
+            coordinate_x,
+            coordinate_y,
             text_to_draw,
         )
     else:
         text_obj = canv.beginText(0, 0)
-
-        start = 0
-        end = element.text_wrap_length
-
-        while end < len(text_to_draw):
-            text_obj.textLine(text_to_draw[start:end])
-            start += element.text_wrap_length
-            end += element.text_wrap_length
-
-        text_obj.textLine(text_to_draw[start:])
+        for i, line in enumerate(element.text_lines):
+            cursor_moved = False
+            if (
+                element.text_line_x_coordinates is not None
+                and element.text_line_x_coordinates[i] - coordinate_x != 0
+            ):
+                text_obj.moveCursor(
+                    element.text_line_x_coordinates[i] - coordinate_x, 0
+                )
+                cursor_moved = True
+            text_obj.textLine(line)
+            if cursor_moved:
+                text_obj.moveCursor(
+                    -1 * (element.text_line_x_coordinates[i] - coordinate_x), 0
+                )
 
         canv.saveState()
         canv.translate(
-            coordinate_x + element.text_x_offset,
-            coordinate_y + element.text_y_offset,
+            coordinate_x,
+            coordinate_y,
         )
         canv.drawText(text_obj)
         canv.restoreState()
 
 
 def draw_image(*args: Union[canvas.Canvas, bytes, float, int]) -> None:
     """Draws an image on the watermark."""
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/element.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/template.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -65,17 +65,14 @@
 def dropdown_to_text(dropdown: Dropdown) -> Text:
     """Converts a dropdown element to a text element."""
 
     result = Text(dropdown.name)
 
     result.font = constants.GLOBAL_FONT
     result.font_color = constants.GLOBAL_FONT_COLOR
-    result.text_x_offset = constants.GLOBAL_TEXT_X_OFFSET
-    result.text_y_offset = constants.GLOBAL_TEXT_Y_OFFSET
-    result.text_wrap_length = constants.GLOBAL_TEXT_WRAP_LENGTH
 
     if dropdown.value is not None:
         result.value = (
             dropdown.choices[dropdown.value]
             if dropdown.value < len(dropdown.choices)
             else ""
         )
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/middleware/text.py` & `PyPDFForm-1.3.0/PyPDFForm/middleware/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
         """Constructs all attributes for the text field."""
 
         super().__init__(element_name, element_value)
 
         self.font = None
         self.font_size = None
         self.font_color = None
-        self.text_x_offset = None
-        self.text_y_offset = None
         self.text_wrap_length = None
         self.max_length = None
         self.comb = None
         self.character_paddings = None
+        self.text_lines = None
+        self.text_line_x_coordinates = None
 
     @property
     def schema_definition(self) -> dict:
         """Json schema definition of the text field."""
 
         result = {"type": "string"}
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm/wrapper.py` & `PyPDFForm-1.3.0/PyPDFForm/wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 """Contains user API for PyPDFForm."""
 
 from __future__ import annotations
 
 from typing import BinaryIO, Dict, Union
 
-from .core import filler, font, font_size
+from .core import filler, font
 from .core import image as image_core
-from .core import template as template_core
 from .core import utils
 from .core import watermark as watermark_core
 from .middleware import adapter, constants
 from .middleware import template as template_middleware
 from .middleware.dropdown import Dropdown
 from .middleware.text import Text
 
@@ -34,23 +33,14 @@
         for each in self.elements.values():
             if isinstance(each, Text):
                 each.font = kwargs.get("global_font", constants.GLOBAL_FONT)
                 each.font_size = kwargs.get("global_font_size")
                 each.font_color = kwargs.get(
                     "global_font_color", constants.GLOBAL_FONT_COLOR
                 )
-                each.text_x_offset = kwargs.get(
-                    "global_text_x_offset", constants.GLOBAL_TEXT_X_OFFSET
-                )
-                each.text_y_offset = kwargs.get(
-                    "global_text_y_offset", constants.GLOBAL_TEXT_Y_OFFSET
-                )
-                each.text_wrap_length = kwargs.get(
-                    "global_text_wrap_length", constants.GLOBAL_TEXT_WRAP_LENGTH
-                )
 
     def read(self) -> bytes:
         """Reads the file stream of a PDF form."""
 
         return self.stream
 
     def __add__(self, other: Wrapper) -> Wrapper:
@@ -77,23 +67,21 @@
             if key in self.elements:
                 self.elements[key].value = value
 
         for key, value in self.elements.items():
             if isinstance(value, Dropdown):
                 self.elements[key] = template_middleware.dropdown_to_text(value)
 
-        font_size.update_text_field_font_sizes(self.stream, self.elements)
+        utils.update_text_field_attributes(self.stream, self.elements)
         if self.read():
             self.elements = template_middleware.set_character_x_paddings(
                 self.stream, self.elements
             )
 
-        self.stream = template_core.remove_all_elements(
-            filler.fill(self.stream, self.elements)
-        )
+        self.stream = utils.remove_all_elements(filler.fill(self.stream, self.elements))
 
         return self
 
     def draw_text(
         self,
         text: str,
         page_number: int,
@@ -104,23 +92,14 @@
         """Draws a text on a PDF form."""
 
         new_element = Text("new")
         new_element.value = text
         new_element.font = kwargs.get("font", constants.GLOBAL_FONT)
         new_element.font_size = kwargs.get("font_size", constants.GLOBAL_FONT_SIZE)
         new_element.font_color = kwargs.get("font_color", constants.GLOBAL_FONT_COLOR)
-        new_element.text_x_offset = kwargs.get(
-            "text_x_offset", constants.GLOBAL_TEXT_X_OFFSET
-        )
-        new_element.text_y_offset = kwargs.get(
-            "text_y_offset", constants.GLOBAL_TEXT_Y_OFFSET
-        )
-        new_element.text_wrap_length = kwargs.get(
-            "text_wrap_length", constants.GLOBAL_TEXT_WRAP_LENGTH
-        )
 
         watermarks = watermark_core.create_watermarks_and_draw(
             self.stream,
             page_number,
             "text",
             [
                 [
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.3.0/PyPDFForm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.9
+Version: 1.3.0
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
-    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"></a>
     <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.9 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.3.0 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
 chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
                     //static.pepy.tech/personalized-badge/
-pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
              [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
```

### Comparing `PyPDFForm-1.2.9/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.3.0/PyPDFForm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.9/README.md` & `PyPDFForm-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center"><img src="https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png"></p>
 <p align="center">
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-isort.yml/badge.svg"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-package.yml/badge.svg"></a>
     <a href="https://codecov.io/gh/chinapandaman/PyPDFForm"><img src="https://codecov.io/gh/chinapandaman/PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE"></a>
     <a href="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"><img src="https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg"></a>
-    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads"></a>
+    <a href="https://pepy.tech/project/pypdfform"><img src="https://static.pepy.tech/personalized-badge/pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads"></a>
     <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-orange.svg"></a>
 </p>
 
 ## Introduction
 
 PyPDFForm is a pure Python library for PDF form processing. 
 It allows filling a PDF form programmatically by creating
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
    isort.yml/badge.svg] [https://github.com/chinapandaman/PyPDFForm/actions/
  workflows/python-package.yml/badge.svg] [https://codecov.io/gh/chinapandaman/
 PyPDFForm/branch/master/graph/badge.svg?token=CSRLN14IFE] [https://github.com/
 chinapandaman/PyPDFForm/actions/workflows/python-publish.yml/badge.svg] [https:
                     //static.pepy.tech/personalized-badge/
-pypdfform?period=total&units=international_system&left_color=black&right_color=magenta&left_text=Downloads]
+pypdfform?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads]
              [https://img.shields.io/badge/License-MIT-orange.svg]
 ## Introduction PyPDFForm is a pure Python library for PDF form processing. It
 allows filling a PDF form programmatically by creating a Python dictionary with
 keys matching its annotated names for elements like text fields and checkboxes.
 It also supports other functionalities such as drawing image and merging
 multiple PDFs together. ## Installing Install using [pip](https://pip.pypa.io/
 en/stable/): ```shell script pip install PyPDFForm ``` ## Quick Example ![Check
```

### Comparing `PyPDFForm-1.2.9/setup.py` & `PyPDFForm-1.3.0/setup.py`

 * *Files identical despite different names*

