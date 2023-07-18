# Comparing `tmp/BinPackerPro-0.0.3.tar.gz` & `tmp/BinPackerPro-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BinPackerPro-0.0.3.tar", last modified: Tue Jul 18 05:53:41 2023, max compression
+gzip compressed data, was "BinPackerPro-0.0.4.tar", last modified: Tue Jul 18 06:16:19 2023, max compression
```

## Comparing `BinPackerPro-0.0.3.tar` & `BinPackerPro-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 05:53:41.874061 BinPackerPro-0.0.3/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.3/LICENSE
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      483 2023-07-18 05:53:41.874148 BinPackerPro-0.0.3/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      148 2023-07-17 12:41:43.000000 BinPackerPro-0.0.3/pyproject.toml
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      609 2023-07-18 05:53:41.874540 BinPackerPro-0.0.3/setup.cfg
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 05:53:41.869955 BinPackerPro-0.0.3/src/
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 05:53:41.871700 BinPackerPro-0.0.3/src/BinPackerPro.egg-info/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      483 2023-07-18 05:53:41.000000 BinPackerPro-0.0.3/src/BinPackerPro.egg-info/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      385 2023-07-18 05:53:41.000000 BinPackerPro-0.0.3/src/BinPackerPro.egg-info/SOURCES.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 05:53:41.000000 BinPackerPro-0.0.3/src/BinPackerPro.egg-info/dependency_links.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       15 2023-07-18 05:53:41.000000 BinPackerPro-0.0.3/src/BinPackerPro.egg-info/top_level.txt
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 05:53:41.873780 BinPackerPro-0.0.3/src/bin_packer_pro/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6185 2023-07-18 05:51:54.000000 BinPackerPro-0.0.3/src/bin_packer_pro/BinPackerPro.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.3/src/bin_packer_pro/__init__.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1002 2023-07-18 05:52:04.000000 BinPackerPro-0.0.3/src/bin_packer_pro/auxiliary_methods.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.3/src/bin_packer_pro/constants.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.3/src/bin_packer_pro/plot.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6135 2023-07-18 05:52:19.000000 BinPackerPro-0.0.3/src/bin_packer_pro/utils.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.395791 BinPackerPro-0.0.4/
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.394371 BinPackerPro-0.0.4/BinPackerPro/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6181 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/BinPackerPro.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.4/BinPackerPro/__init__.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1000 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/auxiliary_methods.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.4/BinPackerPro/constants.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.4/BinPackerPro/plot.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6131 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/utils.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.395616 BinPackerPro-0.0.4/BinPackerPro.egg-info/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      372 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/SOURCES.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/dependency_links.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       31 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/requires.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       13 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/top_level.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.4/LICENSE
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 06:16:19.395875 BinPackerPro-0.0.4/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:13:12.000000 BinPackerPro-0.0.4/README.md
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       79 2023-07-18 06:16:19.396176 BinPackerPro-0.0.4/setup.cfg
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      639 2023-07-18 06:10:37.000000 BinPackerPro-0.0.4/setup.py
```

### Comparing `BinPackerPro-0.0.3/LICENSE` & `BinPackerPro-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.3/src/bin_packer_pro/BinPackerPro.py` & `BinPackerPro-0.0.4/BinPackerPro/BinPackerPro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bin_packer_pro.utils import Packer, Bin, Item
-from bin_packer_pro.plot import plotCubeAt2
+from BinPackerPro.utils import Packer, Bin, Item
+from BinPackerPro.plot import plotCubeAt2
 from matplotlib.backends.backend_pdf import PdfPages
 import matplotlib.pyplot as plt
 
 
 class BinPackerPro:
     def __init__(
         self,
```

### Comparing `BinPackerPro-0.0.3/src/bin_packer_pro/auxiliary_methods.py` & `BinPackerPro-0.0.4/BinPackerPro/auxiliary_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from decimal import Decimal
-from bin_packer_pro.constants import Axis
+from BinPackerPro.constants import Axis
 
 
 def rect_intersect(item1, item2, x, y):
     d1 = item1.get_dimension()
     d2 = item2.get_dimension()
 
     cx1 = item1.position[x] + d1[x]/2
```

### Comparing `BinPackerPro-0.0.3/src/bin_packer_pro/plot.py` & `BinPackerPro-0.0.4/BinPackerPro/plot.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.3/src/bin_packer_pro/utils.py` & `BinPackerPro-0.0.4/BinPackerPro/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from bin_packer_pro.constants import RotationType, Axis
-from bin_packer_pro.auxiliary_methods import intersect, set_to_decimal
+from BinPackerPro.constants import RotationType, Axis
+from BinPackerPro.auxiliary_methods import intersect, set_to_decimal
 
 DEFAULT_NUMBER_OF_DECIMALS = 3
 START_POSITION = [0, 0, 0]
 
 
 class Item:
     def __init__(self, name, width, height, depth, weight):
```

