# Comparing `tmp/dwave-gate-0.2.1.tar.gz` & `tmp/dwave-gate-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-gate-0.2.1.tar", last modified: Thu Jun  1 14:57:32 2023, max compression
+gzip compressed data, was "dwave-gate-0.3.0.tar", last modified: Tue Jul 18 18:58:57 2023, max compression
```

## Comparing `dwave-gate-0.2.1.tar` & `dwave-gate-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11351 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3791 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32825 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/circuit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4836 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/mixedproperty.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/operations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27036 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26782 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/operations/operations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5798 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/primitives.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.857528 dwave-gate-0.2.1/dwave/gate/registers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   617152 2023-06-01 14:57:31.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.cpp
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1332 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.pxd
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15052 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/cyregister.pyx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7049 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/registers/registers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave/gate/simulator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27915 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/operation_generation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43293 2023-06-01 14:57:30.000000 dwave-gate-0.2.1/dwave/gate/simulator/ops.h
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23912 2023-06-01 14:57:30.000000 dwave-gate-0.2.1/dwave/gate/simulator/ops.pxd
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1320438 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave/gate/simulator/simulator.cpp
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7582 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/simulator/simulator.pyx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave/gate/tools/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/counters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5789 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/tools/unitary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3140 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/dwave/gate/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/dwave_gate.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4740 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-01 14:57:32.000000 dwave-gate-0.2.1/dwave_gate.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1027 2023-06-01 14:57:32.861528 dwave-gate-0.2.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-06-01 14:57:20.000000 dwave-gate-0.2.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11351 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4771 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3872 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.045908 dwave-gate-0.3.0/dwave/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      678 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.045908 dwave-gate-0.3.0/dwave/gate/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      742 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35365 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/circuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4836 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/mixedproperty.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.045908 dwave-gate-0.3.0/dwave/gate/operations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/operations/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27920 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/operations/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26742 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/operations/operations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5798 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/primitives.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.045908 dwave-gate-0.3.0/dwave/gate/qir/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/qir/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14660 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/qir/compiler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7119 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/qir/instructions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6350 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/qir/loader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/dwave/gate/registers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/registers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   617152 2023-07-18 18:58:55.000000 dwave-gate-0.3.0/dwave/gate/registers/cyregister.cpp
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1332 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/registers/cyregister.pxd
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15052 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/registers/cyregister.pyx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7049 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/registers/registers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/dwave/gate/simulator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/simulator/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27915 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/simulator/operation_generation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43293 2023-07-18 18:58:54.000000 dwave-gate-0.3.0/dwave/gate/simulator/ops.h
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23912 2023-07-18 18:58:54.000000 dwave-gate-0.3.0/dwave/gate/simulator/ops.pxd
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1320438 2023-07-18 18:58:56.000000 dwave-gate-0.3.0/dwave/gate/simulator/simulator.cpp
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7582 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/simulator/simulator.pyx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/dwave/gate/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      957 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/tools/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3467 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/tools/counters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5790 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/dwave/gate/tools/unitary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-18 18:58:57.049908 dwave-gate-0.3.0/dwave_gate.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4771 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1057 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-18 18:58:57.000000 dwave-gate-0.3.0/dwave_gate.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1189 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-07-18 18:58:57.053908 dwave-gate-0.3.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-07-18 18:58:40.000000 dwave-gate-0.3.0/setup.py
```

### Comparing `dwave-gate-0.2.1/LICENSE` & `dwave-gate-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/PKG-INFO` & `dwave-gate-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: dwave-gate
-Version: 0.2.1
+Version: 0.3.0
 Summary: Gate model library.
 Home-page: https://github.com/dwavesystems/dwave-gate
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: UNKNOWN
 Download-URL: https://github.com/dwavesystems/dwave-gate/releases
 Platform: UNKNOWN
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/dwave-gate.svg
     :target: https://pypi.org/project/dwave-gate
 
 .. image:: https://img.shields.io/pypi/pyversions/dwave-gate.svg
