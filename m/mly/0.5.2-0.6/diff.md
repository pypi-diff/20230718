# Comparing `tmp/mly-0.5.2.tar.gz` & `tmp/mly-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mly-0.5.2.tar", last modified: Tue Jul  4 14:04:58 2023, max compression
+gzip compressed data, was "mly-0.6.tar", last modified: Tue Jul 18 15:37:30 2023, max compression
```

## Comparing `mly-0.5.2.tar` & `mly-0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.495301 mly-0.5.2/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.5.2/LICENSE
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-04 14:04:58.496301 mly-0.5.2/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.5.2/README.md
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.406300 mly-0.5.2/mly/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.5.2/mly/SRD.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.5.2/mly/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10014 2023-06-15 11:06:15.000000 mly-0.5.2/mly/createFileSystem.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.415300 mly-0.5.2/mly/datatools/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-06-09 13:56:57.000000 mly-0.5.2/mly/datatools/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-06-20 13:25:10.000000 mly-0.5.2/mly/datatools/core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-06-09 10:58:15.000000 mly-0.5.2/mly/datatools/datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91856 2023-06-20 13:25:12.000000 mly-0.5.2/mly/datatools/generator.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.488300 mly-0.5.2/mly/datatools/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/test_core.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-05-09 14:56:02.000000 mly-0.5.2/mly/datatools/tests/test_datatools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-06-09 11:10:13.000000 mly-0.5.2/mly/datatools/tests/test_generator.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18633 2023-06-15 10:28:37.000000 mly-0.5.2/mly/exceptions.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.5.2/mly/mlTools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.5.2/mly/models.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    12353 2023-05-04 12:56:19.000000 mly-0.5.2/mly/null_energy_map.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-06-09 11:13:40.000000 mly-0.5.2/mly/offlinefar.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-05-04 12:56:19.000000 mly-0.5.2/mly/plugins.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10153 2023-06-23 11:18:28.000000 mly-0.5.2/mly/projectwave.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.5.2/mly/simulateddetectornoise.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.494301 mly-0.5.2/mly/tests/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.5.2/mly/tests/__init__.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.5.2/mly/tests/test_init.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.5.2/mly/tests/test_tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-06-30 12:02:21.000000 mly-0.5.2/mly/tools.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126803 2023-06-09 13:52:48.000000 mly-0.5.2/mly/validators.py
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-05-09 14:56:02.000000 mly-0.5.2/mly/waveforms.py
-drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-04 14:04:58.410300 mly-0.5.2/mly.egg-info/
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      497 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/PKG-INFO
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      733 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/SOURCES.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/dependency_links.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/requires.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-04 14:04:58.000000 mly-0.5.2/mly.egg-info/top_level.txt
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-07-04 14:04:58.497301 mly-0.5.2/setup.cfg
--rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      954 2023-07-04 12:47:36.000000 mly-0.5.2/setup.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.291577 mly-0.6/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    35148 2023-05-10 08:55:19.000000 mly-0.6/LICENSE
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      495 2023-07-18 15:37:30.291577 mly-0.6/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2021-01-11 16:48:33.000000 mly-0.6/README.md
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.270577 mly-0.6/mly/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)  1433718 2021-05-11 10:43:11.000000 mly-0.6/mly/SRD.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-05-09 14:15:39.000000 mly-0.6/mly/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10014 2023-07-18 09:16:42.000000 mly-0.6/mly/createFileSystem.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.282577 mly-0.6/mly/datatools/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      155 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    22332 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    28108 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    91856 2023-07-18 15:30:16.000000 mly-0.6/mly/datatools/generator.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.286577 mly-0.6/mly/datatools/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       24 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     3438 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_core.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      441 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_datatools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     4975 2023-07-18 09:16:42.000000 mly-0.6/mly/datatools/tests/test_generator.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    18633 2023-07-18 09:16:42.000000 mly-0.6/mly/exceptions.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7770 2022-08-17 15:08:03.000000 mly-0.6/mly/mlTools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     6996 2021-01-11 16:48:33.000000 mly-0.6/mly/models.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7316 2023-07-18 09:16:42.000000 mly-0.6/mly/offlinefar.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     7797 2023-07-18 09:16:42.000000 mly-0.6/mly/plugins.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    10153 2023-07-18 09:16:42.000000 mly-0.6/mly/projectwave.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     8913 2022-03-15 16:16:40.000000 mly-0.6/mly/simulateddetectornoise.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13856 2023-07-18 10:44:50.000000 mly-0.6/mly/skymap_utils.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.290577 mly-0.6/mly/tests/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      728 2021-10-07 09:34:45.000000 mly-0.6/mly/tests/__init__.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     1601 2021-10-08 08:22:16.000000 mly-0.6/mly/tests/test_init.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)     5258 2022-03-02 09:58:19.000000 mly-0.6/mly/tests/test_tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    13037 2023-07-18 09:16:42.000000 mly-0.6/mly/tools.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)   126794 2023-07-18 15:30:30.000000 mly-0.6/mly/validators.py
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)    34282 2023-07-18 09:16:42.000000 mly-0.6/mly/waveforms.py
+drwxrwxr-x   0 vasileios.skliris (44659) vasileios.skliris (44659)        0 2023-07-18 15:37:30.278577 mly-0.6/mly.egg-info/
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      495 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/PKG-INFO
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      730 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        1 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       96 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/requires.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)        4 2023-07-18 15:37:30.000000 mly-0.6/mly.egg-info/top_level.txt
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)       79 2023-07-18 15:37:30.292577 mly-0.6/setup.cfg
+-rw-rw-r--   0 vasileios.skliris (44659) vasileios.skliris (44659)      952 2023-07-18 15:36:55.000000 mly-0.6/setup.py
```

### Comparing `mly-0.5.2/LICENSE` & `mly-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/SRD.py` & `mly-0.6/mly/SRD.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/createFileSystem.py` & `mly-0.6/mly/createFileSystem.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/datatools/core.py` & `mly-0.6/mly/datatools/core.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/datatools/datatools.py` & `mly-0.6/mly/datatools/datatools.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/datatools/generator.py` & `mly-0.6/mly/datatools/generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/datatools/tests/test_core.py` & `mly-0.6/mly/datatools/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/datatools/tests/test_generator.py` & `mly-0.6/mly/datatools/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/exceptions.py` & `mly-0.6/mly/exceptions.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/mlTools.py` & `mly-0.6/mly/mlTools.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/models.py` & `mly-0.6/mly/models.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/offlinefar.py` & `mly-0.6/mly/offlinefar.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/plugins.py` & `mly-0.6/mly/plugins.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/projectwave.py` & `mly-0.6/mly/projectwave.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/simulateddetectornoise.py` & `mly-0.6/mly/simulateddetectornoise.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/tests/__init__.py` & `mly-0.6/mly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/tests/test_init.py` & `mly-0.6/mly/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/tests/test_tools.py` & `mly-0.6/mly/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/tools.py` & `mly-0.6/mly/tools.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly/validators.py` & `mly-0.6/mly/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
             if isinstance(input_shape,tuple): input_shape=[input_shape]
             for i in range(len(models[1][m])):
                 print(input_shape[i],models[1][m][i])
                 #print(DATA[0].__getattribute__(models[1][m][i]).shape)
                 dataList.append(DATA.exportData(models[1][m][i],shape=input_shape[i]))
 
             if len(dataList)==1: dataList=dataList[0]
