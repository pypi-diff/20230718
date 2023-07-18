# Comparing `tmp/mfem-4.5.2.0rc0.tar.gz` & `tmp/mfem-4.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mfem-4.5.2.0rc0.tar", last modified: Mon Mar 27 05:20:44 2023, max compression
+gzip compressed data, was "dist/mfem-4.5.2.1.tar", last modified: Tue Jul 18 02:28:57 2023, max compression
```

## Comparing `mfem-4.5.2.0rc0.tar` & `mfem-4.5.2.1.tar`

### file list

```diff
@@ -1,387 +1,387 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      277 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5676 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4832 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/docs/
--rw-r--r--   0 root         (0) root         (0)    11301 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/docs/changelog.txt
--rw-r--r--   0 root         (0) root         (0)     5160 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/docs/development_memo.txt
--rw-r--r--   0 root         (0) root         (0)    78875 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/docs/example_image.png
--rw-r--r--   0 root         (0) root         (0)     4587 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/docs/install.txt
--rw-r--r--   0 root         (0) root         (0)    26955 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/docs/manual.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/examples/
--rw-r--r--   0 root         (0) root         (0)     3577 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex0.py
--rw-r--r--   0 root         (0) root         (0)     3882 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex0p.py
--rw-r--r--   0 root         (0) root         (0)     7163 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex1.py
--rw-r--r--   0 root         (0) root         (0)    12251 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex10.py
--rw-r--r--   0 root         (0) root         (0)    16639 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex10p.py
--rw-r--r--   0 root         (0) root         (0)     8277 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex11p.py
--rw-r--r--   0 root         (0) root         (0)     8923 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex12p.py
--rw-r--r--   0 root         (0) root         (0)     3464 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex13p.py
--rw-r--r--   0 root         (0) root         (0)     2908 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex14.py
--rw-r--r--   0 root         (0) root         (0)     6928 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex14p.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex15.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex15p.py
--rw-r--r--   0 root         (0) root         (0)     8679 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex16.py
--rw-r--r--   0 root         (0) root         (0)    10018 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex16p.py
--rw-r--r--   0 root         (0) root         (0)    11252 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex17.py
--rw-r--r--   0 root         (0) root         (0)    12744 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex17p.py
--rw-r--r--   0 root         (0) root         (0)     8685 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex18.py
--rw-r--r--   0 root         (0) root         (0)    14460 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex18_common.py
--rw-r--r--   0 root         (0) root         (0)     9264 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex18p.py
--rw-r--r--   0 root         (0) root         (0)    13076 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex19.py
--rw-r--r--   0 root         (0) root         (0)    14825 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex19p.py
--rw-r--r--   0 root         (0) root         (0)     4662 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex1p.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex2.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex20.py
--rw-r--r--   0 root         (0) root         (0)     7146 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex20p.py
--rw-r--r--   0 root         (0) root         (0)    10922 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex21.py
--rw-r--r--   0 root         (0) root         (0)    12080 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex21p.py
--rw-r--r--   0 root         (0) root         (0)    19878 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex22.py
--rw-r--r--   0 root         (0) root         (0)    20146 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex22p.py
--rw-r--r--   0 root         (0) root         (0)    10605 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex23.py
--rw-r--r--   0 root         (0) root         (0)    15039 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex24.py
--rw-r--r--   0 root         (0) root         (0)    15711 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex24p.py
--rw-r--r--   0 root         (0) root         (0)    27591 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex25.py
--rw-r--r--   0 root         (0) root         (0)    26519 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex25p.py
--rw-r--r--   0 root         (0) root         (0)     7489 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex26.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex26p.py
--rw-r--r--   0 root         (0) root         (0)    21653 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex27.py
--rw-r--r--   0 root         (0) root         (0)    23045 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex27p.py
--rw-r--r--   0 root         (0) root         (0)     7490 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex28.py
--rw-r--r--   0 root         (0) root         (0)     9668 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex28p.py
--rw-r--r--   0 root         (0) root         (0)    10924 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex29.py
--rw-r--r--   0 root         (0) root         (0)    11916 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex29p.py
--rw-r--r--   0 root         (0) root         (0)     9103 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex2p.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex3.py
--rw-r--r--   0 root         (0) root         (0)     4603 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex30.py
--rw-r--r--   0 root         (0) root         (0)     5850 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex30p.py
--rw-r--r--   0 root         (0) root         (0)    16770 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex31.py
--rw-r--r--   0 root         (0) root         (0)    18640 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex31p.py
--rw-r--r--   0 root         (0) root         (0)    16912 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex32p.py
--rw-r--r--   0 root         (0) root         (0)    12086 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex33.py
--rw-r--r--   0 root         (0) root         (0)     8356 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex33_common.py
--rw-r--r--   0 root         (0) root         (0)    13117 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex33p.py
--rw-r--r--   0 root         (0) root         (0)    11288 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex3p.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex4.py
--rw-r--r--   0 root         (0) root         (0)     9006 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex4p.py
--rw-r--r--   0 root         (0) root         (0)     9052 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex5.py
--rw-r--r--   0 root         (0) root         (0)    11627 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex5p.py
--rw-r--r--   0 root         (0) root         (0)     5666 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex6.py
--rw-r--r--   0 root         (0) root         (0)    12582 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex6p.py
--rw-r--r--   0 root         (0) root         (0)     4536 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex7.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex7p.py
--rw-r--r--   0 root         (0) root         (0)     7566 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex8.py
--rw-r--r--   0 root         (0) root         (0)     8910 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex8p.py
--rw-r--r--   0 root         (0) root         (0)    11714 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex9.py
--rw-r--r--   0 root         (0) root         (0)     7810 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/ex9p.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/examples/numba/
--rw-r--r--   0 root         (0) root         (0)     3292 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/numba/ex4.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/examples/wrapper_example/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/
--rw-r--r--   0 root         (0) root         (0)     1979 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_1.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_3.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_4.py
--rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_5.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_6.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/matrix_coefficient.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/sparsemat.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/examples/wrapper_example/vector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/headers/
--rw-r--r--   0 root         (0) root         (0)    65070 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/headers/coefficient.hpp
--rw-r--r--   0 root         (0) root         (0)    48838 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/headers/mem_manager.hpp
--rw-r--r--   0 root         (0) root         (0)    38981 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/headers/schwarz.cpp
--rw-r--r--   0 root         (0) root         (0)     4737 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/headers/schwarz.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem/
--rw-r--r--   0 root         (0) root         (0)      593 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem/_par/
--rw-r--r--   0 root         (0) root         (0)      217 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3708 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/array.i
--rw-r--r--   0 root         (0) root         (0)      417 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/auxiliary.i
--rw-r--r--   0 root         (0) root         (0)     3800 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/bilinearform.i
--rw-r--r--   0 root         (0) root         (0)      926 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/bilininteg.i
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/blockmatrix.i
--rw-r--r--   0 root         (0) root         (0)     2335 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/blockoperator.i
--rw-r--r--   0 root         (0) root         (0)      358 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/blockvector.i
--rw-r--r--   0 root         (0) root         (0)     7229 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/coefficient.i
--rw-r--r--   0 root         (0) root         (0)      487 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/coefficient_py.cpp
--rw-r--r--   0 root         (0) root         (0)      391 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/coefficient_py.hpp
--rw-r--r--   0 root         (0) root         (0)      924 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/common_functions.i
--rw-r--r--   0 root         (0) root         (0)      822 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/communication.i
--rw-r--r--   0 root         (0) root         (0)      762 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/complex_fem.i
--rw-r--r--   0 root         (0) root         (0)     1599 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/complex_operator.i
--rw-r--r--   0 root         (0) root         (0)      585 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/constraints.i
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/cpointers.i
--rw-r--r--   0 root         (0) root         (0)      538 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/datacollection.i
--rw-r--r--   0 root         (0) root         (0)     8459 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/densemat.i
--rw-r--r--   0 root         (0) root         (0)      892 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/device.i
--rw-r--r--   0 root         (0) root         (0)      550 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/dist_solver.i
--rw-r--r--   0 root         (0) root         (0)      321 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/doftrans.i
--rw-r--r--   0 root         (0) root         (0)      788 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/element.i
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/eltrans.i
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/error.i
--rw-r--r--   0 root         (0) root         (0)     2662 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/estimators.i
--rw-r--r--   0 root         (0) root         (0)      623 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe.i
--rw-r--r--   0 root         (0) root         (0)      380 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_base.i
--rw-r--r--   0 root         (0) root         (0)      626 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_coll.i
--rw-r--r--   0 root         (0) root         (0)      355 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_fixed_order.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_h1.i
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_l2.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_nd.i
--rw-r--r--   0 root         (0) root         (0)      328 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_nurbs.i
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_pos.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_rt.i
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fe_ser.i
--rw-r--r--   0 root         (0) root         (0)     5968 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fespace.i
--rw-r--r--   0 root         (0) root         (0)      359 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/fespacehierarchy.i
--rw-r--r--   0 root         (0) root         (0)     1292 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/geom.i
--rw-r--r--   0 root         (0) root         (0)      378 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/globals.i
--rw-r--r--   0 root         (0) root         (0)     6461 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/gridfunc.i
--rw-r--r--   0 root         (0) root         (0)      507 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/gslib.i
--rw-r--r--   0 root         (0) root         (0)     2556 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/handle.i
--rw-r--r--   0 root         (0) root         (0)      310 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/hash.i
--rw-r--r--   0 root         (0) root         (0)      609 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/hexahedron.i
--rw-r--r--   0 root         (0) root         (0)      313 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/hybridization.i
--rw-r--r--   0 root         (0) root         (0)    19679 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/hypre.i
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/intrules.i
--rw-r--r--   0 root         (0) root         (0)      250 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/io_stream.i
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/iostream_typemap.hpp
--rw-r--r--   0 root         (0) root         (0)      597 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/istream_typemap.i
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/linearform.i
--rw-r--r--   0 root         (0) root         (0)      856 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/lininteg.i
--rw-r--r--   0 root         (0) root         (0)      662 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/matrix.i
--rw-r--r--   0 root         (0) root         (0)      481 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/mem_manager.i
--rw-r--r--   0 root         (0) root         (0)    18877 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/mesh.i
--rw-r--r--   0 root         (0) root         (0)      514 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/mesh_operators.i
--rw-r--r--   0 root         (0) root         (0)     1882 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/multigrid.i
--rw-r--r--   0 root         (0) root         (0)     1283 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/ncmesh.i
--rw-r--r--   0 root         (0) root         (0)     2079 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/nonlinearform.i
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/nonlininteg.i
--rw-r--r--   0 root         (0) root         (0)      759 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/ode.i
--rw-r--r--   0 root         (0) root         (0)     3244 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/operators.i
--rw-r--r--   0 root         (0) root         (0)     1155 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/ostream_typemap.i
--rw-r--r--   0 root         (0) root         (0)     1786 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pbilinearform.i
--rw-r--r--   0 root         (0) root         (0)     2631 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pfespace.i
--rw-r--r--   0 root         (0) root         (0)     4768 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pgridfunc.i
--rw-r--r--   0 root         (0) root         (0)      540 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/plinearform.i
--rw-r--r--   0 root         (0) root         (0)     2836 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pmesh.i
--rw-r--r--   0 root         (0) root         (0)      844 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pncmesh.i
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pnonlinearform.i
--rw-r--r--   0 root         (0) root         (0)      473 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/point.i
--rw-r--r--   0 root         (0) root         (0)      404 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/prestriction.i
--rw-r--r--   0 root         (0) root         (0)      494 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/psubmesh.i
--rw-r--r--   0 root         (0) root         (0)      480 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/ptransfermap.i
--rw-r--r--   0 root         (0) root         (0)     1099 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pumi.i
--rw-r--r--   0 root         (0) root         (0)     1776 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pycoefficient.hpp
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/pyoperator.hpp
--rw-r--r--   0 root         (0) root         (0)      782 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/qfunction.i
--rw-r--r--   0 root         (0) root         (0)      675 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/qspace.i
--rw-r--r--   0 root         (0) root         (0)      609 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/quadinterpolator.i
--rw-r--r--   0 root         (0) root         (0)      619 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/quadinterpolator_face.i
--rw-r--r--   0 root         (0) root         (0)      621 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/quadrilateral.i
--rw-r--r--   0 root         (0) root         (0)      417 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/restriction.i
--rw-r--r--   0 root         (0) root         (0)      643 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/schwarz.i
--rw-r--r--   0 root         (0) root         (0)      387 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/segment.i
--rw-r--r--   0 root         (0) root         (0)      271 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/sets.i
--rw-r--r--   0 root         (0) root         (0)     7543 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/setup.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/socketstream.i
--rw-r--r--   0 root         (0) root         (0)     2191 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/solvers.i
--rw-r--r--   0 root         (0) root         (0)      361 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/sort_pairs.i
--rw-r--r--   0 root         (0) root         (0)     5770 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/sparsemat.i
--rw-r--r--   0 root         (0) root         (0)      357 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/sparsesmoothers.i
--rw-r--r--   0 root         (0) root         (0)      627 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/stable3d.i
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/std_vectors.i
--rw-r--r--   0 root         (0) root         (0)     2525 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/strumpack.i
--rw-r--r--   0 root         (0) root         (0)      449 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/submesh.i
--rw-r--r--   0 root         (0) root         (0)      475 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/symmat.i
--rw-r--r--   0 root         (0) root         (0)     1238 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/table.i
--rw-r--r--   0 root         (0) root         (0)      613 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/tetrahedron.i
--rw-r--r--   0 root         (0) root         (0)      831 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/tmop.i
--rw-r--r--   0 root         (0) root         (0)      508 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/tmop_amr.i
--rw-r--r--   0 root         (0) root         (0)       99 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/tmop_modules.py
--rw-r--r--   0 root         (0) root         (0)      626 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/tmop_tools.i
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/transfer.i
--rw-r--r--   0 root         (0) root         (0)      437 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/transfermap.i
--rw-r--r--   0 root         (0) root         (0)      601 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/triangle.i
--rw-r--r--   0 root         (0) root         (0)     9455 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/vector.i
--rw-r--r--   0 root         (0) root         (0)      266 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/vertex.i
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/vtk.i
--rw-r--r--   0 root         (0) root         (0)      612 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_par/wedge.i
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem/_ser/
--rw-r--r--   0 root         (0) root         (0)      197 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3962 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/array.i
--rw-r--r--   0 root         (0) root         (0)     4402 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/bilinearform.i
--rw-r--r--   0 root         (0) root         (0)     1260 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/bilininteg.i
--rw-r--r--   0 root         (0) root         (0)     1201 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/blockmatrix.i
--rw-r--r--   0 root         (0) root         (0)     2238 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/blockoperator.i
--rw-r--r--   0 root         (0) root         (0)      353 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/blockvector.i
--rw-r--r--   0 root         (0) root         (0)     7112 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/coefficient.i
--rw-r--r--   0 root         (0) root         (0)      487 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/coefficient_py.cpp
--rw-r--r--   0 root         (0) root         (0)      391 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/coefficient_py.hpp
--rw-r--r--   0 root         (0) root         (0)      837 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/common_functions.i
--rw-r--r--   0 root         (0) root         (0)      690 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/complex_fem.i
--rw-r--r--   0 root         (0) root         (0)     1428 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/complex_operator.i
--rw-r--r--   0 root         (0) root         (0)      562 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/constraints.i
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/cpointers.i
--rw-r--r--   0 root         (0) root         (0)      393 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/datacollection.i
--rw-r--r--   0 root         (0) root         (0)     8471 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/densemat.i
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/device.i
--rw-r--r--   0 root         (0) root         (0)      321 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/doftrans.i
--rw-r--r--   0 root         (0) root         (0)      982 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/element.i
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/eltrans.i
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/error.i
--rw-r--r--   0 root         (0) root         (0)     1371 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/estimators.i
--rw-r--r--   0 root         (0) root         (0)      621 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe.i
--rw-r--r--   0 root         (0) root         (0)      377 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_base.i
--rw-r--r--   0 root         (0) root         (0)      762 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_coll.i
--rw-r--r--   0 root         (0) root         (0)      355 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_fixed_order.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_h1.i
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_l2.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_nd.i
--rw-r--r--   0 root         (0) root         (0)      328 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_nurbs.i
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_pos.i
--rw-r--r--   0 root         (0) root         (0)      322 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_rt.i
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fe_ser.i
--rw-r--r--   0 root         (0) root         (0)     6011 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fespace.i
--rw-r--r--   0 root         (0) root         (0)      359 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/fespacehierarchy.i
--rw-r--r--   0 root         (0) root         (0)     1330 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/geom.i
--rw-r--r--   0 root         (0) root         (0)      378 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/globals.i
--rw-r--r--   0 root         (0) root         (0)     5805 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/gridfunc.i
--rw-r--r--   0 root         (0) root         (0)      421 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/gslib.i
--rw-r--r--   0 root         (0) root         (0)     1280 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/handle.i
--rw-r--r--   0 root         (0) root         (0)      310 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/hash.i
--rw-r--r--   0 root         (0) root         (0)      638 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/hexahedron.i
--rw-r--r--   0 root         (0) root         (0)      349 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/hybridization.i
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/intrules.i
--rw-r--r--   0 root         (0) root         (0)      247 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/io_stream.i
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/iostream_typemap.hpp
--rw-r--r--   0 root         (0) root         (0)      597 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/istream_typemap.i
--rw-r--r--   0 root         (0) root         (0)     1766 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/linearform.i
--rw-r--r--   0 root         (0) root         (0)      659 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/lininteg.i
--rw-r--r--   0 root         (0) root         (0)      708 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/matrix.i
--rw-r--r--   0 root         (0) root         (0)      480 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/mem_manager.i
--rw-r--r--   0 root         (0) root         (0)    18950 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/mesh.i
--rw-r--r--   0 root         (0) root         (0)      566 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/mesh_operators.i
--rw-r--r--   0 root         (0) root         (0)     1945 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/multigrid.i
--rw-r--r--   0 root         (0) root         (0)     1113 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/ncmesh.i
--rw-r--r--   0 root         (0) root         (0)     2182 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/nonlinearform.i
--rw-r--r--   0 root         (0) root         (0)      709 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/nonlininteg.i
--rw-r--r--   0 root         (0) root         (0)      761 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/ode.i
--rw-r--r--   0 root         (0) root         (0)     3095 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/operators.i
--rw-r--r--   0 root         (0) root         (0)     1162 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/ostream_typemap.i
--rw-r--r--   0 root         (0) root         (0)      669 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/point.i
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/pyoperator.hpp
--rw-r--r--   0 root         (0) root         (0)      780 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/qfunction.i
--rw-r--r--   0 root         (0) root         (0)      676 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/qspace.i
--rw-r--r--   0 root         (0) root         (0)      604 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/quadinterpolator.i
--rw-r--r--   0 root         (0) root         (0)      619 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/quadinterpolator_face.i
--rw-r--r--   0 root         (0) root         (0)      648 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/quadrilateral.i
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/restriction.i
--rw-r--r--   0 root         (0) root         (0)      583 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/segment.i
--rw-r--r--   0 root         (0) root         (0)      252 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/sets.i
--rw-r--r--   0 root         (0) root         (0)     6286 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/setup.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/socketstream.i
--rw-r--r--   0 root         (0) root         (0)     2157 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/solvers.i
--rw-r--r--   0 root         (0) root         (0)      361 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/sort_pairs.i
--rw-r--r--   0 root         (0) root         (0)     5734 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/sparsemat.i
--rw-r--r--   0 root         (0) root         (0)      772 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/sparsesmoothers.i
--rw-r--r--   0 root         (0) root         (0)      631 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/stable3d.i
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/std_vectors.i
--rw-r--r--   0 root         (0) root         (0)      449 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/submesh.i
--rw-r--r--   0 root         (0) root         (0)      475 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/symmat.i
--rw-r--r--   0 root         (0) root         (0)     1241 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/table.i
--rw-r--r--   0 root         (0) root         (0)      641 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/tetrahedron.i
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/tmop.i
--rw-r--r--   0 root         (0) root         (0)      397 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/tmop_amr.i
--rw-r--r--   0 root         (0) root         (0)       99 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/tmop_modules.py
--rw-r--r--   0 root         (0) root         (0)      518 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/tmop_tools.i
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/transfer.i
--rw-r--r--   0 root         (0) root         (0)      437 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/transfermap.i
--rw-r--r--   0 root         (0) root         (0)      628 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/triangle.i
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/vector.i
--rw-r--r--   0 root         (0) root         (0)      757 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/vertex.i
--rw-r--r--   0 root         (0) root         (0)      435 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/vtk.i
--rw-r--r--   0 root         (0) root         (0)      611 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/_ser/wedge.i
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/arg_parser.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/array_instantiation_macro.i
--rw-r--r--   0 root         (0) root         (0)     2464 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/array_listtuple_typemap.i
--rw-r--r--   0 root         (0) root         (0)     7380 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/bilininteg_ext.i
--rw-r--r--   0 root         (0) root         (0)    40525 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/chypre.py
--rw-r--r--   0 root         (0) root         (0)     7884 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/coefficient_common.i
--rw-r--r--   0 root         (0) root         (0)     2777 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/complex_fem_ext.i
--rw-r--r--   0 root         (0) root         (0)     2800 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/const_doubleptr_typemap.i
--rw-r--r--   0 root         (0) root         (0)     2977 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/const_intptr_typemap.i
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/cpointers.i
--rw-r--r--   0 root         (0) root         (0)     1645 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/data_size_typemap.i
--rw-r--r--   0 root         (0) root         (0)      481 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/deprecation.i
--rw-r--r--   0 root         (0) root         (0)      586 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/enum_class.i
--rw-r--r--   0 root         (0) root         (0)      368 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/exception.i
--rw-r--r--   0 root         (0) root         (0)      544 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/exception_director.i
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/findpoints.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/generate_bilininteg_ext.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/generate_lininteg_ext.py
--rw-r--r--   0 root         (0) root         (0)     1231 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/handle_template.i
--rw-r--r--   0 root         (0) root         (0)      155 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/hypre_int.i
--rw-r--r--   0 root         (0) root         (0)      111 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/ignore_common_functions.i
--rw-r--r--   0 root         (0) root         (0)      958 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/io_stream.hpp
--rw-r--r--   0 root         (0) root         (0)     9156 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/io_stream_typemap.i
--rw-r--r--   0 root         (0) root         (0)     2162 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/lininteg_ext.i
--rw-r--r--   0 root         (0) root         (0)      356 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/matrix_file.py
--rw-r--r--   0 root         (0) root         (0)      797 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/memorytype_typemap.i
--rw-r--r--   0 root         (0) root         (0)      234 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/mfem_config.i
--rw-r--r--   0 root         (0) root         (0)      763 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/mpi_debug.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/mpi_dtype.py
--rw-r--r--   0 root         (0) root         (0)    56404 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/numba_coefficient.i
--rw-r--r--   0 root         (0) root         (0)    16252 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/numba_coefficient_utils.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/numpy_int_typemap.i
--rw-r--r--   0 root         (0) root         (0)     1856 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/object_array_typemap.i
--rw-r--r--   0 root         (0) root         (0)      734 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/operator_ptr_typemap.i
--rw-r--r--   0 root         (0) root         (0)    16104 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/parcsr_extra.py
--rw-r--r--   0 root         (0) root         (0)     7130 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/pycoefficient.hpp
--rw-r--r--   0 root         (0) root         (0)      499 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/pysolvers.hpp
--rw-r--r--   0 root         (0) root         (0)     1299 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/sparse_utils.py
--rw-r--r--   0 root         (0) root         (0)    11265 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/common/typemap_macros.i
--rw-r--r--   0 root         (0) root         (0)     4178 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/par.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/mfem/ser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5676 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8374 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/mfem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    58974 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 05:20:44.000000 mfem-4.5.2.0rc0/test/
--rw-r--r--   0 root         (0) root         (0)     1636 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_array.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_blockmatrix.py
--rw-r--r--   0 root         (0) root         (0)     1278 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_blockoperator.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_chypre.py
--rw-r--r--   0 root         (0) root         (0)     3346 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_complex_operator.py
--rw-r--r--   0 root         (0) root         (0)    15150 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_complexmg.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_datacollection.py
--rw-r--r--   0 root         (0) root         (0)     1972 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_densemat.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_deprecated.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_dofloc.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_fespace.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_geom.py
--rw-r--r--   0 root         (0) root         (0)     1768 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_gridfunc.py
--rw-r--r--   0 root         (0) root         (0)     3831 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_gz.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_intrules.py
--rw-r--r--   0 root         (0) root         (0)      805 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_memory.py
--rw-r--r--   0 root         (0) root         (0)     3797 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_merge_gridfunction.py
--rw-r--r--   0 root         (0) root         (0)     4135 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_module.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_ncmesh.py
--rw-r--r--   0 root         (0) root         (0)    10236 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_numba.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_periodic_mesh.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_pfespace.py
--rw-r--r--   0 root         (0) root         (0)      528 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_point.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_segment.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_sparsemat.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_stringio.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_table.py
--rw-r--r--   0 root         (0) root         (0)    13613 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_tmop.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-03-27 05:20:33.000000 mfem-4.5.2.0rc0/test/test_vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-18 02:28:46.000000 mfem-4.5.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-18 02:28:46.000000 mfem-4.5.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-18 02:28:57.000000 mfem-4.5.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4832 2023-07-18 02:28:46.000000 mfem-4.5.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/docs/
+-rw-r--r--   0 root         (0) root         (0)    11301 2023-07-18 02:28:46.000000 mfem-4.5.2.1/docs/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)     5160 2023-07-18 02:28:46.000000 mfem-4.5.2.1/docs/development_memo.txt
+-rw-r--r--   0 root         (0) root         (0)    78875 2023-07-18 02:28:46.000000 mfem-4.5.2.1/docs/example_image.png
+-rw-r--r--   0 root         (0) root         (0)     4587 2023-07-18 02:28:46.000000 mfem-4.5.2.1/docs/install.txt
+-rw-r--r--   0 root         (0) root         (0)    26953 2023-07-18 02:28:46.000000 mfem-4.5.2.1/docs/manual.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/examples/
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex0.py
+-rw-r--r--   0 root         (0) root         (0)     3882 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex0p.py
+-rw-r--r--   0 root         (0) root         (0)     7163 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex1.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex10.py
+-rw-r--r--   0 root         (0) root         (0)    16639 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex10p.py
+-rw-r--r--   0 root         (0) root         (0)     8277 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex11p.py
+-rw-r--r--   0 root         (0) root         (0)     8923 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex12p.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex13p.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex14.py
+-rw-r--r--   0 root         (0) root         (0)     6928 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex14p.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex15.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex15p.py
+-rw-r--r--   0 root         (0) root         (0)     8679 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex16.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex16p.py
+-rw-r--r--   0 root         (0) root         (0)    11252 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex17.py
+-rw-r--r--   0 root         (0) root         (0)    12744 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex17p.py
+-rw-r--r--   0 root         (0) root         (0)     8685 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex18.py
+-rw-r--r--   0 root         (0) root         (0)    14460 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex18_common.py
+-rw-r--r--   0 root         (0) root         (0)     9264 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex18p.py
+-rw-r--r--   0 root         (0) root         (0)    13076 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex19.py
+-rw-r--r--   0 root         (0) root         (0)    14825 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex19p.py
+-rw-r--r--   0 root         (0) root         (0)     4662 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex1p.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex2.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex20.py
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex20p.py
+-rw-r--r--   0 root         (0) root         (0)    10922 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex21.py
+-rw-r--r--   0 root         (0) root         (0)    12080 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex21p.py
+-rw-r--r--   0 root         (0) root         (0)    19878 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex22.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex22p.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex23.py
+-rw-r--r--   0 root         (0) root         (0)    15043 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex24.py
+-rw-r--r--   0 root         (0) root         (0)    15711 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex24p.py
+-rw-r--r--   0 root         (0) root         (0)    27591 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex25.py
+-rw-r--r--   0 root         (0) root         (0)    26523 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex25p.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex26.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex26p.py
+-rw-r--r--   0 root         (0) root         (0)    21653 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex27.py
+-rw-r--r--   0 root         (0) root         (0)    23045 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex27p.py
+-rw-r--r--   0 root         (0) root         (0)     7490 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex28.py
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex28p.py
+-rw-r--r--   0 root         (0) root         (0)    10924 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex29.py
+-rw-r--r--   0 root         (0) root         (0)    11916 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex29p.py
+-rw-r--r--   0 root         (0) root         (0)     9103 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex2p.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex3.py
+-rw-r--r--   0 root         (0) root         (0)     4603 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex30.py
+-rw-r--r--   0 root         (0) root         (0)     5850 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex30p.py
+-rw-r--r--   0 root         (0) root         (0)    16776 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex31.py
+-rw-r--r--   0 root         (0) root         (0)    18642 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex31p.py
+-rw-r--r--   0 root         (0) root         (0)    16912 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex32p.py
+-rw-r--r--   0 root         (0) root         (0)    12086 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex33.py
+-rw-r--r--   0 root         (0) root         (0)     8356 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex33_common.py
+-rw-r--r--   0 root         (0) root         (0)    13117 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex33p.py
+-rw-r--r--   0 root         (0) root         (0)    11291 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex3p.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex4.py
+-rw-r--r--   0 root         (0) root         (0)     9006 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex4p.py
+-rw-r--r--   0 root         (0) root         (0)     9052 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex5.py
+-rw-r--r--   0 root         (0) root         (0)    11627 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex5p.py
+-rw-r--r--   0 root         (0) root         (0)     5666 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex6.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex6p.py
+-rw-r--r--   0 root         (0) root         (0)     4536 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex7.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex7p.py
+-rw-r--r--   0 root         (0) root         (0)     7566 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex8.py
+-rw-r--r--   0 root         (0) root         (0)     8910 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex8p.py
+-rw-r--r--   0 root         (0) root         (0)    11714 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex9.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/ex9p.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/examples/numba/
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/numba/ex4.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/examples/wrapper_example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_1.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_3.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_4.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_5.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/chypre/example_6.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/matrix_coefficient.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/sparsemat.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-07-18 02:28:46.000000 mfem-4.5.2.1/examples/wrapper_example/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/headers/
+-rw-r--r--   0 root         (0) root         (0)    65070 2023-07-18 02:28:46.000000 mfem-4.5.2.1/headers/coefficient.hpp
+-rw-r--r--   0 root         (0) root         (0)    48838 2023-07-18 02:28:46.000000 mfem-4.5.2.1/headers/mem_manager.hpp
+-rw-r--r--   0 root         (0) root         (0)    38981 2023-07-18 02:28:46.000000 mfem-4.5.2.1/headers/schwarz.cpp
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-18 02:28:46.000000 mfem-4.5.2.1/headers/schwarz.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem/
+-rw-r--r--   0 root         (0) root         (0)      590 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem/_par/
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/array.i
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/auxiliary.i
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/bilinearform.i
+-rw-r--r--   0 root         (0) root         (0)      926 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/bilininteg.i
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/blockmatrix.i
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/blockoperator.i
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/blockvector.i
+-rw-r--r--   0 root         (0) root         (0)     7229 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/coefficient.i
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/coefficient_py.cpp
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/coefficient_py.hpp
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/common_functions.i
+-rw-r--r--   0 root         (0) root         (0)      822 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/communication.i
+-rw-r--r--   0 root         (0) root         (0)      762 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/complex_fem.i
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/complex_operator.i
+-rw-r--r--   0 root         (0) root         (0)      585 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/constraints.i
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/cpointers.i
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/datacollection.i
+-rw-r--r--   0 root         (0) root         (0)     8459 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/densemat.i
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/device.i
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/dist_solver.i
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/doftrans.i
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/element.i
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/eltrans.i
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/error.i
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/estimators.i
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe.i
+-rw-r--r--   0 root         (0) root         (0)      380 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_base.i
+-rw-r--r--   0 root         (0) root         (0)      626 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_coll.i
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_fixed_order.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_h1.i
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_l2.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_nd.i
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_nurbs.i
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_pos.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_rt.i
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fe_ser.i
+-rw-r--r--   0 root         (0) root         (0)     5968 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fespace.i
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/fespacehierarchy.i
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/geom.i
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/globals.i
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/gridfunc.i
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/gslib.i
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/handle.i
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/hash.i
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/hexahedron.i
+-rw-r--r--   0 root         (0) root         (0)      313 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/hybridization.i
+-rw-r--r--   0 root         (0) root         (0)    19679 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/hypre.i
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/intrules.i
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/io_stream.i
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/iostream_typemap.hpp
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/istream_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/linearform.i
+-rw-r--r--   0 root         (0) root         (0)      856 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/lininteg.i
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/matrix.i
+-rw-r--r--   0 root         (0) root         (0)      481 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/mem_manager.i
+-rw-r--r--   0 root         (0) root         (0)    18877 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/mesh.i
+-rw-r--r--   0 root         (0) root         (0)      514 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/mesh_operators.i
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/multigrid.i
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/ncmesh.i
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/nonlinearform.i
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/nonlininteg.i
+-rw-r--r--   0 root         (0) root         (0)      759 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/ode.i
+-rw-r--r--   0 root         (0) root         (0)     3244 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/operators.i
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/ostream_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pbilinearform.i
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pfespace.i
+-rw-r--r--   0 root         (0) root         (0)     4768 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pgridfunc.i
+-rw-r--r--   0 root         (0) root         (0)      540 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/plinearform.i
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pmesh.i
+-rw-r--r--   0 root         (0) root         (0)      844 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pncmesh.i
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pnonlinearform.i
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/point.i
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/prestriction.i
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/psubmesh.i
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/ptransfermap.i
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pumi.i
+-rw-r--r--   0 root         (0) root         (0)     1776 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pycoefficient.hpp
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/pyoperator.hpp
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/qfunction.i
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/qspace.i
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/quadinterpolator.i
+-rw-r--r--   0 root         (0) root         (0)      619 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/quadinterpolator_face.i
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/quadrilateral.i
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/restriction.i
+-rw-r--r--   0 root         (0) root         (0)      643 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/schwarz.i
+-rw-r--r--   0 root         (0) root         (0)      387 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/segment.i
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/sets.i
+-rw-r--r--   0 root         (0) root         (0)     7543 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/socketstream.i
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/solvers.i
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/sort_pairs.i
+-rw-r--r--   0 root         (0) root         (0)     5770 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/sparsemat.i
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/sparsesmoothers.i
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/stable3d.i
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/std_vectors.i
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/strumpack.i
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/submesh.i
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/symmat.i
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/table.i
+-rw-r--r--   0 root         (0) root         (0)      613 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/tetrahedron.i
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/tmop.i
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/tmop_amr.i
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/tmop_modules.py
+-rw-r--r--   0 root         (0) root         (0)      626 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/tmop_tools.i
+-rw-r--r--   0 root         (0) root         (0)      452 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/transfer.i
+-rw-r--r--   0 root         (0) root         (0)      437 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/transfermap.i
+-rw-r--r--   0 root         (0) root         (0)      601 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/triangle.i
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/vector.i
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/vertex.i
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/vtk.i
+-rw-r--r--   0 root         (0) root         (0)      612 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_par/wedge.i
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem/_ser/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/array.i
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/bilinearform.i
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/bilininteg.i
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/blockmatrix.i
+-rw-r--r--   0 root         (0) root         (0)     2238 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/blockoperator.i
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/blockvector.i
+-rw-r--r--   0 root         (0) root         (0)     7112 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/coefficient.i
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/coefficient_py.cpp
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/coefficient_py.hpp
+-rw-r--r--   0 root         (0) root         (0)      837 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/common_functions.i
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/complex_fem.i
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/complex_operator.i
+-rw-r--r--   0 root         (0) root         (0)      562 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/constraints.i
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/cpointers.i
+-rw-r--r--   0 root         (0) root         (0)      393 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/datacollection.i
+-rw-r--r--   0 root         (0) root         (0)     8471 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/densemat.i
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/device.i
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/doftrans.i
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/element.i
+-rw-r--r--   0 root         (0) root         (0)      963 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/eltrans.i
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/error.i
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/estimators.i
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe.i
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_base.i
+-rw-r--r--   0 root         (0) root         (0)      762 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_coll.i
+-rw-r--r--   0 root         (0) root         (0)      355 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_fixed_order.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_h1.i
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_l2.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_nd.i
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_nurbs.i
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_pos.i
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_rt.i
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fe_ser.i
+-rw-r--r--   0 root         (0) root         (0)     6011 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fespace.i
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/fespacehierarchy.i
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/geom.i
+-rw-r--r--   0 root         (0) root         (0)      378 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/globals.i
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/gridfunc.i
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/gslib.i
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/handle.i
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/hash.i
+-rw-r--r--   0 root         (0) root         (0)      638 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/hexahedron.i
+-rw-r--r--   0 root         (0) root         (0)      349 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/hybridization.i
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/intrules.i
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/io_stream.i
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/iostream_typemap.hpp
+-rw-r--r--   0 root         (0) root         (0)      597 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/istream_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/linearform.i
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/lininteg.i
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/matrix.i
+-rw-r--r--   0 root         (0) root         (0)      480 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/mem_manager.i
+-rw-r--r--   0 root         (0) root         (0)    18950 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/mesh.i
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/mesh_operators.i
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/multigrid.i
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/ncmesh.i
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/nonlinearform.i
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/nonlininteg.i
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/ode.i
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/operators.i
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/ostream_typemap.i
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/point.i
+-rw-r--r--   0 root         (0) root         (0)      818 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/pyoperator.hpp
+-rw-r--r--   0 root         (0) root         (0)      780 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/qfunction.i
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/qspace.i
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/quadinterpolator.i
+-rw-r--r--   0 root         (0) root         (0)      619 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/quadinterpolator_face.i
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/quadrilateral.i
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/restriction.i
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/segment.i
+-rw-r--r--   0 root         (0) root         (0)      252 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/sets.i
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/socketstream.i
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/solvers.i
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/sort_pairs.i
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/sparsemat.i
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/sparsesmoothers.i
+-rw-r--r--   0 root         (0) root         (0)      631 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/stable3d.i
+-rw-r--r--   0 root         (0) root         (0)      995 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/std_vectors.i
+-rw-r--r--   0 root         (0) root         (0)      449 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/submesh.i
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/symmat.i
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/table.i
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/tetrahedron.i
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/tmop.i
+-rw-r--r--   0 root         (0) root         (0)      397 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/tmop_amr.i
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/tmop_modules.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/tmop_tools.i
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/transfer.i
+-rw-r--r--   0 root         (0) root         (0)      437 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/transfermap.i
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/triangle.i
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/vector.i
+-rw-r--r--   0 root         (0) root         (0)      757 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/vertex.i
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/vtk.i
+-rw-r--r--   0 root         (0) root         (0)      611 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/_ser/wedge.i
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/arg_parser.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/array_instantiation_macro.i
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/array_listtuple_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     7380 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/bilininteg_ext.i
+-rw-r--r--   0 root         (0) root         (0)    40525 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/chypre.py
+-rw-r--r--   0 root         (0) root         (0)     7884 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/coefficient_common.i
+-rw-r--r--   0 root         (0) root         (0)     2777 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/complex_fem_ext.i
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/const_doubleptr_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/const_intptr_typemap.i
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/cpointers.i
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/data_size_typemap.i
+-rw-r--r--   0 root         (0) root         (0)      481 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/deprecation.i
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/enum_class.i
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/exception.i
+-rw-r--r--   0 root         (0) root         (0)      544 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/exception_director.i
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/findpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/generate_bilininteg_ext.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/generate_lininteg_ext.py
+-rw-r--r--   0 root         (0) root         (0)     1231 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/handle_template.i
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/hypre_int.i
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/ignore_common_functions.i
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/io_stream.hpp
+-rw-r--r--   0 root         (0) root         (0)     9156 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/io_stream_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/lininteg_ext.i
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/matrix_file.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/memorytype_typemap.i
+-rw-r--r--   0 root         (0) root         (0)      234 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/mfem_config.i
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/mpi_debug.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/mpi_dtype.py
+-rw-r--r--   0 root         (0) root         (0)    56404 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/numba_coefficient.i
+-rw-r--r--   0 root         (0) root         (0)    16252 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/numba_coefficient_utils.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/numpy_int_typemap.i
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/object_array_typemap.i
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/operator_ptr_typemap.i
+-rw-r--r--   0 root         (0) root         (0)    16104 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/parcsr_extra.py
+-rw-r--r--   0 root         (0) root         (0)     7130 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/pycoefficient.hpp
+-rw-r--r--   0 root         (0) root         (0)      499 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/pysolvers.hpp
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/sparse_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11265 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/common/typemap_macros.i
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/par.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-07-18 02:28:46.000000 mfem-4.5.2.1/mfem/ser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8374 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-18 02:28:57.000000 mfem-4.5.2.1/mfem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 02:28:57.000000 mfem-4.5.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    59059 2023-07-18 02:28:46.000000 mfem-4.5.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 02:28:57.000000 mfem-4.5.2.1/test/
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_array.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_blockmatrix.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_blockoperator.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_chypre.py
+-rw-r--r--   0 root         (0) root         (0)     3346 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_complex_operator.py
+-rw-r--r--   0 root         (0) root         (0)    15150 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_complexmg.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_datacollection.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_densemat.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_deprecated.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_dofloc.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_fespace.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_geom.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_gridfunc.py
+-rw-r--r--   0 root         (0) root         (0)     3831 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_gz.py
+-rw-r--r--   0 root         (0) root         (0)     2760 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_intrules.py
+-rw-r--r--   0 root         (0) root         (0)      805 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)     3797 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_merge_gridfunction.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)      898 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_module.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_ncmesh.py
+-rw-r--r--   0 root         (0) root         (0)    10236 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_numba.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_periodic_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_pfespace.py
+-rw-r--r--   0 root         (0) root         (0)      528 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_point.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_segment.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_sparsemat.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_stringio.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_table.py
+-rw-r--r--   0 root         (0) root         (0)    13613 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_tmop.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-18 02:28:46.000000 mfem-4.5.2.1/test/test_vector.py
```

### Comparing `mfem-4.5.2.0rc0/LICENSE` & `mfem-4.5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/PKG-INFO` & `mfem-4.5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfem
-Version: 4.5.2.0rc0
+Version: 4.5.2.1
 Summary: MFEM + PyMFEM (finite element method library)
 Home-page: http://mfem.org
 Download-URL: https://github.com/mfem
 Author: MFEM developement team
 Author-email: 
 Maintainer: S. Shiraiwa
 Maintainer-email: shiraiwa@princeton.edu
