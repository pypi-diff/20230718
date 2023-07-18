# Comparing `tmp/pysqa-0.0.9.tar.gz` & `tmp/pysqa-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqa-0.0.9.tar", last modified: Wed Aug 19 05:34:30 2020, max compression
+gzip compressed data, was "pysqa-0.1.0.tar", last modified: Tue Jul 18 02:39:56 2023, max compression
```

## Comparing `pysqa-0.0.9.tar` & `pysqa-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,62 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1511 2020-08-19 05:32:52.000000 pysqa-0.0.9/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-08-19 05:32:52.000000 pysqa-0.0.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-08-19 05:34:30.000000 pysqa-0.0.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4010 2020-08-19 05:32:52.000000 pysqa-0.0.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16262 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3632 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4769 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/modular.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6905 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/queueadapter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      540 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/queues.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10075 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/remote.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa/wrapper/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1785 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/gent.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1082 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/lsf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/moab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/sge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1963 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/slurm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1084 2020-08-19 05:32:52.000000 pysqa-0.0.9/pysqa/wrapper/torque.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1447 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      500 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-08-19 05:34:30.000000 pysqa-0.0.9/pysqa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-08-19 05:34:30.000000 pysqa-0.0.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2018 2020-08-19 05:32:52.000000 pysqa-0.0.9/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-08-19 05:32:52.000000 pysqa-0.0.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.566938 pysqa-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 02:39:52.000000 pysqa-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 02:39:52.000000 pysqa-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-18 02:39:56.566938 pysqa-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-18 02:39:52.000000 pysqa-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.566938 pysqa-0.1.0/pysqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 02:39:56.566938 pysqa-0.1.0/pysqa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.562938 pysqa-0.1.0/pysqa/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/executor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/executor/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/executor/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.562938 pysqa-0.1.0/pysqa/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/ext/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/ext/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/queueadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.562938 pysqa-0.1.0/pysqa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/utils/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/utils/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.562938 pysqa-0.1.0/pysqa/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/gent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-18 02:39:52.000000 pysqa-0.1.0/pysqa/wrapper/torque.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.558938 pysqa-0.1.0/pysqa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 02:39:56.000000 pysqa-0.1.0/pysqa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-18 02:39:56.566938 pysqa-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-18 02:39:56.000000 pysqa-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:39:56.566938 pysqa-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_gent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_scheduler_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-18 02:39:52.000000 pysqa-0.1.0/tests/test_torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 02:39:52.000000 pysqa-0.1.0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysqa-0.0.9/LICENSE` & `pysqa-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.9/PKG-INFO` & `pysqa-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pysqa
-Version: 0.0.9
+Version: 0.1.0
 Summary: pysqa - simple queue adapter
 Home-page: https://github.com/pyiron/pysqa
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
-Description: The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
 Keywords: pysqa
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: sge
+Provides-Extra: remote
+Provides-Extra: executor
+License-File: LICENSE
+
+The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
```

### Comparing `pysqa-0.0.9/pysqa/basic.py` & `pysqa-0.1.0/pysqa/utils/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # coding: utf-8
 # Copyright (c) Jan Janssen
 
 import getpass
 import importlib
-from jinja2 import Template
 import os
-import subprocess
 import re
+
 import pandas
-from pysqa.queues import Queues
+from jinja2 import Template
+from jinja2.exceptions import TemplateSyntaxError
+
+from pysqa.utils.execute import execute_command
+from pysqa.utils.queues import Queues
 
 
 class BasisQueueAdapter(object):
     """
     The goal of the QueueAdapter class is to make submitting to a queue system as easy as starting another sub process
     locally.
 
     Args:
+        config (dict):
         directory (str): directory containing the queue.yaml files as well as corresponding jinja2 templates for the
                          individual queues.
+        execute_command(funct):
 
     Attributes:
 
         .. attribute:: config
 
             QueueAdapter configuration read from the queue.yaml file.
 
@@ -35,15 +40,15 @@
             Pandas DataFrame representation of the available queues, read from queue.yaml.
 
         .. attribute:: queues
 
             Queues available for auto completion QueueAdapter().queues.<queue name> returns the queue name.
     """
 
-    def __init__(self, config, directory="~/.queues"):
+    def __init__(self, config, directory="~/.queues", execute_command=execute_command):
         self._config = config
         self._fill_queue_dict(queue_lst_dict=self._config["queues"])
         self._load_templates(queue_lst_dict=self._config["queues"], directory=directory)
         if self._config["queue_type"] == "SGE":
             class_name = "SunGridEngineCommands"
             module_name = "pysqa.wrapper.sge"
         elif self._config["queue_type"] == "TORQUE":
@@ -60,21 +65,32 @@
             module_name = "pysqa.wrapper.moab"
         elif self._config["queue_type"] == "GENT":
             class_name = "GentCommands"
             module_name = "pysqa.wrapper.gent"
         elif self._config["queue_type"] == "REMOTE":
             class_name = None
             module_name = None
+        elif self._config["queue_type"] == "FLUX":
+            class_name = "FluxCommands"
+            module_name = "pysqa.wrapper.flux"
         else:
-            raise ValueError()
+            raise ValueError(
+                "The queue_type "
+                + self._config["queue_type"]
+                + " is not found in the list of supported queue types "
+                + str(
+                    ["SGE", "TORQUE", "SLURM", "LSF", "MOAB", "FLUX", "GENT", "REMOTE"]
+                )
+            )
         if self._config["queue_type"] != "REMOTE":
             self._commands = getattr(importlib.import_module(module_name), class_name)()
         self._queues = Queues(self.queue_list)
         self._remote_flag = False
         self._ssh_delete_file_on_remote = True
+        self._execute_command_function = execute_command
 
     @property
     def ssh_delete_file_on_remote(self):
         return self._ssh_delete_file_on_remote
 
     @property
     def remote_flag(self):
@@ -117,51 +133,66 @@
         self,
         queue=None,
         job_name=None,
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
+        dependency_list=None,
         command=None,
