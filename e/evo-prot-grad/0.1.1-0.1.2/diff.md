# Comparing `tmp/evo_prot_grad-0.1.1.tar.gz` & `tmp/evo_prot_grad-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_prot_grad-0.1.1.tar", last modified: Tue Jul 18 03:55:12 2023, max compression
+gzip compressed data, was "evo_prot_grad-0.1.2.tar", last modified: Tue Jul 18 04:26:27 2023, max compression
```

## Comparing `evo_prot_grad-0.1.1.tar` & `evo_prot_grad-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.680956 evo_prot_grad-0.1.1/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 03:55:12.680670 evo_prot_grad-0.1.1/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4278 2023-07-18 03:07:17.000000 evo_prot_grad-0.1.1/README.md
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.670810 evo_prot_grad-0.1.1/evo_prot_grad/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.1/evo_prot_grad/__init__.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.675542 evo_prot_grad-0.1.1/evo_prot_grad/common/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.1/evo_prot_grad/common/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.1/evo_prot_grad/common/embeddings.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    14982 2023-07-18 03:43:54.000000 evo_prot_grad-0.1.1/evo_prot_grad/common/sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2751 2023-07-17 13:44:18.000000 evo_prot_grad-0.1.1/evo_prot_grad/common/tokenizers.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2636 2023-07-06 22:37:51.000000 evo_prot_grad-0.1.1/evo_prot_grad/common/utils.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.678063 evo_prot_grad-0.1.1/evo_prot_grad/experts/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10623 2023-07-17 14:44:58.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/base_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2986 2023-07-17 14:45:12.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/bert_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3015 2023-07-17 13:49:07.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/causallm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2944 2023-07-17 13:48:59.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/esm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3292 2023-07-17 14:45:29.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/evcouplings_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.1/evo_prot_grad/experts/onehot_downstream_regression_expert.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.679143 evo_prot_grad-0.1.1/evo_prot_grad/models/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.1/evo_prot_grad/models/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.1/evo_prot_grad/models/downstream_cnn.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3221 2023-07-17 14:00:59.000000 evo_prot_grad-0.1.1/evo_prot_grad/models/potts.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.673703 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 03:55:12.000000 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-18 03:55:12.000000 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/SOURCES.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-18 03:55:12.000000 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/dependency_links.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       81 2023-07-18 03:55:12.000000 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/requires.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-18 03:55:12.000000 evo_prot_grad-0.1.1/evo_prot_grad.egg-info/top_level.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-18 03:55:12.681057 evo_prot_grad-0.1.1/setup.cfg
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-18 02:53:11.000000 evo_prot_grad-0.1.1/setup.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 03:55:12.680234 evo_prot_grad-0.1.1/test/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.1/test/test_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5099 2023-07-06 23:52:27.000000 evo_prot_grad-0.1.1/test/test_sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.1/test/test_utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.020910 evo_prot_grad-0.1.2/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 04:26:27.020617 evo_prot_grad-0.1.2/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4278 2023-07-18 03:07:17.000000 evo_prot_grad-0.1.2/README.md
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.010586 evo_prot_grad-0.1.2/evo_prot_grad/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.2/evo_prot_grad/__init__.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.015182 evo_prot_grad-0.1.2/evo_prot_grad/common/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/embeddings.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    14982 2023-07-18 03:43:54.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2751 2023-07-17 13:44:18.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/tokenizers.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2636 2023-07-06 22:37:51.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.017848 evo_prot_grad-0.1.2/evo_prot_grad/experts/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10623 2023-07-17 14:44:58.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/base_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2986 2023-07-17 14:45:12.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/bert_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3015 2023-07-17 13:49:07.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/causallm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2944 2023-07-17 13:48:59.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/esm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3292 2023-07-17 14:45:29.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/evcouplings_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/onehot_downstream_regression_expert.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.018995 evo_prot_grad-0.1.2/evo_prot_grad/models/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/downstream_cnn.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    11712 2023-07-18 04:21:56.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/potts.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.012778 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/SOURCES.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/dependency_links.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       28 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/requires.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/top_level.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-18 04:26:27.021018 evo_prot_grad-0.1.2/setup.cfg
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-18 04:25:50.000000 evo_prot_grad-0.1.2/setup.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.020137 evo_prot_grad-0.1.2/test/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.2/test/test_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5099 2023-07-06 23:52:27.000000 evo_prot_grad-0.1.2/test/test_sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.2/test/test_utils.py
```

### Comparing `evo_prot_grad-0.1.1/PKG-INFO` & `evo_prot_grad-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo_prot_grad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evo_prot_grad-0.1.1/README.md` & `evo_prot_grad-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/__init__.py` & `evo_prot_grad-0.1.2/evo_prot_grad/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/common/embeddings.py` & `evo_prot_grad-0.1.2/evo_prot_grad/common/embeddings.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/common/sampler.py` & `evo_prot_grad-0.1.2/evo_prot_grad/common/sampler.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/common/tokenizers.py` & `evo_prot_grad-0.1.2/evo_prot_grad/common/tokenizers.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/common/utils.py` & `evo_prot_grad-0.1.2/evo_prot_grad/common/utils.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/base_experts.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/base_experts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/bert_expert.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/bert_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/causallm_expert.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/causallm_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/esm_expert.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/esm_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/evcouplings_expert.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/evcouplings_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/experts/onehot_downstream_regression_expert.py` & `evo_prot_grad-0.1.2/evo_prot_grad/experts/onehot_downstream_regression_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad/models/downstream_cnn.py` & `evo_prot_grad-0.1.2/evo_prot_grad/models/downstream_cnn.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad.egg-info/PKG-INFO` & `evo_prot_grad-0.1.2/evo_prot_grad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-prot-grad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `evo_prot_grad-0.1.1/evo_prot_grad.egg-info/SOURCES.txt` & `evo_prot_grad-0.1.2/evo_prot_grad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/setup.py` & `evo_prot_grad-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(name='evo_prot_grad',
-      version='0.1.1',
+      version='0.1.2',
       description='Directed evolution of proteins with fast gradient-based discrete MCMC.',
       author='Patrick Emami',
       author_email='Patrick.Emami@nrel.gov',
       url='https://github.nrel.gov/NREL/EvoProtGrad/',
       python_requires='>=3.8',
       install_requires=requirements,
       long_description=readme,
```

### Comparing `evo_prot_grad-0.1.1/test/test_experts.py` & `evo_prot_grad-0.1.2/test/test_experts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/test/test_sampler.py` & `evo_prot_grad-0.1.2/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.1/test/test_utils.py` & `evo_prot_grad-0.1.2/test/test_utils.py`

 * *Files identical despite different names*