```

### Comparing `mfem-4.5.2.0rc0/README.md` & `mfem-4.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/docs/changelog.txt` & `mfem-4.5.2.1/docs/changelog.txt`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/docs/development_memo.txt` & `mfem-4.5.2.1/docs/development_memo.txt`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/docs/example_image.png` & `mfem-4.5.2.1/docs/example_image.png`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/docs/install.txt` & `mfem-4.5.2.1/docs/install.txt`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/docs/manual.txt` & `mfem-4.5.2.1/docs/manual.txt`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
       GridFunction(FiniteElementSpace *f, double *data) is extended to
       support offsets
           v = mfem.GridFunction(fec, <pointer to double>, offset)
       so that following can be wrapped
 	  GridFunction(fes, vec.GetData() + sc)
       the same is used for ParGridFunction
 
-      GridFunction::Save(std::ostream &out) is wrapped as Save(filename, precision=8)
+      GridFunction::Save(std::ostream &out) is wrapped as Save(filename, precision)
       QuadratureFunction::Save(std::ostream &out) is wrapped as Save(filename, precision=8)
 
       GridFunction::WriteToStream(IOString) writes data to io.IOString
       ex)
           mesh = mfem.Mesh(3)
           fec = mfem.H1_FECollection(1)
           fes = mfem.FiniteElementSpace(mesh, fec)
```