@@ -73,18 +72,22 @@
 
     with circuit.context as (q, c):
         ops.X(q[0])
         ops.Hadamard(q[1])
         ops.CZ(q[0], q[1])
         ops.Hadamard(q[1])
 
-You can run the ``dwave.gate.simulator`` simulator on such circuits.
+You can run the ``dwave.gate.simulator`` simulator on such circuits,
 
 >>> from dwave.gate.simulator import simulate
 >>> simulate(circuit)
+
+and then access the resulting state via the state attribute.
+
+>>> circuit.state
 array([0.+0.j, 0.+0.j, 0.+0.j, 1.+0.j])
 
 .. example-end-marker
 
 Installation
 ------------
```

### Comparing `dwave-gate-0.2.1/README.rst` & `dwave-gate-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,22 @@
 
     with circuit.context as (q, c):
         ops.X(q[0])
         ops.Hadamard(q[1])
         ops.CZ(q[0], q[1])
         ops.Hadamard(q[1])
 
-You can run the ``dwave.gate.simulator`` simulator on such circuits.
+You can run the ``dwave.gate.simulator`` simulator on such circuits,
 
 >>> from dwave.gate.simulator import simulate
 >>> simulate(circuit)
+
+and then access the resulting state via the state attribute.
+
+>>> circuit.state
 array([0.+0.j, 0.+0.j, 0.+0.j, 1.+0.j])
 
 .. example-end-marker
 
 Installation
 ------------
```

### Comparing `dwave-gate-0.2.1/dwave/__init__.py` & `dwave-gate-0.3.0/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/__init__.py` & `dwave-gate-0.3.0/dwave/gate/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from dwave.gate.circuit import *
 from dwave.gate.mixedproperty import *
 from dwave.gate.primitives import *
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
```

### Comparing `dwave-gate-0.2.1/dwave/gate/circuit.py` & `dwave-gate-0.3.0/dwave/gate/circuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "Circuit",
     "ParametricCircuit",
     "CircuitContext",
     "ParametricCircuitContext",
 ]
 
 import copy
+from functools import cached_property
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Callable,
     ContextManager,
     Dict,
     Hashable,
@@ -59,15 +60,14 @@
 from dwave.gate.mixedproperty import mixedproperty
 from dwave.gate.primitives import Bit, Qubit
 from dwave.gate.registers.registers import (
     ClassicalRegister,
     QuantumRegister,
     SelfIncrementingRegister,
 )
-from dwave.gate.utils import cached_property
 
 if TYPE_CHECKING:
     from dwave.gate.operations.base import Operation
 
 Qubits = Union[Qubit, Sequence[Qubit]]
 Bits = Union[Bit, Sequence[Bit]]
 
@@ -103,43 +103,69 @@
             self.add_cregister(num_bits=num_bits)
 
         self._state: NDArray = None
         self._density_matrix: NDArray = None
 
         self._locked: bool = False
 
-    def __call__(self, qubits: Qubits) -> None:
+    def __call__(self, qubits: Qubits, bits: Optional[Bits] = None) -> None:
         """Apply all the operations in the circuit within a circuit context.
 
         Args:
             qubits: Qubits on which the circuit operations should be applied. The qubits used in
                 the circuit will be exchanged with the corresponding ones (e.g., with the same
                 index as) in the active context.
+            bits: Bits in which to store measurement values if measurements have been made.
 
         Raises:
             ValueError: If an invalid number of qubits is passed.
             CircuitError: If called outside of an active context.
         """
+        if CircuitContext.active_context is None:
+            raise CircuitError("Can only apply circuit object inside a circuit context.")
+        if CircuitContext.active_context.circuit is self:
+            raise TypeError("Cannot apply circuit in its own context.")
+
         if isinstance(qubits, Qubit):
             qubits = [qubits]
 
         if len(qubits) != len(self.qubits):
             raise ValueError(f"Circuit requires {len(self.qubits)} qubits, got {len(qubits)}.")
 
