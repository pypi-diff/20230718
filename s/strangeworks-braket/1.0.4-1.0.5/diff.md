# Comparing `tmp/strangeworks_braket-1.0.4.tar.gz` & `tmp/strangeworks_braket-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.4.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.5.tar", max compression
```

## Comparing `strangeworks_braket-1.0.4.tar` & `strangeworks_braket-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      457 2023-04-28 10:10:35.110807 strangeworks_braket-1.0.4/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-28 10:10:35.110807 strangeworks_braket-1.0.4/LICENSE
--rw-r--r--   0        0        0     1319 2023-04-28 10:10:52.122973 strangeworks_braket-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      286 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     6794 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/device.py
--rw-r--r--   0        0        0     8503 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/job.py
--rw-r--r--   0        0        0    10889 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/task.py
--rw-r--r--   0        0        0      691 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/utils/serializer.py
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1394 2023-07-18 13:19:14.111787 strangeworks_braket-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     7279 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/device.py
+-rw-r--r--   0        0        0     8503 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/job.py
+-rw-r--r--   0        0        0    10554 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/task.py
+-rw-r--r--   0        0        0      691 2023-07-18 13:19:00.851652 strangeworks_braket-1.0.5/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.5/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.4/LICENSE` & `strangeworks_braket-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.4/strangeworks_braket/device.py` & `strangeworks_braket-1.0.5/strangeworks_braket/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import json
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import strangeworks as sw
 from braket.annealing.problem import Problem
 from braket.aws.aws_device import Device
 from braket.circuits import Circuit
 from braket.device_schema import DeviceCapabilities
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.tasks.quantum_task import QuantumTask
+from braket.tasks.quantum_task_batch import QuantumTaskBatch
 
 from strangeworks_braket.job import StrangeworksQuantumJob
 from strangeworks_braket.task import StrangeworksQuantumTask
 from strangeworks_braket.utils.serializer import pickle_deserializer
 
 
 class StrangeworksDevice(Device):
@@ -49,14 +50,15 @@
         shots: Optional[int]
             The number of shots to run the task for. Defaults to 1000.
         Returns
         -------
         task: QuantumTask (StrangeworksQuantumTask)
             The task that was run.
         """
+
         return StrangeworksQuantumTask.create(
             self.arn, task_specification, shots or 1000, *args, **kwargs
         )
 
     def run_hybrid(
         self,
         filepath: str,
@@ -118,14 +120,27 @@
                     backend.remote_status,
                     backend.slug,
                 )
             )
 
         return devices
 
+    def run_batch(
+        self,
+        task_specifications: Circuit | Problem | List[Circuit | Problem],
+        shots: int | None,
+        max_parallel: int | None,
+        inputs: Dict[str, float] | List[Dict[str, float]] | None,
+        *args,
+        **kwargs,
+    ) -> QuantumTaskBatch:
+        return super().run_batch(
+            task_specifications, shots, max_parallel, inputs, *args, **kwargs
+        )
+
     @property
     def properties(self) -> DeviceCapabilities:
         if self._properties is None:
             payload = {
                 "aws_device_arn": self.arn,
             }
```

### Comparing `strangeworks_braket-1.0.4/strangeworks_braket/job.py` & `strangeworks_braket-1.0.5/strangeworks_braket/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.4/strangeworks_braket/task.py` & `strangeworks_braket-1.0.5/strangeworks_braket/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.schema_common import BraketSchemaBase
 from braket.tasks.annealing_quantum_task_result import AnnealingQuantumTaskResult
 from braket.tasks.gate_model_quantum_task_result import GateModelQuantumTaskResult
 from braket.tasks.quantum_task import QuantumTask
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.types.job import Job, Status
-from strawberryfields.tdm.program import TDMProgram
 
 from strangeworks_braket.utils.serializer import pickle_serializer
 
 
 class StrangeworksQuantumTask(QuantumTask):
     _product_slug = "amazon-braket"
 
@@ -200,15 +199,15 @@
         job = jobs[0]
         return StrangeworksQuantumTask(job)
 
     @staticmethod
     def create(
         device_arn: str,
         task_specification: Union[
-            Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation, TDMProgram
+            Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation
         ],
         shots: int,
         device_parameters: Optional[Dict[str, Any]] = None,
         tags: Optional[Dict[str, str]] = None,
         *args,
         **kwargs,
     ) -> StrangeworksQuantumTask:
@@ -267,15 +266,15 @@
         remix = {to_camel_case(key): value for key, value in d.items()}
         return Job.from_dict(remix)
 
 
 @singledispatch
 def _sw_task_specification(
     task_specification: Union[
-        Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation, TDMProgram
+        Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation
     ]
 ) -> Tuple[str, str]:
     raise NotImplementedError
 
 
 # register a function for each type
 @_sw_task_specification.register
@@ -297,15 +296,7 @@
 
 @_sw_task_specification.register
 def _sw_task_specification_aquila(
     task_specification: AnalogHamiltonianSimulation,
 ) -> Tuple[str, str]:
     task_new_specification = json.dumps(pickle_serializer(task_specification, "json"))
     return "aquila", task_new_specification
-
-
-@_sw_task_specification.register
-def _sw_task_specification_xanadu(
-    task_specification: TDMProgram,
-) -> Tuple[str, str]:
-    task_new_specification = json.dumps(pickle_serializer(task_specification, "json"))
-    return "xanadu", task_new_specification
```

### Comparing `strangeworks_braket-1.0.4/strangeworks_braket/utils/serializer.py` & `strangeworks_braket-1.0.5/strangeworks_braket/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.4/PKG-INFO` & `strangeworks_braket-1.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.4
+Version: 1.0.5
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<3.11.4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: amazon-braket-sdk (>=1.31.1,<2.0.0)
+Requires-Dist: amazon-braket-sdk (==1.42.1)
 Requires-Dist: llvmlite (==0.39.1)
-Requires-Dist: python-jose (>=3.3.0,<4.0.0)
-Requires-Dist: strangeworks (>=0.4.1,<0.5.0)
-Requires-Dist: strangeworks-python-core (>=0.1.6,<0.2.0)
-Requires-Dist: strawberryfields (>=0.23.0,<0.24.0)
+Requires-Dist: python-jose (==3.3.0)
+Requires-Dist: strangeworks (==0.4.4)
+Requires-Dist: strangeworks-core (==0.2.3)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
 more info or access to test features check out the
 [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |
 |---------------|:------------------------|
```