+        **kwargs
     ):
         """
 
         Args:
             queue (str/None):
             job_name (str/None):
             working_directory (str/None):
             cores (int/None):
             memory_max (int/None):
             run_time_max (int/None):
+            dependency_list (list[str]/None:
             command (str/None):
 
         Returns:
             int:
         """
-        if " " in working_directory: 
-            raise ValueError("Whitespaces in the working_directory name are not supported!")
+        if " " in working_directory:
+            raise ValueError(
+                "Whitespaces in the working_directory name are not supported!"
+            )
         working_directory, queue_script_path = self._write_queue_script(
             queue=queue,
             job_name=job_name,
             working_directory=working_directory,
             cores=cores,
             memory_max=memory_max,
             run_time_max=run_time_max,
             command=command,
+            **kwargs
         )
         out = self._execute_command(
-            commands=self._commands.submit_job_command + [queue_script_path],
+            commands=self._list_command_to_be_executed(
+                dependency_list, queue_script_path
+            ),
             working_directory=working_directory,
             split_output=False,
         )
         if out is not None:
             return self._commands.get_job_id_from_output(out)
         else:
             return None
 
+    def _list_command_to_be_executed(self, dependency_list, queue_script_path) -> list:
+        return (
+            self._commands.submit_job_command
+            + self._commands.dependencies(dependency_list)
+            + [queue_script_path]
+        )
+
     def enable_reservation(self, process_id):
         """
 
         Args:
             process_id (int):
 
         Returns:
@@ -251,25 +282,25 @@
             df_selected = df[df["jobid"] == process_id]["status"]
             if len(df_selected) != 0:
                 results_lst.append(df_selected.values[0])
             else:
                 results_lst.append("finished")
         return results_lst
 
-    def get_job_from_remote(self, working_directory, delete_remote=False):
+    def get_job_from_remote(self, working_directory):
         """
         Get the results of the calculation - this is necessary when the calculation was executed on a remote host.
         """
-        pass
+        raise NotImplementedError
 
     def convert_path_to_remote(self, path):
-        pass
+        raise NotImplementedError
 
-    def transfer_file(self, file, transfer_back=False, delete_remote=False):
-        pass
+    def transfer_file(self, file, transfer_back=False):
+        raise NotImplementedError
 
     def check_queue_parameters(
         self, queue, cores=1, run_time_max=None, memory_max=None, active_queue=None
     ):
         """
 
         Args:
@@ -302,14 +333,15 @@
         queue=None,
         job_name=None,
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
         command=None,
+        **kwargs
     ):
         """
 
         Args:
             queue (str/None):
             job_name (str/None):
             working_directory (str/None):
@@ -327,14 +359,15 @@
             queue=queue,
             job_name=job_name,
             working_directory=working_directory,
             cores=cores,
             memory_max=memory_max,
             run_time_max=run_time_max,
             command=command,
+            **kwargs
         )
         if not os.path.exists(working_directory):
             os.makedirs(working_directory)
         queue_script_path = os.path.join(working_directory, "run_queue.sh")
         with open(queue_script_path, "w") as f:
             f.writelines(queue_script)
         return working_directory, queue_script_path
@@ -344,14 +377,15 @@
         queue=None,
         job_name="job.py",
         working_directory=".",
         cores=None,
         memory_max=None,
         run_time_max=None,
         command=None,
+        **kwargs
     ):
         """
 
         Args:
             queue (str/None):
             job_name (str):
             working_directory (str):
@@ -363,15 +397,20 @@
         Returns:
             str:
         """
         if queue is None:
             queue = self._config["queue_primary"]
         self._value_error_if_none(value=command)
         if queue not in self.queue_list:
-            raise ValueError()
+            raise ValueError(
+                "The queue "
+                + queue
+                + " was not found in the list of queues: "
+                + str(self.queue_list)
+            )
         active_queue = self._config["queues"][queue]
         cores, run_time_max, memory_max = self.check_queue_parameters(
             queue=None,
             cores=cores,
             run_time_max=run_time_max,
             memory_max=memory_max,
             active_queue=active_queue,
@@ -380,54 +419,53 @@
         return template.render(
             job_name=job_name,
             working_directory=working_directory,
             cores=cores,
             memory_max=memory_max,
             run_time_max=run_time_max,
             command=command,
+            **kwargs
         )
 
-    @staticmethod
-    def _get_user():
+    def _execute_command(
+        self,
+        commands,
+        working_directory=None,
+        split_output=True,
+        shell=False,
+        error_filename="pysqa.err",
+    ):
         """
 
+        Args:
+            commands (list/str):
+            working_directory (str):
+            split_output (bool):
+            shell (bool):
+            error_filename (str):
+
         Returns:
             str:
         """
-        return getpass.getuser()
+        return self._execute_command_function(
+            commands=commands,
+            working_directory=working_directory,
+            split_output=split_output,
+            shell=shell,
+            error_filename=error_filename,
+        )
 
     @staticmethod
-    def _execute_command(commands, working_directory=None, split_output=True, shell=False):
+    def _get_user():
         """
 
-        Args:
-            commands (list/str):
-            working_directory (str):
-            split_output (bool):
-            shell (bool):
-
         Returns:
             str:
         """
-        if shell and isinstance(commands, list):
-            commands = " ".join(commands)
-        try:
-            out = subprocess.check_output(
-                commands,
-                cwd=working_directory,
-                stderr=subprocess.STDOUT,
-                universal_newlines=True,
-                shell=not isinstance(commands, list),
-            )
-        except subprocess.CalledProcessError:
-            out = None
-        if out is not None and split_output:
-            return out.split("\n")
-        else:
-            return out
+        return getpass.getuser()
 
     @staticmethod
     def _fill_queue_dict(queue_lst_dict):
         """
 
         Args:
             queue_lst_dict (dict):