-        if CircuitContext.active_context is None:
-            raise CircuitError("Can only apply circuit object inside a circuit context.")
-        if CircuitContext.active_context.circuit is self:
-            raise TypeError("Cannot apply circuit in its own context.")
+        if bits:
+            if isinstance(bits, Bit):
+                bits = [bits]
+
+            if len(bits) != len(self.bits):
+                raise ValueError(f"Circuit requires {len(self.bits)} bits, got {len(bits)}.")
+
+            bit_map = dict(zip(self.bits, bits))
 
         qubit_map = dict(zip(self.qubits, qubits))
+
         for op in self.circuit:
             mapped_qubits = [qubit_map[qb] for qb in op.qubits or []]
 
             # NOTE: avoid circular imports; needed to check operation type
-            from dwave.gate.operations.base import ControlledOperation, ParametricOperation
+            from dwave.gate.operations.base import (
+                ControlledOperation,
+                Measurement,
+                ParametricOperation,
+            )
+
+            if isinstance(op, Measurement):
+                if bits:
+                    mapped_bits = [bit_map[qb] for qb in op.bits or []]
+                    op.__class__(qubits=mapped_qubits) | mapped_bits
+                    continue
+                else:
+                    warnings.warn(
+                        "Measurements not stored in circuit bits. "
+                        "Must pass bits to circuit call."
+                    )
 
             if isinstance(op, ParametricOperation):
                 op.__class__(op.parameters, qubits=mapped_qubits)
             elif isinstance(op, ControlledOperation):
                 op.__class__(*mapped_qubits)
             else:
                 op.__class__(qubits=mapped_qubits)
@@ -169,15 +195,15 @@
 
     def append(self, operation: Operation) -> None:
         """Appends an operation to the circuit.
 
         Args:
             operation: Operation to append to the circuit.
         """
-        if self.is_locked() == True:
+        if self.is_locked():
             raise CircuitError(
                 "Circuit is locked and no more operations can be appended. To "
                 "unlock the circuit, call 'Circuit.unlock()' first."
             )
         if not self.parametric:
             # if a parametric operation is called within a non-parameteric circuit, all variables
             # should be replaced by their corresponding parameter values; eval does that
@@ -412,15 +438,16 @@
             del self.bits
 
     def add_qregister(self, num_qubits: int = 0, label: Hashable = None) -> None:
         """Adds a new quantum register to the circuit.
 
         Args:
             num_qubits: Number of qubits in the quantum register (defaults to 0, i.e., empty).
-            label: Quantum register label (defaults to 'qreg' followed by a incrementing integer starting at 0).
+            label: Quantum register label (defaults to 'qreg' followed by a incrementing
+                integer starting at 0).
         """
         if label is None:
             label = f"qreg{len(self.qregisters)}"
 
         if label in self._qregisters:
             raise ValueError(f"Quantum register {label} already present in the circuit.")
 
@@ -433,15 +460,16 @@
             del self.qubits
 
     def add_cregister(self, num_bits: int = 0, label: Hashable = None) -> None:
         """Adds a new classical register to the circuit.
 
         Args:
             num_qubits: Number of bits in the classical register (defaults to 0, i.e., empty).
-            label: Classical register label (defaults to 'creg' followed by a incrementing integer starting at 0).
+            label: Classical register label (defaults to 'creg' followed by a incrementing
+                integer starting at 0).
         """
         if label is None:
             label = f"creg{len(self.cregisters)}"
 
         if label in self._cregisters:
             raise ValueError(f"Classical register {label} already present in the circuit")
 
@@ -624,77 +652,120 @@
         for op in self.circuit:
             if gate_definitions and hasattr(op, "_qasm_decl"):
                 header_str += "\n" + getattr(op, "_qasm_decl") + "\n"
             qasm_str += op.to_qasm(mapping) + ";\n"
 
         return header_str.strip() + "\n\n" + qasm_str.strip()
 
