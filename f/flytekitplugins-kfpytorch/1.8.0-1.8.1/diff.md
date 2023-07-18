# Comparing `tmp/flytekitplugins-kfpytorch-1.8.0.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.8.0.tar", last modified: Tue Jul 11 22:07:20 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.8.1.tar", last modified: Tue Jul 18 18:01:39 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.8.0.tar` & `flytekitplugins-kfpytorch-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.395715 flytekitplugins-kfpytorch-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 22:07:20.395715 flytekitplugins-kfpytorch-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-11 22:06:52.000000 flytekitplugins-kfpytorch-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.391715 flytekitplugins-kfpytorch-1.8.0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.391715 flytekitplugins-kfpytorch-1.8.0/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 22:06:52.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-07-11 22:06:52.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:20.391715 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:20.000000 flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:20.395715 flytekitplugins-kfpytorch-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-11 22:07:11.000000 flytekitplugins-kfpytorch-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.655022 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.655022 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-18 18:01:33.000000 flytekitplugins-kfpytorch-1.8.1/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.8.0/PKG-INFO` & `flytekitplugins-kfpytorch-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.8.0
+Version: 1.8.1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.8.0/README.md` & `flytekitplugins-kfpytorch-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.8.0/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,22 @@
     Use this to run single- or multi-node distributed pytorch elastic training on k8s.
 
     Single-node elastic training is executed in a k8s pod when `nnodes` is set to 1.
     Multi-node training is executed otherwise using a `Pytorch Job <https://github.com/kubeflow/training-operator>`_.
 
     Args:
         nnodes (Union[int, str]): Number of nodes, or the range of nodes in form <minimum_nodes>:<maximum_nodes>.
-        nproc_per_node (Union[int, str]): Number of workers per node. Supported values are [auto, cpu, gpu, int].
+        nproc_per_node (str): Number of workers per node.
         start_method (str): Multiprocessing start method to use when creating workers.
         monitor_interval (int): Interval, in seconds, to monitor the state of workers.
         max_restarts (int): Maximum number of worker group restarts before failing.
     """
 
     nnodes: Union[int, str] = 1
-    nproc_per_node: Union[int, str] = "auto"
+    nproc_per_node: int = 1
     start_method: str = "spawn"
     monitor_interval: int = 5
     max_restarts: int = 0
 
 
 class PyTorchFunctionTask(PythonFunctionTask[PyTorch]):
     """
@@ -272,38 +272,32 @@
         This helper method will be invoked to execute the task.
 
 
         Returns:
             The result of rank zero.
         """
         try:
-            from torch.distributed import run
             from torch.distributed.launcher.api import LaunchConfig, elastic_launch
         except ImportError:
             raise ImportError(TORCH_IMPORT_ERROR_MESSAGE)
 
-        if isinstance(self.task_config.nproc_per_node, str):
-            nproc = run.determine_local_world_size(self.task_config.nproc_per_node)
-        else:
-            nproc = self.task_config.nproc_per_node
-
         dist_env_vars_set = os.environ.get("PET_NNODES") is not None
         if not dist_env_vars_set and self.min_nodes > 1:
             logger.warning(
                 (
                     f"`nnodes` is set to {self.task_config.nnodes} in elastic task but execution appears "
                     "to not run in a `PyTorchJob`. Rendezvous might timeout."
                 )
             )
 
         config = LaunchConfig(
             run_id=flytekit.current_context().execution_id.name,
             min_nodes=self.min_nodes,
             max_nodes=self.max_nodes,
-            nproc_per_node=nproc,
+            nproc_per_node=self.task_config.nproc_per_node,
             rdzv_backend=self.rdzv_backend,  # rdzv settings
             rdzv_endpoint=os.environ.get("PET_RDZV_ENDPOINT", "localhost:0"),
             max_restarts=self.task_config.max_restarts,
             monitor_interval=self.task_config.monitor_interval,
             start_method=self.task_config.start_method,
         )
 
@@ -342,18 +336,31 @@
 
             launcher_target_func = fn_partial
             launcher_args = ()
 
         else:
             raise Exception("Bad start method")
 
-        out = elastic_launch(
-            config=config,
-            entrypoint=launcher_target_func,
-        )(*launcher_args)
+        if self.metadata.retries > 0 and self.task_config.max_restarts == 0:
+            msg = (
+                "Flyte considers exceptions in worker processes of torch elastic tasks as non-recoverable as "
+                "Flyte does not have access to the type of the original exception raised in the child process. Use "
+                "`@task(task_config=Elastic(..., max_restarts=<n>))` to configure retries on the torch elastic launch level."
+            )
+            logger.warning(msg)
+
+        from torch.distributed.elastic.multiprocessing.errors import ChildFailedError
+
+        try:
+            out = elastic_launch(
+                config=config,
+                entrypoint=launcher_target_func,
+            )(*launcher_args)
+        except ChildFailedError as e:
+            raise RuntimeError(e.format_msg())
 
         # `out` is a dictionary of rank (not local rank) -> result
         # Rank 0 returns the result of the task function
         if 0 in out:
             return out[0]
         else:
             raise IgnoreOutputs()
```

### Comparing `flytekitplugins-kfpytorch-1.8.0/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.8.0
+Version: 1.8.1
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.8.0/setup.py` & `flytekitplugins-kfpytorch-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flyteidl>=1.5.1", "flytekit>=1.6.1"]
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

