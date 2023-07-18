# Comparing `tmp/pympipool-0.5.4.tar.gz` & `tmp/pympipool-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.4.tar", last modified: Thu Jul 13 16:24:32 2023, max compression
+gzip compressed data, was "pympipool-0.5.5.tar", last modified: Tue Jul 18 13:53:02 2023, max compression
```

## Comparing `pympipool-0.5.4.tar` & `pympipool-0.5.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-13 16:24:28.000000 pympipool-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 16:24:28.000000 pympipool-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 16:24:32.490979 pympipool-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-13 16:24:28.000000 pympipool-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.486979 pympipool-0.5.4/pympipool/external_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/parallel_executors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/shared_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/external_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/parallel_executors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.486979 pympipool-0.5.4/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 16:24:32.490979 pympipool-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 16:24:32.000000 pympipool-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-13 16:24:28.000000 pympipool-0.5.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-18 13:52:59.000000 pympipool-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 13:52:59.000000 pympipool-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-18 13:53:02.749822 pympipool-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-18 13:52:59.000000 pympipool-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 13:53:02.749822 pympipool-0.5.5/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/external_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/external_interfaces/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/parallel_executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/parallel_executors/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool/shared_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/external_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-18 13:52:59.000000 pympipool-0.5.5/pympipool/shared_functions/parallel_executors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.745822 pympipool-0.5.5/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 13:53:02.000000 pympipool-0.5.5/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 13:53:02.749822 pympipool-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-18 13:53:02.000000 pympipool-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:53:02.749822 pympipool-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-18 13:52:59.000000 pympipool-0.5.5/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 13:52:59.000000 pympipool-0.5.5/versioneer.py
```

### Comparing `pympipool-0.5.4/LICENSE` & `pympipool-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/PKG-INFO` & `pympipool-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.4
+Version: 0.5.5
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.4/README.md` & `pympipool-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/external_interfaces/communication.py` & `pympipool-0.5.5/pympipool/external_interfaces/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/external_interfaces/executor.py` & `pympipool-0.5.5/pympipool/external_interfaces/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 from concurrent.futures import Executor as FutureExecutor, Future
 from queue import Queue
-from threading import Thread
 
+from pympipool.external_interfaces.thread import RaisingThread
 from pympipool.shared_functions.external_interfaces import (
     execute_parallel_tasks,
     execute_serial_tasks,
     cloudpickle_register,
     cancel_items_in_queue,
 )
 
@@ -106,15 +106,15 @@
         enable_slurm_backend=False,
         init_function=None,
         cwd=None,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         super().__init__()
-        self._process = Thread(
+        self._process = RaisingThread(
             target=execute_parallel_tasks,
             kwargs={
                 "future_queue": self._future_queue,
                 "cores": cores,
                 "oversubscribe": oversubscribe,
                 "enable_flux_backend": enable_flux_backend,
                 "enable_slurm_backend": enable_slurm_backend,
@@ -173,15 +173,15 @@
         enable_slurm_backend=False,
         cwd=None,
         sleep_interval=0.1,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         super().__init__()
-        self._process = Thread(
+        self._process = RaisingThread(
             target=execute_serial_tasks,
             kwargs={
                 "future_queue": self._future_queue,
                 "cores": max_workers,
                 "oversubscribe": oversubscribe,
                 "enable_flux_backend": enable_flux_backend,
                 "enable_slurm_backend": enable_slurm_backend,
```

### Comparing `pympipool-0.5.4/pympipool/external_interfaces/pool.py` & `pympipool-0.5.5/pympipool/external_interfaces/pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/parallel_executors/mpiexec.py` & `pympipool-0.5.5/pympipool/parallel_executors/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/parallel_executors/mpipool.py` & `pympipool-0.5.5/pympipool/parallel_executors/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/shared_functions/external_interfaces.py` & `pympipool-0.5.5/pympipool/shared_functions/external_interfaces.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool/shared_functions/parallel_executors.py` & `pympipool-0.5.5/pympipool/shared_functions/parallel_executors.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.5/pympipool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.4
+Version: 0.5.5
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.4/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.5/pympipool.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pympipool.egg-info/dependency_links.txt
 pympipool.egg-info/requires.txt
 pympipool.egg-info/top_level.txt
 pympipool/external_interfaces/__init__.py
 pympipool/external_interfaces/communication.py
 pympipool/external_interfaces/executor.py
 pympipool/external_interfaces/pool.py
+pympipool/external_interfaces/thread.py
 pympipool/parallel_executors/__init__.py
 pympipool/parallel_executors/mpiexec.py
 pympipool/parallel_executors/mpipool.py
 pympipool/shared_functions/__init__.py
 pympipool/shared_functions/external_interfaces.py
 pympipool/shared_functions/parallel_executors.py
 tests/test_communicator_split.py
```

### Comparing `pympipool-0.5.4/setup.py` & `pympipool-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_communicator_split.py` & `pympipool-0.5.5/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_executor.py` & `pympipool-0.5.5/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_future.py` & `pympipool-0.5.5/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_interface.py` & `pympipool-0.5.5/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_multitask.py` & `pympipool-0.5.5/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_parse.py` & `pympipool-0.5.5/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_pool.py` & `pympipool-0.5.5/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_queue.py` & `pympipool-0.5.5/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_task.py` & `pympipool-0.5.5/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_worker.py` & `pympipool-0.5.5/tests/test_worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 def mpi_funct(i):
     from mpi4py import MPI
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
     return i, size, rank
 
 
+def raise_error():
+    raise RuntimeError
+
+
 class TestFuturePool(unittest.TestCase):
     def test_pool_serial(self):
         with Executor(cores=1) as p:
             output = p.submit(calc, i=2)
             self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
@@ -49,14 +53,19 @@
             fs2.result()
 
     def test_pool_serial_map(self):
         with Executor(cores=1) as p:
             output = p.map(calc, [1, 2, 3])
         self.assertEqual(list(output), [np.array(1), np.array(4), np.array(9)])
 
+    def test_executor_exception(self):
+        with self.assertRaises(RuntimeError):
+            with Executor(cores=1) as p:
+                p.submit(raise_error)
+
     def test_pool_multi_core(self):
         with Executor(cores=2) as p:
             output = p.submit(mpi_funct, i=2)
             self.assertEqual(len(p), 1)
             self.assertTrue(isinstance(output, Future))
             self.assertFalse(output.done())
             sleep(1)
```

### Comparing `pympipool-0.5.4/tests/test_worker_memory.py` & `pympipool-0.5.5/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/tests/test_zmq.py` & `pympipool-0.5.5/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.4/versioneer.py` & `pympipool-0.5.5/versioneer.py`

 * *Files identical despite different names*