+    def to_qir(self, add_external: bool = False, bitcode: bool = False) -> Union[str, bytes]:
+        """Compile a circuit into QIR.
+
+        Args:
+            add_external: Whether to add external functions (not defined in QIR). If ``False``,
+                functions marked as external will be decomposed into valid operations (if possible).
+            bitcode: Whether to return QIR as a legible string or as bitcode.
+
+        Returns:
+            Union[str, bytes]: The QIR representation of the circuit.
+        """
+        # import outside toplevel to avoid circular imports
+        from dwave.gate.qir.compiler import qir_module
+
+        module = qir_module(self, add_external=add_external)
+        module.compile()
+
+        if bitcode:
+            return module.bitcode
+        return module.qir
+
+    @classmethod
+    def from_qir(cls, qir: Union[str, bytes], bitcode: bool = False) -> Circuit:
+        """Load a circuit from a QIR string or bitcode.
+
+        Args:
+            qir: The QIR string or bitcode to load into a circuit.
+            bitcode: Whether to expect the QIR as a string or as bitcode.
+
+        Returns:
+            Circuit: The circuit represented by the QIR string or bitcode.
+        """
+        # import outside toplevel to avoid circular imports
+        from dwave.gate.qir.loader import load_qir_bitcode, load_qir_string
+
+        if bitcode:
+            return load_qir_bitcode(qir, cls())
+        return load_qir_string(qir, cls())
+
 
 class ParametricCircuit(Circuit):
     """Class to build and manipulate parametric quantum circuits.
 
     Args:
         num_qubits: Number of qubits in the circuit.
         num_bits: Number of classical bits in the circuit.
     """
 
     def __init__(self, num_qubits: Optional[int] = None, num_bits: Optional[int] = None) -> None:
         self._parameter_register = SelfIncrementingRegister()
 
         super().__init__(num_qubits, num_bits)
 
-    def __call__(self, parameters: List[complex], qubits: Qubits) -> None:
+    def __call__(
+        self, parameters: List[complex], qubits: Qubits, bits: Optional[Bits] = None
+    ) -> None:
         """Apply all the operations in the circuit within a circuit context.
 
         Args:
             parameters: Parameters to apply to any parametric gates.
             qubits: Qubits on which the circuit operations should be applied. The qubits used in
                 the circuit will be exchanged with the corresponding ones (e.g., with the same
                 index as) in the active context.
+            bits: Bits in which to store measurement values if measurements have been made.
 
         Raises:
             ValueError: If an invalid number of qubits are passed.
             CircuitError: If called outside of an active context.
         """
         if CircuitContext.active_context:
             for i, var in enumerate(self._parameter_register):
                 var.set(parameters[i])
 
         # delay reset variables function call to on context exit
         CircuitContext.on_exit_functions.append(self.reset_variables)
 
-        return super().__call__(qubits=qubits)
+        return super().__call__(qubits=qubits, bits=bits)
 
     def unlock(self) -> None:
         """Unlocks the circuit allowing for further operations to be applied."""
         self._parameter_register._frozen = False
         return super().unlock()
 
     def eval(
-        self, parameters: Optional[Sequence[Sequence[complex]]] = None, in_place: bool = False
+        self, parameters: Optional[Sequence[Sequence[complex]]] = None, inplace: bool = False
     ) -> ParametricCircuit:
         """Evaluate circuit operations with explicit parameters.
 
         Args:
             parameters: Parameters to replace operation variables with. Overrides potential variable
                 values. If ``None`` then variable values are used (if existent).
-            in_place: Whether to evaluate the parameters on ``self`` or on a copy of ``self`` (returned).
+            inplace: Whether to evaluate the parameters on ``self`` or on a copy
+                of ``self`` (returned).
 
         Returns:
             ParametricOperation: Either ``self`` or a copy of ``self``.
 
         Raises:
             ValueError: If no parameters are passed and if variable has no set value.
         """
-        circuit = self if in_place else copy.deepcopy(self)
+        circuit = self if inplace else copy.deepcopy(self)
 
         for i, op in enumerate(circuit.circuit):
             eval = getattr(op, "eval", None)
             params = parameters[i] if parameters else None
-            circuit.circuit[i] = eval(params, in_place) if eval else op
+            circuit.circuit[i] = eval(params, inplace) if eval else op
 
         return circuit
 
     def reset_variables(self) -> None:
         """Resets any variables in the parameter register by setting their values to ``None``."""
         for variable in self._parameter_register:
             variable.reset()  # type: ignore