-            scores = 1.0 - trained_models[m].predict(dataList, batch_size=1, verbose=0)[:,columns[m]]
+            scores = 1.0 - trained_models[m](dataList, training=False).numpy()[:,columns[m]]
             scores_collection.append(scores.tolist())
             
         inferencetime=time.time()
         print("INFERENCE TIME:", inferencetime-generationtime)
         
         gps_times=DATA.exportGPS()
```

### Comparing `mly-0.5.2/mly/waveforms.py` & `mly-0.6/mly/waveforms.py`

 * *Files identical despite different names*

### Comparing `mly-0.5.2/mly.egg-info/SOURCES.txt` & `mly-0.6/mly.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 setup.py
 mly/SRD.py
 mly/__init__.py
 mly/createFileSystem.py
 mly/exceptions.py
 mly/mlTools.py
 mly/models.py
-mly/null_energy_map.py
 mly/offlinefar.py
 mly/plugins.py
 mly/projectwave.py
 mly/simulateddetectornoise.py
+mly/skymap_utils.py
 mly/tools.py
 mly/validators.py
 mly/waveforms.py
 mly.egg-info/PKG-INFO
 mly.egg-info/SOURCES.txt
 mly.egg-info/dependency_links.txt
 mly.egg-info/requires.txt
```

### Comparing `mly-0.5.2/setup.py` & `mly-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mly",
-    version="0.5.2",
+    version="0.6",
     author="Vasileios Skliris",
     author_email='vas.skliris@gmail.com',
     description='This tool helps you create training and testing data for ML to use for gravitational wave detection.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://pypi.python.org/pypi/mly/',
     packages=setuptools.find_packages(),
```