### Comparing `mfem-4.5.2.0rc0/examples/ex0.py` & `mfem-4.5.2.1/examples/ex0.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex0p.py` & `mfem-4.5.2.1/examples/ex0p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex1.py` & `mfem-4.5.2.1/examples/ex1.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex10.py` & `mfem-4.5.2.1/examples/ex10.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex10p.py` & `mfem-4.5.2.1/examples/ex10p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex11p.py` & `mfem-4.5.2.1/examples/ex11p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex12p.py` & `mfem-4.5.2.1/examples/ex12p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex13p.py` & `mfem-4.5.2.1/examples/ex13p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex14.py` & `mfem-4.5.2.1/examples/ex14.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex14p.py` & `mfem-4.5.2.1/examples/ex14p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex15.py` & `mfem-4.5.2.1/examples/ex15.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex15p.py` & `mfem-4.5.2.1/examples/ex15p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex16.py` & `mfem-4.5.2.1/examples/ex16.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex16p.py` & `mfem-4.5.2.1/examples/ex16p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex17.py` & `mfem-4.5.2.1/examples/ex17.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex17p.py` & `mfem-4.5.2.1/examples/ex17p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex18.py` & `mfem-4.5.2.1/examples/ex18.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex18_common.py` & `mfem-4.5.2.1/examples/ex18_common.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex18p.py` & `mfem-4.5.2.1/examples/ex18p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex19.py` & `mfem-4.5.2.1/examples/ex19.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex19p.py` & `mfem-4.5.2.1/examples/ex19p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex1p.py` & `mfem-4.5.2.1/examples/ex1p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex2.py` & `mfem-4.5.2.1/examples/ex2.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex20.py` & `mfem-4.5.2.1/examples/ex20.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex20p.py` & `mfem-4.5.2.1/examples/ex20p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex21.py` & `mfem-4.5.2.1/examples/ex21.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex21p.py` & `mfem-4.5.2.1/examples/ex21p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex22.py` & `mfem-4.5.2.1/examples/ex22.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex22p.py` & `mfem-4.5.2.1/examples/ex22p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex23.py` & `mfem-4.5.2.1/examples/ex23.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex24.py` & `mfem-4.5.2.1/examples/ex24.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,29 +86,29 @@
                 return sin(x[0]) * sin(x[1]) * sin(x[2])
             elif dim == 2:
                 return sin(x[0]) * sin(x[1])
             return 0.0
 
         @mfem.jit.vector(shape=(sdim,))
         def gradp_coef(x):
