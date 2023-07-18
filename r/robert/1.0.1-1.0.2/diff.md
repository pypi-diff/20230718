# Comparing `tmp/robert-1.0.1.tar.gz` & `tmp/robert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robert-1.0.1.tar", last modified: Sat Jul  1 07:56:06 2023, max compression
+gzip compressed data, was "robert-1.0.2.tar", last modified: Tue Jul 18 17:02:56 2023, max compression
```

## Comparing `robert-1.0.1.tar` & `robert-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.123300 robert-1.0.1/
--rw-rw-rw-   0        0        0     1099 2023-05-23 09:25:43.000000 robert-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      992 2023-07-01 07:56:06.123300 robert-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2392 2023-06-18 10:39:36.000000 robert-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.104071 robert-1.0.1/robert/
--rw-rw-rw-   0        0        0        0 2023-05-23 09:25:43.000000 robert-1.0.1/robert/__init__.py
--rw-rw-rw-   0        0        0      583 2023-05-23 09:25:43.000000 robert-1.0.1/robert/__main__.py
--rw-rw-rw-   0        0        0     5020 2023-06-17 18:18:26.000000 robert-1.0.1/robert/aqme.py
--rw-rw-rw-   0        0        0     2017 2023-06-20 18:14:41.000000 robert-1.0.1/robert/argument_parser.py
--rw-rw-rw-   0        0        0    15344 2023-06-30 11:54:20.000000 robert-1.0.1/robert/curate.py
--rw-rw-rw-   0        0        0     7529 2023-06-20 18:11:53.000000 robert-1.0.1/robert/generate.py
--rw-rw-rw-   0        0        0    29733 2023-06-30 16:53:53.000000 robert-1.0.1/robert/generate_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.111490 robert-1.0.1/robert/model_params/
--rw-rw-rw-   0        0        0      211 2023-05-23 09:25:43.000000 robert-1.0.1/robert/model_params/ADAB_params.yaml
--rw-rw-rw-   0        0        0      775 2023-06-30 17:01:38.000000 robert-1.0.1/robert/model_params/GB_params.yaml
--rw-rw-rw-   0        0        0       91 2023-06-19 12:21:08.000000 robert-1.0.1/robert/model_params/GP_params.yaml
--rw-rw-rw-   0        0        0       88 2023-06-07 12:49:19.000000 robert-1.0.1/robert/model_params/MVL_params.yaml
--rw-rw-rw-   0        0        0      808 2023-06-07 12:43:39.000000 robert-1.0.1/robert/model_params/NN_params.yaml
--rw-rw-rw-   0        0        0      576 2023-06-30 17:01:41.000000 robert-1.0.1/robert/model_params/RF_params.yaml
--rw-rw-rw-   0        0        0      732 2023-06-30 17:01:45.000000 robert-1.0.1/robert/model_params/VR_params.yaml
--rw-rw-rw-   0        0        0     4374 2023-06-20 17:35:36.000000 robert-1.0.1/robert/predict.py
--rw-rw-rw-   0        0        0    26483 2023-06-21 06:22:51.000000 robert-1.0.1/robert/predict_utils.py
--rw-rw-rw-   0        0        0     5792 2023-07-01 07:20:39.000000 robert-1.0.1/robert/report.py
--rw-rw-rw-   0        0        0     5875 2023-06-20 15:37:54.000000 robert-1.0.1/robert/robert.py
--rw-rw-rw-   0        0        0    37329 2023-07-01 06:59:03.000000 robert-1.0.1/robert/utils.py
--rw-rw-rw-   0        0        0    19418 2023-06-20 15:37:54.000000 robert-1.0.1/robert/verify.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.106828 robert-1.0.1/robert.egg-info/
--rw-rw-rw-   0        0        0      992 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-01 07:56:06.000000 robert-1.0.1/robert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      118 2023-07-01 07:56:06.123300 robert-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1953 2023-07-01 06:58:37.000000 robert-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:56:06.122798 robert-1.0.1/tests/
--rw-rw-rw-   0        0        0     6529 2023-06-19 15:13:27.000000 robert-1.0.1/tests/test_1curate.py
--rw-rw-rw-   0        0        0     6379 2023-06-20 18:16:46.000000 robert-1.0.1/tests/test_2generate.py
--rw-rw-rw-   0        0        0     4289 2023-06-20 19:38:53.000000 robert-1.0.1/tests/test_3verify.py
--rw-rw-rw-   0        0        0     5019 2023-06-20 19:47:48.000000 robert-1.0.1/tests/test_4predict.py
--rw-rw-rw-   0        0        0     4142 2023-06-20 18:05:57.000000 robert-1.0.1/tests/test_5aqme_n_full.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.967943 robert-1.0.2/
+-rw-rw-rw-   0        0        0     1099 2023-05-23 09:25:43.000000 robert-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      992 2023-07-18 17:02:56.967943 robert-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2814 2023-07-18 16:40:13.000000 robert-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.952253 robert-1.0.2/robert/
+-rw-rw-rw-   0        0        0        0 2023-05-23 09:25:43.000000 robert-1.0.2/robert/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-05-23 09:25:43.000000 robert-1.0.2/robert/__main__.py
+-rw-rw-rw-   0        0        0     5035 2023-07-18 16:40:13.000000 robert-1.0.2/robert/aqme.py
+-rw-rw-rw-   0        0        0     2031 2023-07-18 16:40:13.000000 robert-1.0.2/robert/argument_parser.py
+-rw-rw-rw-   0        0        0    15305 2023-07-18 16:40:13.000000 robert-1.0.2/robert/curate.py
+-rw-rw-rw-   0        0        0     8664 2023-07-18 16:40:13.000000 robert-1.0.2/robert/generate.py
+-rw-rw-rw-   0        0        0    32079 2023-07-18 16:40:13.000000 robert-1.0.2/robert/generate_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.967943 robert-1.0.2/robert/model_params/
+-rw-rw-rw-   0        0        0      211 2023-05-23 09:25:43.000000 robert-1.0.2/robert/model_params/ADAB_params.yaml
+-rw-rw-rw-   0        0        0      775 2023-06-30 17:01:38.000000 robert-1.0.2/robert/model_params/GB_params.yaml
+-rw-rw-rw-   0        0        0       91 2023-06-19 12:21:08.000000 robert-1.0.2/robert/model_params/GP_params.yaml
+-rw-rw-rw-   0        0        0       88 2023-06-07 12:49:19.000000 robert-1.0.2/robert/model_params/MVL_params.yaml
+-rw-rw-rw-   0        0        0      808 2023-06-07 12:43:39.000000 robert-1.0.2/robert/model_params/NN_params.yaml
+-rw-rw-rw-   0        0        0      620 2023-07-18 16:40:13.000000 robert-1.0.2/robert/model_params/RF_params.yaml
+-rw-rw-rw-   0        0        0      732 2023-06-30 17:01:45.000000 robert-1.0.2/robert/model_params/VR_params.yaml
+-rw-rw-rw-   0        0        0     4400 2023-07-18 16:40:13.000000 robert-1.0.2/robert/predict.py
+-rw-rw-rw-   0        0        0    26858 2023-07-18 16:43:20.000000 robert-1.0.2/robert/predict_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.967943 robert-1.0.2/robert/report/
+-rw-rw-rw-   0        0        0    37724 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report/AQME.png
+-rw-rw-rw-   0        0        0    43548 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report/CURATE.png
+-rw-rw-rw-   0        0        0    61165 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report/GENERATE.png
+-rw-rw-rw-   0        0        0    32932 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report/PREDICT.png
+-rw-rw-rw-   0        0        0   312641 2023-07-14 10:55:39.000000 robert-1.0.2/robert/report/Robert_logo.jpg
+-rw-rw-rw-   0        0        0    58098 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report/VERIFY.png
+-rw-rw-rw-   0        0        0    14760 2023-07-18 16:40:13.000000 robert-1.0.2/robert/report.py
+-rw-rw-rw-   0        0        0     6760 2023-07-18 16:40:13.000000 robert-1.0.2/robert/robert.py
+-rw-rw-rw-   0        0        0    40258 2023-07-18 16:40:13.000000 robert-1.0.2/robert/utils.py
+-rw-rw-rw-   0        0        0    19671 2023-07-18 16:40:13.000000 robert-1.0.2/robert/verify.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.952253 robert-1.0.2/robert.egg-info/
+-rw-rw-rw-   0        0        0      992 2023-07-18 17:02:56.000000 robert-1.0.2/robert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2023-07-18 17:02:56.000000 robert-1.0.2/robert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:02:56.000000 robert-1.0.2/robert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-07-18 17:02:56.000000 robert-1.0.2/robert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 17:02:56.000000 robert-1.0.2/robert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      118 2023-07-18 17:02:56.967943 robert-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2032 2023-07-18 16:40:13.000000 robert-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:02:56.967943 robert-1.0.2/tests/
+-rw-rw-rw-   0        0        0     6529 2023-06-19 15:13:27.000000 robert-1.0.2/tests/test_1curate.py
+-rw-rw-rw-   0        0        0     6384 2023-07-18 16:40:13.000000 robert-1.0.2/tests/test_2generate.py
+-rw-rw-rw-   0        0        0     4289 2023-06-20 19:38:53.000000 robert-1.0.2/tests/test_3verify.py
+-rw-rw-rw-   0        0        0     5019 2023-07-18 16:40:13.000000 robert-1.0.2/tests/test_4predict.py
+-rw-rw-rw-   0        0        0     4199 2023-07-18 16:40:13.000000 robert-1.0.2/tests/test_5aqme_n_full.py
```

### Comparing `robert-1.0.1/LICENSE` & `robert-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/PKG-INFO` & `robert-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robert
-Version: 1.0.1
+Version: 1.0.2
 Summary: Refiner and Optimizer of a Bunch of Existing Regression Tools
 Home-page: https://github.com/jvalegre/robert
-Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.1.tar.gz
+Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.2.tar.gz
 Author: Juan V. Alegre Requena, David Dalmau
 Author-email: jv.alegre@csic.es
 License: MIT
 Keywords: workflows,machine learning,cheminformatics,data curation,prediction,automated
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `robert-1.0.1/README.md` & `robert-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 ## Documentation  
 Full documentation with installation instructions, technical details and examples can be found in [Read the Docs](https://robert.readthedocs.io).  
 
 Don't miss out the latest hands-on tutorials from our [YouTube channel](https://www.youtube.com/channel/UCHRqI8N61bYxWV9BjbUI4Xw)!  
 
 ## Recommended installation and update guide  
 In a nutshell, ROBERT and its dependencies are installed/updated as follows:  
-1. Install using conda-forge: `conda install -c conda-forge robert`  
-2. Update to the latest version: `pip install robert --upgrade`  
+1. Install using conda-forge (preferred): `conda install -c conda-forge robert`  
+2. Install using pip: `pip install robert`  
+3. Update to the latest version: `pip install robert --upgrade`  
 
 ## Developers and help desk  
 List of main developers and contact emails:  
   - [ ] [Juan V. Alegre-Requena](https://orcid.org/0000-0002-0769-7168). Contact: [jv.alegre@csic.es](mailto:jv.alegre@csic.es)  
   - [ ] [David Dalmau Ginesta](https://orcid.org/0000-0002-2506-6546). Contact: [ddalmau@unizar.es](mailto:ddalmau@unizar.es)  
 
 For suggestions and improvements of the code (greatly appreciated!), please reach out through the issues and pull requests options of Github.  
 
 ## License
 ROBERT is freely available under an [MIT](https://opensource.org/licenses/MIT) License  
 
+## Special acknowledgements
+J.V.A.R. - The acronym ROBERT is dedicated to Prof. ROBERT Paton, who was a mentor to me throughout my years at Colorado State University and who introduced me to the field of cheminformatics. Cheers mate!
+
+D.D.G. - The style of the ROBERT_report.pdf file was created with the help of Oliver Lee (University of St Andrews, 2023).
+
 ## Reference
 If you use any of the ROBERT modules, please include this citation:  
-* Robert v1.0, Alegre-Requena, J. V.; Dalmau, D. 2023. https://github.com/jvalegre/robert.  
+* ROBERT v1.0, Alegre-Requena, J. V.; Dalmau, D. 2023. https://github.com/jvalegre/robert.  
   
 Additionally, please include the corresponding reference for Scikit-learn and SHAP:
 * Pedregosa et al., Scikit-learn: Machine Learning in Python, J. Mach. Learn. Res. 2011, 12, 2825-2830.  
 * Lundberg et al., From local explanations to global understanding with explainable AI for trees, Nat. Mach. Intell. 2020, 2, 56–67.
```

### Comparing `robert-1.0.1/robert/__main__.py` & `robert-1.0.2/robert/__main__.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/robert/aqme.py` & `robert-1.0.2/robert/aqme.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """
 Parameters
 ----------
 
-General
-+++++++
+    csv_name : str, default=''
+        Name of the CSV file containing the database with SMILES and code_name columns. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
+    destination : str, default=None,
+        Directory to create the output file(s).
+    varfile : str, default=None
+        Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
+    y : str, default=''
+        Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
+    qdescp_keywords : str, default=''    
+        Add extra keywords to the AQME-QDESCP run (i.e. qdescp_keywords="--qdescp_atoms ['P']")
+    csearch_keywords : str, default:''
+        Add extra keywords to the AQME-CSEARCH run (i.e. csearch_keywords='--sample 10')
 
-     csv_name : str, default=''
-         Name of the CSV file containing the database with SMILES and code_name columns. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
-     destination : str, default=None,
-         Directory to create the output file(s).
-     varfile : str, default=None
-         Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
-     y : str, default=''
-         Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
-     qdescp_keywords : str, default=''    
-         Add extra keywords to the AQME-QDESCP run (i.e. qdescp_keywords="--qdescp_atoms ['P']")
-     csearch_keywords : str, default:''
-         Add extra keywords to the AQME-CSEARCH run (i.e. csearch_keywords='--sample 10')
 """
 #####################################################.
 #         This file stores the AQME class           #
 #     used to perform the AQME-ROBERT workflow      #
 #####################################################.
 
 import os
 import glob
 import subprocess
 import time
 import shutil
 import sys
+from pathlib import Path
 import pandas as pd
 from robert.utils import (load_variables,
     finish_print,
     load_database
     )
 
 class aqme:
@@ -65,28 +64,29 @@
 
         # run QDESCP to generate descriptors
         cmd_qdescp = ['python', '-m', 'aqme', '--qdescp', '--files', 'CSEARCH/*.sdf', '--program', 'xtb', '--csv_name', f'{self.args.csv_name}']
         _ = self.run_aqme(cmd_qdescp,self.args.qdescp_keywords)
 
         # if no qdesc_atom is set, only keep molecular properties and discard atomic properties
         aqme_db = f'AQME-ROBERT_{self.args.csv_name}'
-        if 'qdescp_atoms' not in self.args.qdescp_keywords:
-            _ = filter_atom_prop(aqme_db)
-
         # ensure that the AQME database was successfully created
         if not os.path.exists(aqme_db):
             self.args.log.write(f"\nx  The initial AQME descriptor protocol did not create any CSV output!")
             sys.exit()
 
+        if 'qdescp_atoms' not in self.args.qdescp_keywords:
+            _ = filter_atom_prop(aqme_db)
+
         # move AQME output files (remove previous runs as well)
         _ = move_aqme()
 
         # finish the printing of the AQME info file
         _ = finish_print(self,start_time,'AQME')
 
+
     def run_aqme(self,command,extra_keywords):
         '''
         Function that runs the AQME jobs
         '''
 
         if extra_keywords != '':
             for keyword in extra_keywords.split():
@@ -100,15 +100,15 @@
         Checks whether AQME is installed
         '''
         
         try:
             from aqme.qprep import qprep
         except ModuleNotFoundError:
             self.args.log.write("x  AQME is not installed (required for the --aqme option)! You can install the program with 'conda install -c conda-forge aqme'")
-            sys.exit()       
+            sys.exit()
 
 
 def filter_atom_prop(aqme_db):
     '''
     Function that filters off atomic properties if no atom was selected in the --qdescp_atoms option
     '''
     
@@ -127,12 +127,12 @@
     '''
     Move raw data from AQME-CSEARCH and -QDESCP runs into the AQME folder
     '''
     
     for file in glob.glob(f'*'):
         if 'CSEARCH' in file or 'QDESCP' in file:
             if os.path.exists(f'AQME/{file}'):
-                if len(file.split('.')) == 1:
+                if len(os.path.basename(Path(file)).split('.')) == 1:
                     shutil.rmtree(f'AQME/{file}')
                 else:
                     os.remove(f'AQME/{file}')
             shutil.move(file, f'AQME/{file}')
```

### Comparing `robert-1.0.1/robert/argument_parser.py` & `robert-1.0.2/robert/argument_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,35 @@
     "curate": False,
     "generate": False,
     "predict": False,
     "verify": False,
     "aqme": False,
     "report": False,
     "cheers": False,
-    "seed": [0,8,19,43,70,233,1989,9999,20394,3948301],
+    "seed": [],
+    "generate_acc": 'mid',
     "destination": None,
     "csv_name" : '',
     "y" : '',
     "discard" : [],
     "ignore" : [],
     "categorical" : "onehot",
     "corr_filter" : True,
     "desc_thres" : 25,
     "thres_y" : 0.001,
     "thres_x" : 0.9,
     "train" : [60,70,80,90],
+    "filter_train" : True,
     "split" : "KN",
     "model" : ['RF','GB','NN','MVL'],
     "custom_params" : None,
     "type" : "reg",
-    "epochs" : 80,
+    "epochs" : 0,
     "error_type" : "rmse",
-    "pfi_epochs" : 30,
+    "pfi_epochs" : 5,
     "pfi_threshold" : 0.04,
     "pfi_filter" : True,
     "pfi_max" : 0,
     "thres_test" : 0.2,
     "kfold" : 5,
     "params_dir" : '',
     "csv_test" : '',
```

### Comparing `robert-1.0.1/robert/curate.py` & `robert-1.0.2/robert/curate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 """
 Parameters
 ----------
 