@@ -734,15 +805,15 @@
     """Class used to handle and store the active context.
 
     Args:
         circuit: Circuit to which the context is attached
     """
 
     _active_context: Optional[CircuitContext] = None
-    """Optional[CircuitContext]: Current active context; can only be one at a time during runtime."""
+    """Current active context; can only be one at a time during runtime."""
     on_exit_functions: List[Callable] = []
     """List of functions that should be called on context exit. Cleared on context exit."""
 
     def __init__(self, circuit: Circuit) -> None:
         self._circuit = circuit
         self._frozen = False
 
@@ -800,15 +871,15 @@
 
         return FrozenContext()
 
     def __enter__(
         self,
     ) -> Registers:
         """Enters the context and sets itself as active."""
-        if self.circuit.is_locked() == True:
+        if self.circuit.is_locked() is True:
             raise CircuitError(
                 "Circuit is locked and no more operations can be appended. To "
                 "unlock the circuit, call 'Circuit.unlock()' first."
             )
 
         if self.active_context is None:
             CircuitContext._active_context = self
```

### Comparing `dwave-gate-0.2.1/dwave/gate/mixedproperty.py` & `dwave-gate-0.3.0/dwave/gate/mixedproperty.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/operations/__init__.py` & `dwave-gate-0.3.0/dwave/gate/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/operations/base.py` & `dwave-gate-0.3.0/dwave/gate/operations/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,28 +49,33 @@
 
 import numpy as np
 
 from dwave.gate.circuit import Circuit, CircuitContext, CircuitError, ParametricCircuit
 from dwave.gate.mixedproperty import mixedproperty
 from dwave.gate.primitives import Bit, Qubit
 from dwave.gate.registers.registers import ClassicalRegister, Variable
-from dwave.gate.simulator.simulator import sample_qubit
 from dwave.gate.tools.unitary import build_controlled_unitary, build_unitary
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 Qubits = Union[Qubit, Sequence[Qubit]]
 Bits = Union[Bit, Sequence[Bit]]
 Parameters = Union[Variable, complex, Sequence[Union[Variable, complex]]]
 
 CustomOperation = TypeVar("CustomOperation", bound="Operation")
 CustomParametricOperation = TypeVar("CustomParametricOperation", bound="ParametricOperation")
 
+# Bounded type operations; exchange for 'typing.Self' after deprecating Python 3.10
+TOperation = TypeVar("TOperation", bound="Operation")
+TPOperation = TypeVar("TPOperation", bound="ParametricOperation")
+TCOperation = TypeVar("TCOperation", bound="ControlledOperation")
+TPCOperation = TypeVar("TPCOperation", bound="ParametricControlledOperation")
+
 
 class OperationError(Exception):
     """Exception to be raised when there is an error with an OperationError."""
 
 
 @overload
 def create_operation(circuit: ParametricCircuit, name: Optional[str] = None) -> Type[CustomParametricOperation]:  # type: ignore
@@ -239,23 +244,26 @@
         Returns:
             list: The OpenQASM 2.0 string representations of the operations qubits.
         """
         if mapping and self.qubits:
             return [f"{mapping[qb][0]}[{mapping[qb][1]}]" for qb in self.qubits]
         return [f"q[{i}]" for i in range(self.num_qubits)]
 
-    def __call__(self, qubits: Optional[Sequence[Qubit]] = None) -> None:
+    def __call__(self, qubits: Optional[Sequence[Qubit]] = None) -> TOperation:
         """Apply (or reapply) the operation within a context.
 
         Args:
             qubits: Qubits on which the operation should be applied. Only
                 required if not already declared in operation.
