# Comparing `tmp/biodigest-0.2.8.tar.gz` & `tmp/biodigest-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biodigest-0.2.8.tar", last modified: Wed Mar 29 09:21:53 2023, max compression
+gzip compressed data, was "biodigest-0.2.9.tar", last modified: Tue Jul 18 12:37:01 2023, max compression
```

## Comparing `biodigest-0.2.8.tar` & `biodigest-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.170585 biodigest-0.2.8/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    35149 2022-02-25 07:45:27.000000 biodigest-0.2.8/LICENSE
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    10897 2023-03-29 09:21:53.170585 biodigest-0.2.8/PKG-INFO
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    10326 2022-06-08 09:21:15.000000 biodigest-0.2.8/README.md
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.166585 biodigest-0.2.8/biodigest/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)       51 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/__init__.py
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.166585 biodigest-0.2.8/biodigest/evaluation/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)       76 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/__init__.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     9467 2022-06-08 09:24:26.000000 biodigest-0.2.8/biodigest/evaluation/background_models.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    13344 2022-06-08 09:24:26.000000 biodigest-0.2.8/biodigest/evaluation/comparator.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     5215 2023-03-28 13:39:53.000000 biodigest-0.2.8/biodigest/evaluation/config.py
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.166585 biodigest-0.2.8/biodigest/evaluation/d_utils/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)       80 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/d_utils/__init__.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     5797 2022-06-08 09:24:26.000000 biodigest-0.2.8/biodigest/evaluation/d_utils/eval_utils.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    30572 2022-09-30 13:24:38.000000 biodigest-0.2.8/biodigest/evaluation/d_utils/plotting_utils.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     8288 2022-06-08 09:24:26.000000 biodigest-0.2.8/biodigest/evaluation/d_utils/runner_utils.py
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.170585 biodigest-0.2.8/biodigest/evaluation/mappers/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)      137 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/mappers/__init__.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     3555 2022-06-08 09:24:26.000000 biodigest-0.2.8/biodigest/evaluation/mappers/disease_getter.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     6577 2022-10-05 12:30:09.000000 biodigest-0.2.8/biodigest/evaluation/mappers/gene_getter.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    13822 2022-09-30 13:24:38.000000 biodigest-0.2.8/biodigest/evaluation/mappers/mapper.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     2926 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/mappers/mapping_transformer.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     5450 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/mappers/mapping_utils.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    11092 2022-02-25 07:45:45.000000 biodigest-0.2.8/biodigest/evaluation/score_calculator.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    12037 2023-03-29 09:20:34.000000 biodigest-0.2.8/biodigest/setup.py
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    29289 2022-10-05 12:30:17.000000 biodigest-0.2.8/biodigest/single_validation.py
-drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-03-29 09:21:53.166585 biodigest-0.2.8/biodigest.egg-info/
--rw-rw-r--   0 kikky     (1000) kikky     (1000)    10897 2023-03-29 09:21:53.000000 biodigest-0.2.8/biodigest.egg-info/PKG-INFO
--rw-rw-r--   0 kikky     (1000) kikky     (1000)      889 2023-03-29 09:21:53.000000 biodigest-0.2.8/biodigest.egg-info/SOURCES.txt
--rw-rw-r--   0 kikky     (1000) kikky     (1000)        1 2023-03-29 09:21:53.000000 biodigest-0.2.8/biodigest.egg-info/dependency_links.txt
--rw-rw-r--   0 kikky     (1000) kikky     (1000)      143 2023-03-29 09:21:53.000000 biodigest-0.2.8/biodigest.egg-info/requires.txt
--rw-rw-r--   0 kikky     (1000) kikky     (1000)       10 2023-03-29 09:21:53.000000 biodigest-0.2.8/biodigest.egg-info/top_level.txt
--rw-rw-r--   0 kikky     (1000) kikky     (1000)       38 2023-03-29 09:21:53.170585 biodigest-0.2.8/setup.cfg
--rw-rw-r--   0 kikky     (1000) kikky     (1000)     1327 2023-03-29 09:21:32.000000 biodigest-0.2.8/setup.py
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.683687 biodigest-0.2.9/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    35149 2022-02-25 07:45:27.000000 biodigest-0.2.9/LICENSE
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    10897 2023-07-18 12:37:01.683687 biodigest-0.2.9/PKG-INFO
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    10326 2022-06-08 09:21:15.000000 biodigest-0.2.9/README.md
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.679687 biodigest-0.2.9/biodigest/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)       51 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/__init__.py
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.683687 biodigest-0.2.9/biodigest/evaluation/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)       76 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/__init__.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     9467 2022-06-08 09:24:26.000000 biodigest-0.2.9/biodigest/evaluation/background_models.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    13344 2022-06-08 09:24:26.000000 biodigest-0.2.9/biodigest/evaluation/comparator.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     5215 2023-03-28 13:39:53.000000 biodigest-0.2.9/biodigest/evaluation/config.py
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.683687 biodigest-0.2.9/biodigest/evaluation/d_utils/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)       80 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/d_utils/__init__.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     5797 2022-06-08 09:24:26.000000 biodigest-0.2.9/biodigest/evaluation/d_utils/eval_utils.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    30572 2022-09-30 13:24:38.000000 biodigest-0.2.9/biodigest/evaluation/d_utils/plotting_utils.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     8288 2022-06-08 09:24:26.000000 biodigest-0.2.9/biodigest/evaluation/d_utils/runner_utils.py
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.683687 biodigest-0.2.9/biodigest/evaluation/mappers/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)      137 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/mappers/__init__.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     3555 2022-06-08 09:24:26.000000 biodigest-0.2.9/biodigest/evaluation/mappers/disease_getter.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     6577 2022-10-05 12:30:09.000000 biodigest-0.2.9/biodigest/evaluation/mappers/gene_getter.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    13822 2022-09-30 13:24:38.000000 biodigest-0.2.9/biodigest/evaluation/mappers/mapper.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     2926 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/mappers/mapping_transformer.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     5450 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/mappers/mapping_utils.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    11092 2022-02-25 07:45:45.000000 biodigest-0.2.9/biodigest/evaluation/score_calculator.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    12037 2023-03-29 09:20:34.000000 biodigest-0.2.9/biodigest/setup.py
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    29289 2022-10-05 12:30:17.000000 biodigest-0.2.9/biodigest/single_validation.py
+drwxrwxr-x   0 kikky     (1000) kikky     (1000)        0 2023-07-18 12:37:01.683687 biodigest-0.2.9/biodigest.egg-info/
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)    10897 2023-07-18 12:37:01.000000 biodigest-0.2.9/biodigest.egg-info/PKG-INFO
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)      889 2023-07-18 12:37:01.000000 biodigest-0.2.9/biodigest.egg-info/SOURCES.txt
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)        1 2023-07-18 12:37:01.000000 biodigest-0.2.9/biodigest.egg-info/dependency_links.txt
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)      143 2023-07-18 12:37:01.000000 biodigest-0.2.9/biodigest.egg-info/requires.txt
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)       10 2023-07-18 12:37:01.000000 biodigest-0.2.9/biodigest.egg-info/top_level.txt
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)       38 2023-07-18 12:37:01.683687 biodigest-0.2.9/setup.cfg
+-rw-rw-r--   0 kikky     (1000) kikky     (1000)     1327 2023-07-18 12:36:31.000000 biodigest-0.2.9/setup.py
```

### Comparing `biodigest-0.2.8/LICENSE` & `biodigest-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/PKG-INFO` & `biodigest-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodigest
-Version: 0.2.8
+Version: 0.2.9
 Summary: In silico Validation of Disease and Gene Sets, Clusterings or Subnetworks (DIGEST)
 Home-page: http://pypi.python.org/pypi/biodigest/
 Author: Klaudia Adamowicz
 Author-email: klaudia.adamowicz@uni-hamburg.de
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `biodigest-0.2.8/README.md` & `biodigest-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/background_models.py` & `biodigest-0.2.9/biodigest/evaluation/background_models.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/comparator.py` & `biodigest-0.2.9/biodigest/evaluation/comparator.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/config.py` & `biodigest-0.2.9/biodigest/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/d_utils/eval_utils.py` & `biodigest-0.2.9/biodigest/evaluation/d_utils/eval_utils.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/d_utils/plotting_utils.py` & `biodigest-0.2.9/biodigest/evaluation/d_utils/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/d_utils/runner_utils.py` & `biodigest-0.2.9/biodigest/evaluation/d_utils/runner_utils.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/mappers/disease_getter.py` & `biodigest-0.2.9/biodigest/evaluation/mappers/disease_getter.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/mappers/gene_getter.py` & `biodigest-0.2.9/biodigest/evaluation/mappers/gene_getter.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/mappers/mapper.py` & `biodigest-0.2.9/biodigest/evaluation/mappers/mapper.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/mappers/mapping_transformer.py` & `biodigest-0.2.9/biodigest/evaluation/mappers/mapping_transformer.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/mappers/mapping_utils.py` & `biodigest-0.2.9/biodigest/evaluation/mappers/mapping_utils.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/evaluation/score_calculator.py` & `biodigest-0.2.9/biodigest/evaluation/score_calculator.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/setup.py` & `biodigest-0.2.9/biodigest/setup.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest/single_validation.py` & `biodigest-0.2.9/biodigest/single_validation.py`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/biodigest.egg-info/PKG-INFO` & `biodigest-0.2.9/biodigest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biodigest
-Version: 0.2.8
+Version: 0.2.9
 Summary: In silico Validation of Disease and Gene Sets, Clusterings or Subnetworks (DIGEST)
 Home-page: http://pypi.python.org/pypi/biodigest/
 Author: Klaudia Adamowicz
 Author-email: klaudia.adamowicz@uni-hamburg.de
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `biodigest-0.2.8/biodigest.egg-info/SOURCES.txt` & `biodigest-0.2.9/biodigest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biodigest-0.2.8/setup.py` & `biodigest-0.2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biodigest",
-    version="0.2.8",
+    version="0.2.9",
     author="Klaudia Adamowicz",
     author_email='klaudia.adamowicz@uni-hamburg.de',
     url='http://pypi.python.org/pypi/biodigest/',
     license='LICENSE',
     description="In silico Validation of Disease and Gene Sets, Clusterings or Subnetworks (DIGEST)",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -20,18 +20,18 @@
         'Programming Language :: Python :: 3.9',
         'Intended Audience :: Science/Research',
         # "License :: OSI Approved :: MIT License",
         # "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.7',
     install_requires=[
-        "pandas>=1.2.0",
-        "numpy>=1.20.0",
-        "scipy>=1.5.4",
+        "pandas==1.2.0",
+        "numpy==1.20.0",
+        "scipy==1.5.4",
         "seaborn==0.11.2",
         "biothings_client==0.2.6",
         "gseapy==0.10.5",
         "psutil==5.9.0",
-        "requests>=2.26.0",
-        "pycairo>=1.20.1",
+        "requests==2.26.0",
+        "pycairo==1.20.1",
     ]
 )
```