@@ -444,15 +482,24 @@
         Args:
             queue_lst_dict (dict):
             directory (str):
         """
         for queue_dict in queue_lst_dict.values():
             if "script" in queue_dict.keys():
                 with open(os.path.join(directory, queue_dict["script"]), "r") as f:
-                    queue_dict["template"] = Template(f.read())
+                    try:
+                        queue_dict["template"] = Template(f.read())
+                    except TemplateSyntaxError as error:
+                        raise TemplateSyntaxError(
+                            message="File: "
+                            + queue_dict["script"]
+                            + " - "
+                            + error.message,
+                            lineno=error.lineno,
+                        )
 
     @staticmethod
     def _value_error_if_none(value):
         """
 
         Args:
             value (str/None):
```

### Comparing `pysqa-0.0.9/pysqa/modular.py` & `pysqa-0.1.0/pysqa/ext/modular.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 # coding: utf-8
 # Copyright (c) Jan Janssen
 
 import pandas
-from pysqa.basic import BasisQueueAdapter
+
+from pysqa.utils.basic import BasisQueueAdapter
+from pysqa.utils.execute import execute_command
 
 
 class ModularQueueAdapter(BasisQueueAdapter):
-    def __init__(self, config, directory="~/.queues"):
-        super(ModularQueueAdapter, self).__init__(config=config, directory=directory)
+    def __init__(self, config, directory="~/.queues", execute_command=execute_command):
+        super(ModularQueueAdapter, self).__init__(
+            config=config, directory=directory, execute_command=execute_command
+        )
         self._queue_to_cluster_dict = {
             k: v["cluster"] for k, v in self._config["queues"].items()
         }
         for v in self._queue_to_cluster_dict.values():
             if v not in self._config["cluster"]:
-                raise ValueError()
+                raise ValueError(
+                    "The cluster "
+                    + v
+                    + " was not found in the list of clusters "
+                    + str(list(self._config["cluster"].keys()))
+                )
 
     def submit_job(
         self,
         queue=None,
         job_name=None,
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
+        dependency_list=None,
         command=None,
+        **kwargs
     ):
         """
 
         Args:
             queue (str/None):
             job_name (str/None):
             working_directory (str/None):
             cores (int/None):
             memory_max (int/None):
             run_time_max (int/None):
+            dependency_list (list/None):
             command (str/None):
 
         Returns:
             int:
         """
         working_directory, queue_script_path = self._write_queue_script(
             queue=queue,
             job_name=job_name,
             working_directory=working_directory,
             cores=cores,
             memory_max=memory_max,
             run_time_max=run_time_max,
             command=command,
+            **kwargs
         )
         cluster_module = self._queue_to_cluster_dict[queue]
-        commands = (
-            self._switch_cluster_command(cluster_module=cluster_module)
-            + self._commands.submit_job_command
-            + [queue_script_path]
-        )
+        commands = self._switch_cluster_command(
+            cluster_module=cluster_module
+        ) + self._list_command_to_be_executed(dependency_list, queue_script_path)
         out = self._execute_command(
-            commands=commands, 
-            working_directory=working_directory, 
-            split_output=False, 
+            commands=commands,
+            working_directory=working_directory,
+            split_output=False,
             shell=True,
         )
         if out is not None:
             cluster_queue_id = self._commands.get_job_id_from_output(out)
             cluster_queue_id *= 10
             cluster_queue_id += self._config["cluster"].index(cluster_module)
             return cluster_queue_id
@@ -133,15 +144,15 @@
             out = self._execute_command(
                 commands=cluster_commands + self._commands.get_queue_status_command,
                 split_output=False,
                 shell=True,
             )
             df = self._commands.convert_queue_status(queue_status_output=out)
             df_lst.append(df)
-        df = pandas.concat(df_lst, axis=1, sort=False).reset_index(drop=True)
+        df = pandas.concat(df_lst, axis=0, sort=False).reset_index(drop=True)
         if user is None:
             return df
         else:
             return df[df["user"] == user]
 
     @staticmethod
     def _resolve_queue_id(process_id, cluster_dict):
```

### Comparing `pysqa-0.0.9/pysqa/queueadapter.py` & `pysqa-0.1.0/pysqa/queueadapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # coding: utf-8
 # Copyright (c) Jan Janssen
 
 import os
-import yaml
-from pysqa.basic import BasisQueueAdapter
-from pysqa.modular import ModularQueueAdapter
-from pysqa.remote import RemoteQueueAdapter
+
+from pysqa.ext.modular import ModularQueueAdapter
+from pysqa.utils.basic import BasisQueueAdapter
+from pysqa.utils.config import read_config
+from pysqa.utils.execute import execute_command
 
 __author__ = "Jan Janssen"
 __copyright__ = "Copyright 2019, Jan Janssen"
 __version__ = "0.0.3"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
@@ -39,24 +40,63 @@
 
             Pandas DataFrame representation of the available queues, read from queue.yaml.
 
         .. attribute:: queues
 
             Queues available for auto completion QueueAdapter().queues.<queue name> returns the queue name.
     """
-    def __init__(self, directory="~/.queues"):
-        config = self._read_config(file_name=os.path.join(directory, "queue.yaml"))
-        if config["queue_type"] in ["SGE", "TORQUE", "SLURM", "LSF", "MOAB"]:
-            self._adapter = BasisQueueAdapter(config=config, directory=directory)
-        elif config["queue_type"] in ["GENT"]:
-            self._adapter = ModularQueueAdapter(config=config, directory=directory)
-        elif config["queue_type"] in ["REMOTE"]:
-            self._adapter = RemoteQueueAdapter(config=config, directory=directory)
+
+    def __init__(self, directory="~/.queues", execute_command=execute_command):
+        queue_yaml = os.path.join(directory, "queue.yaml")
+        clusters_yaml = os.path.join(directory, "clusters.yaml")
+        self._adapter = None
+        if os.path.exists(queue_yaml):
+            self._queue_dict = {
+                "default": set_queue_adapter(
+                    config=read_config(file_name=queue_yaml),
+                    directory=directory,
+                    execute_command=execute_command,
+                )
+            }
+            primary_queue = "default"
+        elif os.path.exists(clusters_yaml):
+            config = read_config(file_name=clusters_yaml)
+            self._queue_dict = {
+                k: set_queue_adapter(
+                    config=read_config(file_name=os.path.join(directory, v)),
+                    directory=directory,
+                    execute_command=execute_command,
+                )
+                for k, v in config["cluster"].items()
+            }
+            primary_queue = config["cluster_primary"]
         else:
-            raise ValueError
+            raise ValueError(
+                "Neither a queue.yaml file nor a clusters.yaml file were found in "
+                + directory
+            )
+        self._adapter = self._queue_dict[primary_queue]
+
+    def list_clusters(self):
+        """
+        List available computing clusters for remote submission
+
+        Returns:
+            list: List of computing clusters
+        """
+        return list(self._queue_dict.keys())
+
+    def switch_cluster(self, cluster_name):
+        """
+        Switch to a different computing cluster
+
+        Args:
+            cluster_name (str): name of the computing cluster
+        """
+        self._adapter = self._queue_dict[cluster_name]
 
     @property
     def config(self):
         """
 
         Returns:
             dict:
@@ -102,74 +142,79 @@
         self,
         queue=None,
         job_name=None,
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
+        dependency_list=None,
         command=None,
+        **kwargs
     ):
         """
         Submits command to the given queue.
 
         Args:
             queue (str/None):  Name of the queue to submit to, must be one of the names configured for this adapter
-            job_name (str/None):  Name of the job for the underlying queuing system
-            working_directory (str/None):  Directory to run the job in
-            cores (int/None):  Number of hardware threads requested
-            memory_max (int/None):  Amount of memory requested per node in GB
-            run_time_max (int/None):  Maximum runtime in seconds
-            command (str/None):  shell command to run in the job
+                               (optional)
+            job_name (str/None):  Name of the job for the underlying queuing system (optional)
+            working_directory (str/None):  Directory to run the job in (optional)
+            cores (int/None):  Number of hardware threads requested (optional)
+            memory_max (int/None):  Amount of memory requested per node in GB (optional)
+            run_time_max (int/None):  Maximum runtime in seconds (optional)
+            dependency_list(list[str]/None: Job ids of jobs to be completed before starting (optional)
+            command (str/None): shell command to run in the job
+            **kwargs: allows writing additional parameters to the job submission script if they are available in the
+                      corresponding template.
 
         Returns:
-            int:
+            int: Job id received from the queuing system for the job which was submitted \
         """
         return self._adapter.submit_job(
             queue=queue,
             job_name=job_name,
             working_directory=working_directory,
             cores=cores,
             memory_max=memory_max,
             run_time_max=run_time_max,
+            dependency_list=dependency_list,
             command=command,
+            **kwargs
         )
 
     def enable_reservation(self, process_id):
         """
 
         Args:
             process_id (int):
 
         Returns:
             str:
         """
         return self._adapter.enable_reservation(process_id=process_id)
 
-    def get_job_from_remote(self, working_directory, delete_remote=False):
+    def get_job_from_remote(self, working_directory):
         """
         Get the results of the calculation - this is necessary when the calculation was executed on a remote host.
 
         Args:
             working_directory (str):
-            delete_remote (bool):
         """
-        self._adapter.get_job_from_remote(working_directory=working_directory, delete_remote=delete_remote)
+        self._adapter.get_job_from_remote(working_directory=working_directory)
 
-    def transfer_file_to_remote(self, file, transfer_back=False, delete_remote=False):
+    def transfer_file_to_remote(self, file, transfer_back=False):
         """
 
         Args:
             file (str):
             transfer_back (bool):
-            delete_remote (bool):
-
         Returns:
             str:
         """
-        self._adapter.transfer_file(file=file, transfer_back=transfer_back, delete_remote=delete_remote)
+        self._adapter.transfer_file(file=file, transfer_back=transfer_back)
 
     def convert_path_to_remote(self, path):
         """
 
         Args:
             path (str):
 
@@ -249,19 +294,40 @@
             queue=queue,
             cores=cores,
             run_time_max=run_time_max,
             memory_max=memory_max,
             active_queue=active_queue,
         )
 
-    @staticmethod
-    def _read_config(file_name="queue.yaml"):
-        """
 