-     csv_name : str, default=''
-         Name of the CSV file containing the database. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
-     y : str, default=''
-         Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
-     discard : list, default=[]
-         List containing the columns of the input CSV file that will not be included as descriptors
-         in the curated CSV file (i.e. ['name','SMILES']).
-     ignore : list, default=[]
-         List containing the columns of the input CSV file that will be ignored during the curation process
-         (i.e. ['name','SMILES']). The descriptors will be included in the curated CSV file. The y value
-         is automatically ignored.
-     destination : str, default=None,
-         Directory to create the output file(s).
-     varfile : str, default=None
-         Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
-     categorical : str, default='onehot'
-         Mode to convert data from columns with categorical variables. As an example, a variable containing 4
-         types of C atoms (i.e. primary, secondary, tertiary, quaternary) will be converted into categorical
-         variables. Options: 
-            1. 'onehot' (for one-hot encoding, ROBERT will create a descriptor for each type of
-               C atom using 0s and 1s to indicate whether the C type is present)
-            2. 'numbers' (to describe the C atoms with numbers: 1, 2, 3, 4).
-     corr_filter : bool, default=True
-         Activate the correlation filters of descriptors. Two filters will be performed based on the correlation
-         of the descriptors with other descriptors (x filter) and the y values (y filter).
-     desc_thres : float, default=25
-         Threshold for the descriptor-to-datapoints ratio to deactivate the correlation filter. By default,
-         the correlation filter is disabled if there are 25 times more datapoints than descriptors.
-     thres_x : float, default=0.9
-         Thresolhold to discard descriptors based on high R**2 correlation with other descriptors (i.e. 
-         if thres_x=0.9, variables that show R**2 > 0.9 will be discarded).
-     thres_y : float, default=0.001
-         Thresolhold to discard descriptors with poor correlation with the y values based on R**2 (i.e.
-         if thres_y=0.001, variables that show R**2 < 0.01 will be discarded).
+    csv_name : str, default=''
+        Name of the CSV file containing the database. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
+    y : str, default=''
+        Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
+    discard : list, default=[]
+        List containing the columns of the input CSV file that will not be included as descriptors
+        in the curated CSV file (i.e. ['name','SMILES']).
+    ignore : list, default=[]
+        List containing the columns of the input CSV file that will be ignored during the curation process
+        (i.e. ['name','SMILES']). The descriptors will be included in the curated CSV file. The y value
+        is automatically ignored.
+    destination : str, default=None,
+        Directory to create the output file(s).
+    varfile : str, default=None
+        Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
+    categorical : str, default='onehot'
+        Mode to convert data from columns with categorical variables. As an example, a variable containing 4
+        types of C atoms (i.e. primary, secondary, tertiary, quaternary) will be converted into categorical
+        variables. Options: 
+        1. 'onehot' (for one-hot encoding, ROBERT will create a descriptor for each type of
+        C atom using 0s and 1s to indicate whether the C type is present)
+        2. 'numbers' (to describe the C atoms with numbers: 1, 2, 3, 4).
+    corr_filter : bool, default=True
+        Activate the correlation filters of descriptors. Two filters will be performed based on the correlation
+        of the descriptors with other descriptors (x filter) and the y values (y filter).
+    desc_thres : float, default=25
+        Threshold for the descriptor-to-datapoints ratio to deactivate the correlation filter. By default,
+        the correlation filter is disabled if there are 25 times more datapoints than descriptors.
+    thres_x : float, default=0.9
+        Thresolhold to discard descriptors based on high R**2 correlation with other descriptors (i.e. 
+        if thres_x=0.9, variables that show R**2 > 0.9 will be discarded).
+    thres_y : float, default=0.001
+        Thresolhold to discard descriptors with poor correlation with the y values based on R**2 (i.e.
+        if thres_y=0.001, variables that show R**2 < 0.01 will be discarded).
+
 """
 #####################################################.
 #         This file stores the CURATE class         #
 #               used in data curation               #
 #####################################################.
 
 import time
@@ -168,54 +169,59 @@
 
     def correlation_filter(self, csv_df):
         """
         Discards a) correlated variables and b) variables that do not correlate with the y values, based
         on R**2 values.
         """
 
-        txt_corr = f'\no  Correlation filter activated with these thresholds: thres_x = {self.args.thres_x}, thres_y = {self.args.thres_y}'
-        # don't remove descriptors if there are too few descriptors (after 25 times more datapoints)
+        txt_corr = ''
+
+        # loosen correlation filters if there are too few descriptors
         n_descps = len(csv_df.columns)-len(self.args.ignore)-1 # all columns - ignored - y
+        if self.args.desc_thres and n_descps*self.args.desc_thres < len(csv_df[self.args.y]):
+            self.args.thres_x = 0.95
+            self.args.thres_y = 0.0001
+            txt_corr += f'\nx  WARNING! The number of descriptors ({n_descps}) is {self.args.desc_thres} times lower than the number of datapoints ({len(csv_df[self.args.y])}), the correlation filters are loosen to thres_x = 0.95 and thres_y = 0.0001! Default thresholds (0.9 and 0.001) can be used with "--desc_thres False"'
+
+        txt_corr += f'\no  Correlation filter activated with these thresholds: thres_x = {self.args.thres_x}, thres_y = {self.args.thres_y}'
+
         descriptors_drop = []
-        if not n_descps*self.args.desc_thres < len(csv_df[self.args.y]):
-            txt_corr += f'\n   Excluded descriptors:'
-            for i,column in enumerate(csv_df.columns):
-                if column not in descriptors_drop and column not in self.args.ignore and column != self.args.y:
-                    # finds the descriptors with low correlation to the response values
-                    try:
-                        _, _, r_value_y, _, _ = stats.linregress(csv_df[column],csv_df[self.args.y])
-                        rsquared_y = r_value_y**2
-                        if rsquared_y < self.args.thres_y:
-                            descriptors_drop.append(column)
-                            txt_corr += f'\n   - {column}: R**2 = {round(rsquared_y,2)} with the {self.args.y} values'
-                    except ValueError: # this avoids X descriptors where the majority of the values are the same
+        txt_corr += f'\n   Excluded descriptors:'
+        for i,column in enumerate(csv_df.columns):
+            if column not in descriptors_drop and column not in self.args.ignore and column != self.args.y:
+                # finds the descriptors with low correlation to the response values
+                try:
+                    _, _, r_value_y, _, _ = stats.linregress(csv_df[column],csv_df[self.args.y])
+                    rsquared_y = r_value_y**2
+                    if rsquared_y < self.args.thres_y:
                         descriptors_drop.append(column)
-                        txt_corr += f'\n   - {column}: error in R**2 with the {self.args.y} values (are all the values the same?)'
-
-                    # finds correlated descriptors
-                    if column != csv_df.columns[-1] and column not in descriptors_drop:
-                        for j,column2 in enumerate(csv_df.columns):
-                            if j > i and column2 not in self.args.ignore and column not in descriptors_drop and column2 not in descriptors_drop and column2 != self.args.y:
-                                _, _, r_value_x, _, _ = stats.linregress(csv_df[column],csv_df[column2])
-                                rsquared_x = r_value_x**2
-                                if rsquared_x > self.args.thres_x:
-                                    # discard the column with less correlation with the y values
-                                    _, _, r_value_y2, _, _ = stats.linregress(csv_df[column2],csv_df[self.args.y])
-                                    rsquared_y2 = r_value_y2**2
-                                    if rsquared_y >= rsquared_y2:
-                                        descriptors_drop.append(column2)
-                                        txt_corr += f'\n   - {column2}: R**2 = {round(rsquared_x,2)} with {column}'
-                                    else:
-                                        descriptors_drop.append(column)
-                                        txt_corr += f'\n   - {column}: R**2 = {round(rsquared_x,2)} with {column2}'
-            
-            if len(descriptors_drop) == 0:
-                txt_corr += f'\n   -  No descriptors were removed'
-        else:
-            txt_corr += f'\n   x The number of descriptors ({n_descps}) is {self.args.desc_thres} times lower than the number of datapoints ({len(csv_df[self.args.y])}), the correlation filter was disabled! The ratio of this filter can be adjusted with the desc_thres option'
+                        txt_corr += f'\n   - {column}: R**2 = {round(rsquared_y,2)} with the {self.args.y} values'
+                except ValueError: # this avoids X descriptors where the majority of the values are the same
+                    descriptors_drop.append(column)
+                    txt_corr += f'\n   - {column}: error in R**2 with the {self.args.y} values (are all the values the same?)'
+
+                # finds correlated descriptors
+                if column != csv_df.columns[-1] and column not in descriptors_drop:
+                    for j,column2 in enumerate(csv_df.columns):
+                        if j > i and column2 not in self.args.ignore and column not in descriptors_drop and column2 not in descriptors_drop and column2 != self.args.y:
+                            _, _, r_value_x, _, _ = stats.linregress(csv_df[column],csv_df[column2])
+                            rsquared_x = r_value_x**2
+                            if rsquared_x > self.args.thres_x:
+                                # discard the column with less correlation with the y values
+                                _, _, r_value_y2, _, _ = stats.linregress(csv_df[column2],csv_df[self.args.y])
+                                rsquared_y2 = r_value_y2**2
+                                if rsquared_y >= rsquared_y2:
+                                    descriptors_drop.append(column2)
+                                    txt_corr += f'\n   - {column2}: R**2 = {round(rsquared_x,2)} with {column}'
+                                else:
+                                    descriptors_drop.append(column)
+                                    txt_corr += f'\n   - {column}: R**2 = {round(rsquared_x,2)} with {column2}'
+        
+        if len(descriptors_drop) == 0:
+            txt_corr += f'\n   -  No descriptors were removed'
 
         self.args.log.write(txt_corr)
 
         # drop descriptors that did not pass the filters
         csv_df_filtered = csv_df.drop(descriptors_drop, axis=1)
         txt_csv = f'\no  {len(csv_df_filtered.columns)} columns remaining after applying duplicate and correlation filters:\n'
         txt_csv += '\n'.join(f'   - {var}' for var in csv_df_filtered.columns)
```

### Comparing `robert-1.0.1/robert/generate.py` & `robert-1.0.2/robert/generate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 """
 Parameters
 ----------
 