+
+        Returns:
+            Operation: The applied operation (copy of the called operation).
         """
         qubits = qubits or self.qubits
-        self.__class__(qubits)
+        return self.__class__(qubits)
 
     def __eq__(self, op: Operation) -> bool:
         """Returns whether two operations are considered equal."""
         name_eq = op.__class__.__name__ == self.__class__.__name__
         return name_eq and op.qubits == self.qubits
 
     def __str__(self) -> str:
@@ -379,30 +387,30 @@
 
     @property
     def parameters(self):
         """Parameters of the operation."""
         return self._parameters
 
     def eval(
-        self, parameters: Optional[Sequence[complex]] = None, in_place: bool = False
+        self, parameters: Optional[Sequence[complex]] = None, inplace: bool = False
     ) -> ParametricOperation:
         """Evaluate operation with explicit parameters.
 
         Args:
             parameters: Parameters to replace operation variables with. Overrides potential variable
                 values. If ``None`` then variable values are used (if existent).
-            in_place: Whether to evaluate the parameters on ``self`` or on a copy of ``self`` (returned).
+            inplace: Whether to evaluate the parameters on ``self`` or on a copy of ``self`` (returned).
 
         Returns:
             ParametricOperation: Either ``self`` or a copy of ``self``.
 
         Raises:
             ValueError: If no parameters are passed and if variable has no set value.
         """
-        op = self if in_place else copy.deepcopy(self)
+        op = self if inplace else copy.deepcopy(self)
 
         for i, p in enumerate(op.parameters):
             if isinstance(p, Variable):
                 if parameters:
                     op.parameters[i] = parameters[i]
                 elif p.value:
                     op.parameters[i] = p.value
@@ -438,23 +446,26 @@
                 f"Operation '{cls.name} requires "
                 f"{cls._num_params} parameters, got {len(params)}."
             )
 
         # cast to list for convention
         return list(params)
 
-    def __call__(self, qubits: Optional[Sequence[Qubit]] = None):
+    def __call__(self, qubits: Optional[Sequence[Qubit]] = None) -> TPOperation:
         """Apply (or reapply) the operation within a context.
 
         Args:
             qubits: Qubits on which the operation should be applied. Only
                 required if not already declared in operation.
+
+        Returns:
+            Operation: The applied operation (copy of the called operation).
         """
         qubits = qubits or self.qubits
-        self.__class__(self.parameters, qubits)
+        return self.__class__(self.parameters, qubits)
 
 
 class ControlledOperation(Operation):
     """Generic controlled operation.
 
     Args:
         control: Qubit(s) on which the target operation is controlled.
@@ -502,26 +513,29 @@
 
         super().__init__(qubits=qubits, **kwargs)
 
     def __call__(
         self,
         control: Optional[Sequence[Qubit]] = None,
         target: Optional[Sequence[Qubit]] = None,
-    ):
+    ) -> TCOperation:
         """Apply (or reapply) the operation within a context.
 
         Args:
             control: Control qubits. Only required if not already declared in operation.
             target: Target qubits on which the operation should be applied. Only
                 required if not already declared in operation.
+
+        Returns:
+            Operation: The applied operation (copy of the called operation).
         """
         control = control or self.control
         target = target or self.target
 
-        self.__class__(control, target)  # type: ignore
+        return self.__class__(control, target)  # type: ignore
 
     @mixedproperty
     def num_qubits(cls, self) -> int:
         """Number of qubits that the operation supports."""
         if not cls._num_qubits and cls.num_control and cls.num_target:
             cls._num_qubits = cls.num_control + cls.num_target
 
@@ -617,26 +631,29 @@
     ):
         # ControlledOperation.__init__(self, control, target, **kwargs)
         super().__init__(control, target, parameters=parameters, **kwargs)
         self._parameters = self._check_parameters(parameters)
 
     def __call__(
         self, control: Optional[Sequence[Qubit]] = None, target: Optional[Sequence[Qubit]] = None
-    ):
+    ) -> TPCOperation:
         """Apply (or reapply) the operation within a context.
 
         Args:
             control: Control qubits. Only required if not already declared in operation.
             target: Target qubits on which the operation should be applied. Only
                 required if not already declared in operation.
+
+        Returns:
+            Operation: The applied operation (copy of the called operation).
         """
         control = control or self.control
         target = target or self.target
 