-        Args:
-            file_name (str):
+def set_queue_adapter(config, directory, execute_command=execute_command):
+    """
+    Initialize the queue adapter
 
-        Returns:
-            dict:
-        """
-        with open(file_name, "r") as f:
-            return yaml.load(f, Loader=yaml.FullLoader)
+    Args:
+        config (dict): configuration for one cluster
+        directory (str): directory which contains the queue configurations
+    """
+    if config["queue_type"] in ["SGE", "TORQUE", "SLURM", "LSF", "MOAB", "FLUX"]:
+        return BasisQueueAdapter(
+            config=config, directory=directory, execute_command=execute_command
+        )
+    elif config["queue_type"] in ["GENT"]:
+        return ModularQueueAdapter(
+            config=config, directory=directory, execute_command=execute_command
+        )
+    elif config["queue_type"] in ["REMOTE"]:
+        # The RemoteQueueAdapter has additional dependencies, namely paramiko and tqdm.
+        # By moving the import to this line it only fails when the user specifies the
+        # RemoteQueueAdapter in their pysqa configuration.
+        from pysqa.ext.remote import RemoteQueueAdapter
+
+        return RemoteQueueAdapter(
+            config=config, directory=directory, execute_command=execute_command
+        )
+    else:
+        raise ValueError(
+            "The queue_type "
+            + config["queue_type"]
+            + " is not found in the list of supported queue types "
+            + str(["SGE", "TORQUE", "SLURM", "LSF", "MOAB", "FLUX", "GENT", "REMOTE"])
+        )
```

### Comparing `pysqa-0.0.9/pysqa/queues.py` & `pysqa-0.1.0/pysqa/utils/queues.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.0.9/pysqa/remote.py` & `pysqa-0.1.0/pysqa/ext/remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,169 +1,176 @@
 # coding: utf-8
 # Copyright (c) Jan Janssen
 
 import json
 import os
+import warnings
+
 import pandas
 import paramiko
-import warnings
 from tqdm import tqdm
-from pysqa.basic import BasisQueueAdapter
+
+from pysqa.utils.basic import BasisQueueAdapter
+from pysqa.utils.execute import execute_command
 
 
 class RemoteQueueAdapter(BasisQueueAdapter):
-    def __init__(self, config, directory="~/.queues"):
-        super(RemoteQueueAdapter, self).__init__(config=config, directory=directory)
-        self._ssh_host = config['ssh_host']
-        self._ssh_username = config['ssh_username']
-        self._ssh_known_hosts = os.path.abspath(os.path.expanduser(config['known_hosts']))
-        self._ssh_key = os.path.abspath(os.path.expanduser(config['ssh_key']))
-        self._ssh_remote_config_dir = config['ssh_remote_config_dir']
-        self._ssh_remote_path = config['ssh_remote_path']
-        self._ssh_local_path = os.path.abspath(os.path.expanduser(config['ssh_local_path']))
-        if 'ssh_delete_file_on_remote' in config.keys():
-            self._ssh_delete_file_on_remote = config['ssh_delete_file_on_remote']
+    def __init__(self, config, directory="~/.queues", execute_command=execute_command):
+        super(RemoteQueueAdapter, self).__init__(
+            config=config, directory=directory, execute_command=execute_command
+        )
+        self._ssh_host = config["ssh_host"]
+        self._ssh_username = config["ssh_username"]
+        self._ssh_known_hosts = os.path.abspath(
+            os.path.expanduser(config["known_hosts"])
+        )
+        self._ssh_key = os.path.abspath(os.path.expanduser(config["ssh_key"]))
+        self._ssh_remote_config_dir = config["ssh_remote_config_dir"]
+        self._ssh_remote_path = config["ssh_remote_path"]
+        self._ssh_local_path = os.path.abspath(
+            os.path.expanduser(config["ssh_local_path"])
+        )
+        if "ssh_delete_file_on_remote" in config.keys():
+            self._ssh_delete_file_on_remote = config["ssh_delete_file_on_remote"]
         else:
             self._ssh_delete_file_on_remote = True
-        if 'ssh_port' in config.keys():
-            self._ssh_port = config['ssh_port']
+        if "ssh_port" in config.keys():
+            self._ssh_port = config["ssh_port"]
         else:
             self._ssh_port = 22
-        self._ssh_continous_connection = 'ssh_continous_connection' in config.keys()
-        if self._ssh_continous_connection:
-            self._ssh_connection = self._open_ssh_connection()
+        if "ssh_continous_connection" in config.keys():
+            self._ssh_continous_connection = config["ssh_continous_connection"]
         else:
-            self._ssh_connection = None
+            self._ssh_continous_connection = False
+        self._ssh_connection = None
         self._remote_flag = True
-        
+
     def convert_path_to_remote(self, path):
         working_directory = os.path.abspath(os.path.expanduser(path))
-        return self._get_remote_working_dir(
-            working_directory=working_directory
-        )
+        return self._get_remote_working_dir(working_directory=working_directory)
 
     def submit_job(
         self,
         queue=None,
         job_name=None,
         working_directory=None,
         cores=None,
         memory_max=None,
         run_time_max=None,
+        dependency_list=None,
         command=None,
     ):
+        if dependency_list is not None:
+            raise NotImplementedError(
+                "Submitting jobs with dependencies to a remote cluster is not yet supported."
+            )
         self._transfer_data_to_remote(working_directory=working_directory)
         output = self._execute_remote_command(command=command)
         return int(output.split()[-1])
 
     def enable_reservation(self, process_id):
         """
 
         Args:
             process_id (int):
 
         Returns:
             str:
         """
         return self._execute_remote_command(
-            command=self._reservation_command(
-                job_id=process_id
-            )
+            command=self._reservation_command(job_id=process_id)
         )
 
     def delete_job(self, process_id):
         """
 
         Args:
             process_id (int):
 
         Returns:
             str:
         """
         return self._execute_remote_command(
-            command=self._delete_command(
-                job_id=process_id
-            )
+            command=self._delete_command(job_id=process_id)
         )
 
     def get_queue_status(self, user=None):
         """
 
         Args:
             user (str):
 
         Returns:
             pandas.DataFrame:
         """
         df = pandas.DataFrame(
             json.loads(
-                self._execute_remote_command(
-                    command=self._get_queue_status_command()
-                )
+                self._execute_remote_command(command=self._get_queue_status_command())
             )
         )
         if user is None:
             return df
         else:
             return df[df["user"] == user]
 
-    def get_job_from_remote(self, working_directory, delete_remote=False):
+    def get_job_from_remote(self, working_directory):
         """
         Get the results of the calculation - this is necessary when the calculation was executed on a remote host.
         """
         working_directory = os.path.abspath(os.path.expanduser(working_directory))
         remote_working_directory = self._get_remote_working_dir(
             working_directory=working_directory
         )
         remote_dict = json.loads(
             self._execute_remote_command(
-                command='python -m pysqa.cmd --list --working_directory ' + remote_working_directory
+                command="python -m pysqa --list --working_directory "
+                + remote_working_directory
             )
         )
-        for d in remote_dict['dirs']:
+        for d in remote_dict["dirs"]:
             local_dir = self._get_file_transfer(
-                file=d,
-                local_dir=remote_working_directory,
-                remote_dir=working_directory
+                file=d, local_dir=remote_working_directory, remote_dir=working_directory
             )
             os.makedirs(local_dir, exist_ok=True)
         file_dict = {}
-        for f in remote_dict['files']:
+        for f in remote_dict["files"]:
             local_file = self._get_file_transfer(
-                file=f,
-                local_dir=remote_working_directory,
-                remote_dir=working_directory
+                file=f, local_dir=remote_working_directory, remote_dir=working_directory
             )
             file_dict[local_file] = f
         self._transfer_files(file_dict=file_dict, sftp=None, transfer_back=True)
-        if delete_remote:
-            self._execute_remote_command(
-                command="rm -r " + remote_working_directory
-            )
+        if self._ssh_delete_file_on_remote:
+            self._execute_remote_command(command="rm -r " + remote_working_directory)
 
-    def transfer_file(self, file, transfer_back=False, delete_remote=False):
+    def transfer_file(self, file, transfer_back=False):
         working_directory = os.path.abspath(os.path.expanduser(file))
         remote_working_directory = self._get_remote_working_dir(
             working_directory=working_directory
         )
         self._create_remote_dir(directory=os.path.dirname(remote_working_directory))
-        self._transfer_files(file_dict={working_directory: remote_working_directory},
-                             sftp=None,
-                             transfer_back=transfer_back)
-        if delete_remote and transfer_back:
-            self._execute_remote_command(
-                command="rm " + remote_working_directory
-            )
+        self._transfer_files(
+            file_dict={working_directory: remote_working_directory},
+            sftp=None,
+            transfer_back=transfer_back,
+        )
+        if self._ssh_delete_file_on_remote and transfer_back:
+            self._execute_remote_command(command="rm " + remote_working_directory)
 
     def __del__(self):
-        self._ssh_connection.close()
+        if self._ssh_connection is not None:
+            self._ssh_connection.close()
+
+    def _check_ssh_connection(self):
+        if self._ssh_connection is None:
+            self._ssh_connection = self._open_ssh_connection()
 
     def _transfer_files(self, file_dict, sftp=None, transfer_back=False):
         if sftp is None:
             if self._ssh_continous_connection:
+                self._check_ssh_connection()
                 ssh = self._ssh_connection
             else:
                 ssh = self._open_ssh_connection()
             sftp_client = ssh.open_sftp()
         else:
             sftp_client = sftp
         for file_src, file_dst in tqdm(file_dict.items()):
@@ -176,92 +183,88 @@
                 sftp_client.put(file_src, file_dst)
         if sftp is None:
             sftp_client.close()
 
     def _open_ssh_connection(self):
         ssh = paramiko.SSHClient()
         ssh.load_host_keys(self._ssh_known_hosts)
-        ssh.connect(hostname=self._ssh_host,
-                    port=self._ssh_port,
-                    username=self._ssh_username,
-                    key_filename=self._ssh_key)
+        ssh.connect(
+            hostname=self._ssh_host,
+            port=self._ssh_port,
+            username=self._ssh_username,
+            key_filename=self._ssh_key,
+        )
         return ssh
 
     def _remote_command(self):
-        return 'python -m pysqa.cmd --config_directory ' + self._ssh_remote_config_dir + ' '
+        return "python -m pysqa --config_directory " + self._ssh_remote_config_dir + " "
 
     def _get_queue_status_command(self):
-        return self._remote_command() + '--status'
+        return self._remote_command() + "--status"
 
     def _submit_command(
-            self,
-            queue=None,
-            job_name=None,
-            working_directory=None,
-            cores=None,
-            memory_max=None,
-            run_time_max=None,
-            command_str=None
+        self,
+        queue=None,
+        job_name=None,
+        working_directory=None,
+        cores=None,
+        memory_max=None,
+        run_time_max=None,
+        command_str=None,
     ):
-        command = self._remote_command() + '--submit '
+        command = self._remote_command() + "--submit "
         if queue is not None:
-            command += '--queue ' + queue + ' '
+            command += "--queue " + queue + " "
         if job_name is not None:
-            command += '--job_name ' + job_name + ' '
+            command += "--job_name " + job_name + " "
         if working_directory is not None:
-            command += '--working_directory ' + working_directory + ' '
+            command += "--working_directory " + working_directory + " "
         if cores is not None:
-            command += '--cores ' + cores + ' '
+            command += "--cores " + cores + " "
         if memory_max is not None:
-            command += '--memory ' + memory_max + ' '
+            command += "--memory " + memory_max + " "
         if run_time_max is not None:
-            command += '--run_time ' + run_time_max + ' '
+            command += "--run_time " + run_time_max + " "
         if command_str is not None:
             command += '--command "' + command_str + '" '
         return command
 
     def _delete_command(self, job_id):
-        return self._remote_command() + '--delete --id ' + str(job_id)
+        return self._remote_command() + "--delete --id " + str(job_id)
 
     def _reservation_command(self, job_id):
-        return self._remote_command() + '--reservation --id ' + str(job_id)
+        return self._remote_command() + "--reservation --id " + str(job_id)
 
     def _execute_remote_command(self, command):
         if self._ssh_continous_connection:
+            self._check_ssh_connection()
             ssh = self._ssh_connection
         else:
             ssh = self._open_ssh_connection()
         stdin, stdout, stderr = ssh.exec_command(command)
         warnings.warn(stderr.read().decode())
         output = stdout.read().decode()
         if not self._ssh_continous_connection:
             ssh.close()
         return output
 
     def _get_remote_working_dir(self, working_directory):
         return os.path.join(
             self._ssh_remote_path,
-            os.path.relpath(
-                working_directory,
-                self._ssh_local_path
-            )
+            os.path.relpath(working_directory, self._ssh_local_path),
         )
 
     def _create_remote_dir(self, directory):
         if isinstance(directory, str):
-            self._execute_remote_command(
-                command="mkdir -p " + directory
-            )
+            self._execute_remote_command(command="mkdir -p " + directory)
         elif isinstance(directory, list):
             command = "mkdir -p "
             for d in directory:
                 command += d + " "
-            self._execute_remote_command(
-                command=command
-            )
+            self._execute_remote_command(command=command)
         else:
             raise TypeError()
 
     def _transfer_data_to_remote(self, working_directory):
         working_directory = os.path.abspath(os.path.expanduser(working_directory))
         remote_working_directory = self._get_remote_working_dir(
             working_directory=working_directory
@@ -269,22 +272,33 @@
         file_dict = {}
         new_dir_list = []
         for p, folder, files in os.walk(working_directory):
             new_dir_list.append(
                 self._get_file_transfer(
                     file=p,
                     local_dir=working_directory,
-                    remote_dir=remote_working_directory
+                    remote_dir=remote_working_directory,
                 )
             )
             for f in files:
                 file_path = os.path.join(p, f)
                 file_dict[file_path] = self._get_file_transfer(
                     file=file_path,
                     local_dir=working_directory,
-                    remote_dir=remote_working_directory)
+                    remote_dir=remote_working_directory,
+                )
         self._create_remote_dir(directory=new_dir_list)
         self._transfer_files(file_dict=file_dict, sftp=None, transfer_back=False)
 
+    def _get_user(self):
+        """
+
+        Returns:
+            str:
+        """
+        return self._ssh_username
+
     @staticmethod
     def _get_file_transfer(file, local_dir, remote_dir):
-        return os.path.abspath(os.path.join(remote_dir, os.path.relpath(file, local_dir)))
+        return os.path.abspath(
+            os.path.join(remote_dir, os.path.relpath(file, local_dir))
+        )
```

### Comparing `pysqa-0.0.9/pysqa/wrapper/gent.py` & `pysqa-0.1.0/pysqa/wrapper/gent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import pandas
-from pysqa.wrapper.slurm import SlurmCommands
 
+from pysqa.wrapper.slurm import SlurmCommands
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2019, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
@@ -17,28 +17,43 @@
 __status__ = "development"
 __date__ = "Feb 9, 2019"
 
 
 class GentCommands(SlurmCommands):
     @staticmethod
     def get_job_id_from_output(queue_submit_output):
-          return int(queue_submit_output.splitlines()[-1].rstrip().lstrip().split(';')[0])
+        return int(queue_submit_output.splitlines()[-1].rstrip().lstrip().split(";")[0])
 
     @staticmethod
     def get_queue_from_output(queue_submit_output):
-          return str(queue_submit_output.splitlines()[-1].rstrip().lstrip().split(';')[1])
+        return str(queue_submit_output.splitlines()[-1].rstrip().lstrip().split(";")[1])
 
     @staticmethod
     def convert_queue_status(queue_status_output):
         qstat = queue_status_output.splitlines()
-        queue = qstat[0].split(':')[1].strip()
-        if len(qstat) <= 1: # first row contains cluster name, check if there are jobs
+        queue = qstat[0].split(":")[1].strip()
+        if len(qstat) <= 1:  # first row contains cluster name, check if there are jobs
             return None
 
-        line_split_lst = [line.split('|') for line in qstat[1:]]
-        job_id_lst, user_lst, status_lst, job_name_lst, queue_lst = zip(*[(int(jobid), user, status.lower(), jobname, queue)
-                                                               for jobid, user, status, jobname in line_split_lst])
-        return pandas.DataFrame({'cluster': queue_lst,
-                                 'jobid': job_id_lst,
-                                 'user': user_lst,
-                                 'jobname': job_name_lst,
-                                 'status': status_lst})
+        line_split_lst = [line.split("|") for line in qstat[1:]]
+        job_id_lst, user_lst, status_lst, job_name_lst, queue_lst = zip(
+            *[
+                (int(jobid), user, status.lower(), jobname, queue)
+                for jobid, user, status, jobname in line_split_lst
+            ]
+        )
+        return pandas.DataFrame(
+            {
+                "cluster": queue_lst,
+                "jobid": job_id_lst,
+                "user": user_lst,
+                "jobname": job_name_lst,
+                "status": status_lst,
+            }
+        )
+
+    @staticmethod
+    def dependencies(dependency_list) -> list:
+        if dependency_list is not None:
+            raise NotImplementedError()
+        else:
+            return []
```

### Comparing `pysqa-0.0.9/pysqa/wrapper/lsf.py` & `pysqa-0.1.0/pysqa/wrapper/lsf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
+from pysqa.wrapper.generic import SchedulerCommands
+
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2019, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Feb 9, 2019"
 
 
-class LsfCommands(object):
+class LsfCommands(SchedulerCommands):
     @property
     def submit_job_command(self):
         return ["bsub", "-terse"]
 
     @property
     def delete_job_command(self):
         return ["bkill"]
 
     @property
-    def enable_reservation_command(self):
-        raise NotImplementedError()
-
-    @property
     def get_queue_status_command(self):
         return ["qstat", "-x"]
-
-    @staticmethod
-    def get_job_id_from_output(queue_submit_output):
-        raise NotImplementedError()
-
-    @staticmethod
-    def convert_queue_status(queue_status_output):
-        raise NotImplementedError()
```

### Comparing `pysqa-0.0.9/pysqa/wrapper/sge.py` & `pysqa-0.1.0/pysqa/wrapper/sge.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
+import defusedxml.ElementTree as ETree
 import pandas
-import defusedxml.cElementTree as ETree
+
+from pysqa.wrapper.generic import SchedulerCommands
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2019, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "production"
 __date__ = "Feb 9, 2019"
 
 
-class SunGridEngineCommands(object):
+class SunGridEngineCommands(SchedulerCommands):
     @property
     def submit_job_command(self):
         return ["qsub", "-terse"]
 
     @property
     def delete_job_command(self):
         return ["qdel"]
@@ -31,32 +33,29 @@
         return ["qalter", "-R", "y"]
 
     @property
     def get_queue_status_command(self):
         return ["qstat", "-xml"]
 
     @staticmethod
-    def get_job_id_from_output(queue_submit_output):
-        return int(queue_submit_output)
-
-    @staticmethod
     def convert_queue_status(queue_status_output):
         def leaf_to_dict(leaf):
             return [
                 {sub_child.tag: sub_child.text for sub_child in child} for child in leaf
             ]
 
         tree = ETree.fromstring(queue_status_output)
         df_running_jobs = pandas.DataFrame(leaf_to_dict(leaf=tree[0]))
         df_pending_jobs = pandas.DataFrame(leaf_to_dict(leaf=tree[1]))
-        df_merge = df_running_jobs.append(df_pending_jobs, sort=True)
-        df_merge.loc[df_merge.state == "r", 'state'] = "running"
-        df_merge.loc[df_merge.state == "qw", 'state'] = "pending"
-        df_merge.loc[df_merge.state == "Eqw", 'state'] = "error"
+        df_merge = pandas.concat([df_running_jobs, df_pending_jobs], sort=True)
+        df_merge.loc[df_merge.state == "r", "state"] = "running"
+        df_merge.loc[df_merge.state == "qw", "state"] = "pending"
+        df_merge.loc[df_merge.state == "Eqw", "state"] = "error"
         return pandas.DataFrame(
             {
                 "jobid": pandas.to_numeric(df_merge.JB_job_number),
                 "user": df_merge.JB_owner,
                 "jobname": df_merge.JB_name,
                 "status": df_merge.state,
+                "working_directory": [""] * len(df_merge),
             }
         )
```

### Comparing `pysqa-0.0.9/pysqa/wrapper/slurm.py` & `pysqa-0.1.0/pysqa/wrapper/slurm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,74 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
 import pandas
 
+from pysqa.wrapper.generic import SchedulerCommands
 
 __author__ = "Jan Janssen"
 __copyright__ = (
     "Copyright 2019, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
 __version__ = "1.0"
 __maintainer__ = "Jan Janssen"
 __email__ = "janssen@mpie.de"
 __status__ = "development"
 __date__ = "Feb 9, 2019"
 
 
-class SlurmCommands(object):
+class SlurmCommands(SchedulerCommands):
     @property
     def submit_job_command(self):
         return ["sbatch", "--parsable"]
 
     @property
     def delete_job_command(self):
         return ["scancel"]
 
     @property
-    def enable_reservation_command(self):
-        raise NotImplementedError()
-
-    @property
     def get_queue_status_command(self):
-        return ["squeue", "--format", "%A|%u|%t|%j", "--noheader"]
+        return ["squeue", "--format", "%A|%u|%t|%.15j|%Z", "--noheader"]
 
     @staticmethod
     def get_job_id_from_output(queue_submit_output):
-        return int(queue_submit_output.splitlines()[-1].rstrip().lstrip())
+        return int(queue_submit_output.splitlines()[-1].rstrip().lstrip().split()[-1])
 
     @staticmethod
     def convert_queue_status(queue_status_output):
         line_split_lst = [line.split("|") for line in queue_status_output.splitlines()]
         if len(line_split_lst) != 0:
-            job_id_lst, user_lst, status_lst, job_name_lst = zip(
+            job_id_lst, user_lst, status_lst, job_name_lst, working_directory_lst = zip(
                 *[
-                    (int(jobid), user, status.lower(), jobname)
-                    for jobid, user, status, jobname in line_split_lst
+                    (int(jobid), user, status.lower(), jobname, working_directory)
+                    for jobid, user, status, jobname, working_directory in line_split_lst
                 ]
             )
-        else: 
-            job_id_lst, user_lst, status_lst, job_name_lst = [], [], [], []
+        else:
+            job_id_lst, user_lst, status_lst, job_name_lst, working_directory_lst = (
+                [],
+                [],
+                [],
+                [],
+                [],
+            )
         df = pandas.DataFrame(
             {
                 "jobid": job_id_lst,
                 "user": user_lst,
                 "jobname": job_name_lst,
                 "status": status_lst,
+                "working_directory": working_directory_lst,
             }
         )
-        df.loc[df.status == "r", 'status'] = "running"
-        df.loc[df.status == "pd", 'status'] = "pending"
+        df.loc[df.status == "r", "status"] = "running"
+        df.loc[df.status == "pd", "status"] = "pending"
         return df
+
+    @staticmethod
+    def dependencies(dependency_list) -> list:
+        if dependency_list is not None:
+            return ["--dependency=afterok:" + ",".join(dependency_list)]
+        else:
+            return []
```

### Comparing `pysqa-0.0.9/pysqa.egg-info/PKG-INFO` & `pysqa-0.1.0/pysqa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pysqa
-Version: 0.0.9
+Version: 0.1.0
 Summary: pysqa - simple queue adapter
 Home-page: https://github.com/pyiron/pysqa
 Author: Jan Janssen
 Author-email: janssen@mpie.de
 License: BSD
-Description: The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
 Keywords: pysqa
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: sge
+Provides-Extra: remote
+Provides-Extra: executor
+License-File: LICENSE
+
+The goal of pysqa is to make submitting to an HPC cluster as easy as starting another subprocess. This is based on the assumption that even though modern queuing systems allow for an wide range of different configuration, most users submit the majority of their jobs with very similar parameters. Therefore pysqa allows the users to store their submission scripts as jinja2 templates for quick access. After the submission pysqa allows the users to track the progress of their jobs, delete them or enable reservations using the built-in functionality of the queuing system. The currently supported queuing systems are: LFS, MOAB, SGE, SLURM, TORQUE.
```

### Comparing `pysqa-0.0.9/setup.py` & `pysqa-0.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,24 +16,30 @@
     license='BSD',
 
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Topic :: Scientific/Engineering :: Physics',
                  'License :: OSI Approved :: BSD License',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7'],
+                 'Programming Language :: Python :: 3.7',
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11'
+                ],
 
     keywords='pysqa',
     packages=find_packages(exclude=["*tests*"]),
-    install_requires=['defusedxml>=0.5.0',
-                      'jinja2>=2.10.1',
-                      'pandas>=0.24.2',
-                      'paramiko>=2.4.2',
-                      'pyyaml>=5.1.2',
-                      'tqdm>=4.35.0'],
+    install_requires=['jinja2>=3.1.2', 'pandas>=2.0.3', 'pyyaml>=6.0'],
+    extras_require={
+        "sge": ['defusedxml>=0.7.1'],
+        "remote": ['paramiko>=3.2.0', 'tqdm>=4.65.0'],
+        "executor": ['pympipool>=0.5.4', 'cloudpickle>=2.2.1'],
+    },
     cmdclass=versioneer.get_cmdclass(),
-    )
+    entry_points={
+            "console_scripts": [
+                'pysqa=pysqa.cmd:command_line',
+                'pysqa-executor=pysqa.executor.backend:command_line'
+            ]
+    }
+)
```

### Comparing `pysqa-0.0.9/versioneer.py` & `pysqa-0.1.0/versioneer.py`

 * *Files identical despite different names*

