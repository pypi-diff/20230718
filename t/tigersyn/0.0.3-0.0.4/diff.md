# Comparing `tmp/tigersyn-0.0.3.tar.gz` & `tmp/tigersyn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigersyn-0.0.3.tar", last modified: Mon Jul 17 10:08:45 2023, max compression
+gzip compressed data, was "tigersyn-0.0.4.tar", last modified: Tue Jul 18 02:16:30 2023, max compression
```

## Comparing `tigersyn-0.0.3.tar` & `tigersyn-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.290538 tigersyn-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      755 2023-07-17 10:08:45.288513 tigersyn-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-07-17 07:50:52.000000 tigersyn-0.0.3/README.md
--rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 10:08:45.290538 tigersyn-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-17 10:08:04.000000 tigersyn-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.229515 tigersyn-0.0.3/tigersyn/
--rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.3/tigersyn/__init__.py
--rw-rw-rw-   0        0        0     2199 2023-07-17 10:07:35.000000 tigersyn-0.0.3/tigersyn/syn.py
--rw-rw-rw-   0        0        0     3948 2023-07-17 09:52:58.000000 tigersyn-0.0.3/tigersyn/syn_tool.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:08:45.287556 tigersyn-0.0.3/tigersyn.egg-info/
--rw-rw-rw-   0        0        0      755 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 10:08:45.000000 tigersyn-0.0.3/tigersyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.645455 tigersyn-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-07-17 07:49:07.000000 tigersyn-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      948 2023-07-18 02:16:30.644458 tigersyn-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-07-18 02:14:57.000000 tigersyn-0.0.4/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-17 06:43:23.000000 tigersyn-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 02:16:30.646463 tigersyn-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-18 02:08:42.000000 tigersyn-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.586833 tigersyn-0.0.4/tigersyn/
+-rw-rw-rw-   0        0        0       28 2023-07-17 09:40:04.000000 tigersyn-0.0.4/tigersyn/__init__.py
+-rw-rw-rw-   0        0        0     2275 2023-07-17 14:31:32.000000 tigersyn-0.0.4/tigersyn/syn.py
+-rw-rw-rw-   0        0        0     3899 2023-07-18 02:00:16.000000 tigersyn-0.0.4/tigersyn/syn_tool.py
+drwxrwxrwx   0        0        0        0 2023-07-18 02:16:30.641456 tigersyn-0.0.4/tigersyn.egg-info/
+-rw-rw-rw-   0        0        0      948 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 02:16:30.000000 tigersyn-0.0.4/tigersyn.egg-info/top_level.txt
```

### Comparing `tigersyn-0.0.3/LICENSE` & `tigersyn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tigersyn-0.0.3/setup.py` & `tigersyn-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-VESION = '0.0.3'
+VESION = '0.0.4'
 DESCRIPTION = 'Processing MRI images based on deep-learning'
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: MIT License',
     "Operating System :: Microsoft :: Windows"
 ]
```

### Comparing `tigersyn-0.0.3/tigersyn/syn.py` & `tigersyn-0.0.4/tigersyn/syn.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,17 @@
         input = [input]
 
     input_file_list = input
     if os.path.isdir(input[0]):
         input_file_list = glob.glob(join(input[0], '*.nii'))
         input_file_list += glob.glob(join(input[0], '*.nii.gz'))
 
+    elif '*' in input[0]:
+        input_file_list = glob.glob(input[0])
+
     output_dir = output
 
     print('Total nii files:', len(input_file_list))
     count = 0
     for f in input_file_list:
         count += 1
         t = time.time()
```

### Comparing `tigersyn-0.0.3/tigersyn/syn_tool.py` & `tigersyn-0.0.4/tigersyn/syn_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,47 +3,32 @@
 import sys
 
 import nibabel as nib
 from nilearn.image import reorder_img
 import numpy as np
 import onnxruntime as ort
 
-model_servers = ["https://github.com/StanleyWangTW/tigersyn/releases/download/v0.0.2-alpha/mprage_syntheseg_v001_unet.onnx"]
-# determine if application is a script file or frozen exe
-if getattr(sys, 'frozen', False):
-    application_path = os.path.dirname(sys.executable)
-elif __file__:
-    application_path = os.path.dirname(os.path.abspath(__file__))
-
-model_path = join(application_path, 'models')
-print(model_path)
-os.makedirs(model_path, exist_ok=True)
-
 label_all = dict()
 label_all['syntheseg'] = (
     2, 3, 4, 5, 7, 8, 10, 11, 12, 13, 14, 15, 16, 17, 18, 26,
     28, 41, 42, 43, 44, 46, 47, 49, 50, 51, 52, 53, 54, 58, 60
 )
 
-def read_nib(input_nib):
-    """nib to 5D numpy"""
-    return input_nib.get_fdata()[None, None, ...]
-
-def save_nib(data_nib, ftemplate, postfix):
-    output_file = ftemplate.replace('@@@@', postfix)
-    nib.save(data_nib, output_file)
-    print('Writing output file: ', output_file)
-    return output_file
+model_servers = [
+    'https://github.com/StanleyWangTW/tigersyn/releases/download/modelhub/'
+]
 
-def read_file(model_ff, input_file):
-    """load nib and reorder"""
-    input_nib = nib.load(input_file)
-    vol_nib = reorder_img(input_nib, resample="continuous")
-    return vol_nib
+# determine if application is a script file or frozen exe
+if getattr(sys, 'frozen', False):
+    application_path = os.path.dirname(sys.executable)
+elif __file__:
+    application_path = os.path.dirname(os.path.abspath(__file__))
 
+model_path = join(application_path, 'models')
+os.makedirs(model_path, exist_ok=True)
 
 def download(url, file_name):
     import urllib.request
     import certifi
     import shutil
     import ssl
     context = ssl.create_default_context(cafile=certifi.where())
@@ -59,33 +44,49 @@
         fn = f
     else:
         fn = f + '.onnx'
 
     model_file = join(model_path, fn)
 
     if not os.path.exists(model_file):
-        
         for server in model_servers:
             try:
                 print(f'Downloading model files....')
-                model_url = server
+                model_url = server + fn
                 print(model_url, model_file)
                 download(model_url, model_file)
                 download_ok = True
                 print('Download finished...')
                 break
             except:
                 download_ok = False
 
         if not download_ok:
             raise ValueError('Server error. Please check the model name or internet connection.')
                 
     return model_file
 
 
+def read_nib(input_nib):
+    """nib to 5D numpy"""
+    return input_nib.get_fdata()[None, None, ...]
+
+def save_nib(data_nib, ftemplate, postfix):
+    output_file = ftemplate.replace('@@@@', postfix)
+    nib.save(data_nib, output_file)
+    print('Writing output file: ', output_file)
+    return output_file
+
+def read_file(model_ff, input_file):
+    """load nib and reorder"""
+    input_nib = nib.load(input_file)
+    vol_nib = reorder_img(input_nib, resample="continuous")
+    return vol_nib
+
+
 def get_mode(model_ff):
     seg_mode, version, model_str = basename(model_ff).split('_')[1:4]  # aseg43, bet
     #print(seg_mode, version , model_str)
 
     return seg_mode, version, model_str
 
 def normalize(data):
```