-        self.__class__(self.parameters, control, target)  # type: ignore
+        return self.__class__(self.parameters, control, target)  # type: ignore
 
     @mixedproperty(self_required=True)
     def matrix(cls, self) -> NDArray:
         """The matrix representation of the parametric controlled operation."""
         self._target_matrix = cls.target_operation(self.parameters).matrix
 
         # signature of super required for correct self to be passed along (do not remove)
@@ -705,14 +722,17 @@
             num_samples: The number of samples to to return.
             as_bitstring: Whether to return the samples as bitstrings or as
                 lists of integers (default).
 
         Returns:
             List[Union[int, str]]: The measurement samples for each qubit.
         """
+        # NOTE: avoid circular imports; operations used in simulator
+        from dwave.gate.simulator.simulator import sample_qubit
+
         if self.state is None:
             raise CircuitError(
                 "Measurement has no state. Likely due to circuit not having been simulated."
             )
 
         if qubits is None:
             qubits = self._measured_qubit_indices
```

### Comparing `dwave-gate-0.2.1/dwave/gate/operations/operations.py` & `dwave-gate-0.3.0/dwave/gate/operations/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     "CHadamard",
     "CRX",
     "CRY",
     "CRZ",
     "CRotation",
     "CSWAP",
     "Fredkin",  # alias
-    "CCNOT",
-    "CCX",  # alias
+    "CCX",
+    "CCNOT",  # alias
     "Toffoli",  # alias
 ]
 
 import cmath
 import math
 from typing import Mapping, Optional, Type
 
@@ -66,15 +66,14 @@
 from dwave.gate.mixedproperty import mixedproperty
 from dwave.gate.operations.base import (
     ControlledOperation,
     Operation,
     ParametricControlledOperation,
     ParametricOperation,
 )
-from dwave.gate.primitives import Qubit
 
 #####################################
 # Non-parametric single-qubit gates #
 #####################################
 
 
 class Identity(Operation):
```

### Comparing `dwave-gate-0.2.1/dwave/gate/primitives.py` & `dwave-gate-0.3.0/dwave/gate/primitives.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/registers/__init__.py` & `dwave-gate-0.3.0/dwave/gate/registers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/registers/cyregister.cpp` & `dwave-gate-0.3.0/dwave/gate/registers/cyregister.cpp`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/registers/cyregister.pxd` & `dwave-gate-0.3.0/dwave/gate/registers/cyregister.pxd`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/registers/cyregister.pyx` & `dwave-gate-0.3.0/dwave/gate/registers/cyregister.pyx`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/registers/registers.py` & `dwave-gate-0.3.0/dwave/gate/registers/registers.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/__init__.py` & `dwave-gate-0.3.0/dwave/gate/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/operation_generation.py` & `dwave-gate-0.3.0/dwave/gate/simulator/operation_generation.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/ops.h` & `dwave-gate-0.3.0/dwave/gate/simulator/ops.h`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/ops.pxd` & `dwave-gate-0.3.0/dwave/gate/simulator/ops.pxd`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/simulator.cpp` & `dwave-gate-0.3.0/dwave/gate/simulator/simulator.cpp`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/simulator/simulator.pyx` & `dwave-gate-0.3.0/dwave/gate/simulator/simulator.pyx`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/tools/__init__.py` & `dwave-gate-0.3.0/dwave/gate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/tools/counters.py` & `dwave-gate-0.3.0/dwave/gate/tools/counters.py`

 * *Files identical despite different names*

### Comparing `dwave-gate-0.2.1/dwave/gate/tools/unitary.py` & `dwave-gate-0.3.0/dwave/gate/tools/unitary.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     from dwave.gate.operations.base import ControlledOperation, Operation
 
 
 #####################
 # Circuit functions #
 #####################
 
+
 # TODO: exchange for something better; only here for testing matrix creation
 # for custom operations; controlled operations only works with single
 # control and target; no support for any other multi-qubit gates
 @lru_cache(maxsize=128)
 def build_unitary(circuit) -> NDArray:
     """Builds the circuit unitary by multiplying together the operation matrices.
