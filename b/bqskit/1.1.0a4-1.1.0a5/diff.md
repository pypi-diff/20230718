# Comparing `tmp/bqskit-1.1.0a4.tar.gz` & `tmp/bqskit-1.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqskit-1.1.0a4.tar", last modified: Tue Jul 18 11:33:04 2023, max compression
+gzip compressed data, was "bqskit-1.1.0a5.tar", last modified: Tue Jul 18 11:35:06 2023, max compression
```

## Comparing `bqskit-1.1.0a4.tar` & `bqskit-1.1.0a5.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.693669 bqskit-1.1.0a4/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2527 2022-09-19 11:52:09.000000 bqskit-1.1.0a4/LICENSE
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4849 2023-07-18 11:33:17.693669 bqskit-1.1.0a4/PKG-INFO
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3338 2022-09-19 11:52:09.000000 bqskit-1.1.0a4/README.md
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.440333 bqskit-1.1.0a4/bqskit/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2954 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.456999 bqskit-1.1.0a4/bqskit/compiler/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1568 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6098 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/basepass.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    51186 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/compiler/compile.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    19140 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/compiler.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7955 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/gateset.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4043 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/machine.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7432 2023-07-15 16:56:39.000000 bqskit-1.1.0a4/bqskit/compiler/passdata.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      242 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/status.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/task.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3529 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/compiler/workflow.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.456999 bqskit-1.1.0a4/bqskit/exec/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1085 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/exec/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      685 2023-01-19 22:11:21.000000 bqskit-1.1.0a4/bqskit/exec/results.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      575 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/exec/runner.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.463666 bqskit-1.1.0a4/bqskit/exec/runners/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      461 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/exec/runners/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1174 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/exec/runners/ibmq.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12733 2023-07-15 16:54:41.000000 bqskit-1.1.0a4/bqskit/exec/runners/quest.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      675 2022-09-19 11:52:09.000000 bqskit-1.1.0a4/bqskit/exec/runners/sim.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.466999 bqskit-1.1.0a4/bqskit/ext/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ext/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.466999 bqskit-1.1.0a4/bqskit/ext/cirq/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      256 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ext/cirq/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2221 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/ext/cirq/models.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1208 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ext/cirq/translate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      569 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/ext/honeywell.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.470333 bqskit-1.1.0a4/bqskit/ext/pytket/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      270 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ext/pytket/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1269 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ext/pytket/translate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.473666 bqskit-1.1.0a4/bqskit/ext/qiskit/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      348 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ext/qiskit/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-07-15 16:54:47.000000 bqskit-1.1.0a4/bqskit/ext/qiskit/models.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1219 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ext/qiskit/translate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.473666 bqskit-1.1.0a4/bqskit/ext/qutip/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      263 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ext/qutip/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1279 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ext/qutip/translate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2281 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/ext/rigetti.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1951 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ext/supermarq.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.487000 bqskit-1.1.0a4/bqskit/ir/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2161 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)   112825 2023-07-15 14:06:43.000000 bqskit-1.1.0a4/bqskit/ir/circuit.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1822 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ir/gate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.497000 bqskit-1.1.0a4/bqskit/ir/gates/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2796 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1158 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/barrier.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5017 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/circuitgate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.500333 bqskit-1.1.0a4/bqskit/ir/gates/composed/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      516 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4045 2023-01-19 20:43:03.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/controlled.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3483 2023-01-19 20:43:03.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/daggergate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7183 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/frozenparam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3144 2023-01-19 20:43:03.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/tagged.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7673 2022-10-27 12:13:07.000000 bqskit-1.1.0a4/bqskit/ir/gates/composed/vlg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2308 2023-01-19 22:11:21.000000 bqskit-1.1.0a4/bqskit/ir/gates/composedgate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.533667 bqskit-1.1.0a4/bqskit/ir/gates/constant/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2969 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      895 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/b.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1260 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/ccx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      915 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/ch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1242 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/clock.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1313 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/cpi.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      748 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/cs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1391 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/csum.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1447 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/csumd.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      812 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/ct.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      798 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/cx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      751 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/cy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      749 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/cz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      756 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/h.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1493 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/hd.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2299 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/identity.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1126 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/iswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1472 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/itoffoli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1680 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/pd.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1463 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/permutation.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2087 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/rccx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      561 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/s.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      576 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/sdg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1261 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/shift.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      922 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/sqrtcnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      952 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/sqrtiswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2951 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/subswap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1715 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/swap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      786 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/sx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      845 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/sycamore.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      620 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/t.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/tdg.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1163 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      604 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/x.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1076 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/xx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      608 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/y.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1072 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/yy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      606 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/z.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1100 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constant/zz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1816 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/constantgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1355 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/generalgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2420 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/measure.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.553667 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1818 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2518 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ccp.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1820 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cp.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2524 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cphase.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2005 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/crx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1998 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cry.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1970 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/crz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3439 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cu.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2444 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/fsim.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3411 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/pauli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2772 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/phasedxz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2415 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2903 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rxx.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2402 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ry.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2239 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ryy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1754 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2052 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rzz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2212 2023-03-22 18:11:26.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u1.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2275 2023-07-13 18:28:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u1q.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2118 2022-08-31 17:16:53.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u2.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3617 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7452 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u8.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3135 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/gates/parameterized/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      354 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/qubitgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      630 2023-07-15 13:59:20.000000 bqskit-1.1.0a4/bqskit/ir/gates/quditgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      357 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/gates/qutritgate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6710 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/interval.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13048 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/iterator.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.553667 bqskit-1.1.0a4/bqskit/ir/lang/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      517 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/lang/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      615 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/lang/language.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.557000 bqskit-1.1.0a4/bqskit/ir/lang/qasm2/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      344 2022-08-17 01:47:54.000000 bqskit-1.1.0a4/bqskit/ir/lang/qasm2/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2666 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/lang/qasm2/parser.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1194 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/lang/qasm2/qasm2.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    31359 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/lang/qasm2/visitor.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7090 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/location.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4843 2023-07-15 16:35:30.000000 bqskit-1.1.0a4/bqskit/ir/operation.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.560334 bqskit-1.1.0a4/bqskit/ir/opt/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1501 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/opt/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.567000 bqskit-1.1.0a4/bqskit/ir/opt/cost/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1108 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2284 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/differentiable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1147 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/function.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.567000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      563 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/__init__.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.567000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/cost/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      288 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/cost/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1541 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.570334 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/residuals/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      318 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/residuals/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1602 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2258 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/generator.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1391 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/cost/residual.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6696 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/instantiater.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.573667 bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      382 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3027 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/minimization.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2641 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/qfactor.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1048 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/minimizer.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.573667 bqskit-1.1.0a4/bqskit/ir/opt/minimizers/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      339 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/opt/minimizers/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1802 2023-02-28 01:32:46.000000 bqskit-1.1.0a4/bqskit/ir/opt/minimizers/ceres.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      471 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/minimizers/lbfgs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1020 2023-07-15 16:55:35.000000 bqskit-1.1.0a4/bqskit/ir/opt/minimizers/scipy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1217 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/multistartgen.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.577001 bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      293 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1953 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/diagonal.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1826 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/random.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3477 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/point.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14991 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/ir/region.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1828 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/ir/structure.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.580334 bqskit-1.1.0a4/bqskit/passes/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    10691 2023-07-15 14:12:48.000000 bqskit-1.1.0a4/bqskit/passes/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      778 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/alias.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.587001 bqskit-1.1.0a4/bqskit/passes/control/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1260 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/control/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2346 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/dothendecide.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1681 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/dowhileloop.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8140 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/foreach.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1960 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/ifthenelse.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3330 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/paralleldo.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1012 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.597001 bqskit-1.1.0a4/bqskit/passes/control/predicates/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      972 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1201 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/andpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1984 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/change.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/count.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1013 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/multi.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1027 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/notpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1196 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/orpredicate.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      739 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/physical.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1018 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/single.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1073 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/predicates/width.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1516 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/control/whileloop.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      919 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/group.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.600334 bqskit-1.1.0a4/bqskit/passes/io/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      466 2022-08-13 15:35:15.000000 bqskit-1.1.0a4/bqskit/passes/io/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1740 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/io/checkpoint.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7234 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/io/intermediate.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.603668 bqskit-1.1.0a4/bqskit/passes/mapping/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1050 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      939 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/apply.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8207 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/embed.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.607001 bqskit-1.1.0a4/bqskit/passes/mapping/layout/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      385 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/layout/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3241 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/layout/pam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2802 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/layout/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13590 2023-07-15 16:40:50.000000 bqskit-1.1.0a4/bqskit/passes/mapping/pam.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.610334 bqskit-1.1.0a4/bqskit/passes/mapping/placement/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      402 2023-07-13 16:33:54.000000 bqskit-1.1.0a4/bqskit/passes/mapping/placement/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2179 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/placement/greedy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1046 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/placement/trivial.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.610334 bqskit-1.1.0a4/bqskit/passes/mapping/routing/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      367 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/routing/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1682 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/routing/pam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1229 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/routing/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    18683 2023-07-15 16:41:02.000000 bqskit-1.1.0a4/bqskit/passes/mapping/sabre.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1214 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/mapping/setmodel.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9823 2023-07-15 16:37:33.000000 bqskit-1.1.0a4/bqskit/passes/mapping/topology.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/measure.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      456 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/noop.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.617001 bqskit-1.1.0a4/bqskit/passes/partitioning/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      641 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3250 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/cluster.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8805 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/greedy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13108 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/quick.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13619 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/scan.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1786 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/partitioning/single.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.620334 bqskit-1.1.0a4/bqskit/passes/processing/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      616 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/processing/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6358 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/processing/exhaustive.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3388 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/passes/processing/iterative.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12368 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/processing/rebase.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5282 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/processing/scan.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5143 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/processing/substitute.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.630335 bqskit-1.1.0a4/bqskit/passes/rules/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      710 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/rules/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/rules/ch2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/rules/cnot2ch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/rules/cnot2cy.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-07-15 16:50:38.000000 bqskit-1.1.0a4/bqskit/passes/rules/cnot2cz.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/rules/cy2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-07-15 16:51:29.000000 bqskit-1.1.0a4/bqskit/passes/rules/cz2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1567 2023-07-15 16:51:45.000000 bqskit-1.1.0a4/bqskit/passes/rules/swap2cnot.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1032 2023-07-15 16:51:51.000000 bqskit-1.1.0a4/bqskit/passes/rules/u3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1753 2023-07-15 16:56:39.000000 bqskit-1.1.0a4/bqskit/passes/rules/zxzxz.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.633668 bqskit-1.1.0a4/bqskit/passes/search/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      731 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/passes/search/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2425 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/frontier.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      926 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/generator.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.640335 bqskit-1.1.0a4/bqskit/passes/search/generators/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      810 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4173 2023-07-15 16:52:38.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/fourparam.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2606 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/middleout.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4132 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/seed.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7161 2023-07-15 16:52:51.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/simple.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4032 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/single.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2358 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/stair.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5056 2023-07-15 16:53:06.000000 bqskit-1.1.0a4/bqskit/passes/search/generators/wide.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1287 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/heuristic.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.640335 bqskit-1.1.0a4/bqskit/passes/search/heuristics/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      368 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/passes/search/heuristics/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2737 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/heuristics/astar.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1115 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/heuristics/dijkstra.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1617 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/search/heuristics/greedy.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.647001 bqskit-1.1.0a4/bqskit/passes/synthesis/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      771 2023-07-15 14:12:54.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12455 2023-07-15 14:17:22.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/leap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4261 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/pas.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    10759 2023-07-15 16:56:15.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/qfast.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12979 2023-07-15 16:53:31.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/qpredict.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8602 2023-07-15 14:17:22.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/qsearch.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1729 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/synthesis.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1230 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/synthesis/target.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.657002 bqskit-1.1.0a4/bqskit/passes/util/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      931 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/passes/util/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      618 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/compress.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5023 2023-07-15 16:53:49.000000 bqskit-1.1.0a4/bqskit/passes/util/conversion.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1321 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/converttou3.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3549 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/extend.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2716 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/fill.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1940 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/log.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1019 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/random.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1403 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/record.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/unfold.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1091 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/passes/util/update.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.660335 bqskit-1.1.0a4/bqskit/qis/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2154 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20134 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/graph.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8060 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/pauli.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4943 2023-01-23 16:58:30.000000 bqskit-1.1.0a4/bqskit/qis/permutation.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.663668 bqskit-1.1.0a4/bqskit/qis/state/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      462 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/state/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14029 2023-07-15 16:55:57.000000 bqskit-1.1.0a4/bqskit/qis/state/state.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      660 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/state/statemap.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3713 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/state/system.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.670335 bqskit-1.1.0a4/bqskit/qis/unitary/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      808 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/differentiable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1282 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/meta.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1739 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/optimizable.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3813 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/unitary.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12154 2023-01-19 20:43:03.000000 bqskit-1.1.0a4/bqskit/qis/unitary/unitarybuilder.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15603 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/qis/unitary/unitarymatrix.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.680335 bqskit-1.1.0a4/bqskit/runtime/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6364 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      551 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/address.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3319 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/attached.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    22189 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/base.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15713 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/detached.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      530 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/direction.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1659 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/future.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    11817 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/manager.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      441 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/message.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      379 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/result.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3734 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/task.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    25392 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/runtime/worker.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.687002 bqskit-1.1.0a4/bqskit/utils/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      593 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/utils/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2342 2022-09-19 11:52:10.000000 bqskit-1.1.0a4/bqskit/utils/cachedclass.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      408 2023-01-19 20:43:03.000000 bqskit-1.1.0a4/bqskit/utils/docs.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4311 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/utils/math.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      525 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/utils/random.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.690335 bqskit-1.1.0a4/bqskit/utils/test/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      371 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/utils/test/__init__.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13812 2023-07-15 16:37:50.000000 bqskit-1.1.0a4/bqskit/utils/test/strategies.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20786 2022-08-13 15:35:16.000000 bqskit-1.1.0a4/bqskit/utils/test/types.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5284 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/utils/typing.py
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      216 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/bqskit/version.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.446999 bqskit-1.1.0a4/bqskit.egg-info/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4849 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/PKG-INFO
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9576 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/SOURCES.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)        1 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/dependency_links.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      181 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/entry_points.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)      145 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/requires.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)        7 2023-07-18 11:33:17.000000 bqskit-1.1.0a4/bqskit.egg-info/top_level.txt
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1021 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/pyproject.toml
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)       38 2023-07-18 11:33:17.693669 bqskit-1.1.0a4/setup.cfg
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3030 2023-07-15 13:59:16.000000 bqskit-1.1.0a4/setup.py
-drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:33:17.690335 bqskit-1.1.0a4/tests/
--rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6031 2022-09-19 11:52:11.000000 bqskit-1.1.0a4/tests/test_conftest.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.961706 bqskit-1.1.0a5/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2527 2022-09-19 11:52:09.000000 bqskit-1.1.0a5/LICENSE
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4849 2023-07-18 11:35:19.961706 bqskit-1.1.0a5/PKG-INFO
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3338 2022-09-19 11:52:09.000000 bqskit-1.1.0a5/README.md
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.725037 bqskit-1.1.0a5/bqskit/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2954 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.738370 bqskit-1.1.0a5/bqskit/compiler/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1568 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6098 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/basepass.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    51186 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/compiler/compile.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    19140 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/compiler.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7955 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/gateset.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4043 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/machine.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7432 2023-07-15 16:56:39.000000 bqskit-1.1.0a5/bqskit/compiler/passdata.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      242 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/status.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/task.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3529 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/compiler/workflow.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.741703 bqskit-1.1.0a5/bqskit/exec/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1085 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/exec/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      685 2023-01-19 22:11:21.000000 bqskit-1.1.0a5/bqskit/exec/results.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      575 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/exec/runner.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.745037 bqskit-1.1.0a5/bqskit/exec/runners/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      461 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/exec/runners/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1174 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/exec/runners/ibmq.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12733 2023-07-15 16:54:41.000000 bqskit-1.1.0a5/bqskit/exec/runners/quest.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      675 2022-09-19 11:52:09.000000 bqskit-1.1.0a5/bqskit/exec/runners/sim.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.751704 bqskit-1.1.0a5/bqskit/ext/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ext/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.751704 bqskit-1.1.0a5/bqskit/ext/cirq/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      256 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ext/cirq/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2221 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/ext/cirq/models.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1208 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ext/cirq/translate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      569 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/ext/honeywell.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.755037 bqskit-1.1.0a5/bqskit/ext/pytket/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      270 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ext/pytket/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1269 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ext/pytket/translate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.758370 bqskit-1.1.0a5/bqskit/ext/qiskit/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      348 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ext/qiskit/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1923 2023-07-15 16:54:47.000000 bqskit-1.1.0a5/bqskit/ext/qiskit/models.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1219 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ext/qiskit/translate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.758370 bqskit-1.1.0a5/bqskit/ext/qutip/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      263 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ext/qutip/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1279 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ext/qutip/translate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2281 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/ext/rigetti.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1951 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ext/supermarq.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.768370 bqskit-1.1.0a5/bqskit/ir/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2161 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)   112825 2023-07-15 14:06:43.000000 bqskit-1.1.0a5/bqskit/ir/circuit.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1822 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ir/gate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.778370 bqskit-1.1.0a5/bqskit/ir/gates/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2796 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1158 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/barrier.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5017 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/circuitgate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.781704 bqskit-1.1.0a5/bqskit/ir/gates/composed/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      516 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4045 2023-01-19 20:43:03.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/controlled.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3483 2023-01-19 20:43:03.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/daggergate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7183 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/frozenparam.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3144 2023-01-19 20:43:03.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/tagged.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7673 2022-10-27 12:13:07.000000 bqskit-1.1.0a5/bqskit/ir/gates/composed/vlg.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2308 2023-01-19 22:11:21.000000 bqskit-1.1.0a5/bqskit/ir/gates/composedgate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.818371 bqskit-1.1.0a5/bqskit/ir/gates/constant/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2969 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      895 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/b.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1260 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/ccx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      915 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/ch.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1242 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/clock.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1313 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/cpi.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      748 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/cs.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1391 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/csum.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1447 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/csumd.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      812 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/ct.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      798 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/cx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      751 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/cy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      749 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/cz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      756 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/h.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1493 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/hd.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2299 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/identity.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1126 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/iswap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1472 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/itoffoli.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1680 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/pd.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1463 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/permutation.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2087 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/rccx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      561 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/s.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      576 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/sdg.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1261 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/shift.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      922 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/sqrtcnot.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      952 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/sqrtiswap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2951 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/subswap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1715 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/swap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      786 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/sx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      845 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/sycamore.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      620 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/t.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/tdg.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1163 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/unitary.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      604 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/x.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1076 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/xx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      608 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/y.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1072 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/yy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      606 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/z.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1100 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constant/zz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1816 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/constantgate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1355 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/generalgate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2420 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/measure.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.838371 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1818 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2518 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ccp.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1820 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cp.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2524 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cphase.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2005 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/crx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1998 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cry.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1970 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/crz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3439 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cu.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2444 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/fsim.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3411 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/pauli.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2772 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/phasedxz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2415 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2903 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rxx.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2402 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ry.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2239 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ryy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1754 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2052 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rzz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2212 2023-03-22 18:11:26.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u1.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2275 2023-07-13 18:28:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u1q.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2118 2022-08-31 17:16:53.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u2.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3617 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u3.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7452 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u8.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3135 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/gates/parameterized/unitary.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      354 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/qubitgate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      630 2023-07-15 13:59:20.000000 bqskit-1.1.0a5/bqskit/ir/gates/quditgate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      357 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/gates/qutritgate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6710 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/interval.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13048 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/iterator.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.841705 bqskit-1.1.0a5/bqskit/ir/lang/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      517 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/lang/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      615 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/lang/language.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.845038 bqskit-1.1.0a5/bqskit/ir/lang/qasm2/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      344 2022-08-17 01:47:54.000000 bqskit-1.1.0a5/bqskit/ir/lang/qasm2/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2666 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/lang/qasm2/parser.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1194 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/lang/qasm2/qasm2.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    31359 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/lang/qasm2/visitor.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7090 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/location.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4843 2023-07-15 16:35:30.000000 bqskit-1.1.0a5/bqskit/ir/operation.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.848371 bqskit-1.1.0a5/bqskit/ir/opt/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1501 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/opt/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.851705 bqskit-1.1.0a5/bqskit/ir/opt/cost/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1108 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2284 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/differentiable.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1147 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/function.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.851705 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      563 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/__init__.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.855038 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/cost/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      288 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/cost/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1541 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.858372 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/residuals/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      318 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/residuals/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1602 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2258 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/generator.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1391 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/cost/residual.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6696 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/instantiater.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.858372 bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      382 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3027 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/minimization.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2641 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/qfactor.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1048 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/minimizer.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.865038 bqskit-1.1.0a5/bqskit/ir/opt/minimizers/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      339 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/opt/minimizers/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1802 2023-02-28 01:32:46.000000 bqskit-1.1.0a5/bqskit/ir/opt/minimizers/ceres.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      471 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/minimizers/lbfgs.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1020 2023-07-15 16:55:35.000000 bqskit-1.1.0a5/bqskit/ir/opt/minimizers/scipy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1217 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/multistartgen.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.865038 bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      293 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1953 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/diagonal.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1826 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/random.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3477 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/point.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14991 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/ir/region.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1828 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/ir/structure.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.871705 bqskit-1.1.0a5/bqskit/passes/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    10691 2023-07-15 14:12:48.000000 bqskit-1.1.0a5/bqskit/passes/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      778 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/alias.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.875038 bqskit-1.1.0a5/bqskit/passes/control/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1260 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/control/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2346 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/dothendecide.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1681 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/dowhileloop.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8140 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/foreach.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1960 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/ifthenelse.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3330 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/paralleldo.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1012 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.885038 bqskit-1.1.0a5/bqskit/passes/control/predicates/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      972 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1201 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/andpredicate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1984 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/change.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1796 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/count.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1013 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/multi.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1027 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/notpredicate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1196 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/orpredicate.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      739 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/physical.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1018 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/single.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1073 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/predicates/width.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1516 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/control/whileloop.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      919 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/group.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.885038 bqskit-1.1.0a5/bqskit/passes/io/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      466 2022-08-13 15:35:15.000000 bqskit-1.1.0a5/bqskit/passes/io/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1740 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/io/checkpoint.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7234 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/io/intermediate.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.891705 bqskit-1.1.0a5/bqskit/passes/mapping/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1050 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      939 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/apply.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8207 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/embed.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.895039 bqskit-1.1.0a5/bqskit/passes/mapping/layout/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      385 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/layout/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3241 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/layout/pam.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2802 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/layout/sabre.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13590 2023-07-15 16:40:50.000000 bqskit-1.1.0a5/bqskit/passes/mapping/pam.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.895039 bqskit-1.1.0a5/bqskit/passes/mapping/placement/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      402 2023-07-13 16:33:54.000000 bqskit-1.1.0a5/bqskit/passes/mapping/placement/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2179 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/placement/greedy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1046 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/placement/trivial.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.898372 bqskit-1.1.0a5/bqskit/passes/mapping/routing/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      367 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/routing/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1682 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/routing/pam.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1229 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/routing/sabre.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    18683 2023-07-15 16:41:02.000000 bqskit-1.1.0a5/bqskit/passes/mapping/sabre.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1214 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/mapping/setmodel.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9823 2023-07-15 16:37:33.000000 bqskit-1.1.0a5/bqskit/passes/mapping/topology.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/measure.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      456 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/noop.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.901705 bqskit-1.1.0a5/bqskit/passes/partitioning/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      641 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3250 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/cluster.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8805 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/greedy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13108 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/quick.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13619 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/scan.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1786 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/partitioning/single.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.908372 bqskit-1.1.0a5/bqskit/passes/processing/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      616 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/processing/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6358 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/processing/exhaustive.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3388 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/passes/processing/iterative.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12368 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/processing/rebase.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5282 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/processing/scan.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5143 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/processing/substitute.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.915039 bqskit-1.1.0a5/bqskit/passes/rules/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      710 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/rules/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/rules/ch2cnot.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1636 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/rules/cnot2ch.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/rules/cnot2cy.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-07-15 16:50:38.000000 bqskit-1.1.0a5/bqskit/passes/rules/cnot2cz.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1631 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/rules/cy2cnot.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1580 2023-07-15 16:51:29.000000 bqskit-1.1.0a5/bqskit/passes/rules/cz2cnot.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1567 2023-07-15 16:51:45.000000 bqskit-1.1.0a5/bqskit/passes/rules/swap2cnot.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1032 2023-07-15 16:51:51.000000 bqskit-1.1.0a5/bqskit/passes/rules/u3.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1753 2023-07-15 16:56:39.000000 bqskit-1.1.0a5/bqskit/passes/rules/zxzxz.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.918372 bqskit-1.1.0a5/bqskit/passes/search/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      731 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/passes/search/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2425 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/frontier.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      926 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/generator.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.921706 bqskit-1.1.0a5/bqskit/passes/search/generators/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      810 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4173 2023-07-15 16:52:38.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/fourparam.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2606 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/middleout.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4132 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/seed.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     7161 2023-07-15 16:52:51.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/simple.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4032 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/single.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2358 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/stair.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5056 2023-07-15 16:53:06.000000 bqskit-1.1.0a5/bqskit/passes/search/generators/wide.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1287 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/heuristic.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.925039 bqskit-1.1.0a5/bqskit/passes/search/heuristics/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      368 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/passes/search/heuristics/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2737 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/heuristics/astar.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1115 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/heuristics/dijkstra.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1617 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/search/heuristics/greedy.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.931706 bqskit-1.1.0a5/bqskit/passes/synthesis/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      771 2023-07-15 14:12:54.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12455 2023-07-15 14:17:22.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/leap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4261 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/pas.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    10759 2023-07-15 16:56:15.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/qfast.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12979 2023-07-15 16:53:31.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/qpredict.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8602 2023-07-15 14:17:22.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/qsearch.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1729 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/synthesis.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1230 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/synthesis/target.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.938372 bqskit-1.1.0a5/bqskit/passes/util/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      931 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/passes/util/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      618 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/compress.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5023 2023-07-15 16:53:49.000000 bqskit-1.1.0a5/bqskit/passes/util/conversion.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1321 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/converttou3.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3549 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/extend.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2716 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/fill.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1940 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/log.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1019 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/random.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1403 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/record.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      635 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/unfold.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1091 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/passes/util/update.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.938372 bqskit-1.1.0a5/bqskit/qis/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2154 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20134 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/graph.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     8060 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/pauli.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4943 2023-01-23 16:58:30.000000 bqskit-1.1.0a5/bqskit/qis/permutation.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.941706 bqskit-1.1.0a5/bqskit/qis/state/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      462 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/state/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    14029 2023-07-15 16:55:57.000000 bqskit-1.1.0a5/bqskit/qis/state/state.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      660 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/state/statemap.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3713 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/state/system.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.948372 bqskit-1.1.0a5/bqskit/qis/unitary/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      808 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2310 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/differentiable.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1282 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/meta.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1739 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/optimizable.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3813 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/unitary.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    12154 2023-01-19 20:43:03.000000 bqskit-1.1.0a5/bqskit/qis/unitary/unitarybuilder.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15603 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/qis/unitary/unitarymatrix.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.955039 bqskit-1.1.0a5/bqskit/runtime/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6364 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      551 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/address.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3319 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/attached.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    22189 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/base.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    15713 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/detached.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      530 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/direction.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1659 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/future.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    11817 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/manager.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      441 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/message.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      379 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/result.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3734 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/task.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    25392 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/runtime/worker.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.958373 bqskit-1.1.0a5/bqskit/utils/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      593 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/utils/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     2342 2022-09-19 11:52:10.000000 bqskit-1.1.0a5/bqskit/utils/cachedclass.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      408 2023-01-19 20:43:03.000000 bqskit-1.1.0a5/bqskit/utils/docs.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4311 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/utils/math.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      525 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/utils/random.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.961706 bqskit-1.1.0a5/bqskit/utils/test/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      371 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/utils/test/__init__.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    13812 2023-07-15 16:37:50.000000 bqskit-1.1.0a5/bqskit/utils/test/strategies.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)    20786 2022-08-13 15:35:16.000000 bqskit-1.1.0a5/bqskit/utils/test/types.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     5284 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/bqskit/utils/typing.py
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      216 2023-07-18 11:35:11.000000 bqskit-1.1.0a5/bqskit/version.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.728370 bqskit-1.1.0a5/bqskit.egg-info/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     4849 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/PKG-INFO
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     9576 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/SOURCES.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)        1 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/dependency_links.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      181 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/entry_points.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)      145 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/requires.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)        7 2023-07-18 11:35:19.000000 bqskit-1.1.0a5/bqskit.egg-info/top_level.txt
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     1021 2023-07-15 13:59:16.000000 bqskit-1.1.0a5/pyproject.toml
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)       38 2023-07-18 11:35:19.961706 bqskit-1.1.0a5/setup.cfg
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     3030 2023-07-18 11:34:27.000000 bqskit-1.1.0a5/setup.py
+drwxr-xr-x   0 edyounis  (1000) edyounis  (1000)        0 2023-07-18 11:35:19.961706 bqskit-1.1.0a5/tests/
+-rw-r--r--   0 edyounis  (1000) edyounis  (1000)     6031 2022-09-19 11:52:11.000000 bqskit-1.1.0a5/tests/test_conftest.py
```

### Comparing `bqskit-1.1.0a4/LICENSE` & `bqskit-1.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/PKG-INFO` & `bqskit-1.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqskit
-Version: 1.1.0a4
+Version: 1.1.0a5
 Summary: Berkeley Quantum Synthesis Toolkit
 Home-page: https://github.com/BQSKit/bqskit
 Author: LBNL - BQSKit developers
 Author-email: edyounis@lbl.gov
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/BQSKit/bqskit/issues
 Project-URL: Source Code, https://github.com/BQSKit/bqskit
