# Comparing `tmp/sluurp-0.2.3.tar.gz` & `tmp/sluurp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sluurp-0.2.3.tar", last modified: Tue Jun 27 09:03:13 2023, max compression
+gzip compressed data, was "sluurp-0.2.4.tar", last modified: Tue Jul 18 08:32:33 2023, max compression
```

## Comparing `sluurp-0.2.3.tar` & `sluurp-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/
--rw-r--r--   0 payno     (1001) payno     (1001)     1102 2023-06-27 08:38:21.000000 sluurp-0.2.3/LICENSE.md
--rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-06-27 09:03:13.730248 sluurp-0.2.3/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)       82 2023-06-27 08:38:21.000000 sluurp-0.2.3/README.md
--rw-r--r--   0 payno     (1001) payno     (1001)      107 2023-06-27 08:38:21.000000 sluurp-0.2.3/pyproject.toml
--rw-r--r--   0 payno     (1001) payno     (1001)      874 2023-06-27 09:03:13.730248 sluurp-0.2.3/setup.cfg
--rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-27 08:38:21.000000 sluurp-0.2.3/setup.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.726248 sluurp-0.2.3/src/
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/src/sluurp/
--rw-r--r--   0 payno     (1001) payno     (1001)       65 2023-06-27 09:02:46.000000 sluurp-0.2.3/src/sluurp/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1200 2023-06-27 08:38:21.000000 sluurp-0.2.3/src/sluurp/executor.py
--rw-r--r--   0 payno     (1001) payno     (1001)    12865 2023-06-27 09:02:09.000000 sluurp-0.2.3/src/sluurp/job.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1509 2023-06-27 08:38:21.000000 sluurp-0.2.3/src/sluurp/utils.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-06-27 09:03:13.730248 sluurp-0.2.3/src/sluurp.egg-info/
--rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      307 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       63 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/requires.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        7 2023-06-27 09:03:13.000000 sluurp-0.2.3/src/sluurp.egg-info/top_level.txt
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-18 08:32:33.666896 sluurp-0.2.4/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1102 2023-06-27 08:38:21.000000 sluurp-0.2.4/LICENSE.md
+-rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-07-18 08:32:33.666896 sluurp-0.2.4/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)       82 2023-06-27 08:38:21.000000 sluurp-0.2.4/README.md
+-rw-r--r--   0 payno     (1001) payno     (1001)      107 2023-06-27 08:38:21.000000 sluurp-0.2.4/pyproject.toml
+-rw-r--r--   0 payno     (1001) payno     (1001)      874 2023-07-18 08:32:33.666896 sluurp-0.2.4/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-27 08:38:21.000000 sluurp-0.2.4/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-18 08:32:33.662896 sluurp-0.2.4/src/
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-18 08:32:33.662896 sluurp-0.2.4/src/sluurp/
+-rw-r--r--   0 payno     (1001) payno     (1001)       65 2023-07-18 08:30:31.000000 sluurp-0.2.4/src/sluurp/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1200 2023-06-27 08:38:21.000000 sluurp-0.2.4/src/sluurp/executor.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12863 2023-07-18 08:30:03.000000 sluurp-0.2.4/src/sluurp/job.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1509 2023-06-27 08:38:21.000000 sluurp-0.2.4/src/sluurp/utils.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-18 08:32:33.666896 sluurp-0.2.4/src/sluurp.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)      784 2023-07-18 08:32:33.000000 sluurp-0.2.4/src/sluurp.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      307 2023-07-18 08:32:33.000000 sluurp-0.2.4/src/sluurp.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-07-18 08:32:33.000000 sluurp-0.2.4/src/sluurp.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       63 2023-07-18 08:32:33.000000 sluurp-0.2.4/src/sluurp.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        7 2023-07-18 08:32:33.000000 sluurp-0.2.4/src/sluurp.egg-info/top_level.txt
```

### Comparing `sluurp-0.2.3/LICENSE.md` & `sluurp-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.3/PKG-INFO` & `sluurp-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluurp
-Version: 0.2.3
+Version: 0.2.4
 Summary: API to submit shell script through slurm SBATCH
 Home-page: https://gitlab.esrf.fr/tomotools/sluurp
 Author: ESRF
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/tomotools/sluurp
 Project-URL: Documentation, https://tomotools.gitlab-pages.esrf.fr/sluurp/
```

### Comparing `sluurp-0.2.3/setup.cfg` & `sluurp-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.3/src/sluurp/executor.py` & `sluurp-0.2.4/src/sluurp/executor.py`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.3/src/sluurp/job.py` & `sluurp-0.2.4/src/sluurp/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
             elif key == "job_name":
                 slurm_ressources.append(f"#SBATCH -J '{value}'")
             elif key == "walltime":
                 slurm_ressources.append(f"#SBATCH -t {value}")
             elif key == "python_venv":
                 preprocessing.append(f"source {value}")
             else:
-                raise KeyError(f"Unknow slurm configuration key: {key}")
+                _logger.info(f"Unknow slurm configuration key: {key}")
         return tuple(slurm_ressources), tuple(preprocessing)
 
 
 def get_job_status(job_id):
     if job_id is None:
         return "error"
     elif not has_scontrol_available():
```

### Comparing `sluurp-0.2.3/src/sluurp/utils.py` & `sluurp-0.2.4/src/sluurp/utils.py`

 * *Files identical despite different names*

### Comparing `sluurp-0.2.3/src/sluurp.egg-info/PKG-INFO` & `sluurp-0.2.4/src/sluurp.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sluurp
-Version: 0.2.3
+Version: 0.2.4
 Summary: API to submit shell script through slurm SBATCH
 Home-page: https://gitlab.esrf.fr/tomotools/sluurp
 Author: ESRF
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/tomotools/sluurp
 Project-URL: Documentation, https://tomotools.gitlab-pages.esrf.fr/sluurp/
```