-            out = np.zeros(shape, dtype=np.float)
+            out = np.zeros(shape, dtype=np.float64)
             if dim == 3:
                 out[0] = cos(x[0]) * sin(x[1]) * sin(x[2])
                 out[1] = sin(x[0]) * cos(x[1]) * sin(x[2])
                 out[2] = sin(x[0]) * sin(x[1]) * cos(x[2])
             elif dim == 2:
                 out[0] = cos(x[0]) * sin(x[1])
                 out[1] = sin(x[0]) * cos(x[1])
                 if len(x) == 3:
                     out[2] = 0.0
             return out
 
         @mfem.jit.vector(vdim=sdim, interface="c++")
         def v_coef(x, out):
-            out = np.zeros(shape, dtype=np.float)
+            out = np.zeros(shape, dtype=np.float64)
             if dim == 3:
                 out[0] = sin(kappa * x[1])
                 out[1] = sin(kappa * x[2])
                 out[2] = sin(kappa * x[0])
             else:
                 out[0] = sin(kappa * x[1])
                 out[1] = sin(kappa * x[0])
```

### Comparing `mfem-4.5.2.0rc0/examples/ex24p.py` & `mfem-4.5.2.1/examples/ex24p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex25.py` & `mfem-4.5.2.1/examples/ex25.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex25p.py` & `mfem-4.5.2.1/examples/ex25p.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
         D[i] = (det / (dxs[i]**2))
 
     return D
 
 
 def detJ_JT_J_inv_abs_f(x):
     dim = shape[0]