```

### Comparing `bqskit-1.1.0a4/README.md` & `bqskit-1.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/__init__.py` & `bqskit-1.1.0a5/bqskit/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/__init__.py` & `bqskit-1.1.0a5/bqskit/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/basepass.py` & `bqskit-1.1.0a5/bqskit/compiler/basepass.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/compile.py` & `bqskit-1.1.0a5/bqskit/compiler/compile.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/compiler.py` & `bqskit-1.1.0a5/bqskit/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/gateset.py` & `bqskit-1.1.0a5/bqskit/compiler/gateset.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/machine.py` & `bqskit-1.1.0a5/bqskit/compiler/machine.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/passdata.py` & `bqskit-1.1.0a5/bqskit/compiler/passdata.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/task.py` & `bqskit-1.1.0a5/bqskit/compiler/task.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/compiler/workflow.py` & `bqskit-1.1.0a5/bqskit/compiler/workflow.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/__init__.py` & `bqskit-1.1.0a5/bqskit/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/results.py` & `bqskit-1.1.0a5/bqskit/exec/results.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/runner.py` & `bqskit-1.1.0a5/bqskit/exec/runner.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/runners/ibmq.py` & `bqskit-1.1.0a5/bqskit/exec/runners/ibmq.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/runners/quest.py` & `bqskit-1.1.0a5/bqskit/exec/runners/quest.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/exec/runners/sim.py` & `bqskit-1.1.0a5/bqskit/exec/runners/sim.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/__init__.py` & `bqskit-1.1.0a5/bqskit/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/cirq/models.py` & `bqskit-1.1.0a5/bqskit/ext/cirq/models.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/cirq/translate.py` & `bqskit-1.1.0a5/bqskit/ext/cirq/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/honeywell.py` & `bqskit-1.1.0a5/bqskit/ext/honeywell.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/pytket/translate.py` & `bqskit-1.1.0a5/bqskit/ext/pytket/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/qiskit/models.py` & `bqskit-1.1.0a5/bqskit/ext/qiskit/models.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/qiskit/translate.py` & `bqskit-1.1.0a5/bqskit/ext/qiskit/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/qutip/translate.py` & `bqskit-1.1.0a5/bqskit/ext/qutip/translate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/rigetti.py` & `bqskit-1.1.0a5/bqskit/ext/rigetti.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ext/supermarq.py` & `bqskit-1.1.0a5/bqskit/ext/supermarq.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/circuit.py` & `bqskit-1.1.0a5/bqskit/ir/circuit.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gate.py` & `bqskit-1.1.0a5/bqskit/ir/gate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/barrier.py` & `bqskit-1.1.0a5/bqskit/ir/gates/barrier.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/circuitgate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/circuitgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/controlled.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/controlled.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/daggergate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/daggergate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/frozenparam.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/frozenparam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/tagged.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/tagged.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composed/vlg.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composed/vlg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/composedgate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/composedgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/b.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/b.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/ccx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/ccx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/ch.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/ch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/clock.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/clock.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/cpi.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/cpi.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/cs.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/cs.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/csum.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/csum.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/csumd.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/csumd.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/ct.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/ct.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/cx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/cx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/cy.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/cy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/cz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/cz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/h.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/h.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/hd.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/hd.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/identity.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/identity.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/iswap.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/iswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/itoffoli.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/itoffoli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/pd.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/pd.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/permutation.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/permutation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/rccx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/rccx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/s.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/s.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/sdg.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/sdg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/shift.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/shift.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/sqrtcnot.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/sqrtcnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/sqrtiswap.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/sqrtiswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/subswap.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/subswap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/swap.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/swap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/sx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/sx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/sycamore.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/sycamore.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/t.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/t.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/tdg.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/tdg.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/unitary.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/x.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/x.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/xx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/xx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/y.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/y.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/yy.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/yy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/z.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/z.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constant/zz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constant/zz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/constantgate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/constantgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/generalgate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/generalgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/measure.py` & `bqskit-1.1.0a5/bqskit/ir/gates/measure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ccp.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ccp.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cp.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cp.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cphase.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cphase.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/crx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/crx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cry.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cry.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/crz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/crz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/cu.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/cu.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/fsim.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/fsim.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/pauli.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/pauli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/phasedxz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/phasedxz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rxx.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rxx.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ry.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ry.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/ryy.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/ryy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/rzz.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/rzz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u1.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u1.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u1q.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u1q.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u2.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u2.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u3.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/u8.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/u8.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/parameterized/unitary.py` & `bqskit-1.1.0a5/bqskit/ir/gates/parameterized/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/gates/quditgate.py` & `bqskit-1.1.0a5/bqskit/ir/gates/quditgate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/interval.py` & `bqskit-1.1.0a5/bqskit/ir/interval.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/iterator.py` & `bqskit-1.1.0a5/bqskit/ir/iterator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/lang/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/lang/language.py` & `bqskit-1.1.0a5/bqskit/ir/lang/language.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/lang/qasm2/parser.py` & `bqskit-1.1.0a5/bqskit/ir/lang/qasm2/parser.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/lang/qasm2/qasm2.py` & `bqskit-1.1.0a5/bqskit/ir/lang/qasm2/qasm2.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/lang/qasm2/visitor.py` & `bqskit-1.1.0a5/bqskit/ir/lang/qasm2/visitor.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/location.py` & `bqskit-1.1.0a5/bqskit/ir/location.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/operation.py` & `bqskit-1.1.0a5/bqskit/ir/operation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/differentiable.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/differentiable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/function.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/function.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/__init__.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/cost/hilbertschmidt.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/functions/residuals/hilbertschmidt.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/generator.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/generator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/cost/residual.py` & `bqskit-1.1.0a5/bqskit/ir/opt/cost/residual.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/instantiater.py` & `bqskit-1.1.0a5/bqskit/ir/opt/instantiater.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/minimization.py` & `bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/minimization.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/instantiaters/qfactor.py` & `bqskit-1.1.0a5/bqskit/ir/opt/instantiaters/qfactor.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/minimizer.py` & `bqskit-1.1.0a5/bqskit/ir/opt/minimizer.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/minimizers/ceres.py` & `bqskit-1.1.0a5/bqskit/ir/opt/minimizers/ceres.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/minimizers/scipy.py` & `bqskit-1.1.0a5/bqskit/ir/opt/minimizers/scipy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/multistartgen.py` & `bqskit-1.1.0a5/bqskit/ir/opt/multistartgen.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/diagonal.py` & `bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/diagonal.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/opt/multistartgens/random.py` & `bqskit-1.1.0a5/bqskit/ir/opt/multistartgens/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/point.py` & `bqskit-1.1.0a5/bqskit/ir/point.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/region.py` & `bqskit-1.1.0a5/bqskit/ir/region.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/ir/structure.py` & `bqskit-1.1.0a5/bqskit/ir/structure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/alias.py` & `bqskit-1.1.0a5/bqskit/passes/alias.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/control/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/dothendecide.py` & `bqskit-1.1.0a5/bqskit/passes/control/dothendecide.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/dowhileloop.py` & `bqskit-1.1.0a5/bqskit/passes/control/dowhileloop.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/foreach.py` & `bqskit-1.1.0a5/bqskit/passes/control/foreach.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/ifthenelse.py` & `bqskit-1.1.0a5/bqskit/passes/control/ifthenelse.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/paralleldo.py` & `bqskit-1.1.0a5/bqskit/passes/control/paralleldo.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicate.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/andpredicate.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/andpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/change.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/change.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/count.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/count.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/multi.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/multi.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/notpredicate.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/notpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/orpredicate.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/orpredicate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/physical.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/physical.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/single.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/predicates/width.py` & `bqskit-1.1.0a5/bqskit/passes/control/predicates/width.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/control/whileloop.py` & `bqskit-1.1.0a5/bqskit/passes/control/whileloop.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/group.py` & `bqskit-1.1.0a5/bqskit/passes/group.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/io/checkpoint.py` & `bqskit-1.1.0a5/bqskit/passes/io/checkpoint.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/io/intermediate.py` & `bqskit-1.1.0a5/bqskit/passes/io/intermediate.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/apply.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/apply.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/embed.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/embed.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/layout/pam.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/layout/pam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/layout/sabre.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/layout/sabre.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/pam.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/pam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/placement/greedy.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/placement/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/placement/trivial.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/placement/trivial.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/routing/pam.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/routing/pam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/routing/sabre.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/routing/sabre.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/sabre.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/sabre.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/setmodel.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/setmodel.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/mapping/topology.py` & `bqskit-1.1.0a5/bqskit/passes/mapping/topology.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/measure.py` & `bqskit-1.1.0a5/bqskit/passes/measure.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/cluster.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/cluster.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/greedy.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/quick.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/quick.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/scan.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/scan.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/partitioning/single.py` & `bqskit-1.1.0a5/bqskit/passes/partitioning/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/exhaustive.py` & `bqskit-1.1.0a5/bqskit/passes/processing/exhaustive.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/iterative.py` & `bqskit-1.1.0a5/bqskit/passes/processing/iterative.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/rebase.py` & `bqskit-1.1.0a5/bqskit/passes/processing/rebase.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/scan.py` & `bqskit-1.1.0a5/bqskit/passes/processing/scan.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/processing/substitute.py` & `bqskit-1.1.0a5/bqskit/passes/processing/substitute.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/ch2cnot.py` & `bqskit-1.1.0a5/bqskit/passes/rules/ch2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/cnot2ch.py` & `bqskit-1.1.0a5/bqskit/passes/rules/cnot2ch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/cnot2cy.py` & `bqskit-1.1.0a5/bqskit/passes/rules/cnot2cy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/cnot2cz.py` & `bqskit-1.1.0a5/bqskit/passes/rules/cnot2cz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/cy2cnot.py` & `bqskit-1.1.0a5/bqskit/passes/rules/cy2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/cz2cnot.py` & `bqskit-1.1.0a5/bqskit/passes/rules/cz2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/swap2cnot.py` & `bqskit-1.1.0a5/bqskit/passes/rules/swap2cnot.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/u3.py` & `bqskit-1.1.0a5/bqskit/passes/rules/u3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/rules/zxzxz.py` & `bqskit-1.1.0a5/bqskit/passes/rules/zxzxz.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/search/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/frontier.py` & `bqskit-1.1.0a5/bqskit/passes/search/frontier.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generator.py` & `bqskit-1.1.0a5/bqskit/passes/search/generator.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/fourparam.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/fourparam.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/middleout.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/middleout.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/seed.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/seed.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/simple.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/simple.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/single.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/single.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/stair.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/stair.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/generators/wide.py` & `bqskit-1.1.0a5/bqskit/passes/search/generators/wide.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/heuristic.py` & `bqskit-1.1.0a5/bqskit/passes/search/heuristic.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/heuristics/astar.py` & `bqskit-1.1.0a5/bqskit/passes/search/heuristics/astar.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/heuristics/dijkstra.py` & `bqskit-1.1.0a5/bqskit/passes/search/heuristics/dijkstra.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/search/heuristics/greedy.py` & `bqskit-1.1.0a5/bqskit/passes/search/heuristics/greedy.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/leap.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/leap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/pas.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/pas.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/qfast.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/qfast.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/qpredict.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/qpredict.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/qsearch.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/qsearch.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/synthesis.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/synthesis.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/synthesis/target.py` & `bqskit-1.1.0a5/bqskit/passes/synthesis/target.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/__init__.py` & `bqskit-1.1.0a5/bqskit/passes/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/compress.py` & `bqskit-1.1.0a5/bqskit/passes/util/compress.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/conversion.py` & `bqskit-1.1.0a5/bqskit/passes/util/conversion.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/converttou3.py` & `bqskit-1.1.0a5/bqskit/passes/util/converttou3.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/extend.py` & `bqskit-1.1.0a5/bqskit/passes/util/extend.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/fill.py` & `bqskit-1.1.0a5/bqskit/passes/util/fill.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/log.py` & `bqskit-1.1.0a5/bqskit/passes/util/log.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/random.py` & `bqskit-1.1.0a5/bqskit/passes/util/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/record.py` & `bqskit-1.1.0a5/bqskit/passes/util/record.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/unfold.py` & `bqskit-1.1.0a5/bqskit/passes/util/unfold.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/passes/util/update.py` & `bqskit-1.1.0a5/bqskit/passes/util/update.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/__init__.py` & `bqskit-1.1.0a5/bqskit/qis/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/graph.py` & `bqskit-1.1.0a5/bqskit/qis/graph.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/pauli.py` & `bqskit-1.1.0a5/bqskit/qis/pauli.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/permutation.py` & `bqskit-1.1.0a5/bqskit/qis/permutation.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/state/state.py` & `bqskit-1.1.0a5/bqskit/qis/state/state.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/state/statemap.py` & `bqskit-1.1.0a5/bqskit/qis/state/statemap.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/state/system.py` & `bqskit-1.1.0a5/bqskit/qis/state/system.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/__init__.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/differentiable.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/differentiable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/meta.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/meta.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/optimizable.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/optimizable.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/unitary.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/unitary.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/unitarybuilder.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/unitarybuilder.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/qis/unitary/unitarymatrix.py` & `bqskit-1.1.0a5/bqskit/qis/unitary/unitarymatrix.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/__init__.py` & `bqskit-1.1.0a5/bqskit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/address.py` & `bqskit-1.1.0a5/bqskit/runtime/address.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/attached.py` & `bqskit-1.1.0a5/bqskit/runtime/attached.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/base.py` & `bqskit-1.1.0a5/bqskit/runtime/base.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/detached.py` & `bqskit-1.1.0a5/bqskit/runtime/detached.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/direction.py` & `bqskit-1.1.0a5/bqskit/runtime/direction.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/future.py` & `bqskit-1.1.0a5/bqskit/runtime/future.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/manager.py` & `bqskit-1.1.0a5/bqskit/runtime/manager.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/task.py` & `bqskit-1.1.0a5/bqskit/runtime/task.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/runtime/worker.py` & `bqskit-1.1.0a5/bqskit/runtime/worker.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/__init__.py` & `bqskit-1.1.0a5/bqskit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/cachedclass.py` & `bqskit-1.1.0a5/bqskit/utils/cachedclass.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/math.py` & `bqskit-1.1.0a5/bqskit/utils/math.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/random.py` & `bqskit-1.1.0a5/bqskit/utils/random.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/test/strategies.py` & `bqskit-1.1.0a5/bqskit/utils/test/strategies.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/test/types.py` & `bqskit-1.1.0a5/bqskit/utils/test/types.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit/utils/typing.py` & `bqskit-1.1.0a5/bqskit/utils/typing.py`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/bqskit.egg-info/PKG-INFO` & `bqskit-1.1.0a5/bqskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bqskit
-Version: 1.1.0a4
+Version: 1.1.0a5
 Summary: Berkeley Quantum Synthesis Toolkit
 Home-page: https://github.com/BQSKit/bqskit
 Author: LBNL - BQSKit developers
 Author-email: edyounis@lbl.gov
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/BQSKit/bqskit/issues
 Project-URL: Source Code, https://github.com/BQSKit/bqskit
```

### Comparing `bqskit-1.1.0a4/bqskit.egg-info/SOURCES.txt` & `bqskit-1.1.0a5/bqskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/pyproject.toml` & `bqskit-1.1.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bqskit-1.1.0a4/setup.py` & `bqskit-1.1.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     project_urls={
         'Bug Tracker': 'https://github.com/BQSKit/bqskit/issues',
         'Source Code': 'https://github.com/BQSKit/bqskit',
         'Documentation': 'https://bqskit.readthedocs.io/en/latest',
     },
     packages=find_packages(exclude=['examples*', 'test*']),
     install_requires=[
-        'bqskitrs>=0.4.0rc4',
+        'bqskitrs>=0.4.0rc5',
         'lark-parser',
         'numpy>=1.22.0',
         'scipy>=1.8.0',
         'typing-extensions>=4.0.0',
     ],
     python_requires='>=3.8, <4',
     entry_points={
```

### Comparing `bqskit-1.1.0a4/tests/test_conftest.py` & `bqskit-1.1.0a5/tests/test_conftest.py`

 * *Files identical despite different names*