-General
-+++++++
+    csv_name : str, default=''
+        Name of the CSV file containing the database. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
+    y : str, default=''
+        Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
+    discard : list, default=[]
+        List containing the columns of the input CSV file that will not be included as descriptors
+        in the curated CSV file (i.e. ['name','SMILES']).
+    ignore : list, default=[]
+        List containing the columns of the input CSV file that will be ignored during the curation process
+        (i.e. ['name','SMILES']). The descriptors will be included in the curated CSV file. The y value
+        is automatically ignored.
+    destination : str, default=None
+        Directory to create the output file(s).
+    varfile : str, default=None
+        Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
+    train : list, default=[60,70,80,90]
+        Proportions of the training set to use in the ML scan. The numbers are relative to the training 
+        set proportion (i.e. 40 = 40% training data).
+    filter_train : bool, default=True
+        Disables the 90% training size in databases with less than 50 entries.
+    split : str, default='KN'
+        Mode for splitting data. Options: 
+        1. 'KN' (k-neighbours clustering-based splitting)
+        2. 'RND' (random splitting).  
+    model : list, default=['RF','GB','NN','MVL'] (regression) and default=['RF','GB','NN','AdaB'] (classification) 
+        ML models available: 
+        1. 'RF' (Random forest)
+        2. 'MVL' (Multivariate lineal models)
+        3. 'GB' (Gradient boosting)
+        4. 'NN' (MLP neural network)
+        5. 'GP' (Gaussian Process)
+        6. 'AdaB' (AdaBoost)
+        7. 'VR' (Voting regressor combining RF, GB and NN)
+    custom_params : str, default=None
+        Define new parameters for the ML models used in the hyperoptimization workflow. The path
+        to the folder containing all the yaml files should be specified (i.e. custom_params='YAML_FOLDER')
+    type : str, default='reg'
+        Type of the pedictions. Options: 
+        1. 'reg' (Regressor)
+        2. 'clas' (Classifier)
+    seed : list, default=[]
+        Random seeds used in the ML predictor models, data splitting and other protocols. If seed 
+        is not adjusted manually, the generate_acc option will set the values for seed.
+    epochs : int, default=0
+        Number of epochs for the hyperopt optimization. If epochs is not adjusted manually, the 
+        generate_acc option will set the values for epochs.
+    generate_acc : str, default='mid'
+        Accuracy of the workflow performed in GENERATE in terms of seed and epochs. Options:
+        1. 'low', fastest and least accurate protocol (seed = [0,8,19], epochs = 20)
+        2. 'mid', compromise between 'low' and 'high' accurate protocol (seed = [0,8,19,43,70,233], 
+        epochs = 40)
+        3. 'high', slowest and most accurate protocol (seed = [0,8,19,43,70,233,1989,9999,20394,3948301], 
+        epochs = 100)
+    error_type : str, default: rmse (regression), acc (classification)
+        Target value used during the hyperopt optimization. Options:
+        Regression:
+        1. rmse (root-mean-square error)
+        2. mae (mean absolute error)
+        3. r2 (R-squared, not recommended since R2 might be good even with high errors in small datasets)
+        Classification:
+        1. mcc (Matthew's correlation coefficient)
+        2. f1 (F1 score)
+        3. acc (accuracy, fraction of correct predictions)
+    pfi_filter : bool, default=True
+        Activate the PFI filter of descriptors.
+    pfi_epochs : int, default=5
+        Sets the number of times a feature is randomly shuffled during the PFI analysis
+        (standard from sklearn webpage: 5).
+    pfi_threshold : float, default=0.04
+        The PFI filter is X% of the model's score (% adjusted, 0.04 = 4% of the total score during PFI).
+        For regression, a value of 0.04 is recommended. For classification, the filter is turned off
+        by default if pfi_threshold is 0.04.
+    pfi_max : int, default=0
+        Number of features to keep after the PFI filter. If pfi_max is 0, all the features that pass the PFI
+        filter are used.
 
-     csv_name : str, default=''
-         Name of the CSV file containing the database. A path can be provided (i.e. 'C:/Users/FOLDER/FILE.csv'). 
-     y : str, default=''
-         Name of the column containing the response variable in the input CSV file (i.e. 'solubility'). 
-     discard : list, default=[]
-         List containing the columns of the input CSV file that will not be included as descriptors
-         in the curated CSV file (i.e. ['name','SMILES']).
-     ignore : list, default=[]
-         List containing the columns of the input CSV file that will be ignored during the curation process
-         (i.e. ['name','SMILES']). The descriptors will be included in the curated CSV file. The y value
-         is automatically ignored.
-     destination : str, default=None
-         Directory to create the output file(s).
-     varfile : str, default=None
-         Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
-     train : list, default=[60,70,80,90]
-         Proportions of the training set to use in the ML scan. The numbers are relative to the training 
-         set proportion (i.e. 40 = 40% training data).
-     split : str, default='KN'
-         Mode for splitting data. Options: 
-            1. 'KN' (k-neighbours clustering-based splitting)
-            2. 'RND' (random splitting).  
-     model : list, default=['RF','GB','NN','MVL'] (regression) and default=['RF','GB','NN','AdaB'] (classification) 
-         ML models available: 
-            1. 'RF' (Random forest)
-            2. 'MVL' (Multivariate lineal models)
-            3. 'GB' (Gradient boosting)
-            4. 'NN' (MLP neural network)
-            5. 'GP' (Gaussian Process)
-            6. 'AdaB' (AdaBoost)
-            7. 'VR' (Voting regressor combining RF, GB and NN)
-     custom_params : str, default=None
-         Define new parameters for the ML models used in the hyperoptimization workflow. The path
-         to the folder containing all the yaml files should be specified (i.e. custom_params='YAML_FOLDER')
-     type : str, default='reg'
-         Type of the pedictions. Options: 
-            1. 'reg' (Regressor)
-            2. 'clas' (Classifier)
-     seed : list, default=[0,8,19,43,70,233,1989,9999,20394,3948301]
-         Random seeds used in the ML predictor models, data splitting and other protocols.
-     epochs : int, default=80
-         Number of epochs for the hyperopt optimization.
-     error_type : str, default: rmse (regression), acc (classification)
-         Target value used during the hyperopt optimization. Options:
-         Regression:
-            1. rmse (root-mean-square error)
-            2. mae (mean absolute error)
-            3. r2 (R-squared, not recommended since R2 might be good even with high errors in small datasets)
-         Classification:
-            1. mcc (Matthew's correlation coefficient)
-            2. f1 (F1 score)
-            3. acc (accuracy, fraction of correct predictions)
-     pfi_filter : bool, default=True
-         Activate the PFI filter of descriptors.
-     pfi_epochs : int, default=30
-         Sets the number of times a feature is randomly shuffled during the PFI analysis
-         (standard from sklearn webpage: 30).
-     pfi_threshold : float, default=0.04
-         The PFI filter is X% of the model's score (% adjusted, 0.04 = 4% of the total score during PFI).
-         For regression, a value of 0.04 is recommended. For classification, the filter is turned off
-         by default if pfi_threshold is 0.04.
-     pfi_max : int, default=0
-         Number of features to keep after the PFI filter. If pfi_max is 0, all the features that pass the PFI
-         filter are used.
 """
 #####################################################.
 #        This file stores the GENERATE class        #
 #             used in model generation              #
 #####################################################.
 
 import time
@@ -107,14 +116,20 @@
 
         # load default and user-specified variables
         self.args = load_variables(kwargs, "generate")
 
         # load database, discard user-defined descriptors and perform data checks
         csv_df, csv_X, csv_y = load_database(self,self.args.csv_name,"generate")
 
+        # if there are less than 50 datapoints, the 90% training size is disabled by default
+        if self.args.filter_train:
+            if len(csv_df[self.args.y]) < 50 and 90 in self.args.train:
+                self.args.train.remove(90)
+                self.args.log.write(f'\nx    WARNING! The database contains {len(csv_df[self.args.y])} datapoints, the 90% training size will be excluded (too few validation points to reach a reliable result). You can include this size using "--filter_train False".')
+
         # scan different ML models
         txt_heatmap = f"\no  Starting heatmap scan with {len(self.args.model)} ML models ({self.args.model}) and {len(self.args.train)} training sizes ({self.args.train})."
 
         # scan different training partition sizes
         cycle = 1
         txt_heatmap += f'\n   Heatmap generation:'
         self.args.log.write(txt_heatmap)
```

### Comparing `robert-1.0.1/robert/generate_utils.py` & `robert-1.0.2/robert/generate_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 from pathlib import Path
 import random
 import pandas as pd
 import numpy as np
 import seaborn as sb
 from matplotlib import pyplot as plt
 import matplotlib.colors as mcolor
+# for users with no intel architectures. This part has to be before the sklearn imports
+# try:
+#     from sklearnex import patch_sklearn
+#     patch_sklearn(verbose=False)
+# except (ModuleNotFoundError,ImportError):
+#     pass
 from sklearn.cluster import KMeans
 import yaml
 import json
 import glob
 from pkg_resources import resource_filename
 from sklearn.inspection import permutation_importance
 from hyperopt import fmin, tpe, hp, STATUS_OK, Trials
@@ -334,14 +340,36 @@
     X_train_scaled, X_valid_scaled = standardize(self,Xy_data['X_train'],Xy_data['X_valid'])
     Xy_data['X_train_scaled'] = X_train_scaled
     Xy_data['X_valid_scaled'] = X_valid_scaled
 
     # also store the descriptors used (the labels disappear after data_split() )
     Xy_data['X_descriptors'] = csv_X.columns.tolist()
 
+    # discard descriptors with NaN values after standardization. This might happen when using descriptor
+    # columns that after the data split contain only one unique value in one of the sets (i.e., 0,0,0,0,0)
+    columns_nan = []
+    for column in Xy_data['X_train_scaled'].columns:
+        if Xy_data['X_train_scaled'][column].isnull().values.any():
+            columns_nan.append(column)
+        elif Xy_data['X_valid_scaled'][column].isnull().values.any():
+            columns_nan.append(column)
+
+    if len(columns_nan) > 0:
+        nan_print = '   x  Variables removed for having NaN values after standardization:'
+        for column_nan in columns_nan:
+            nan_print += f'\n      - {column_nan}'
+            Xy_data['X_descriptors'].remove(column_nan)
+            Xy_data['X_train_scaled'] = Xy_data['X_train_scaled'].drop(column_nan, axis=1)
+            Xy_data['X_valid_scaled'] = Xy_data['X_valid_scaled'].drop(column_nan, axis=1)
+            Xy_data['X_train'] = Xy_data['X_train'].drop(column_nan, axis=1)
+            Xy_data['X_valid'] = Xy_data['X_valid'].drop(column_nan, axis=1)
+            csv_X = csv_X.drop(column_nan, axis=1)
+
+        self.args.log.write(nan_print)
+
     return Xy_data
 
 
 def data_split(self,csv_X,csv_y,size,seed):
 
     if size == 100:
         # if there is no validation set, use all the points
@@ -419,40 +447,62 @@
 
 def PFI_workflow(self, csv_df, ML_model, size, Xy_data, seed):
     # filter off parameters with low PFI (not relevant in the model)
     name_csv_hyperopt = f"Raw_data/No_PFI/{ML_model}_{size}_{seed}"
     path_csv = self.args.destination.joinpath(f'{name_csv_hyperopt}.csv')
     PFI_df = pd.read_csv(path_csv)
     PFI_dict = pd_to_dict(PFI_df) # (using a dict to keep the same format of load_model)
-    PFI_discard = PFI_filter(self,Xy_data,PFI_dict,ML_model,size,seed)
+    PFI_discard_cols = PFI_filter(self,Xy_data,PFI_dict,seed)
 
     # generate new X datasets and store the descriptors used for the PFI-filtered model
+    desc_keep = len(Xy_data['X_train'].columns)
+    
+    # if the filter does not remove any descriptors based on the PFI threshold, or the 
+    # proportion of descriptors:total datapoints is higher than 1:3, then the filter takes
+    # the minimum value of 1 and 2:
+    #   1. 25% less descriptors than the No PFI original model
+    #   2. Proportion of 1:3 of descriptors:total datapoints (training + validation)
+    total_points = len(Xy_data['y_train'])+len(Xy_data['y_valid'])
+    n_descp_PFI = desc_keep-len(PFI_discard_cols)
+    if n_descp_PFI > 0.33*total_points or n_descp_PFI == desc_keep or n_descp_PFI == 0:
+        option_one = int(0.75*len(Xy_data['X_train'].columns))
+        option_two = int(0.33*total_points)
+        pfi_max = min(option_one,option_two)
+    else:
+        pfi_max = self.args.pfi_max
+    
     discard_idx, descriptors_PFI = [],[]
-    desc_keep = len(Xy_data['X_train'])
-    if self.args.pfi_max != 0:
-        desc_keep = self.args.pfi_max
-    for _,column in enumerate(Xy_data['X_train']):
-        if column not in PFI_discard and len(descriptors_PFI) < desc_keep:
-            descriptors_PFI.append(column)
-        else:
-            discard_idx.append(column)
-    Xy_data_PFI = Xy_data.copy()
+    # just in case none of the descriptors passed the PFI filter
+    # select only the most important deascriptors until the pfi_max limit
+    if n_descp_PFI == 0:
+        descriptors_PFI = PFI_discard_cols[:pfi_max]
+        discard_idx = PFI_discard_cols[len(PFI_discard_cols)-pfi_max:]
 
+    else:
+        if pfi_max != 0:
+            desc_keep = pfi_max
+        for _,column in enumerate(Xy_data['X_train'].columns):
+            if column not in PFI_discard_cols and len(descriptors_PFI) < desc_keep:
+                descriptors_PFI.append(column)
+            else:
+                discard_idx.append(column)
+
+    Xy_data_PFI = Xy_data.copy()
     Xy_data_PFI['X_train'] = Xy_data['X_train'].drop(discard_idx, axis=1)
     Xy_data_PFI['X_valid'] = Xy_data['X_valid'].drop(discard_idx, axis=1)
     Xy_data_PFI['X_train_scaled'], Xy_data_PFI['X_valid_scaled'] = standardize(self,Xy_data_PFI['X_train'],Xy_data_PFI['X_valid'])
     PFI_dict['X_descriptors'] = descriptors_PFI
     if 'max_features' in  PFI_dict and PFI_dict['max_features'] > len(descriptors_PFI):
         PFI_dict['max_features'] = len(descriptors_PFI)
 
     # updates the model's error and descriptors used from the corresponding No_PFI CSV file 
     # (the other parameters remain the same)
     opt_target = load_n_predict(PFI_dict, Xy_data_PFI, hyperopt=True)
     PFI_dict[PFI_dict['error_type']] = opt_target
-    
+
     # save CSV file
     name_csv_hyperopt_PFI = name_csv_hyperopt.replace('No_PFI','PFI')
     path_csv_PFI = self.args.destination.joinpath(f'{name_csv_hyperopt_PFI}_PFI')
     csv_PFI_df = pd.DataFrame.from_dict(PFI_dict, orient='index')
     csv_PFI_df = csv_PFI_df.transpose()
     _ = csv_PFI_df.to_csv(f'{path_csv_PFI}.csv', index = None, header=True)
 
@@ -469,49 +519,43 @@
 
     # save the csv file
     if os.path.exists(self.args.destination.joinpath(f"Raw_data/PFI/{ML_model}_{size}_{seed}_PFI.csv")):
         db_name = self.args.destination.joinpath(f"Raw_data/PFI/{ML_model}_{size}_{seed}_PFI_db")
         _ = csv_df.to_csv(f'{db_name}.csv', index = None, header=True)
 
 
-def PFI_filter(self,Xy_data,PFI_dict,ML_model,size,seed):
+def PFI_filter(self,Xy_data,PFI_dict,seed):
 
     # load and fit model
     loaded_model = load_model(PFI_dict)
     loaded_model.fit(Xy_data['X_train_scaled'], Xy_data['y_train'])
 
     # we use the validation set during PFI as suggested by the sklearn team:
     # "Using a held-out set makes it possible to highlight which features contribute the most to the 
     # generalization power of the inspected model. Features that are important on the training set 
     # but not on the held-out set might cause the model to overfit."
     score_model = loaded_model.score(Xy_data['X_valid_scaled'], Xy_data['y_valid'])
     perm_importance = permutation_importance(loaded_model, Xy_data['X_valid_scaled'], Xy_data['y_valid'], n_repeats=self.args.pfi_epochs, random_state=seed)
-
-    # transforms the values into a list and sort the PFI values with the descriptors names
-    desc_list, PFI_values, PFI_sd = [],[],[]
-    for i,desc in enumerate(Xy_data['X_train']):
-        desc_list.append(desc)
+    # transforms the values into a list and sort the PFI values with the descriptor names
+    descp_cols, PFI_values, PFI_sd = [],[],[]
+    for i,desc in enumerate(Xy_data['X_train'].columns):
+        descp_cols.append(desc) # includes lists of descriptors not column names!
         PFI_values.append(perm_importance.importances_mean[i])
         PFI_sd.append(perm_importance.importances_std[i])
   
-    PFI_values, PFI_sd, desc_list = (list(t) for t in zip(*sorted(zip(PFI_values, PFI_sd, desc_list), reverse=True)))
+    PFI_values, PFI_sd, descp_cols = (list(t) for t in zip(*sorted(zip(PFI_values, PFI_sd, descp_cols), reverse=True)))
 
     # PFI filter
-    PFI_discard = []
+    PFI_discard_cols = []
     PFI_thres = abs(self.args.pfi_threshold*score_model)
-    for i in reversed(range(len(PFI_values))):
+    for i in range(len(PFI_values)):
         if PFI_values[i] < PFI_thres:
-            PFI_discard.append(desc_list[i])
-
-    # disconnect the PFI filter if none of the variables pass the filter
-    if len(PFI_discard) == len(PFI_values):
-        PFI_discard = []
-        self.args.log.write(f'   x The PFI filter was disabled for model {ML_model}_{size}_{seed} (no variables passed)')
+            PFI_discard_cols.append(descp_cols[i])
 
-    return PFI_discard
+    return PFI_discard_cols
 
 
 def filter_seed(self, name_csv):
     '''
     Check which seed led to the best results
     '''
```

### Comparing `robert-1.0.1/robert/model_params/GB_params.yaml` & `robert-1.0.2/robert/model_params/GB_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/robert/model_params/NN_params.yaml` & `robert-1.0.2/robert/model_params/NN_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/robert/model_params/RF_params.yaml` & `robert-1.0.2/robert/model_params/RF_params.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 # min weight to be leaf node
 min_weight_fraction_leaf: [0]
 
 # use oob samples
 oob_score: [True,False]
 
-# complexity parameter for pruning
+# complexity parameter for pruning, I can't set it to 0 or the RF model breaks
 ccp_alpha : [0]
 
 # number of samples to draw for bootstrap
 max_samples : [0.25,0.5,0.75,1]
```

### Comparing `robert-1.0.1/robert/model_params/VR_params.yaml` & `robert-1.0.2/robert/model_params/VR_params.yaml`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/robert/predict.py` & `robert-1.0.2/robert/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """
 Parameters
 ----------
 
-General
-+++++++
+    destination : str, default=None,
+        Directory to create the output file(s).
+    varfile : str, default=None
+        Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
+    params_dir : str, default=''
+        Folder containing the database and parameters of the ML model.
+    csv_test : str, default=''
+        Name of the CSV file containing the test set (if any). A path can be provided (i.e. 
+        'C:/Users/FOLDER/FILE.csv'). 
+    t_value : float, default=2
+        t-value that will be the threshold to identify outliers (check tables for t-values elsewhere).
+        The higher the t-value the more restrictive the analysis will be (i.e. there will be more 
+        outliers with t-value=1 than with t-value = 4).
+    shap_show : int, default=10,
+        Number of descriptors shown in the plot of the SHAP analysis.
+    pfi_show : int, default=10,
+        Number of descriptors shown in the plot of the PFI analysis.
+    pfi_epochs : int, default=5,
+        Sets the number of times a feature is randomly shuffled during the PFI analysis
+        (standard from sklearn webpage: 5).
+    names : str, default=''
+        Column of the names for each datapoint. Names are used to print outliers.
 
-     destination : str, default=None,
-         Directory to create the output file(s).
-     varfile : str, default=None
-         Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
-     params_dir : str, default=''
-         Folder containing the database and parameters of the ML model.
-     csv_test : str, default=''
-         Name of the CSV file containing the test set (if any). A path can be provided (i.e. 
-         'C:/Users/FOLDER/FILE.csv'). 
-     t_value : float, default=2
-         t-value that will be the threshold to identify outliers (check tables for t-values elsewhere).
-         The higher the t-value the more restrictive the analysis will be (i.e. there will be more 
-         outliers with t-value=1 than with t-value = 4).
-     shap_show : int, default=10,
-         Number of descriptors shown in the plot of the SHAP analysis.
-     pfi_show : int, default=10,
-         Number of descriptors shown in the plot of the PFI analysis.
-     pfi_epochs : int, default=30,
-         Sets the number of times a feature is randomly shuffled during the PFI analysis
-         (standard from sklearn webpage: 30).
-     names : str, default=''
-         Column of the names for each datapoint. Names are used to print outliers.
 """
 #####################################################.
 #        This file stores the PREDICT class         #
 #    used to analyze and generate ML predictors     #
 #####################################################.
 
 import os
@@ -43,15 +41,16 @@
     PFI_plot,
     outlier_plot
     )
 from robert.utils import (load_variables,
     load_db_n_params,
     pd_to_dict,
     load_n_predict,
-    finish_print
+    finish_print,
+    print_pfi
 )
 
 class predict:
     """
     Class containing all the functions from the PREDICT module.
 
     Parameters
@@ -71,14 +70,17 @@
         if 'GENERATE/Best_model' in self.args.params_dir:
             params_dirs = [f'{self.args.params_dir}/No_PFI',f'{self.args.params_dir}/PFI']
         else:
             params_dirs = [self.args.params_dir]
 
         for params_dir in params_dirs:
             if os.path.exists(params_dir):
+
+                _ = print_pfi(self,params_dir)
+
                 # load and ML model parameters, and add standardized descriptors
                 Xy_data, params_df, _, _ = load_db_n_params(self,params_dir,"verify",True) # module 'verify' since PREDICT follows similar protocols
 
                 # load test set and add standardized descriptors
                 if self.args.csv_test != '':
                     Xy_data = load_test(self, Xy_data, params_df)
```

### Comparing `robert-1.0.1/robert/predict_utils.py` & `robert-1.0.2/robert/predict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 import ast
 from pathlib import Path
 import pandas as pd
 import numpy as np
 import seaborn as sb
 from matplotlib import pyplot as plt
 import matplotlib.patches as mpatches
+# for users with no intel architectures. This part has to be before the sklearn imports
+# try:
+#     from sklearnex import patch_sklearn
+#     patch_sklearn(verbose=False)
+# except (ModuleNotFoundError,ImportError):
+#     pass
 from sklearn.metrics import ConfusionMatrixDisplay
 from sklearn.inspection import permutation_importance
 import shap
 from robert.curate import curate
 from robert.utils import (
     load_model,
     standardize,
@@ -171,15 +177,15 @@
 
 def graph_clas(self,loaded_model,Xy_data,params_dict,set_type,path_n_suffix):
     '''
     Plot a confusion matrix with the prediction vs actual values
     '''
     
     matrix = ConfusionMatrixDisplay.from_estimator(loaded_model, Xy_data[f'X_{set_type}_scaled'], Xy_data[f'y_{set_type}'], normalize="true", cmap='Blues') 
-    matrix.ax_.set_title(f'Confusion Matrix for the {set_type} set of {os.path.basename(path_n_suffix)}', fontsize=14)
+    matrix.ax_.set_title(f'Confusion Matrix for the {set_type} set of {os.path.basename(path_n_suffix)}', fontsize=14, weight='bold')
     plt.xlabel(f'Predicted {params_dict["y"]}', fontsize=14)
     plt.ylabel(f'{params_dict["y"]}', fontsize=14)
     plt.gcf().axes[0].tick_params(size=14)
     plt.gcf().axes[1].tick_params(size=14)
     clas_plot_file = f'{os.path.dirname(path_n_suffix)}/Results_{os.path.basename(path_n_suffix)}_{set_type}.png'
     plt.savefig(f'{clas_plot_file}', dpi=300, bbox_inches='tight')
 
@@ -441,14 +447,16 @@
     axis_limit = max(outliers_data['train_scaled'], key=abs)
     if max(outliers_data['valid_scaled'], key=abs) > axis_limit:
         axis_limit = max(outliers_data['valid_scaled'], key=abs)
     if 'test_scaled' in outliers_data:
         if max(outliers_data['test_scaled'], key=abs) > axis_limit:
             axis_limit = max(outliers_data['test_scaled'], key=abs)
     axis_limit = axis_limit+0.5
+    if axis_limit < 2.5: # this fixes a problem when representing rectangles in graphs with low SDs
+        axis_limit = 2.5
     plt.ylim(-axis_limit, axis_limit)
     plt.xlim(-axis_limit, axis_limit)
 
     # plot rectangles in corners
     diff_tvalue = axis_limit - self.args.t_value
     Rectangle_top = mpatches.Rectangle(xy=(axis_limit, axis_limit), width=-diff_tvalue, height=-diff_tvalue, facecolor='grey', alpha=0.3)
     Rectangle_bottom = mpatches.Rectangle(xy=(-(axis_limit), -(axis_limit)), width=diff_tvalue, height=diff_tvalue, facecolor='grey', alpha=0.3)
```

### Comparing `robert-1.0.1/robert/robert.py` & `robert-1.0.2/robert/robert.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,55 +21,59 @@
 ###                                                                ###
 ######################################################################
 ######################################################################.
 
 
 import os
 from pathlib import Path
+import pandas as pd
 from robert.curate import curate
 from robert.generate import generate
 from robert.verify import verify
 from robert.predict import predict
 from robert.report import report
 from robert.aqme import aqme
-from robert.utils import command_line_args
+from robert.utils import (command_line_args,missing_inputs)
 
 
 def main():
     """
-    Main function of AQME, acts as the starting point when the program is run through a terminal
+    Main function of ROBERT, acts as the starting point when the program is run through a terminal
     """
 
     # load user-defined arguments from command line
     args = command_line_args()
     args.command_line = True
 
     # if no modules are called, the full workflow is activated
     full_workflow = False
     if not args.curate and not args.generate and not args.predict:
         if not args.cheers and not args.verify and not args.report:
             full_workflow = True
 
     # AQME
     if args.aqme:
+        # save the csv_name and y values from AQME workflows
+        args = missing_inputs(args,print_err=True)
+
         full_workflow = True
         aqme(
             csv_name=args.csv_name,
             varfile=args.varfile,
             y=args.y,
             command_line=args.command_line,
             destination=args.destination,
             qdescp_keywords=args.qdescp_keywords,
             csearch_keywords=args.csearch_keywords,
             discard=args.discard,
             ignore=args.ignore
         )
 
-        # set the path to the database created by AQME to continue in the full_workflow
-        args.csv_name = Path(os.path.dirname(args.csv_name)).joinpath(f'AQME-ROBERT_{os.path.basename(args.csv_name)}')
+        # adjust argument names after running AQME
+        args = set_aqme_args(args)
 
     # CURATE
     if args.curate or full_workflow:
         curate(
             varfile=args.varfile,
             command_line=args.command_line,
             destination=args.destination,
@@ -99,14 +103,16 @@
             discard=args.discard,
             ignore=args.ignore,
             train=args.train,
             split=args.split,
             model=args.model,
             type=args.type,
             seed=args.seed,
+            generate_acc=args.generate_acc,
+            filter_train=args.filter_train,
             epochs=args.epochs,
             error_type=args.error_type,
             custom_params=args.custom_params,
             pfi_epochs=args.pfi_epochs,
             pfi_threshold=args.pfi_threshold,
             pfi_filter=args.pfi_filter,
             pfi_max=args.pfi_max,
@@ -145,12 +151,33 @@
             command_line=args.command_line,
             destination=args.destination,
             report_modules=args.report_modules
         )
     
     # CHEERS
     if args.cheers:
-        print('o  Blimey! This module was designed to thank my mate ROBERT Paton, who was a mentor to me throughout my years at Colorado State University, and who introduced me to the field of cheminformatics.\n')
+        print('o  Blimey! This module was designed to thank ROBERT Paton, who was a mentor to me throughout my years at Colorado State University, and who introduced me to the field of cheminformatics. Cheers mate!\n')
+
+
+def set_aqme_args(args):
+    """
+    Changes arguments to couple AQME with ROBERT
+    """
+
+    # set the path to the database created by AQME to continue in the full_workflow
+    args.csv_name = Path(os.path.dirname(args.csv_name)).joinpath(f'AQME-ROBERT_{os.path.basename(args.csv_name)}')
+    aqme_df = pd.read_csv(args.csv_name)
+
+    # ignore the names and SMILES of the molecules
+    for column in aqme_df.columns:
+        if column.lower() in ['smiles','code_name'] and column not in args.ignore:
+            args.ignore.append(column)
+
+    # set the names for the outlier analysis
+    for column in aqme_df.columns:
+        if column.lower() == 'code_name' and args.names == '':
+            args.names = column
 
+    return args
 
 if __name__ == "__main__":
     main()
```

### Comparing `robert-1.0.1/robert/utils.py` & `robert-1.0.2/robert/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 import yaml
 import ast
 import shutil
 from pathlib import Path
 import pandas as pd
 import numpy as np
 from scipy import stats
-from sklearnex import patch_sklearn
-patch_sklearn(verbose=False)
+# for users with no intel architectures. This part has to be before the sklearn imports
+# try:
+#     from sklearnex import patch_sklearn
+#     patch_sklearn(verbose=False)
+# except (ModuleNotFoundError,ImportError):
+#     pass
+from pkg_resources import resource_filename
 from sklearn.metrics import mean_absolute_error, mean_squared_error
 from sklearn.metrics import matthews_corrcoef, accuracy_score, f1_score
 from robert.argument_parser import set_options, var_dict
 from sklearn.ensemble import (
     RandomForestRegressor,
     GradientBoostingRegressor,
     AdaBoostRegressor,
@@ -31,15 +36,15 @@
     VotingClassifier)
 from sklearn.gaussian_process import GaussianProcessRegressor, GaussianProcessClassifier
 from sklearn.neural_network import MLPRegressor, MLPClassifier
 from sklearn.linear_model import LinearRegression
 import warnings # this avoids warnings from sklearn
 warnings.filterwarnings("ignore")
 
-robert_version = "1.0.1"
+robert_version = "1.0.2"
 time_run = time.strftime("%Y/%m/%d %H:%M:%S", time.localtime())
 robert_ref = f"ROBERT v {robert_version}, Dalmau, D.; Alegre-Requena, J. V., 2023. https://github.com/jvalegre/robert"
 
 
 # load paramters from yaml file
 def load_from_yaml(self):
     """
@@ -48,15 +53,15 @@
     """
 
     txt_yaml = f"\no  Importing ROBERT parameters from {self.varfile}"
     error_yaml = False
     # Variables will be updated from YAML file
     try:
         if os.path.exists(self.varfile):
-            if os.path.splitext(self.varfile)[1] in [".yaml", ".yml", ".txt"]:
+            if os.path.basename(Path(self.varfile)).split('.')[1] in ["yaml", "yml", "txt"]:
                 with open(self.varfile, "r") as file:
                     try:
                         param_list = yaml.load(file, Loader=yaml.SafeLoader)
                     except (yaml.scanner.ScannerError,yaml.parser.ParserError):
                         txt_yaml = f'\nx  Error while reading {self.varfile}. Edit the yaml file and try again (i.e. use ":" instead of "=" to specify variables)'
                         error_yaml = True
         if not error_yaml:
@@ -135,14 +140,17 @@
             arg_name = arg.split("--")[1].strip()
         elif arg.find("-") > -1:
             arg_name = arg.split("-")[1].strip()
         if arg_name in bool_args:
             value = True
         if value == "None":
             value = None
+        if value == "False":
+            value = False
+
         if arg_name in ("h", "help"):
             print(f"o  ROBERT v {robert_version} is installed correctly! For more information about the available options, see the documentation in https://github.com/jvalegre/robert")
             sys.exit()
         else:
             # this "if" allows to use * to select multiple files in multiple OS
             if arg_name.lower() == 'files' and value.find('*') > -1:
                 kwargs[arg_name] = glob.glob(value)
@@ -209,42 +217,67 @@
 
             self.log = Logger(self.destination / logger_1, logger_2)
             self.log.write(f"ROBERT v {robert_version} {time_run} \nCitation: {robert_ref}\n")
 
             if self.command_line:
                 self.log.write(f"Command line used in ROBERT: robert {' '.join([str(elem) for elem in sys.argv[1:]])}\n")
 
+        elif robert_module.upper() == 'REPORT':
+            self.path_icons = Path(resource_filename("robert", "report"))
+
+        # # using or not the intelex accelerator might affect the results
+        # if robert_module.upper() in ['GENERATE','VERIFY','PREDICT']:
+        #     try:
+        #         from sklearnex import patch_sklearn
+        #         pass
+        #     except (ModuleNotFoundError,ImportError):
+        #         self.log.write(f"\nWARNING! The scikit-learn-intelex accelerator is not installed, the results might vary if it is installed and the execution times might become much longer (if available, use 'pip install scikit-learn-intelex')")
+
         if robert_module.upper() == 'CURATE':
             self.log.write(f"\no  Starting data curation with the CURATE module")
-
-            if str(self.corr_filter).upper() == 'FALSE':
-                self.corr_filter = False
             
             self.thres_x = float(self.thres_x)
             self.thres_y = float(self.thres_y)
             self.desc_thres = float(self.desc_thres)
 
         elif robert_module.upper() == 'GENERATE':
             self.log.write(f"\no  Starting generation of ML models with the GENERATE module")
-
-            if str(self.pfi_filter).upper() == 'FALSE':
-                self.pfi_filter = False
-
+            
             # Check if the folders exist and if they do, delete and replace them
             folder_names = [self.initial_dir.joinpath('GENERATE/Best_model/No_PFI'), self.initial_dir.joinpath('GENERATE/Raw_data/No_PFI')]
             if self.pfi_filter:
                 folder_names.append(self.initial_dir.joinpath('GENERATE/Best_model/PFI'))
                 folder_names.append(self.initial_dir.joinpath('GENERATE/Raw_data/PFI'))
             _ = create_folders(folder_names)
 
+            for i,val in enumerate(self.train):
+                self.train[i] = int(val)
+
             self.pfi_epochs = int(self.pfi_epochs)
             self.pfi_threshold = float(self.pfi_threshold)
             self.epochs = int(self.epochs)
             self.pfi_max = int(self.pfi_max)
 
+            # set seeds and epochs depending on precision
+            if len(self.seed) == 0:
+                if self.generate_acc == 'low':
+                    self.seed = [0,8,19]
+                elif self.generate_acc == 'mid':
+                    self.seed = [0,8,19,43,70,233]
+                elif self.generate_acc == 'high':
+                    self.seed = [0,8,19,43,70,233,1989,9999,20394,3948301]
+            
+            if self.epochs == 0:
+                if self.generate_acc == 'low':
+                    self.epochs = 20
+                elif self.generate_acc == 'mid':
+                    self.epochs = 40
+                elif self.generate_acc == 'high':
+                    self.epochs = 100
+        
             if self.type.lower() == 'clas':
                 if self.model == ['RF','GB','NN','MVL']:
                     self.model = ['RF','GB','NN','AdaB']
             
             models_gen = [] # use capital letters in all the models
             for model_type in self.model:
                 models_gen.append(model_type.upper())
@@ -310,37 +343,57 @@
     if os.path.exists(self.destination):
         shutil.rmtree(self.destination)
     self.destination.mkdir(exist_ok=True, parents=True)
 
     return self
 
 
+def missing_inputs(self,print_err=False):
+    """
+    Gives the option to input missing variables in the terminal
+    """
+
+    if self.csv_name == '':
+        if print_err:
+            print('\nx  Specify the name of your CSV file with the csv_name option!')
+        else:
+            self.log.write('\nx  Specify the name of your CSV file with the csv_name option!')
+        self.csv_name = input('Enter the name of your CSV file: ')
+        if not print_err:
+            self.log.write(f"   -  csv_name option set to {self.csv_name} by the user")
+
+    if self.y == '':
+        if print_err:
+            print(f"\nx  Specify a y value (column name) with the y option! (i.e. y='solubility')")
+        else:
+            self.log.write(f"\nx  Specify a y value (column name) with the y option! (i.e. y='solubility')")
+        self.y = input('Enter the column with y values: ')
+        if not print_err:
+            self.log.write(f"   -  y option set to {self.y} by the user")
+
+    return self
+
 def sanity_checks(self, type_checks, module, columns_csv):
     """
     Check that different variables are set correctly
     """
 
     curate_valid = True
     if type_checks == 'initial' and module.lower() not in ['verify','predict']:
-        if self.csv_name == '':
-            self.log.write('\nx  Specify the name of your CSV file with the csv_name option!')
-            curate_valid = False
+
+        self = missing_inputs(self)
 
         path_csv = ''
         if os.getcwd() in f"{self.csv_name}":
             path_csv = self.csv_name
         elif self.csv_name != '':
             path_csv = f"{Path(os.getcwd()).joinpath(self.csv_name)}"
         if not os.path.exists(path_csv) or self.csv_name == '':
             self.log.write(f'\nx  The path of your CSV file doesn\'t exist! You specified: {self.csv_name}')
             curate_valid = False
-        
-        if self.y == '':
-            self.log.write(f"\nx  Specify a y value (column name) with the y option! (i.e. y='solubility')")
-            curate_valid = False
 
         if module.lower() == 'curate':
             if self.categorical.lower() not in ['onehot','numbers']:
                 self.log.write(f"\nx  The categorical option used is not valid! Options: 'onehot', 'numbers'")
                 curate_valid = False
 
             elif float(self.thres_x) > 1 or float(self.thres_x) < 0:
@@ -352,14 +405,18 @@
                 curate_valid = False
         
         elif module.lower() == 'generate':
             if self.split.lower() not in ['kn','rnd']:
                 self.log.write(f"\nx  The split option used is not valid! Options: 'KN', 'RND'")
                 curate_valid = False
 
+            if self.generate_acc.lower() not in ['low','mid','high']:
+                self.log.write(f"\nx  The generate_acc option used is not valid! Options: 'low', 'mid', 'high'")
+                curate_valid = False
+
             for model_type in self.model:
                 if model_type.upper() not in ['RF','MVL','GB','GP','ADAB','NN','VR'] or len(self.model) == 0:
                     self.log.write(f"\nx  The model option used is not valid! Options: 'RF', 'MVL', 'GB', 'ADAB', 'NN', 'VR'")
                     curate_valid = False
                 if model_type.upper() == 'MVL' and self.type.lower() == 'clas':
                     self.log.write(f"\nx  Multivariate linear models (MVL in the model_type option) are not compatible with classificaton!")                 
                     curate_valid = False
@@ -541,15 +598,15 @@
                                 min_samples_split=params['min_samples_split'],
                                 min_samples_leaf=params['min_samples_leaf'],
                                 min_weight_fraction_leaf=params['min_weight_fraction_leaf'],
                                 oob_score=params['oob_score'],
                                 ccp_alpha=params['ccp_alpha'],
                                 max_samples=params['max_samples'],
                                 random_state=params['seed'],
-                                n_jobs=-1)
+                                n_jobs=None)
 
         if params['model'].upper() == 'VR':
             r1 = loaded_model
 
     if params['model'].upper() in ['GB','VR']:    
         loaded_model = GradientBoostingRegressor(max_depth=params['max_depth'], 
                                 max_features=params['max_features'],
@@ -593,15 +650,15 @@
         loaded_model = GaussianProcessRegressor(n_restarts_optimizer=params['n_restarts_optimizer'],
                                 random_state=params['seed'])
 
     if params['model'].upper() == 'VR':
         loaded_model = VotingRegressor([('rf', r1), ('gb', r2), ('nn', r3)])
 
     if params['model'].upper() == 'MVL':
-        loaded_model = LinearRegression(n_jobs=-1)
+        loaded_model = LinearRegression(n_jobs=None)
 
     return loaded_model
 
 
 def load_model_clas(params):
 
     if params['model'].upper() in ['RF','VR']:     
@@ -611,15 +668,15 @@
                                 min_samples_split=params['min_samples_split'],
                                 min_samples_leaf=params['min_samples_leaf'],
                                 min_weight_fraction_leaf=params['min_weight_fraction_leaf'],
                                 oob_score=params['oob_score'],
                                 ccp_alpha=params['ccp_alpha'],
                                 max_samples=params['max_samples'],
                                 random_state=params['seed'],
-                                n_jobs=-1)
+                                n_jobs=None)
 
         if params['model'].upper() == 'VR':
             r1 = loaded_model
 
     if params['model'].upper() in ['GB','VR']:    
         loaded_model = GradientBoostingClassifier(max_depth=params['max_depth'], 
                                 max_features=params['max_features'],
@@ -658,15 +715,15 @@
 
         if params['model'].upper() == 'VR':
             r3 = loaded_model
 
     if params['model'].upper() == 'GP':
         loaded_model = GaussianProcessClassifier(n_restarts_optimizer=params['n_restarts_optimizer'],
                                 random_state=params['seed'],
-                                n_jobs=-1)
+                                n_jobs=None)
 
     if params['model'].upper() == 'VR':
         loaded_model = VotingClassifier([('rf', r1), ('gb', r2), ('nn', r3)])
 
     return loaded_model
 
 