-    D = np.zeros(dim, dtype=np.float)
+    D = np.zeros(dim, dtype=np.float64)
 
     dxs = np.empty(dim, dtype=np.complex128)
     det = complex(1.0)
     StretchFunction(x, dxs)
     for i in range(dim):
         det *= dxs[i]
     for i in range(dim):
@@ -698,15 +698,15 @@
         for i in range(dim):
             D[i] = (dxs[i]**2 / det)
     return D
 
 
 def detJ_inv_JT_J_abs_f(x):
     dim = shape[0]
-    D = np.zeros(dim, dtype=np.float)
+    D = np.zeros(dim, dtype=np.float64)
 
     dxs = np.empty(dim, dtype=np.complex128)
     det = 1.0
     StretchFunction(x, dxs)
     for i in range(dim):
         det *= dxs[i]
     # in the 2D case the coefficient is scalar 1/det(J)
```

### Comparing `mfem-4.5.2.0rc0/examples/ex26.py` & `mfem-4.5.2.1/examples/ex26.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex26p.py` & `mfem-4.5.2.1/examples/ex26p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex27.py` & `mfem-4.5.2.1/examples/ex27.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex27p.py` & `mfem-4.5.2.1/examples/ex27p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex28.py` & `mfem-4.5.2.1/examples/ex28.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex28p.py` & `mfem-4.5.2.1/examples/ex28p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex29.py` & `mfem-4.5.2.1/examples/ex29.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex29p.py` & `mfem-4.5.2.1/examples/ex29p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex2p.py` & `mfem-4.5.2.1/examples/ex2p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex3.py` & `mfem-4.5.2.1/examples/ex3.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex30.py` & `mfem-4.5.2.1/examples/ex30.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex30p.py` & `mfem-4.5.2.1/examples/ex30p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex31.py` & `mfem-4.5.2.1/examples/ex31.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
             dsol_sock << "solution\n" << mesh << dsol
             dsol_sock.flush()
             dsol_sock << "window_geometry 0 375 400 350 " << "window_title 'Curl of solution'"
             dsol_sock.flush()
 
 
 def E_exact(x):
