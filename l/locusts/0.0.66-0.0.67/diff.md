# Comparing `tmp/locusts-0.0.66.tar.gz` & `tmp/locusts-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/TMB-CSB/Sarti/Work/locusts_pkg/dist/.tmp-zqiglycz/locusts-0.0.66.tar", last modified: Tue Jul 18 13:07:31 2023, max compression
+gzip compressed data, was "/data/TMB-CSB/Sarti/Work/locusts_pkg/dist/.tmp-5clyrs3p/locusts-0.0.67.tar", last modified: Tue Jul 18 13:31:06 2023, max compression
```

## Comparing `locusts-0.0.66.tar` & `locusts-0.0.67.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     1074 2020-10-04 13:43:43.000000 locusts-0.0.66/LICENSE
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      140 2020-11-24 18:17:40.000000 locusts-0.0.66/MANIFEST.in
--rw-r--r--   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:07:31.000000 locusts-0.0.66/PKG-INFO
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     6034 2020-10-17 23:43:16.000000 locusts-0.0.66/README.md
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      104 2021-02-08 19:14:59.000000 locusts-0.0.66/pyproject.toml
--rw-r--r--   0 sartie   (200184947) sartie   (200184947)       38 2023-07-18 13:07:31.000000 locusts-0.0.66/setup.cfg
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     2106 2020-09-11 14:54:56.000000 locusts-0.0.66/setup.py
-drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/
-drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)       23 2023-07-18 13:07:11.000000 locusts-0.0.66/src/locusts/__init__.py
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      158 2023-03-15 16:41:53.000000 locusts-0.0.66/src/locusts/data_transfer_protocol.sh
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     7934 2021-04-22 09:30:56.000000 locusts-0.0.66/src/locusts/environment.py
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)     2504 2021-05-03 22:40:39.000000 locusts-0.0.66/src/locusts/inner_template_manager.txt
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)    55729 2023-03-01 15:34:55.000000 locusts-0.0.66/src/locusts/manager.py
--rwxr-x---   0 sartie   (200184947) sartie   (200184947)      730 2021-06-05 15:50:01.000000 locusts-0.0.66/src/locusts/outer_template_manager.txt
--rw-rw----   0 sartie   (200184947) sartie   (200184947)     5931 2022-08-19 17:56:29.000000 locusts-0.0.66/src/locusts/support.py
--rw-r-----   0 sartie   (200184947) sartie   (200184947)    11287 2022-10-15 09:46:32.000000 locusts-0.0.66/src/locusts/swarm.py
-drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/
--rw-r-----   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/PKG-INFO
--rw-r-----   0 sartie   (200184947) sartie   (200184947)      427 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/SOURCES.txt
--rw-r-----   0 sartie   (200184947) sartie   (200184947)        1 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/dependency_links.txt
--rw-r-----   0 sartie   (200184947) sartie   (200184947)        8 2023-07-18 13:07:31.000000 locusts-0.0.66/src/locusts.egg-info/top_level.txt
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:31:06.000000 locusts-0.0.67/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     1074 2020-10-04 13:43:43.000000 locusts-0.0.67/LICENSE
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      140 2020-11-24 18:17:40.000000 locusts-0.0.67/MANIFEST.in
+-rw-r--r--   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:31:06.000000 locusts-0.0.67/PKG-INFO
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     6034 2020-10-17 23:43:16.000000 locusts-0.0.67/README.md
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      104 2021-02-08 19:14:59.000000 locusts-0.0.67/pyproject.toml
+-rw-r--r--   0 sartie   (200184947) sartie   (200184947)       38 2023-07-18 13:31:06.000000 locusts-0.0.67/setup.cfg
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     2106 2020-09-11 14:54:56.000000 locusts-0.0.67/setup.py
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:31:06.000000 locusts-0.0.67/src/
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)       23 2023-07-18 13:30:50.000000 locusts-0.0.67/src/locusts/__init__.py
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      158 2023-03-15 16:41:53.000000 locusts-0.0.67/src/locusts/data_transfer_protocol.sh
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     7934 2021-04-22 09:30:56.000000 locusts-0.0.67/src/locusts/environment.py
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)     2504 2021-05-03 22:40:39.000000 locusts-0.0.67/src/locusts/inner_template_manager.txt
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)    55729 2023-07-18 13:30:18.000000 locusts-0.0.67/src/locusts/manager.py
+-rwxr-x---   0 sartie   (200184947) sartie   (200184947)      730 2021-06-05 15:50:01.000000 locusts-0.0.67/src/locusts/outer_template_manager.txt
+-rw-rw----   0 sartie   (200184947) sartie   (200184947)     5931 2022-08-19 17:56:29.000000 locusts-0.0.67/src/locusts/support.py
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)    11287 2022-10-15 09:46:32.000000 locusts-0.0.67/src/locusts/swarm.py
+drwxr-xr-x   0 sartie   (200184947) sartie   (200184947)        0 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts.egg-info/
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)     7250 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts.egg-info/PKG-INFO
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)      427 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts.egg-info/SOURCES.txt
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)        1 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts.egg-info/dependency_links.txt
+-rw-r-----   0 sartie   (200184947) sartie   (200184947)        8 2023-07-18 13:31:06.000000 locusts-0.0.67/src/locusts.egg-info/top_level.txt
```

### Comparing `locusts-0.0.66/LICENSE` & `locusts-0.0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/PKG-INFO` & `locusts-0.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusts
-Version: 0.0.66
+Version: 0.0.67
 Summary: Distributes many short tasks on multicore and hpc systems
 Home-page: https://github.com/pypa/sampleproject
 Author: Edoardo Sarti
 Author-email: edoardo.sarti@gmail.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

### Comparing `locusts-0.0.66/README.md` & `locusts-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/setup.py` & `locusts-0.0.67/setup.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts/environment.py` & `locusts-0.0.67/src/locusts/environment.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts/inner_template_manager.txt` & `locusts-0.0.67/src/locusts/inner_template_manager.txt`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts/manager.py` & `locusts-0.0.67/src/locusts/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,20 +588,20 @@
                 stdout=subprocess.PIPE
            )
         p.wait()
         time.sleep(30)
         if DEBUG:
             print("COMMAND", " ".join(jhcp2_cmd))
             p = subprocess.Popen(
-                jhcp_cmd2,
+                jhcp2_cmd,
                 stdout=subprocess.PIPE
             )
         else:
             p = subprocess.Popen(
-                jhcp_cmd2,
+                jhcp2_cmd,
                 stderr=devnull,
                 stdout=subprocess.PIPE
            )
         p.wait()
  
         all_completed = True
         resubmit_IDs = []
```

### Comparing `locusts-0.0.66/src/locusts/outer_template_manager.txt` & `locusts-0.0.67/src/locusts/outer_template_manager.txt`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts/support.py` & `locusts-0.0.67/src/locusts/support.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts/swarm.py` & `locusts-0.0.67/src/locusts/swarm.py`

 * *Files identical despite different names*

### Comparing `locusts-0.0.66/src/locusts.egg-info/PKG-INFO` & `locusts-0.0.67/src/locusts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locusts
-Version: 0.0.66
+Version: 0.0.67
 Summary: Distributes many short tasks on multicore and hpc systems
 Home-page: https://github.com/pypa/sampleproject
 Author: Edoardo Sarti
 Author-email: edoardo.sarti@gmail.com
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
 Project-URL: Say Thanks!, http://saythanks.io/to/example
```