@@ -814,14 +871,16 @@
         self.args.log.write(f"\nx  The folder with the model and database ({path_db}) does not exist! Did you use the destination=PATH option in the other modules?")
         sys.exit()
 
     return Xy_data_df, Xy_path, params_df, params_path, suffix, suffix_title
 
 
 def load_print(self,params_name,suffix,params_df,point_count):
+    if '.csv' in params_name:
+        params_name = params_name.split('.csv')[0]
     txt_load = f'\no  ML model {params_name} {suffix} and Xy database were loaded, including:'
     txt_load += f'\n   - Target value: {params_df["y"][0]}'
     txt_load += f'\n   - Model: {params_df["model"][0]}'
     txt_load += f'\n   - Descriptors: {params_df["X_descriptors"][0]}'
     txt_load += f'\n   - Training points: {point_count["train"]}'
     txt_load += f'\n   - Validation points: {point_count["valid"]}'
     if 'test' in point_count:
@@ -829,8 +888,15 @@
     self.args.log.write(txt_load)
 
 
 def pd_to_dict(PFI_df):
     PFI_df_dict = {}
     for column in PFI_df.columns:
         PFI_df_dict[column] = PFI_df[column][0]
-    return PFI_df_dict
+    return PFI_df_dict
+
+
+def print_pfi(self,params_dir):
+    if 'No_PFI' in params_dir:
+        self.args.log.write('\n\n------- Starting model with all variables (No PFI) -------')
+    else:
+        self.args.log.write('\n\n------- Starting model with PFI filter (only important descriptors used) -------')
```

### Comparing `robert-1.0.1/robert/verify.py` & `robert-1.0.2/robert/verify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 """
 Parameters
 ----------
 
-General
-+++++++
+    destination : str, default=None,
+        Directory to create the output file(s).
+    varfile : str, default=None
+        Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
+    params_dir : str, default=''
+        Folder containing the database and parameters of the ML model to analyze.
+    thres_test : float, default=0.2,
+        Threshold used to determine if a test pasess. It is determined in % units of diference between
+        the R2 (MCC in classificators) of the model and the test (i.e., 0.2 = 20% difference with the 
+        original value). Test passes if:
+        1. y-mean and y-shuffle tests: decreases more than X% (from original R2, regressors, or MCC, 
+        classificators) or the error is greated than X% (from original MAE and RMSE for regressors)
+        2. One-hot encoding test: decreases more than X%
+        3. K-fold cross validation: decreases less than X%
+    kfold : int, default=5,
+        The training set is split into a K number of folds in the cross-validation test (i.e. 5-fold CV).
 
-     destination : str, default=None,
-         Directory to create the output file(s).
-     varfile : str, default=None
-         Option to parse the variables using a yaml file (specify the filename, i.e. varfile=FILE.yaml).  
-     params_dir : str, default=''
-         Folder containing the database and parameters of the ML model to analyze.
-     thres_test : float, default=0.2,
-         Threshold used to determine if a test pasess. It is determined in % units of diference between
-         the R2 (MCC in classificators) of the model and the test (i.e., 0.2 = 20% difference with the 
-         original value). Test passes if:
-            1. y-mean and y-shuffle tests: decreases more than X% (from original R2, regressors, or MCC, 
-            classificators) or the error is greated than X% (from original MAE and RMSE for regressors)
-            2. One-hot encoding test: decreases more than X%
-            3. K-fold cross validation: decreases less than X%
-     kfold : int, default=5,
-         The training set is split into a K number of folds in the cross-validation test (i.e. 5-fold CV).
 """
 #####################################################.
 #        This file stores the VERIFY class          #
 #           used for ML model analysis              #
 #####################################################.
 
 import os
 import time
 from matplotlib import pyplot as plt
 import numpy as np
 from pathlib import Path
 import seaborn as sb
 from statistics import mode
