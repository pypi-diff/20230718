# Comparing `tmp/helperfns-0.0.6.tar.gz` & `tmp/helperfns-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\helperfns-0.0.6.tar", last modified: Thu Jul 13 11:24:38 2023, max compression
+gzip compressed data, was "dist\helperfns-0.0.7.tar", last modified: Tue Jul 18 07:28:43 2023, max compression
```

## Comparing `helperfns-0.0.6.tar` & `helperfns-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.195171 helperfns-0.0.6/
--rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     8507 2023-07-13 11:24:38.177169 helperfns-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6791 2023-07-13 11:18:11.000000 helperfns-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.020171 helperfns-0.0.6/helperfns/
--rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.6/helperfns/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.100172 helperfns-0.0.6/helperfns/tables/
--rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.6/helperfns/tables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.104171 helperfns-0.0.6/helperfns/text/
--rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.6/helperfns/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.107168 helperfns-0.0.6/helperfns/torch/
--rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.6/helperfns/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.127172 helperfns-0.0.6/helperfns/torch/accuracy/
--rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.6/helperfns/torch/accuracy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.137172 helperfns-0.0.6/helperfns/torch/models/
--rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.6/helperfns/torch/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.146171 helperfns-0.0.6/helperfns/torch/text/
--rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.6/helperfns/torch/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.159167 helperfns-0.0.6/helperfns/utils/
--rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.6/helperfns/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.173168 helperfns-0.0.6/helperfns/visualization/
--rw-rw-rw-   0        0        0    12054 2023-07-13 11:18:19.000000 helperfns-0.0.6/helperfns/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 11:24:38.095171 helperfns-0.0.6/helperfns.egg-info/
--rw-rw-rw-   0        0        0     8507 2023-07-13 11:24:34.000000 helperfns-0.0.6/helperfns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-13 11:24:37.000000 helperfns-0.0.6/helperfns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 11:24:35.000000 helperfns-0.0.6/helperfns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-07-13 11:24:36.000000 helperfns-0.0.6/helperfns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 11:24:36.000000 helperfns-0.0.6/helperfns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 11:24:38.202191 helperfns-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2157 2023-07-13 11:24:08.000000 helperfns-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.059188 helperfns-0.0.7/
+-rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     8864 2023-07-18 07:28:43.056183 helperfns-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7134 2023-07-18 07:26:06.000000 helperfns-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:42.964195 helperfns-0.0.7/helperfns/
+-rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.7/helperfns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.014193 helperfns-0.0.7/helperfns/tables/
+-rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.7/helperfns/tables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.017183 helperfns-0.0.7/helperfns/text/
+-rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.7/helperfns/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.020182 helperfns-0.0.7/helperfns/torch/
+-rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.7/helperfns/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.023180 helperfns-0.0.7/helperfns/torch/accuracy/
+-rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.7/helperfns/torch/accuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.026183 helperfns-0.0.7/helperfns/torch/models/
+-rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.7/helperfns/torch/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.034182 helperfns-0.0.7/helperfns/torch/text/
+-rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.7/helperfns/torch/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.038184 helperfns-0.0.7/helperfns/utils/
+-rw-rw-rw-   0        0        0     1836 2023-07-18 07:21:36.000000 helperfns-0.0.7/helperfns/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.051181 helperfns-0.0.7/helperfns/visualization/
+-rw-rw-rw-   0        0        0    12414 2023-07-18 07:18:34.000000 helperfns-0.0.7/helperfns/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:28:43.010199 helperfns-0.0.7/helperfns.egg-info/
+-rw-rw-rw-   0        0        0     8864 2023-07-18 07:28:41.000000 helperfns-0.0.7/helperfns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-18 07:28:42.000000 helperfns-0.0.7/helperfns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:28:41.000000 helperfns-0.0.7/helperfns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-18 07:28:42.000000 helperfns-0.0.7/helperfns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 07:28:42.000000 helperfns-0.0.7/helperfns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 07:28:43.060192 helperfns-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2023-07-18 07:26:39.000000 helperfns-0.0.7/setup.py
```

### Comparing `helperfns-0.0.6/LICENSE` & `helperfns-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/PKG-INFO` & `helperfns-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -117,27 +117,41 @@
 ### utils
 
 utils package comes with a simple helper function for converting seconds to hours, minutes and seconds.
 
 Example:
 
 ```python
+from helperfns.utils import hms_string
+
 start = time.time()
 for i in range(100000):
    pass
 end = time.time()
 
+print(hms_string(end - start))
 ```
 
 Output:
 
 ```shell
 '0:00:00.01'
 ```
 