-    E = np.zeros(shape, dtype=np.float)
+    E = np.zeros(shape, dtype=np.float64)
     if dim == 1:
         E[0] = 1.1 * sin(kappa * x[0] + 0.0 * pi)
         E[1] = 1.2 * sin(kappa * x[0] + 0.4 * pi)
         E[2] = 1.3 * sin(kappa * x[0] + 0.9 * pi)
     elif dim == 2:
         E[0] = 1.1 * sin(kappa * sqrt1_2 * (x[0] + x[1]) + 0.0 * pi)
         E[1] = 1.2 * sin(kappa * sqrt1_2 * (x[0] + x[1]) + 0.4 * pi)
@@ -297,15 +297,15 @@
 
         for i in range(3):
             E[i] = E[i]*cos(kappa * x[2])
     return E
 
 
 def CurlE_exact(x):
-    dE = np.zeros(shape, dtype=np.float)
+    dE = np.zeros(shape, dtype=np.float64)
     if dim == 1:
         c4 = cos(kappa * x[0] + 0.4 * pi)
         c9 = cos(kappa * x[0] + 0.9 * pi)
 
         dE[0] = 0.0
         dE[1] = -1.3 * c9
         dE[2] = 1.2 * c4
@@ -337,15 +337,15 @@
         dE[2] = -sqrt1_2 * (1.1 * c0 - 1.2 * c4) * ck
         for i in range(3):
             dE[i] = dE[i]*kappa
     return dE
 
 
 def f_exact(x):