+# for users with no intel architectures. This part has to be before the sklearn imports
+# try:
+#     from sklearnex import patch_sklearn
+#     patch_sklearn(verbose=False)
+# except (ModuleNotFoundError,ImportError):
+    # pass
 from sklearn.model_selection import cross_val_score
 from robert.utils import (load_variables,
     load_db_n_params,
     load_model,
     pd_to_dict,
     load_n_predict,
     finish_print,
-    get_prediction_results
+    get_prediction_results,
+    print_pfi
 )
 
 
 class verify:
     """
     Class containing all the functions from the VERIFY module.
 
@@ -67,14 +72,16 @@
             params_dirs = [f'{self.args.params_dir}/No_PFI',f'{self.args.params_dir}/PFI']
         else:
             params_dirs = [self.args.params_dir]
 
         for params_dir in params_dirs:
             if os.path.exists(params_dir):
 
+                _ = print_pfi(self,params_dir)
+
                 # load and ML model parameters, and add standardized descriptors
                 Xy_data, params_df, params_path, suffix_title = load_db_n_params(self,params_dir,"verify",True)
                 
                 # set the parameters for each ML model of the hyperopt optimization
                 params_dict = pd_to_dict(params_df) # (using a dict to keep the same format of load_model)
 
                 # this dictionary will keep the results of the tests
```

### Comparing `robert-1.0.1/robert.egg-info/PKG-INFO` & `robert-1.0.2/robert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robert
-Version: 1.0.1
+Version: 1.0.2
 Summary: Refiner and Optimizer of a Bunch of Existing Regression Tools
 Home-page: https://github.com/jvalegre/robert
-Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.1.tar.gz
+Download-URL: https://github.com/jvalegre/robert/archive/refs/tags/1.0.2.tar.gz
 Author: Juan V. Alegre Requena, David Dalmau
 Author-email: jv.alegre@csic.es
 License: MIT
 Keywords: workflows,machine learning,cheminformatics,data curation,prediction,automated
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `robert-1.0.1/robert.egg-info/SOURCES.txt` & `robert-1.0.2/robert.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,12 +23,18 @@
 robert/model_params/ADAB_params.yaml
 robert/model_params/GB_params.yaml
 robert/model_params/GP_params.yaml
 robert/model_params/MVL_params.yaml
 robert/model_params/NN_params.yaml
 robert/model_params/RF_params.yaml
 robert/model_params/VR_params.yaml
+robert/report/AQME.png
+robert/report/CURATE.png
+robert/report/GENERATE.png
+robert/report/PREDICT.png
+robert/report/Robert_logo.jpg
+robert/report/VERIFY.png
 tests/test_1curate.py
 tests/test_2generate.py
 tests/test_3verify.py
 tests/test_4predict.py
 tests/test_5aqme_n_full.py
```

### Comparing `robert-1.0.1/setup.py` & `robert-1.0.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
-version="1.0.1"
+version="1.0.2"
 setup(
     name="robert",
     packages=find_packages(exclude=["tests"]),
-    package_data={"robert": ["model_params/*"]},
+    package_data={"robert": ["model_params/*","report/*"]},
     version=version,
     license="MIT",
     description="Refiner and Optimizer of a Bunch of Existing Regression Tools",
     long_description="Documentation in Read The Docs: https://robert.readthedocs.io",
     long_description_content_type="text/markdown",
     author="Juan V. Alegre Requena, David Dalmau",
     author_email="jv.alegre@csic.es",
@@ -29,23 +29,22 @@
         "Programming Language :: Python :: 3.7",  # Specify which python versions you want to support
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     install_requires=[
         "PyYAML",
-        "pandas>=2.0",
+        "pandas>=2.0.3,<2.1",
         "progress",
-        "numpy>=1.23,<1.24",
-        "matplotlib>=3.7.1",
+        "numpy>=1.24,<1.25",
+        "matplotlib>=3.7,<3.8",
         "seaborn",
         "scipy",
-        "scikit-learn>=1.2,<1.3",
+        "scikit-learn==1.3.0", # fixed to make ROBERT reproducible when using the same version
         "hyperopt",
-        "numba",
-        "shap",
-        "scikit-learn-intelex",
-        # requires also "conda install -c conda-forge gtk3 glib weasyprint" for report.py
+        "numba>=0.57,<0.58",
+        "shap>=0.42,<0.43",
+        # requires also "conda install -c conda-forge gtk3 glib weasyprint pango" for report.py
     ],
     python_requires=">=3.0",
     include_package_data=True,
 )
```

### Comparing `robert-1.0.1/tests/test_1curate.py` & `robert-1.0.2/tests/test_1curate.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/tests/test_2generate.py` & `robert-1.0.2/tests/test_2generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             cmd_robert = cmd_robert + ["--pfi_max", "2"]
         elif test_job == 'reduced_random':
             cmd_robert = cmd_robert + ["--split", "rnd"]
         elif test_job == 'reduced_clas':
             cmd_robert = cmd_robert + ["--type", "clas"]
     else: # needed to define the variables, change if default options change
         model_list = ['RF','GB','NN','MVL']
-        train_list = [60,70,80,90]
+        train_list = [60,70,80]
     
     cmd_robert = cmd_robert + [
         "--model", f"{model_list}",
         "--train", f"{train_list}"]
 
     subprocess.run(cmd_robert)
 
@@ -135,17 +135,17 @@
             if folder == 'No_PFI':
                 if test_job != 'reduced_clas':
                     desc_list = ['x2', 'x5', 'x6', 'x7', 'x8', 'x9', 'x10', 'x11', 'Csub-Csub', 'Csub-H', 'Csub-O', 'H-O']
                 else:
                     desc_list = ['x1', 'x2', 'x3', 'x5', 'x6', 'x7', 'x8', 'x9', 'x10']
             elif folder == 'PFI':
                 if test_job == 'reduced':
-                    desc_list = ['x6', 'x7', 'x10']
+                    desc_list = ['x6', 'x7', 'x9', 'x10']
                     assert db_best['Set'][0] == 'Training'
-                    assert db_best['Set'][1] == 'Training'
+                    assert db_best['Set'][1] == 'Validation'
                     assert db_best['Set'][2] == 'Training'
                     assert db_best['Set'][3] == 'Validation'
                 elif test_job =='reduced_PFImax':
                     desc_list = ['x6', 'x7']
                 elif test_job == 'reduced_random':
                     desc_list = ['x6', 'x7', 'x10']
                     assert db_best['Set'][0] == 'Validation'
```

### Comparing `robert-1.0.1/tests/test_3verify.py` & `robert-1.0.2/tests/test_3verify.py`

 * *Files identical despite different names*

### Comparing `robert-1.0.1/tests/test_4predict.py` & `robert-1.0.2/tests/test_4predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,22 +94,22 @@
                 assert 'Points Train:Validation = 29:8' in outlines[i+1]
             else:
                 assert 'Points Train:Validation:Test = 29:8:9' in outlines[i+1]
         elif 'x  There are missing descriptors' in line:
             categor_test = True
         if 'Outlier values saved in' in line and 'No_PFI' in line:
             if test_job == "names":
-                assert '-  19 (' in outlines[i+2]
+                assert '-  21 (' in outlines[i+2]
                 break
             elif test_job != "clas":
                 assert 'x  No names option' in outlines[i+1]             
                 if test_job == "t_value":
                     assert 'Train: 0 outliers' in outlines[i+2]
                 else:
-                    assert 'Train: 2 outliers' in outlines[i+2]
+                    assert 'Train: 1 outliers' in outlines[i+2]
                 if test_job == "t_value":
                     assert 'Validation: 0 outliers' in outlines[i+3]
                 else:
                     assert 'Validation: 0 outliers' in outlines[i+3]
                 if test_job == "csv_test":
                     assert 'Test: 0 outliers' in outlines[i+4]
                 break
```

### Comparing `robert-1.0.1/tests/test_5aqme_n_full.py` & `robert-1.0.2/tests/test_5aqme_n_full.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,41 +51,44 @@
     cmd_robert = [
         "python",
         "-m",
         "robert",
         "--csv_name", csv_var,
         '--y', y_var,
         "--ignore", ignore_var,
-        "--epochs", "5"
+        "--epochs", "5",
+        "--seed", "[0]",
+        "--model", "['GB']",
+        "--train", "[60]",
+        "--pfi_epochs", "1"
     ]
 
     if test_job == 'full_workflow':
         cmd_robert = cmd_robert + ["--discard", "['xtest']"]
 
     elif test_job == 'aqme':
         cmd_robert = cmd_robert + ["--aqme","--csearch_keywords", "--sample 2", 
-                    "--qdescp_keywords", "--qdescp_atoms ['C']", "--model", "['RF']",
-                    "--train", "[60]"]
+                    "--qdescp_keywords", "--qdescp_atoms ['C']"]
 
     subprocess.run(cmd_robert)
 
     # check that all the plots, CSV and DAT files are created
+    # find ROBERT_report.pdf
+    assert os.path.exists(f'{path_main}/ROBERT_report.pdf')
+    
     # CURATE folder
     assert len(glob.glob(f'{path_main}/CURATE/*.png')) == 1
     assert len(glob.glob(f'{path_main}/CURATE/*.dat')) == 1
     assert len(glob.glob(f'{path_main}/CURATE/*.csv')) == 2
 
     # GENERATE folder
     folders_gen = ['No_PFI','PFI']
     for folder in folders_gen:
         csv_amount = glob.glob(f'{path_main}/GENERATE/Raw_data/{folder}/*.csv')
-        if test_job == 'aqme':
-            assert len(csv_amount) == 2
-        else:
-            assert len(csv_amount) == 32
+        assert len(csv_amount) == 2
         best_amount = glob.glob(f'{path_main}/GENERATE/Best_model/{folder}/*.csv')
         assert len(best_amount) == 2
 
     # VERIFY folder
     assert len(glob.glob(f'{path_main}/VERIFY/*.png')) == 2
     assert len(glob.glob(f'{path_main}/VERIFY/*.dat')) == 3
```