+It also comes with a helper functions for normalizing an image so that it can be ploted using matplot lib:
+
+Example:
+
+```python
+from helperfns.utils import normalize_image
+
+image = normalize_image(image)
+plt.imshow(image.permute(1, 2, 0).cpu().numpy())
+```
+
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
```

### Comparing `helperfns-0.0.6/README.md` & `helperfns-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -81,27 +81,41 @@
 ### utils
 
 utils package comes with a simple helper function for converting seconds to hours, minutes and seconds.
 
 Example:
 
 ```python
+from helperfns.utils import hms_string
+
 start = time.time()
 for i in range(100000):
    pass
 end = time.time()
 
+print(hms_string(end - start))
 ```
 
 Output:
 
 ```shell
 '0:00:00.01'
 ```
 
+It also comes with a helper functions for normalizing an image so that it can be ploted using matplot lib:
+
+Example:
+
+```python
+from helperfns.utils import normalize_image
+
+image = normalize_image(image)
+plt.imshow(image.permute(1, 2, 0).cpu().numpy())
+```
+
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
```

### Comparing `helperfns-0.0.6/helperfns/tables/__init__.py` & `helperfns-0.0.7/helperfns/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/helperfns/text/__init__.py` & `helperfns-0.0.7/helperfns/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/helperfns/torch/accuracy/__init__.py` & `helperfns-0.0.7/helperfns/torch/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/helperfns/torch/models/__init__.py` & `helperfns-0.0.7/helperfns/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/helperfns/torch/text/__init__.py` & `helperfns-0.0.7/helperfns/torch/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.6/helperfns/visualization/__init__.py` & `helperfns-0.0.7/helperfns/visualization/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_images: Plots the images and display them.
     plot_images_predictions: Plots the images with their predictions and display them.
+    plot_classification_report: Plots the classification report.
 
     Examples
     --------
     >>> y_true = [random.randint(0, 1) for _ in range (100)]
     >>> y_pred = [random.randint(0, 1) for _ in range (100)]
     >>> classes =["dog", "cat"]
     >>> plot_complicated_confusion_matrix(y_true, y_pred, classes)
@@ -117,14 +118,15 @@
     None
 
     See Also
     --------
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images: Plots the images and display them.
     plot_images_predictions: Plots the images with their predictions and display them.
+    plot_classification_report: Plots the classification report.
 
     Examples
     --------
     >>> y_true = [random.randint(0, 1) for _ in range (100)]
     >>> y_pred = [random.randint(0, 1) for _ in range (100)]
     >>> classes =["dog", "cat"]
     >>> plot_simple_confusion_matrix(y_true, y_pred, classes)
@@ -204,14 +206,15 @@
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images_predictions: Plots the images with their predictions and display them.
+    plot_classification_report: Plots the classification report.
 
     Examples
     --------
     >>> plot_images(images[:24], true_labels[:24], cols=8)
     """
 
     assert len(images) == len(
@@ -233,15 +236,15 @@
     images: list,
     labels_true: list,
     labels_pred: list,
     classes: list = [],
     cols: int = 5,
     rows: int = 3,
     fontsize: int = 16,
-):
+) -> None:
     """
     Plot images predictions
 
     This function simply plots predicted images. Images with wrongly predicted labels their
     labels will be red and green otherwise.
 
     Parameters
@@ -270,14 +273,15 @@
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images: Plots the images and display them.
+    plot_classification_report: Plots the classification report.
 
     Examples
     --------
     >>> plot_images_predictions(images, true_labels, preds, classes=["dog", "cat"] ,cols=8)
 
     """
     assert (
@@ -342,14 +346,15 @@
             Axe object from matplotlib
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images: Plots the images and display them.
+    plot_images_predictions: Plots the images with their predictions and display them.
 
     Examples
     --------
     >>> fig, ax = plot_classification_report(labels, preds,
                     title='Classification Report',
                     figsize=(10, 5), dpi=70,
                     target_names = classes)
```

### Comparing `helperfns-0.0.6/helperfns.egg-info/PKG-INFO` & `helperfns-0.0.7/helperfns.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
 Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -117,27 +117,41 @@
 ### utils
 
 utils package comes with a simple helper function for converting seconds to hours, minutes and seconds.
 
 Example:
 
 ```python
+from helperfns.utils import hms_string
+
 start = time.time()
 for i in range(100000):
    pass
 end = time.time()
 
+print(hms_string(end - start))
 ```
 
 Output:
 
 ```shell
 '0:00:00.01'
 ```
 
+It also comes with a helper functions for normalizing an image so that it can be ploted using matplot lib:
+
+Example:
+
+```python
+from helperfns.utils import normalize_image
+
+image = normalize_image(image)
+plt.imshow(image.permute(1, 2, 0).cpu().numpy())
+```
+
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
```

### Comparing `helperfns-0.0.6/setup.py` & `helperfns-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "This package provide some python helper functions that are useful in machine learning."
 # setting up
 setup(
     name="helperfns",
     version=VERSION,
     author="Crispen Gari",
     author_email="<crispengari@gmail.com>",
```