-    f = np.zeros(shape, dtype=np.float)
+    f = np.zeros(shape, dtype=np.float64)
     if dim == 1:
         s0 = sin(kappa * x[0] + 0.0 * pi)
         s4 = sin(kappa * x[0] + 0.4 * pi)
         s9 = sin(kappa * x[0] + 0.9 * pi)
 
         f[0] = 2.2 * s0 + 1.2 * sqrt1_2 * s4
         f[1] = (1.2 * (2.0 + kappa * kappa) * s4 +
```

### Comparing `mfem-4.5.2.0rc0/examples/ex31p.py` & `mfem-4.5.2.1/examples/ex31p.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         dE[2] = -sqrt1_2 * (1.1 * c0 - 1.2 * c4) * ck
         for i in range(3):
             dE[i] = dE[i]*kappa
     return dE
 
 
 def f_exact(x):
-    f = np.zeros(vdim, dtype=np.float)
+    f = np.zeros(vdim, dtype=np.float64)
     if dim == 1:
         s0 = sin(kappa * x[0] + 0.0 * pi)
         s4 = sin(kappa * x[0] + 0.4 * pi)
         s9 = sin(kappa * x[0] + 0.9 * pi)
 
         f[0] = 2.2 * s0 + 1.2 * sqrt1_2 * s4
         f[1] = (1.2 * (2.0 + kappa * kappa) * s4 +
```

### Comparing `mfem-4.5.2.0rc0/examples/ex32p.py` & `mfem-4.5.2.1/examples/ex32p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex33.py` & `mfem-4.5.2.1/examples/ex33.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex33_common.py` & `mfem-4.5.2.1/examples/ex33_common.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex33p.py` & `mfem-4.5.2.1/examples/ex33p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex3p.py` & `mfem-4.5.2.1/examples/ex3p.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     # 15. Compute and print the L^2 norm of the error.
     err = x.ComputeL2Error(E_exact)
     if verbose:  # note that err should be evaulated on all nodes
         print("|| E_h - E ||_{L^2} = " + "{:g}".format(err))
 
     # 16. Save the refined mesh and the solution in parallel. This output can
     #     be viewed later using GLVis: "glvis -np <np> -m mesh -g sol".
-    x.Save('sol.'+smyid)
+    x.Save('sol.'+smyid, 8)
     pmesh.Print('mesh.'+smyid)
 
     # 17. Send the solution by socket to a GLVis server
     if visualization:
         sol_sock = mfem.socketstream("localhost", 19916)
         sol_sock.precision(8)
         sol_sock << "parallel " << nprc << " " << myid << "\n"
```

### Comparing `mfem-4.5.2.0rc0/examples/ex4.py` & `mfem-4.5.2.1/examples/ex4.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex4p.py` & `mfem-4.5.2.1/examples/ex4p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex5.py` & `mfem-4.5.2.1/examples/ex5.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex5p.py` & `mfem-4.5.2.1/examples/ex5p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex6.py` & `mfem-4.5.2.1/examples/ex6.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex6p.py` & `mfem-4.5.2.1/examples/ex6p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex7.py` & `mfem-4.5.2.1/examples/ex7.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex7p.py` & `mfem-4.5.2.1/examples/ex7p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex8.py` & `mfem-4.5.2.1/examples/ex8.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex8p.py` & `mfem-4.5.2.1/examples/ex8p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex9.py` & `mfem-4.5.2.1/examples/ex9.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/ex9p.py` & `mfem-4.5.2.1/examples/ex9p.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/numba/ex4.py` & `mfem-4.5.2.1/examples/numba/ex4.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_1.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_1.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_2.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_2.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_3.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_3.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_4.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_4.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_5.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_5.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/chypre/example_6.py` & `mfem-4.5.2.1/examples/wrapper_example/chypre/example_6.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/matrix_coefficient.py` & `mfem-4.5.2.1/examples/wrapper_example/matrix_coefficient.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/examples/wrapper_example/vector.py` & `mfem-4.5.2.1/examples/wrapper_example/vector.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/headers/coefficient.hpp` & `mfem-4.5.2.1/headers/coefficient.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/headers/mem_manager.hpp` & `mfem-4.5.2.1/headers/mem_manager.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/headers/schwarz.cpp` & `mfem-4.5.2.1/headers/schwarz.cpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/headers/schwarz.hpp` & `mfem-4.5.2.1/headers/schwarz.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/__init__.py` & `mfem-4.5.2.1/mfem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         tb.print_stack()
     elif pymfem_debug > 2: # debug = 3
         import traceback as tb
         print(''.join(tb.format_list([tb.extract_stack(limit = 2)[0],])))
 
     print(message)
 
-__version__ = '4.5.2.0rc0'
+__version__ = '4.5.2.1'
```

### Comparing `mfem-4.5.2.0rc0/mfem/_par/array.i` & `mfem-4.5.2.1/mfem/_par/array.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/bilinearform.i` & `mfem-4.5.2.1/mfem/_par/bilinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/bilininteg.i` & `mfem-4.5.2.1/mfem/_par/bilininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/blockmatrix.i` & `mfem-4.5.2.1/mfem/_par/blockmatrix.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/blockoperator.i` & `mfem-4.5.2.1/mfem/_par/blockoperator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/coefficient.i` & `mfem-4.5.2.1/mfem/_par/coefficient.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/common_functions.i` & `mfem-4.5.2.1/mfem/_par/common_functions.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/communication.i` & `mfem-4.5.2.1/mfem/_par/communication.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/complex_fem.i` & `mfem-4.5.2.1/mfem/_par/complex_fem.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/complex_operator.i` & `mfem-4.5.2.1/mfem/_par/complex_operator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/constraints.i` & `mfem-4.5.2.1/mfem/_par/constraints.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/datacollection.i` & `mfem-4.5.2.1/mfem/_par/datacollection.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/densemat.i` & `mfem-4.5.2.1/mfem/_par/densemat.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/device.i` & `mfem-4.5.2.1/mfem/_par/device.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/dist_solver.i` & `mfem-4.5.2.1/mfem/_par/dist_solver.i`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 %module(package="mfem._par") dist_solver
 %{
 #include "mfem.hpp"      
-#include "miniapps/shifted/dist_solver.hpp"
+#include "miniapps/common/dist_solver.hpp"
 #include "pyoperator.hpp"
 #include "../common/pysolvers.hpp"
 #include "../common/pycoefficient.hpp"  
 #include "numpy/arrayobject.h"    
 %}
 
 %init %{
 import_array();
 %}
 
 %inline %{
-#include "miniapps/shifted/dist_solver.cpp"
+#include "miniapps/common/dist_solver.cpp"
 %}
 
 
 %include "exception.i"
 %import "element.i"
 %import "../common/exception.i"
 
 %import "coefficient.i"
 %import "pgridfunc.i"
 %import "pmesh.i"
 %import "solvers.i"
 
-%include "miniapps/shifted/dist_solver.hpp"
+%include "miniapps/common/dist_solver.hpp"
```

### Comparing `mfem-4.5.2.0rc0/mfem/_par/element.i` & `mfem-4.5.2.1/mfem/_par/element.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/eltrans.i` & `mfem-4.5.2.1/mfem/_par/eltrans.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/estimators.i` & `mfem-4.5.2.1/mfem/_par/estimators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/fe.i` & `mfem-4.5.2.1/mfem/_par/fe.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/fe_coll.i` & `mfem-4.5.2.1/mfem/_par/fe_coll.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/fespace.i` & `mfem-4.5.2.1/mfem/_par/fespace.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/geom.i` & `mfem-4.5.2.1/mfem/_par/geom.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/gridfunc.i` & `mfem-4.5.2.1/mfem/_par/gridfunc.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/handle.i` & `mfem-4.5.2.1/mfem/_par/handle.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/hexahedron.i` & `mfem-4.5.2.1/mfem/_par/hexahedron.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/hypre.i` & `mfem-4.5.2.1/mfem/_par/hypre.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/intrules.i` & `mfem-4.5.2.1/mfem/_par/intrules.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/istream_typemap.i` & `mfem-4.5.2.1/mfem/_par/istream_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/linearform.i` & `mfem-4.5.2.1/mfem/_par/linearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/lininteg.i` & `mfem-4.5.2.1/mfem/_par/lininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/matrix.i` & `mfem-4.5.2.1/mfem/_par/matrix.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/mesh.i` & `mfem-4.5.2.1/mfem/_par/mesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/mesh_operators.i` & `mfem-4.5.2.1/mfem/_par/mesh_operators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/multigrid.i` & `mfem-4.5.2.1/mfem/_par/multigrid.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/ncmesh.i` & `mfem-4.5.2.1/mfem/_par/ncmesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/nonlinearform.i` & `mfem-4.5.2.1/mfem/_par/nonlinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/nonlininteg.i` & `mfem-4.5.2.1/mfem/_par/nonlininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/ode.i` & `mfem-4.5.2.1/mfem/_par/ode.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/operators.i` & `mfem-4.5.2.1/mfem/_par/operators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/ostream_typemap.i` & `mfem-4.5.2.1/mfem/_par/ostream_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pbilinearform.i` & `mfem-4.5.2.1/mfem/_par/pbilinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pfespace.i` & `mfem-4.5.2.1/mfem/_par/pfespace.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pgridfunc.i` & `mfem-4.5.2.1/mfem/_par/pgridfunc.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/plinearform.i` & `mfem-4.5.2.1/mfem/_par/plinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pmesh.i` & `mfem-4.5.2.1/mfem/_par/pmesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pncmesh.i` & `mfem-4.5.2.1/mfem/_par/pncmesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pnonlinearform.i` & `mfem-4.5.2.1/mfem/_par/pnonlinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pumi.i` & `mfem-4.5.2.1/mfem/_par/pumi.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pycoefficient.hpp` & `mfem-4.5.2.1/mfem/_par/pycoefficient.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/pyoperator.hpp` & `mfem-4.5.2.1/mfem/_par/pyoperator.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/qfunction.i` & `mfem-4.5.2.1/mfem/_par/qfunction.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/qspace.i` & `mfem-4.5.2.1/mfem/_par/qspace.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/quadinterpolator.i` & `mfem-4.5.2.1/mfem/_par/quadinterpolator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/quadinterpolator_face.i` & `mfem-4.5.2.1/mfem/_par/quadinterpolator_face.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/quadrilateral.i` & `mfem-4.5.2.1/mfem/_par/quadrilateral.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/schwarz.i` & `mfem-4.5.2.1/mfem/_par/schwarz.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/setup.py` & `mfem-4.5.2.1/mfem/_par/setup.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/socketstream.i` & `mfem-4.5.2.1/mfem/_par/socketstream.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/solvers.i` & `mfem-4.5.2.1/mfem/_par/solvers.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/sparsemat.i` & `mfem-4.5.2.1/mfem/_par/sparsemat.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/stable3d.i` & `mfem-4.5.2.1/mfem/_par/stable3d.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/std_vectors.i` & `mfem-4.5.2.1/mfem/_par/std_vectors.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/strumpack.i` & `mfem-4.5.2.1/mfem/_par/strumpack.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/table.i` & `mfem-4.5.2.1/mfem/_par/table.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/tetrahedron.i` & `mfem-4.5.2.1/mfem/_par/tetrahedron.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/tmop.i` & `mfem-4.5.2.1/mfem/_par/tmop.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/tmop_tools.i` & `mfem-4.5.2.1/mfem/_par/tmop_tools.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/triangle.i` & `mfem-4.5.2.1/mfem/_par/triangle.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/vector.i` & `mfem-4.5.2.1/mfem/_par/vector.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_par/wedge.i` & `mfem-4.5.2.1/mfem/_par/wedge.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/array.i` & `mfem-4.5.2.1/mfem/_ser/array.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/bilinearform.i` & `mfem-4.5.2.1/mfem/_ser/bilinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/bilininteg.i` & `mfem-4.5.2.1/mfem/_ser/bilininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/blockmatrix.i` & `mfem-4.5.2.1/mfem/_ser/blockmatrix.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/blockoperator.i` & `mfem-4.5.2.1/mfem/_ser/blockoperator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/coefficient.i` & `mfem-4.5.2.1/mfem/_ser/coefficient.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/common_functions.i` & `mfem-4.5.2.1/mfem/_ser/common_functions.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/complex_fem.i` & `mfem-4.5.2.1/mfem/_ser/complex_fem.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/complex_operator.i` & `mfem-4.5.2.1/mfem/_ser/complex_operator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/constraints.i` & `mfem-4.5.2.1/mfem/_ser/constraints.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/densemat.i` & `mfem-4.5.2.1/mfem/_ser/densemat.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/device.i` & `mfem-4.5.2.1/mfem/_ser/device.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/element.i` & `mfem-4.5.2.1/mfem/_ser/element.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/eltrans.i` & `mfem-4.5.2.1/mfem/_ser/eltrans.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/estimators.i` & `mfem-4.5.2.1/mfem/_ser/estimators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/fe.i` & `mfem-4.5.2.1/mfem/_ser/fe.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/fe_coll.i` & `mfem-4.5.2.1/mfem/_ser/fe_coll.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/fespace.i` & `mfem-4.5.2.1/mfem/_ser/fespace.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/geom.i` & `mfem-4.5.2.1/mfem/_ser/geom.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/gridfunc.i` & `mfem-4.5.2.1/mfem/_ser/gridfunc.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/handle.i` & `mfem-4.5.2.1/mfem/_ser/handle.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/hexahedron.i` & `mfem-4.5.2.1/mfem/_ser/hexahedron.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/intrules.i` & `mfem-4.5.2.1/mfem/_ser/intrules.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/istream_typemap.i` & `mfem-4.5.2.1/mfem/_ser/istream_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/linearform.i` & `mfem-4.5.2.1/mfem/_ser/linearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/lininteg.i` & `mfem-4.5.2.1/mfem/_ser/lininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/matrix.i` & `mfem-4.5.2.1/mfem/_ser/matrix.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/mesh.i` & `mfem-4.5.2.1/mfem/_ser/mesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/mesh_operators.i` & `mfem-4.5.2.1/mfem/_ser/mesh_operators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/multigrid.i` & `mfem-4.5.2.1/mfem/_ser/multigrid.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/ncmesh.i` & `mfem-4.5.2.1/mfem/_ser/ncmesh.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/nonlinearform.i` & `mfem-4.5.2.1/mfem/_ser/nonlinearform.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/nonlininteg.i` & `mfem-4.5.2.1/mfem/_ser/nonlininteg.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/ode.i` & `mfem-4.5.2.1/mfem/_ser/ode.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/operators.i` & `mfem-4.5.2.1/mfem/_ser/operators.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/ostream_typemap.i` & `mfem-4.5.2.1/mfem/_ser/ostream_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/point.i` & `mfem-4.5.2.1/mfem/_ser/point.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/pyoperator.hpp` & `mfem-4.5.2.1/mfem/_ser/pyoperator.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/qfunction.i` & `mfem-4.5.2.1/mfem/_ser/qfunction.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/qspace.i` & `mfem-4.5.2.1/mfem/_ser/qspace.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/quadinterpolator.i` & `mfem-4.5.2.1/mfem/_ser/quadinterpolator.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/quadinterpolator_face.i` & `mfem-4.5.2.1/mfem/_ser/quadinterpolator_face.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/quadrilateral.i` & `mfem-4.5.2.1/mfem/_ser/quadrilateral.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/segment.i` & `mfem-4.5.2.1/mfem/_ser/segment.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/setup.py` & `mfem-4.5.2.1/mfem/_ser/setup.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/socketstream.i` & `mfem-4.5.2.1/mfem/_ser/socketstream.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/solvers.i` & `mfem-4.5.2.1/mfem/_ser/solvers.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/sparsemat.i` & `mfem-4.5.2.1/mfem/_ser/sparsemat.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/sparsesmoothers.i` & `mfem-4.5.2.1/mfem/_ser/sparsesmoothers.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/stable3d.i` & `mfem-4.5.2.1/mfem/_ser/stable3d.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/std_vectors.i` & `mfem-4.5.2.1/mfem/_ser/std_vectors.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/table.i` & `mfem-4.5.2.1/mfem/_ser/table.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/tetrahedron.i` & `mfem-4.5.2.1/mfem/_ser/tetrahedron.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/tmop.i` & `mfem-4.5.2.1/mfem/_ser/tmop.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/tmop_tools.i` & `mfem-4.5.2.1/mfem/_ser/tmop_tools.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/triangle.i` & `mfem-4.5.2.1/mfem/_ser/triangle.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/vector.i` & `mfem-4.5.2.1/mfem/_ser/vector.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/vertex.i` & `mfem-4.5.2.1/mfem/_ser/vertex.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/_ser/wedge.i` & `mfem-4.5.2.1/mfem/_ser/wedge.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/arg_parser.py` & `mfem-4.5.2.1/mfem/common/arg_parser.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/array_instantiation_macro.i` & `mfem-4.5.2.1/mfem/common/array_instantiation_macro.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/array_listtuple_typemap.i` & `mfem-4.5.2.1/mfem/common/array_listtuple_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/bilininteg_ext.i` & `mfem-4.5.2.1/mfem/common/bilininteg_ext.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/chypre.py` & `mfem-4.5.2.1/mfem/common/chypre.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/coefficient_common.i` & `mfem-4.5.2.1/mfem/common/coefficient_common.i`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 %}
   
 %pythonappend MatrixRestrictedCoefficient::MatrixRestrictedCoefficient %{
     self._ref_to_mc = mc
 %}
 
 %pythonappend SumCoefficient::SumCoefficient %{
-    if len(args) > 0 and isinstance(agrs[0], Coefficient):
+    if len(args) > 0 and isinstance(args[0], Coefficient):
           self.linkA = args[0]
-    if len(args) > 1 and isinstance(agrs[1], Coefficient):
+    if len(args) > 1 and isinstance(args[1], Coefficient):
           self.linkB = args[0]
 
 %}
 %pythonappend SumCoefficient::SetACoef %{
     self.linkA = A    
 %}    
 %pythonappend SumCoefficient::SetBCoef %{
```

### Comparing `mfem-4.5.2.0rc0/mfem/common/complex_fem_ext.i` & `mfem-4.5.2.1/mfem/common/complex_fem_ext.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/const_doubleptr_typemap.i` & `mfem-4.5.2.1/mfem/common/const_doubleptr_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/const_intptr_typemap.i` & `mfem-4.5.2.1/mfem/common/const_intptr_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/data_size_typemap.i` & `mfem-4.5.2.1/mfem/common/data_size_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/enum_class.i` & `mfem-4.5.2.1/mfem/common/enum_class.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/exception_director.i` & `mfem-4.5.2.1/mfem/common/exception_director.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/findpoints.py` & `mfem-4.5.2.1/mfem/common/findpoints.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/generate_bilininteg_ext.py` & `mfem-4.5.2.1/mfem/common/generate_bilininteg_ext.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/generate_lininteg_ext.py` & `mfem-4.5.2.1/mfem/common/generate_lininteg_ext.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/handle_template.i` & `mfem-4.5.2.1/mfem/common/handle_template.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/io_stream.hpp` & `mfem-4.5.2.1/mfem/common/io_stream.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 namespace PyMFEM
 {
 class wFILE
 {
     private:
        int _isSTDOUT;
-       char _filename[255];
+       char _filename[65535];
        int _precision=8;
        bool _temporary=false;
     public:
        wFILE(void){
 	 strcpy(_filename, "__stdout__");
 	 _isSTDOUT = 1;
 	 _temporary = 0;
```

### Comparing `mfem-4.5.2.0rc0/mfem/common/io_stream_typemap.i` & `mfem-4.5.2.1/mfem/common/io_stream_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/lininteg_ext.i` & `mfem-4.5.2.1/mfem/common/lininteg_ext.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/memorytype_typemap.i` & `mfem-4.5.2.1/mfem/common/memorytype_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/mpi_debug.py` & `mfem-4.5.2.1/mfem/common/mpi_debug.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/mpi_dtype.py` & `mfem-4.5.2.1/mfem/common/mpi_dtype.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/numba_coefficient.i` & `mfem-4.5.2.1/mfem/common/numba_coefficient.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/numba_coefficient_utils.py` & `mfem-4.5.2.1/mfem/common/numba_coefficient_utils.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/object_array_typemap.i` & `mfem-4.5.2.1/mfem/common/object_array_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/operator_ptr_typemap.i` & `mfem-4.5.2.1/mfem/common/operator_ptr_typemap.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/parcsr_extra.py` & `mfem-4.5.2.1/mfem/common/parcsr_extra.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/pycoefficient.hpp` & `mfem-4.5.2.1/mfem/common/pycoefficient.hpp`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/sparse_utils.py` & `mfem-4.5.2.1/mfem/common/sparse_utils.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/common/typemap_macros.i` & `mfem-4.5.2.1/mfem/common/typemap_macros.i`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/par.py` & `mfem-4.5.2.1/mfem/par.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem/ser.py` & `mfem-4.5.2.1/mfem/ser.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/mfem.egg-info/PKG-INFO` & `mfem-4.5.2.1/mfem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfem
-Version: 4.5.2.0rc0
+Version: 4.5.2.1
 Summary: MFEM + PyMFEM (finite element method library)
 Home-page: http://mfem.org
 Download-URL: https://github.com/mfem
 Author: MFEM developement team
 Author-email: 
 Maintainer: S. Shiraiwa
 Maintainer-email: shiraiwa@princeton.edu
```

### Comparing `mfem-4.5.2.0rc0/mfem.egg-info/SOURCES.txt` & `mfem-4.5.2.1/mfem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/setup.py` & `mfem-4.5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 
 repos = {"mfem": "https://github.com/mfem/mfem.git",
          "libceed": "https://github.com/CEED/libCEED.git",
          "gklib": "https://github.com/KarypisLab/GKlib",
          "metis": "https://github.com/KarypisLab/METIS", }
 repos_sha = {
     # "mfem": "2f6eb8838f8f5e8359abba0dd3434c8cc7147012",
-    "mfem": "00b2a0705f647e17a1d4ffcb289adca503f28d42",  # version 4.5.2
+    #"mfem": "00b2a0705f647e17a1d4ffcb289adca503f28d42", # version 4.5.2
+    "mfem": "962774d5ffa84ceed3bc670e52388250ee028da1",  # version 4.5.2 + distsolve
     "gklib": "a7f8172703cf6e999dd0710eb279bba513da4fec",
     "metis": "94c03a6e2d1860128c2d0675cbbb86ad4f261256", }
 
 rootdir = os.path.abspath(os.path.dirname(__file__))
 extdir = os.path.join(rootdir, 'external')
 if not os.path.exists(extdir):
     os.mkdir(os.path.join(rootdir, 'external'))
```

### Comparing `mfem-4.5.2.0rc0/test/test_array.py` & `mfem-4.5.2.1/test/test_array.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_blockmatrix.py` & `mfem-4.5.2.1/test/test_blockmatrix.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_blockoperator.py` & `mfem-4.5.2.1/test/test_blockoperator.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_chypre.py` & `mfem-4.5.2.1/test/test_chypre.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_complex_operator.py` & `mfem-4.5.2.1/test/test_complex_operator.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_complexmg.py` & `mfem-4.5.2.1/test/test_complexmg.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_datacollection.py` & `mfem-4.5.2.1/test/test_datacollection.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_densemat.py` & `mfem-4.5.2.1/test/test_densemat.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_dofloc.py` & `mfem-4.5.2.1/test/test_dofloc.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_fespace.py` & `mfem-4.5.2.1/test/test_fespace.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_geom.py` & `mfem-4.5.2.1/test/test_geom.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_gridfunc.py` & `mfem-4.5.2.1/test/test_gridfunc.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_gz.py` & `mfem-4.5.2.1/test/test_gz.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_intrules.py` & `mfem-4.5.2.1/test/test_intrules.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_memory.py` & `mfem-4.5.2.1/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_merge_gridfunction.py` & `mfem-4.5.2.1/test/test_merge_gridfunction.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_mesh.py` & `mfem-4.5.2.1/test/test_mesh.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_module.py` & `mfem-4.5.2.1/test/test_module.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_ncmesh.py` & `mfem-4.5.2.1/test/test_ncmesh.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_numba.py` & `mfem-4.5.2.1/test/test_numba.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_periodic_mesh.py` & `mfem-4.5.2.1/test/test_periodic_mesh.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_pfespace.py` & `mfem-4.5.2.1/test/test_pfespace.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_point.py` & `mfem-4.5.2.1/test/test_point.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_segment.py` & `mfem-4.5.2.1/test/test_segment.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_sparsemat.py` & `mfem-4.5.2.1/test/test_sparsemat.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_table.py` & `mfem-4.5.2.1/test/test_table.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_tmop.py` & `mfem-4.5.2.1/test/test_tmop.py`

 * *Files identical despite different names*

### Comparing `mfem-4.5.2.0rc0/test/test_vector.py` & `mfem-4.5.2.1/test/test_vector.py`

 * *Files identical despite different names*