```

### Comparing `dwave-gate-0.2.1/dwave_gate.egg-info/PKG-INFO` & `dwave-gate-0.3.0/dwave_gate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: dwave-gate
-Version: 0.2.1
+Version: 0.3.0
 Summary: Gate model library.
 Home-page: https://github.com/dwavesystems/dwave-gate
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: UNKNOWN
 Download-URL: https://github.com/dwavesystems/dwave-gate/releases
 Platform: UNKNOWN
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/dwave-gate.svg
     :target: https://pypi.org/project/dwave-gate
 
 .. image:: https://img.shields.io/pypi/pyversions/dwave-gate.svg
@@ -73,18 +72,22 @@
 
     with circuit.context as (q, c):
         ops.X(q[0])
         ops.Hadamard(q[1])
         ops.CZ(q[0], q[1])
         ops.Hadamard(q[1])
 
-You can run the ``dwave.gate.simulator`` simulator on such circuits.
+You can run the ``dwave.gate.simulator`` simulator on such circuits,
 
 >>> from dwave.gate.simulator import simulate
 >>> simulate(circuit)
+
+and then access the resulting state via the state attribute.
+
+>>> circuit.state
 array([0.+0.j, 0.+0.j, 0.+0.j, 1.+0.j])
 
 .. example-end-marker
 
 Installation
 ------------
```

### Comparing `dwave-gate-0.2.1/dwave_gate.egg-info/SOURCES.txt` & `dwave-gate-0.3.0/dwave_gate.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 setup.cfg
 setup.py
 dwave/__init__.py
 dwave/gate/__init__.py
 dwave/gate/circuit.py
 dwave/gate/mixedproperty.py
 dwave/gate/primitives.py
-dwave/gate/utils.py
 dwave/gate/operations/__init__.py
 dwave/gate/operations/base.py
 dwave/gate/operations/operations.py
+dwave/gate/qir/__init__.py
+dwave/gate/qir/compiler.py
+dwave/gate/qir/instructions.py
+dwave/gate/qir/loader.py
 dwave/gate/registers/__init__.py
 dwave/gate/registers/cyregister.cpp
 dwave/gate/registers/cyregister.pxd
 dwave/gate/registers/cyregister.pyx
 dwave/gate/registers/registers.py
 dwave/gate/simulator/__init__.py
 dwave/gate/simulator/operation_generation.py
```

### Comparing `dwave-gate-0.2.1/pyproject.toml` & `dwave-gate-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'oldest-supported-numpy',
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.cibuildwheel]
 build-verbosity = "1"
 skip = "pp* *musllinux*"
-before-test = "pip install -r {project}/requirements_dev.txt"
+before-test = "pip install pyqir==0.8.2 && pip install -r {project}/requirements_dev.txt"
 test-command = "pytest {project}/tests"
 before-build = "pip install cgen==2020.1 && python {project}/dwave/gate/simulator/operation_generation.py"
 
 [tool.cibuildwheel.linux]
 archs = "x86_64 aarch64"
 manylinux-x86_64-image = "manylinux2014"
 manylinux-aarch64-image = "manylinux2014"
@@ -24,9 +24,13 @@
 archs = "x86_64 arm64"
 
 [tool.cibuildwheel.windows]
 archs = "AMD64"
 # before-build = "pip install delvewheel"
 # repair-wheel-command = "delvewheel repair -w {dest_dir} {wheel}"
 
+[[tool.cibuildwheel.overrides]]
+select = "*aarch64*"
+before-test = "pip install -r {project}/requirements_dev.txt"
+
 [tool.pyright]
 reportUnusedExpression = false
```

### Comparing `dwave-gate-0.2.1/setup.cfg` & `dwave-gate-0.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 classifiers = 
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -18,15 +17,15 @@
 download_url = https://github.com/dwavesystems/dwave-gate/releases
 version = attr: dwave.gate.__version__
 author = D-Wave Systems Inc.
 author_email = tools@dwavesys.com
 description = Gate model library.
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 zip_safe = False
 
 [pycodestyle]
 max-line-length = 100
 
 [tool:pytest]
```

### Comparing `dwave-gate-0.2.1/setup.py` & `dwave-gate-0.3.0/setup.py`

 * *Files identical despite different names*

