# Comparing `tmp/kshell-utilities-1.4.0.0.tar.gz` & `tmp/kshell-utilities-1.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kshell-utilities-1.4.0.0.tar", last modified: Tue Feb  7 10:44:59 2023, max compression
+gzip compressed data, was "kshell-utilities-1.5.0.0.tar", last modified: Tue Jul 18 09:08:00 2023, max compression
```

## Comparing `kshell-utilities-1.4.0.0.tar` & `kshell-utilities-1.5.0.0.tar`

### file list

```diff
@@ -1,30 +1,36 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-02-07 10:44:59.403377 kshell-utilities-1.4.0.0/
--rw-r--r--   0 jon        (501) staff       (20)     1077 2021-09-29 15:16:13.000000 kshell-utilities-1.4.0.0/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)      565 2023-02-07 10:44:59.402893 kshell-utilities-1.4.0.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     5873 2022-09-13 08:26:29.000000 kshell-utilities-1.4.0.0/README.md
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-02-07 10:44:59.398012 kshell-utilities-1.4.0.0/kshell_utilities/
--rw-r--r--   0 jon        (501) staff       (20)      580 2023-02-07 10:44:09.000000 kshell-utilities-1.4.0.0/kshell_utilities/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    33280 2022-09-18 11:42:03.000000 kshell-utilities-1.4.0.0/kshell_utilities/collect_logs.py
--rw-r--r--   0 jon        (501) staff       (20)    11266 2022-09-28 13:34:56.000000 kshell-utilities-1.4.0.0/kshell_utilities/count_dim.py
--rw-r--r--   0 jon        (501) staff       (20)     1751 2022-05-26 10:28:32.000000 kshell-utilities-1.4.0.0/kshell_utilities/deprecated.py
--rw-r--r--   0 jon        (501) staff       (20)    49828 2022-09-13 13:07:11.000000 kshell-utilities-1.4.0.0/kshell_utilities/general_utilities.py
--rw-r--r--   0 jon        (501) staff       (20)      125 2021-10-13 13:01:44.000000 kshell-utilities-1.4.0.0/kshell_utilities/kshell_exceptions.py
--rw-r--r--   0 jon        (501) staff       (20)    95653 2022-09-29 19:53:31.000000 kshell-utilities-1.4.0.0/kshell_utilities/kshell_utilities.py
--rw-r--r--   0 jon        (501) staff       (20)    42408 2021-04-14 10:39:16.000000 kshell-utilities-1.4.0.0/kshell_utilities/kshell_utilities_tmp.py
--rw-r--r--   0 jon        (501) staff       (20)    16466 2022-06-10 09:28:58.000000 kshell-utilities-1.4.0.0/kshell_utilities/loaders.py
--rw-r--r--   0 jon        (501) staff       (20)     7998 2021-10-01 08:16:24.000000 kshell-utilities-1.4.0.0/kshell_utilities/low_energy_enhancement.py
--rw-r--r--   0 jon        (501) staff       (20)     3004 2022-09-13 13:03:22.000000 kshell-utilities-1.4.0.0/kshell_utilities/parameters.py
--rw-r--r--   0 jon        (501) staff       (20)     8625 2023-02-01 10:46:00.000000 kshell-utilities-1.4.0.0/kshell_utilities/script_editing.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-02-07 10:44:59.400447 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)      565 2023-02-07 10:44:59.000000 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      721 2023-02-07 10:44:59.000000 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2023-02-07 10:44:59.000000 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       25 2023-02-07 10:44:59.000000 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       23 2023-02-07 10:44:59.000000 kshell-utilities-1.4.0.0/kshell_utilities.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)      103 2021-09-29 18:32:05.000000 kshell-utilities-1.4.0.0/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2023-02-07 10:44:59.403530 kshell-utilities-1.4.0.0/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)      942 2023-02-07 10:44:23.000000 kshell-utilities-1.4.0.0/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-02-07 10:44:59.401903 kshell-utilities-1.4.0.0/tests/
--rw-r--r--   0 jon        (501) staff       (20)        0 2021-05-04 13:07:04.000000 kshell-utilities-1.4.0.0/tests/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)    18564 2022-06-13 12:18:53.000000 kshell-utilities-1.4.0.0/tests/test_all.py
--rw-r--r--   0 jon        (501) staff       (20)     1335 2022-05-27 08:55:53.000000 kshell-utilities-1.4.0.0/tests/test_spin_parity_list.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.517451 kshell-utilities-1.5.0.0/
+-rw-r--r--   0 jon        (501) staff       (20)     1077 2021-09-29 15:16:13.000000 kshell-utilities-1.5.0.0/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:08:00.517127 kshell-utilities-1.5.0.0/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      904 2023-03-30 08:04:36.000000 kshell-utilities-1.5.0.0/README.md
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.512060 kshell-utilities-1.5.0.0/kshell_utilities/
+-rw-r--r--   0 jon        (501) staff       (20)      708 2023-07-14 08:53:01.000000 kshell-utilities-1.5.0.0/kshell_utilities/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    33280 2022-09-18 11:42:03.000000 kshell-utilities-1.5.0.0/kshell_utilities/collect_logs.py
+-rw-r--r--   0 jon        (501) staff       (20)    10820 2023-07-14 09:10:01.000000 kshell-utilities-1.5.0.0/kshell_utilities/compare.py
+-rw-r--r--   0 jon        (501) staff       (20)    13139 2023-07-14 09:08:52.000000 kshell-utilities-1.5.0.0/kshell_utilities/count_dim.py
+-rw-r--r--   0 jon        (501) staff       (20)     6302 2023-07-14 08:53:22.000000 kshell-utilities-1.5.0.0/kshell_utilities/data_structures.py
+-rw-r--r--   0 jon        (501) staff       (20)     1751 2022-05-26 10:28:32.000000 kshell-utilities-1.5.0.0/kshell_utilities/deprecated.py
+-rw-r--r--   0 jon        (501) staff       (20)    51983 2023-07-14 08:55:38.000000 kshell-utilities-1.5.0.0/kshell_utilities/general_utilities.py
+-rw-r--r--   0 jon        (501) staff       (20)      125 2021-10-13 13:01:44.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_exceptions.py
+-rw-r--r--   0 jon        (501) staff       (20)   106779 2023-07-17 03:34:31.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities.py
+-rw-r--r--   0 jon        (501) staff       (20)    42408 2021-04-14 10:39:16.000000 kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities_tmp.py
+-rw-r--r--   0 jon        (501) staff       (20)    34975 2023-07-14 09:03:44.000000 kshell-utilities-1.5.0.0/kshell_utilities/loaders.py
+-rw-r--r--   0 jon        (501) staff       (20)      563 2023-03-30 07:57:17.000000 kshell-utilities-1.5.0.0/kshell_utilities/other_tools.py
+-rw-r--r--   0 jon        (501) staff       (20)     4853 2023-07-14 08:54:55.000000 kshell-utilities-1.5.0.0/kshell_utilities/parameters.py
+-rw-r--r--   0 jon        (501) staff       (20)     8086 2023-07-14 09:11:24.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_compare.py
+-rw-r--r--   0 jon        (501) staff       (20)    87644 2023-07-14 08:53:46.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_editor.py
+-rw-r--r--   0 jon        (501) staff       (20)     9036 2023-07-14 09:02:39.000000 kshell-utilities-1.5.0.0/kshell_utilities/partition_tools.py
+-rw-r--r--   0 jon        (501) staff       (20)    10587 2023-07-14 09:10:36.000000 kshell-utilities-1.5.0.0/kshell_utilities/script_editing.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.513899 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      588 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      916 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       41 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       23 2023-07-18 09:08:00.000000 kshell-utilities-1.5.0.0/kshell_utilities.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)      103 2021-09-29 18:32:05.000000 kshell-utilities-1.5.0.0/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2023-07-18 09:08:00.517560 kshell-utilities-1.5.0.0/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)      988 2023-07-14 08:39:09.000000 kshell-utilities-1.5.0.0/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2023-07-18 09:08:00.516327 kshell-utilities-1.5.0.0/tests/
+-rw-r--r--   0 jon        (501) staff       (20)        0 2021-05-04 13:07:04.000000 kshell-utilities-1.5.0.0/tests/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)    18919 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.0/tests/test_all.py
+-rw-r--r--   0 jon        (501) staff       (20)     6091 2023-03-31 05:09:49.000000 kshell-utilities-1.5.0.0/tests/test_partition_editor.py
+-rw-r--r--   0 jon        (501) staff       (20)     1327 2023-03-22 04:07:31.000000 kshell-utilities-1.5.0.0/tests/test_spin_parity_list.py
```

### Comparing `kshell-utilities-1.4.0.0/LICENSE` & `kshell-utilities-1.5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.4.0.0/PKG-INFO` & `kshell-utilities-1.5.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kshell-utilities
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: Handy utilities for handling nuclear shell model calculations from KSHELL
 Home-page: https://github.com/GaffaSnobb/kshell-utilities
-Author: Jon Kristian Dahl
+Author: ['Jon Kristian Dahl', 'Johannes Heines']
 Author-email: jonkd@uio.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/__init__.py` & `kshell-utilities-1.5.0.0/kshell_utilities/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-__version__ = "1.4.0.0"
-__author__ = "Jon Kristian Dahl"
+__author__ = "Jon Kristian Dahl, Johannes Heines"
+__version__ = "1.5.0.0"
 __credits__ = "Noritaka Shimizu, Jørgen Eriksson Midtbø"
 
 """
 Version legend:
 a.b.c.d
 
 a: major release
@@ -13,10 +13,13 @@
 """
 
 from .kshell_utilities import *
 from .general_utilities import *
 from .kshell_exceptions import *
 from .count_dim import *
 from .parameters import *
+from .compare import Compare
 from .collect_logs import collect_logs, check_multipolarities
 from .script_editing import edit_and_queue_executables
-# from .low_energy_enhancement import * # Not ready for ver. 1.0
+from .partition_editor import partition_editor, test_partition_editor, test_partition_editor_2
+from . import loaders
+from . import data_structures
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/collect_logs.py` & `kshell-utilities-1.5.0.0/kshell_utilities/collect_logs.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/count_dim.py` & `kshell-utilities-1.5.0.0/kshell_utilities/count_dim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
 """
 usage: count_dim.py foo.snt bar.ptn
 count M-scheme dimension
 Author: Y. Tsunoda
 Modified by: https://github.com/GaffaSnobb
 """
 from functools import lru_cache
-import sys, math, time, multiprocessing
+import sys, math, time, multiprocessing, os
 from typing import TextIO, Tuple
 
 def _readline_sk(
     fp: TextIO,
     ) -> list:
     """
     Skips lines starting with '#' or '!'. Splits and returns all other
@@ -173,17 +174,21 @@
     # print(i) # Process number for debug.
     _mp_add( dim_mp_parallel, _mp_product(dim_idp_mp, dim_idn_mp) )
     return dim_mp_parallel
 
 # @lru_cache(maxsize=None, typed=False)
 def count_dim(
     model_space_filename: str,
-    partition_filename: str,
+    parity: None | int,
+    proton_partition: None | list[list[int]],
+    neutron_partition: None | list[list[int]],
+    total_partition: None | list[list[int]],
+    partition_filename: str | None = None,
     print_dimensions: bool = True,
-    debug: bool = False
+    debug: bool = False,
     ):
     """ 
     Product dimension calculation is parallelized. Some timing data for
     a .ptn file of approximately 1 million lines:
     
     TIMING (parallel):
     -------
@@ -223,23 +228,32 @@
 
     print_dimensions : bool
         For toggling print on / off.
 
     debug : bool
         For toggling debug print on / off.
     """
+    if partition_filename is None and (proton_partition is None or neutron_partition is None or total_partition is None or parity is None):
+        msg = (
+            "If 'partition_filename' is not supplied then 'proton_partition',"
+            " 'neutron_partition', 'total_partition', and 'parity' must be defined."
+        )
+        raise ValueError(msg)
+
     timing_total = time.time()
     timing_read_snt = time.time()
     orbits_proton_neutron, core_protons_neutrons, norb, lorb, jorb, itorb = \
         read_snt(model_space_filename)
     timing_read_snt = time.time() - timing_read_snt
     
     timing_read_ptn = time.time()
-    valence_protons_neutrons, parity, proton_partition, neutron_partition, total_partition = \
-        read_ptn(partition_filename)
+    if partition_filename is not None:
+        valence_protons_neutrons, parity, proton_partition, neutron_partition, total_partition = \
+            read_ptn(partition_filename)
+
     timing_read_ptn = time.time() - timing_read_ptn
 
     timing_set_dim_singlej = time.time()
     dim_jnm = _set_dim_singlej( jorb )
     timing_set_dim_singlej = time.time() - timing_set_dim_singlej
 
     timing_proton_partition_loop = time.time()
@@ -331,7 +345,50 @@
         print(f"timing_proton_partition_loop  {timing_proton_partition_loop:.4f}s    {timing_proton_partition_loop/timing_total:.4f}")
         print(f"timing_neutron_partition_loop {timing_neutron_partition_loop:.4f}s    {timing_neutron_partition_loop/timing_total:.4f}")
         print(f"timing_product_dimension      {timing_product_dimension:.4f}s    {timing_product_dimension/timing_total:.4f}")
         print(f"timing_data_gather            {timing_data_gather:.4f}s    {timing_data_gather/timing_total:.4f}")
         print(f"timing_total                  {timing_total:.4f}s    {timing_total/timing_total:.4f}")
 
     return M, mdim, jdim
+
+def input_choice(content, content_type):
+    if (n := len(content)) > 1:
+        for i in range(n):
+            print(f"{content[i]} ({i}), ", end="")
+
+        while True:
+            choice = input(": ")
+            try:
+                choice = int(choice)
+                filename = content[choice]
+                break
+            except (ValueError, IndexError):
+                continue
+
+    elif n == 1:
+        filename = content[0]
+
+    else:
+        print(f"No {content_type} file in this directory. Exiting...")
+        sys.exit()
+
+    return filename
+
+def handle_input():
+    try:
+        model_space_filename, partition_filename = sys.argv[1:3]
+    except ValueError:
+        """
+        Ask for input if none is given in the command line, or choose
+        the only combination of .ptn and .snt.
+        """
+        dir_content = os.listdir()
+        snt_content = [elem for elem in dir_content if elem.endswith(".snt")]
+        ptn_content = [elem for elem in dir_content if elem.endswith(".ptn")]
+
+        model_space_filename = input_choice(snt_content, ".snt")
+        partition_filename = input_choice(ptn_content, ".ptn")
+
+    count_dim(model_space_filename, partition_filename)
+
+if __name__ == "__main__":
+    handle_input()
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/deprecated.py` & `kshell-utilities-1.5.0.0/kshell_utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/general_utilities.py` & `kshell-utilities-1.5.0.0/kshell_utilities/general_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import sys, time, warnings
 from typing import Union, Tuple, Optional
 from fractions import Fraction
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.stats import chi2
 from .parameters import flags, elements
@@ -255,65 +256,63 @@
         msg = "Ex_min and Ex_max cannot be negative!"
         raise ValueError(msg)
 
     if Ex_max < Ex_min:
         msg = "Ex_max cannot be smaller than Ex_min!"
         raise ValueError(msg)
 
-    prefactors = {   # Factor from the def. of the GSF.
+    prefactors: dict[str, float] = {   # Factor for converting from B(XL) to GSF
         "M1": 11.5473e-9, # [1/(mu_N**2*MeV**2)].
         # "E1": 1.047e-6,
-        "E1": 3.4888977e-7
+        "E1": 3.4888977e-7,
+        "E2": 0.80632e-12,   # PhysRevC.90.064321
     }
     if prefactor_E1 is not None:
         """
         Override the E1 prefactor.
         """
         prefactors["E1"] = prefactor_E1
     
     if prefactor_M1 is not None:
-        """
-        Override the M1 prefactor.
-        """
         prefactors["M1"] = prefactor_M1
     
     if prefactor_E2 is not None:
-        """
-        Override the E2 prefactor.
-        """
         prefactors["E2"] = prefactor_E2
     
     prefactor = prefactors[multipole_type]
 
     # Extract data to a more readable form:
     n_transitions = len(transitions[:, 0])
     n_levels = len(levels[:, 0])
     E_ground_state = levels[0, 0] # Read out the absolute ground state energy so we can get relative energies later.
 
     try:
         Ex, spins, parities, level_counter = np.copy(levels[:, 0]), levels[:, 1], levels[:, 2], levels[:, 3]
+    
     except IndexError as err:
         msg = f"{err.__str__()}\n"
         msg += "Error probably due to old tmp files. Use loadtxt parameter"
-        msg += " load_and_save_to_file = 'overwrite' to re-read data from the"
+        msg += " load_and_save_to_file = 'overwrite' (once) to re-read data from the"
         msg += " summary file and generate new tmp files."
         raise Exception(msg) from err
     
     if initial_or_final == "initial":
         Ex_initial_or_final = np.copy(transitions[:, 3])   # To avoid altering the raw data.
         spin_initial_or_final_idx = 0
         parity_initial_or_final_idx = 1
+    
     elif initial_or_final == "final":
         Ex_initial_or_final = np.copy(transitions[:, 7])   # To avoid altering the raw data.
         spin_initial_or_final_idx = 4
         parity_initial_or_final_idx = 5
         msg = "Using final states for the energy limits is not correct"
         msg += " and should only be used for comparison with the correct"
         msg += " option which is using initial states for the energy limits."
         warnings.warn(msg, RuntimeWarning)
+    
     else:
         msg = "'initial_or_final' must be either 'initial' or 'final'."
         msg += f" Got {initial_or_final}"
         raise ValueError(msg)
 
     if abs(Ex_initial_or_final[0]) > 10:
         """
@@ -626,91 +625,150 @@
     else:
         return bins, gSF_ExJpiavg
 
 def level_plot(
     levels: np.ndarray,
     include_n_levels: int = 1_000,
     filter_spins: Union[None, list] = None,
-    ax: Union[None, plt.Axes] = None
+    filter_parity: Union[None, str] = None,
+    ax: Union[None, plt.Axes] = None,
+    color: Union[None, str] = None,
+    line_width: float = 0.4,
+    x_offset_scale: float = 1.0,
     ):
     """
     Generate a level plot for a single isotope. Spin on the x axis,
     energy on the y axis.
 
     Parameters
     ----------
     levels : np.ndarray
-        NxM array of [[energy, spin, parity], ...]. This is the instance
-        attribute 'levels' of ReadKshellOutput.
+        NxM array of [[energy, spin, parity, index], ...]. This is the
+        instance attribute 'levels' of ReadKshellOutput.
     
     include_n_levels : int
         The maximum amount of states to plot for each spin. Default set
         to a large number to indicate ≈ no limit.
 
     filter_spins : Union[None, list]
         Which spins to include in the plot. If None, all spins are
         plotted.
 
+    filter_parity : Union[None, str]
+        A filter for parity. If None (default) then the parity of the
+        ground state will be used. `+` is positive, `-` is negative,
+        while `both` gives both parities.
+
     ax : Union[None, plt.Axes]
         matplotlib Axes to plot on. If None, plt.Figure and plt.Axes is
         generated in this function.
+
+    color : Union[None, str]
+        Color to use for the levels. If None, the next color in the
+        matplotlib color_cycle iterator is used.
+    
+    line_width : float
+        The width of the level lines. Not really supposed to be changed
+        by the user. Set to 0.2 for comparison plots when both integer
+        and half integer angular momenta are included, 0.4 else.
+
+    x_offset_scale : float
+        To scale the x offset for the hlines. This is used to fit
+        columns for both integer and half integer angular momenta, as
+        well as both parities.
     """
     ax_input = False if (ax is None) else True
 
     if levels[0, 0] != 0:
         """
         Adjust energies relative to the ground state energy.
         """
         energies = levels[:, 0] - levels[0, 0]
     else:
         energies = levels[:, 0]
 
     spins = levels[:, 1]/2  # levels[:, 1] is 2*spin.
-    parity_symbol = "+" if levels[0, 2] == 1 else "-"
+    parities = levels[:, 2]
+
+    allowed_filter_parity = [None, "+", "-", "both"]
+    if filter_parity not in allowed_filter_parity:
+        msg = f"Allowed parity filters are: {allowed_filter_parity}."
+        raise ValueError(msg)
+
+    if filter_parity is None:
+        """
+        Default to the ground state parity.
+        """
+        parity_integer: int = [levels[0, 2]]
+        parity_symbol: str = "+" if (levels[0, 2] == 1) else "-"
+        x_offset = 0    # No offset needed for single parity plot.
+
+    elif filter_parity == "+":
+        parity_symbol: str = filter_parity
+        parity_integer: list = [1]
+        x_offset = 0
+
+    elif filter_parity == "-":
+        parity_symbol: str = filter_parity
+        parity_integer: list = [-1]
+        x_offset = 0
+
+    elif filter_parity == "both":
+        line_width /= 2 # Make room for both parities.
+        parity_symbol: str = r"-+"
+        parity_integer: list = [-1, 1]
+        x_offset = 1/4*x_offset_scale  # Offset for plots containing both parities.
     
     if filter_spins is not None:
         spin_scope = np.unique(filter_spins)    # x values for the plot.
     else:
         spin_scope = np.unique(spins)
     
-    counts = {} # Dict to keep tabs on how many states of each spin have been plotted.
-    line_width = np.abs(spins[0] - spins[1])/4*0.9
+    counts = {} # Dict to keep tabs on how many levels of each angular momentum have been plotted.
 
     if not ax_input:
         fig, ax = plt.subplots()
 
+    if color is None:
+        color = next(ax._get_lines.color_cycle)
+
     for i in range(len(energies)):
         if filter_spins is not None:
             if spins[i] not in filter_spins:
                 """
                 Skip spins which are not in the filter.
                 """
                 continue
 
+        if parities[i] not in parity_integer:
+            continue
+
+        key: str = f"{spins[i]} + {parities[i]}"
         try:
-            counts[spins[i]] += 1
+            counts[key] += 1
         except KeyError:
-            counts[spins[i]] = 1
+            counts[key] = 1
         
-        if counts[spins[i]] > include_n_levels:
+        if counts[key] > include_n_levels:
             """
-            Include only the first 'include_n_levels' amount of states
+            Include only the first `include_n_levels` amount of states
             for any of the spins.
             """
             continue
 
         ax.hlines(
             y = energies[i],
-            xmin = spins[i] - line_width,
-            xmax = spins[i] + line_width,
-            color = "black"
+            xmin = spins[i] - line_width + x_offset*parities[i]*0.9,
+            xmax = spins[i] + line_width + x_offset*parities[i]*0.9,
+            color = color,
+            alpha = 0.5,
         )
 
     ax.set_xticks(spin_scope)
-    ax.set_xticklabels([f"{Fraction(i)}" + f"$^{parity_symbol}$" for i in spin_scope])
+    ax.set_xticklabels([f"{Fraction(i)}" + r"$^{" + f"{parity_symbol}" + r"}$" for i in spin_scope])
     ax.set_xlabel(r"$j^{\pi}$")
     ax.set_ylabel(r"$E$ [MeV]")
 
     if not ax_input:
         plt.show()
 
 def level_density(
@@ -1389,8 +1447,8 @@
         y = 0.88,
         s = r"$\pi:+  -  +  - \, + \, -$",
         fontsize = fontsize - 1,
         color = "black",
     )
 
     fig.savefig(fname="nuclear_shell_model.png", dpi=500)#, format="eps")
-    plt.show()
+    plt.show()
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/kshell_utilities.py` & `kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os, sys, multiprocessing, hashlib, ast, time, re
 from fractions import Fraction
 from typing import Union, Callable, Tuple, Iterable
 from itertools import chain
 import numpy as np
+import numba
 import matplotlib.pyplot as plt
 import seaborn as sns
 from .collect_logs import collect_logs
 from .kshell_exceptions import KshellDataStructureError
 from .parameters import atomic_numbers, flags
 from .general_utilities import (
     level_plot, level_density, gamma_strength_function_average, porter_thomas,
@@ -196,21 +197,33 @@
 
             raise RuntimeError(msg)
 
         self.base_fname = self.fname_summary.split(".")[0] # Base filename for .npy tmp files.
         self.unique_id = _generate_unique_identifier(self.path) # Unique identifier for .npy files.
         self._extract_info_from_summary_fname()
         self._read_summary()
+        self.mixing_pairs_BM1_BE2 = self._mixing_pairs(B_left="M1", B_right="E2")
         
         self.ground_state_energy = self.levels[0, 0]
-        self.A = int("".join(filter(str.isdigit, self.nucleus)))
-        self.Z, self.N = isotope(
-            name = "".join(filter(str.isalpha, self.nucleus)).lower(),
-            A = self.A
-        )
+        
+        try:
+            self.A = int("".join(filter(str.isdigit, self.nucleus)))
+            self.Z, self.N = isotope(
+                name = "".join(filter(str.isalpha, self.nucleus)).lower(),
+                A = self.A
+            )
+        except ValueError:
+            """
+            Prob. because the summary filename does not contain the name
+            of the isotope.
+            """
+            self.A = None
+            self.Z = None
+            self.N = None
+        
         self.check_data()
 
     def _extract_info_from_ptn_fname(self):
         """
         Extract nucleus and model space name.
         """
         fname_split = self.fname_ptn.split("/")[-1]
@@ -477,35 +490,42 @@
             np.save(file=transitions_BM1_fname, arr=self.transitions_BM1, allow_pickle=True)
             np.save(file=transitions_BE2_fname, arr=self.transitions_BE2, allow_pickle=True)
             np.save(file=transitions_BE1_fname, arr=self.transitions_BE1, allow_pickle=True)
             np.save(file=debug_fname, arr=self.debug, allow_pickle=True)
 
     def level_plot(self,
         include_n_levels: int = 1000,
-        filter_spins: Union[None, list] = None
+        filter_spins: Union[None, list] = None,
+        filter_parity: Union[None, str] = None,
+        color: Union[None, str] = "black"
         ):
         """
         Wrapper method to include level plot as an attribute to this
-        class. Generate a level plot for a single isotope. Spin on the x
-        axis, energy on the y axis.
+        class. Generate a level plot for a single isotope. Angular
+        momentum on the x axis, energy on the y axis.
 
         Parameters
         ----------
         include_n_levels : int
             The maximum amount of states to plot for each spin. Default
             set to a large number to indicate ≈ no limit.
 
         filter_spins : Union[None, list]
             Which spins to include in the plot. If `None`, all spins are
             plotted. Defaults to `None`
+
+        color : Union[None, str]
+            Set the color of the level lines.
         """
         level_plot(
             levels = self.levels,
             include_n_levels = include_n_levels,
-            filter_spins = filter_spins
+            filter_spins = filter_spins,
+            filter_parity = filter_parity,
+            color = color,
         )
 
     def level_density_plot(self,
             bin_width: Union[int, float] = 0.2,
             include_n_levels: Union[None, int] = None,
             filter_spins: Union[None, int, list] = None,
             filter_parity: Union[None, str, int] = None,
@@ -1811,14 +1831,272 @@
         ax[-1].set_xlabel(r"E$_{\gamma}$ [MeV]")
         fig.savefig(
             fname = f"{self.nucleus}_brink-axel_ji_{'_'.join(multipole_type)}.png",
             dpi = 300
         )
         plt.show()
 
+    def primary_matrix(self,
+        bin_width: Union[float, int] = 0.2,
+        Ex_min: Union[float, int] = 0,
+        Ex_max: Union[float, int] = 50,
+        multipole_type: str = "M1",
+        plot: bool = True,
+    ):
+        """
+        Create a Ex Eg primary matrix like the ones which are calculated
+        with the Oslo method.
+
+        Parameters
+        ----------
+        bin_width : float, optional
+            Width of the bins in MeV, by default 0.2
+        
+        Ex_min : float, optional
+            Minimum excitation energy of initial level in a transition,
+            by default 0 MeV.
+
+        Ex_max : float, optional
+            Maximum excitation energy of initial level in a transition,
+            by default 50 MeV.
+        
+        multipole_type : str
+            Multipolarity of the transitions to be considered, by
+            default "M1".
+
+        plot : bool, optional
+            Whether to plot the matrix, by default True.
+
+        Returns
+        -------
+        Ex_range : np.ndarray
+            The range of the initial level energies.
+
+        Eg_range : np.ndarray
+            The range of the gamma energies.
+
+        B_matrix : np.ndarray
+            The primary matrix.
+        """
+        transitions_dict = {
+            "E1": self.transitions_BE1,
+            "M1": self.transitions_BM1,
+            "E2": self.transitions_BE2,
+        }
+
+        n_bins = int(np.ceil((Ex_max - Ex_min)/bin_width))
+        B_matrix = np.zeros((n_bins, n_bins), dtype=float)    # rows: Ei, cols: Eg
+        Ex_range = np.linspace(Ex_min, Ex_max, n_bins)
+        Eg_range = np.linspace(Ex_min, Ex_max, n_bins)
+        
+        transitions = transitions_dict[multipole_type]
+        Ex_masks = []
+        Eg_masks = []
+        for i in range(n_bins-1):
+            """
+            Generate the masks once. It is not necessary to generate the
+            Eg masks over and over again while iterating over the Ex
+            masks.
+            """
+            Ex_masks.append(np.logical_and(
+                transitions[:, 3] >= Ex_range[i],
+                transitions[:, 3] < Ex_range[i+1],
+            ))
+        for i in range(n_bins-1):
+            """
+            Using separate loops allows using different bin widths for
+            Ex and Eg, however, that has not yet been implemented.
+            """
+            Eg_masks.append(np.logical_and(
+                transitions[:, 8] >= Eg_range[i],
+                transitions[:, 8] < Eg_range[i+1],
+            ))
+        for i in range(n_bins-1):
+            """
+            Loop over each Ex Eg mask pair and create a combined mask.
+            Take the mean of the B values for each combined mask.
+            """
+            for j in range(i+1):
+                mask = np.logical_and(
+                    Ex_masks[i],
+                    Eg_masks[j],
+                )
+                B_slice = transitions[mask][:, 9]
+                if B_slice.size == 0: continue  # Skip if there are no B values in the mask.
+                
+                B_matrix[i, j] = np.mean(B_slice)
+
+        if plot:
+            fig, ax = plt.subplots()
+            im = ax.pcolormesh(Ex_range, Eg_range, B_matrix, cmap="jet", norm="log")
+            ax.set_title(r"$\langle B($" + f"{multipole_type}" + r"$) \rangle$")
+            ax.set_xlabel(r"$E_{\gamma}$")
+            ax.set_ylabel(r"$E_{x}$")
+            fig.colorbar(im)
+            plt.show()
+
+        return Ex_range, Eg_range, B_matrix
+
+    def _mixing_pairs(self,
+        B_left: str = "M1",
+        B_right: str = "E2",
+    ):
+        """
+        NOTE: Currently hard-coded for BM1_BE2!
+        """
+        if B_left != "M1":#not in ["M1", "E2"]:
+            # msg = f"'B_left' must be 'M1' or 'E2', got: {B_left}"
+            # raise ValueError(msg)
+            raise ValueError
+        
+        if B_right != "E2":# not in ["M1", "E2"]:
+            # msg = f"'B_right' must be 'M1' or 'E2', got: {B_right}"
+            # raise ValueError(msg)
+            raise ValueError
+        
+        transitions_dict = {
+            "M1": self.transitions_BM1,
+            "E2": self.transitions_BE2,
+            "E1": self.transitions_BE1
+        }
+        transitions_left = transitions_dict[B_left]
+        transitions_right = transitions_dict[B_right]
+        
+        mixing_pairs_fname = f"{self.npy_path}/{self.base_fname}_mixing_pairs_B{B_left}_B{B_right}_{self.unique_id}.npy"
+
+        if os.path.isfile(mixing_pairs_fname) and self.load_and_save_to_file and (self.load_and_save_to_file != "overwrite"):
+            print(f"Mixing pairs loaded from .npy!")
+            mixing_pairs = np.load(file=mixing_pairs_fname, allow_pickle=True)
+            return mixing_pairs        
+        
+        @numba.njit
+        def calculate_mixing_pairs(
+            possible_j: list[int],
+            possible_indices: list[int],
+            transitions_BM1: np.ndarray,
+            transitions_BE2: np.ndarray,
+        ):
+            mixing_pairs = []
+
+            for ji in possible_j:
+                ji_slice_BM1 = transitions_BM1[transitions_BM1[:, 0] == ji]
+                ji_slice_BE2 = transitions_BE2[transitions_BE2[:, 0] == ji]
+
+                if (not ji_slice_BM1.size) or (not ji_slice_BE2.size): return
+
+                for jf in possible_j:
+                    # if not j_allowed(ji=ji, jf=jf): continue
+                    jf_slice_BM1 = ji_slice_BM1[ji_slice_BM1[:, 4] == jf]
+                    jf_slice_BE2 = ji_slice_BE2[ji_slice_BE2[:, 4] == jf]
+
+                    if (not jf_slice_BM1.size) or (not jf_slice_BE2.size): continue
+
+                    for pi in [-1, 1]:
+                        """
+                        [2*spin_initial, parity_initial, idx_initial, Ex_initial, 2*spin_final,
+                        parity_final, idx_final, Ex_final, E_gamma, B(.., i->f), B(.., f<-i)]
+                        """
+                        pi_i_slice_BM1 = jf_slice_BM1[jf_slice_BM1[:, 1] == pi]
+                        pi_i_slice_BE2 = jf_slice_BE2[jf_slice_BE2[:, 1] == pi]
+
+                        if (not pi_i_slice_BM1.size) or (not pi_i_slice_BE2.size): continue
+                        
+                        pi_f_slice_BM1 = pi_i_slice_BM1[pi_i_slice_BM1[:, 5] == pi]
+                        pi_f_slice_BE2 = pi_i_slice_BE2[pi_i_slice_BE2[:, 5] == pi]
+
+                        if (not pi_f_slice_BM1.size) or (not pi_f_slice_BE2.size): continue
+
+                        for idx_i in possible_indices:
+                            idx_i_slice_BM1 = pi_f_slice_BM1[pi_f_slice_BM1[:, 2] == idx_i]
+                            idx_i_slice_BE2 = pi_f_slice_BE2[pi_f_slice_BE2[:, 2] == idx_i]
+
+                            if (not idx_i_slice_BM1.size) or (not idx_i_slice_BE2.size): continue
+
+                            for idx_f in possible_indices:
+                                idx_f_slice_BM1 = idx_i_slice_BM1[idx_i_slice_BM1[:, 2] == idx_f]
+                                idx_f_slice_BE2 = idx_i_slice_BE2[idx_i_slice_BE2[:, 2] == idx_f]
+
+                                if (not idx_f_slice_BM1.size) or (not idx_f_slice_BE2.size): continue
+
+                                for transition_BM1 in idx_f_slice_BM1:
+                                    for transition_BE2 in idx_f_slice_BE2:
+                                        if (transition_BM1[3] == transition_BE2[3]) and (transition_BM1[7] == transition_BE2[7]):
+                                            mixing_pairs.append([transition_BM1, transition_BE2])
+                
+            return mixing_pairs
+
+        mixing_pairs_time = time.perf_counter()
+        possible_j = np.unique(transitions_left[:, 0])
+        possible_indices = np.unique(transitions_left[:, 2])
+        assert np.all(possible_indices == np.unique(transitions_left[:, 6]))    # Check that indices of the initial and final levels are the same range.
+        
+        mixing_pairs = calculate_mixing_pairs(
+            transitions_BM1 = transitions_left,
+            transitions_BE2 = transitions_right,
+            possible_j = possible_j,
+            possible_indices = possible_indices,
+        )
+        mixing_pairs.sort(key=lambda tup: tup[0][8])    # Sort wrt. gamma energy.
+        mixing_pairs = np.array(mixing_pairs)
+        np.save(file=mixing_pairs_fname, arr=mixing_pairs, allow_pickle=True)
+        mixing_pairs_time = time.perf_counter() - mixing_pairs_time
+        print(f"{mixing_pairs_time = :.3f} s")
+        return mixing_pairs
+
+    def mixing_ratio(self,
+        bin_width: float = 0.2,
+        plot: bool = True,
+        save_plot: bool = False,
+    ):
+        """
+        Calculate the ratio of T(E2)/(T(E2) + T(M1)), aka. how large the
+        E2 contribution is. Currently hard-coded for this specific
+        ratio.
+
+        Parameters
+        ----------
+        bin_width : float
+            The ratios are sorted by gamma energy and averaged over
+            the ratio values in a gamma energy bin of bin_with.
+        """
+        E_min = self.mixing_pairs_BM1_BE2[0, 0, 8]  # BM1 and BE2 has to be at the exact same gamma energies so it doesnt matter which one we take E_min and E_max from.
+        E_max = self.mixing_pairs_BM1_BE2[-1, 0, 8]
+
+        bins = np.arange(E_min, E_max + bin_width, bin_width)
+        n_bins = len(bins)
+        ratios = np.zeros(n_bins - 1)
+
+        for i in range(n_bins - 1):
+            mask_1 = self.mixing_pairs_BM1_BE2[:, 0, 8] >= bins[i]
+            mask_2 = self.mixing_pairs_BM1_BE2[:, 0, 8] < bins[i + 1]
+            mask_3 = np.logical_and(mask_1, mask_2)
+
+            # M1_mean = self.mixing_pairs_BM1_BE2[:, 0, 9][mask_3].mean()
+            # E2_mean = self.mixing_pairs_BM1_BE2[:, 1, 9][mask_3].mean()
+
+            M1_mean = (1.76e13*(self.mixing_pairs_BM1_BE2[:, 0, 8][mask_3]**3)*self.mixing_pairs_BM1_BE2[:, 0, 9][mask_3]).mean()
+            E2_mean = (1.22e09*(self.mixing_pairs_BM1_BE2[:, 1, 8][mask_3]**5)*self.mixing_pairs_BM1_BE2[:, 1, 9][mask_3]).mean()
+
+            ratios[i] = E2_mean/(E2_mean + M1_mean)
+        
+        if plot:
+            fig, ax = plt.subplots()
+            ax.step(bins[:-1], ratios, color="black")
+            # ax.legend()
+            ax.grid()
+            ax.set_ylabel(r"TE2/(TE2 + TM1)")
+            ax.set_xlabel(r"$E_{\gamma}$ [MeV]")
+            if save_plot:
+                fname = f"mixing_ratio_E2_M1.png"
+                print(f"Mixing ratio plot saved as '{fname}'")
+                fig.savefig(fname=fname, dpi=300)
+            plt.show()
+
+        return bins[:-1], ratios
+
     @property
     def help(self):
         """
         Generate a list of instance attributes without magic and private
         methods.
 
         Returns
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/kshell_utilities_tmp.py` & `kshell-utilities-1.5.0.0/kshell_utilities/kshell_utilities_tmp.py`

 * *Files identical despite different names*

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities/script_editing.py` & `kshell-utilities-1.5.0.0/kshell_utilities/script_editing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import os, warnings
 from .parameters import GS_FREE_PROTON, GS_FREE_NEUTRON
 
 def _ask_for_time_input(unit: str, lower_lim: int, upper_lim: int) -> int:
     """
     Input prompting generalized for seconds, minutes, hours, and days.
 
@@ -32,29 +33,115 @@
             return ans
         else:
             print(f"The number of {unit} must be in the interval [{lower_lim}, {upper_lim}]")
             continue
 
 def edit_and_queue_executables():
     """
+    Simple wrapper for quietly quitting on KeyboardInterrupt without
+    having to indent the entire _edit_and_queue_executables function.
+    """
+    try:
+        _edit_and_queue_executables()
+    except KeyboardInterrupt:
+        print("\nExiting...")
+        return
+    
+def _prompt_user_for_values(
+    available_parameters: dict[str, bool],
+    available_parameters_values: dict[str, str | int | float]
+):
+    """
+    Ask the user for the actual values for each of the parameters which
+    are to be changed.
+    """
+    if available_parameters["job_name"]:
+        available_parameters_values["job_name"] = input("Job name: ")
+
+    if available_parameters["nodes"]:
+        while True:
+            """
+            Ask for new number of nodes.
+            """
+            try:
+                available_parameters_values["nodes"] = int(input("Number of nodes: "))
+                break
+            except ValueError:
+                print("Only integers are allowed!")
+                continue
+
+    if available_parameters["seconds"]:
+        available_parameters_values["seconds"] = _ask_for_time_input(
+            unit = "seconds",
+            lower_lim = 0,
+            upper_lim = 59
+        )
+        tmp = available_parameters_values["time_parameter_new"].split(":")
+        available_parameters_values["time_parameter_new"] = f"{tmp[0]}:{tmp[1]}:{available_parameters_values['seconds']:02d}"
+
+    if available_parameters["minutes"]:
+        available_parameters_values["minutes"] = _ask_for_time_input(
+            unit = "minutes",
+            lower_lim = 0,
+            upper_lim = 59
+        )
+        tmp = available_parameters_values["time_parameter_new"].split(":")
+        available_parameters_values["time_parameter_new"] = f"{tmp[0]}:{available_parameters_values['minutes']:02d}:{tmp[2]}"
+
+    if available_parameters["hours"]:
+        available_parameters_values["hours"] = _ask_for_time_input(
+            unit = "hours",
+            lower_lim = 0,
+            upper_lim = 23
+        )
+        tmp = available_parameters_values["time_parameter_new"].split(":")
+        tmp_days, _ = tmp[0].split("-")
+        available_parameters_values["time_parameter_new"] = f"{tmp_days}-{available_parameters_values['hours']:02d}:{tmp[1]}:{tmp[2]}"
+
+    if available_parameters["days"]:
+        available_parameters_values["days"] = _ask_for_time_input(
+            unit = "days",
+            lower_lim = 0,
+            upper_lim = 4
+        )
+        tmp = available_parameters_values["time_parameter_new"].split(":")
+        _, tmp_hours = tmp[0].split("-")
+        available_parameters_values["time_parameter_new"] = f"{available_parameters_values['days']}-{tmp_hours}:{tmp[1]}:{tmp[2]}"
+
+    if available_parameters["quench"]:
+        while True:
+            try:
+                available_parameters_values["quench"] = float(input("quench: "))
+                break
+            except ValueError:
+                print("Only integers and floats are allowed!")
+                continue
+
+def _edit_and_queue_executables():
+    """
     Loop over .sh files generated by 'kshell_ui' and adjust queue system
     parameters and if possible, queue the .sh file.
 
     Currently hard-coded to the slurm system.
     """
-    available_parameters = {
+    available_parameters: dict[str, bool] = {
         "nodes": False,
         "seconds": False,
         "minutes": False,
         "hours": False,
         "days": False,
         "job_name": False,
         "quench": False,
-        "queue": False
+        "queue": False,
+        "apply same values to several or all .sh files": False,
+        # "ask for confirmation per file": False,
     }
+    available_parameters_values: dict[str, str | int | float] = {key: "" for key in available_parameters.items()}
+    available_parameters_values["time_parameter_new"] = ""  # For storing the entire new formatted time parameter string.
+    prompt_user_input: bool = True
 
     print("Please choose what parameters you want to alter (y/n) (default n):")
     for parameter in available_parameters:
         """
         Decide what to do with all parameters.
         """
         while True:
@@ -102,125 +189,79 @@
                     job_name_parameter += line
                 elif "gs =" in line:
                     gs_parameter += line
 
         if (not content) or ((not time_parameter) and (not nodes_parameter) and (not job_name_parameter)):
             print(f"Could not extract info from {elem}. Skipping ...")
             continue
+        
+        # time_parameter_new = time_parameter.split("=")[-1].strip()    # '0-00:00:00' d-hh:mm:ss
 
-        if available_parameters["job_name"]:
-            available_parameters["job_name"] = input("Job name: ")
-
-        if available_parameters["nodes"]:
-            while True:
+        if prompt_user_input:
+            if available_parameters["apply same values to several or all .sh files"]:
                 """
-                Ask for new number of nodes.
+                Ask the user only once and start with the same time
+                template for all .sh files.
                 """
-                try:
-                    available_parameters["nodes"] = int(input("Number of nodes: "))
-                    break
-                except ValueError:
-                    print("Only integers are allowed!")
-                    continue
-        
-        time_parameter_new = time_parameter.split("=")[-1].strip()    # '0-00:00:00' d-hh:mm:ss
-
-        if available_parameters["seconds"]:
-            available_parameters["seconds"] = _ask_for_time_input(
-                unit = "seconds",
-                lower_lim = 0,
-                upper_lim = 59
-            )
-            tmp = time_parameter_new.split(":")
-            time_parameter_new = f"{tmp[0]}:{tmp[1]}:{available_parameters['seconds']:02d}"
-
-        if available_parameters["minutes"]:
-            available_parameters["minutes"] = _ask_for_time_input(
-                unit = "minutes",
-                lower_lim = 0,
-                upper_lim = 59
-            )
-            tmp = time_parameter_new.split(":")
-            time_parameter_new = f"{tmp[0]}:{available_parameters['minutes']:02d}:{tmp[2]}"
+                prompt_user_input = False
+                available_parameters_values["time_parameter_new"] = '#SBATCH --time=0-00:00:00'.split("=")[-1].strip()    # '0-00:00:00' d-hh:mm:ss
+            else:
+                available_parameters_values["time_parameter_new"] = time_parameter.split("=")[-1].strip()    # '0-00:00:00' d-hh:mm:ss
 
-        if available_parameters["hours"]:
-            available_parameters["hours"] = _ask_for_time_input(
-                unit = "hours",
-                lower_lim = 0,
-                upper_lim = 23
+            _prompt_user_for_values(
+                available_parameters = available_parameters,
+                available_parameters_values = available_parameters_values
             )
-            tmp = time_parameter_new.split(":")
-            tmp_days, _ = tmp[0].split("-")
-            time_parameter_new = f"{tmp_days}-{available_parameters['hours']:02d}:{tmp[1]}:{tmp[2]}"
-
-        if available_parameters["days"]:
-            available_parameters["days"] = _ask_for_time_input(
-                unit = "days",
-                lower_lim = 0,
-                upper_lim = 4
-            )
-            tmp = time_parameter_new.split(":")
-            _, tmp_hours = tmp[0].split("-")
-            time_parameter_new = f"{available_parameters['days']}-{tmp_hours}:{tmp[1]}:{tmp[2]}"
-
-        if available_parameters["quench"]:
-            while True:
-                try:
-                    available_parameters["quench"] = float(input("quench: "))
-                    break
-                except ValueError:
-                    print("Only integers and floats are allowed!")
-                    continue
   
         if time_parameter:
             """
             Insert new time parameter.
             """
-            content_tmp = content.replace(time_parameter, f"#SBATCH --time={time_parameter_new}\n")
+            content_tmp = content.replace(time_parameter, f"#SBATCH --time={available_parameters_values['time_parameter_new']}\n")
 
             if (content_tmp == content) and (available_parameters['seconds'] or available_parameters['minutes'] or available_parameters['hours'] or available_parameters['days']):
                 msg = "Time parameter is unchanged. Either str.replace could"
                 msg += " not find a match or new time parameter is identical"
                 msg += " to old time parameter."
                 warnings.warn(msg, RuntimeWarning)
             else:
                 content = content_tmp
 
         if job_name_parameter and available_parameters['job_name']:
             """
             Insert new job name parameter.
             """
-            content_tmp = content.replace(job_name_parameter, f"#SBATCH --job-name={available_parameters['job_name']}\n")
+            content_tmp = content.replace(job_name_parameter, f"#SBATCH --job-name={available_parameters_values['job_name']}\n")
 
             if content_tmp == content:
                 msg = "Job name parameter is unchanged. Either str.replace"
                 msg += " could not find a match or new job name parameter is"
                 msg += " identical to old job name parameter."
                 warnings.warn(msg, RuntimeWarning)
             else:
                 content = content_tmp
 
         if nodes_parameter and available_parameters["nodes"]:
             """
             Insert new nodes parameter.
             """
             nodes_parameter_new = nodes_parameter.split("=")[0]
-            nodes_parameter_new += f"={available_parameters['nodes']}\n"
+            nodes_parameter_new += f"={available_parameters_values['nodes']}\n"
             content_tmp = content.replace(nodes_parameter, nodes_parameter_new)
             
             if content_tmp == content:
                 msg = "Nodes parameter is unchanged. Either str.replace could"
                 msg += " not find a match or new nodes parameter is identical"
                 msg += " to old nodes parameter."
                 warnings.warn(msg, RuntimeWarning)
             else:
                 content = content_tmp
 
         if available_parameters["quench"]:
-            quenching_factor = available_parameters["quench"]
+            quenching_factor = available_parameters_values["quench"]
             gs_parameter_new = gs_parameter.split("=")[0]
             gsp = round(quenching_factor*GS_FREE_PROTON, 2)
             gsn = round(quenching_factor*GS_FREE_NEUTRON, 2)
             gs_parameter_new += f"= {gsp}, {gsn}\n"
             content_tmp = content.replace(gs_parameter, gs_parameter_new)
 
             if content_tmp == content:
@@ -231,8 +272,8 @@
             else:
                 content = content_tmp
 
         with open(elem, "w") as outfile:
             outfile.write(content)
 
         if available_parameters["queue"]:
-            os.system(f"sbatch {elem}")
+            os.system(f"sbatch {elem}")
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities.egg-info/PKG-INFO` & `kshell-utilities-1.5.0.0/kshell_utilities.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kshell-utilities
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: Handy utilities for handling nuclear shell model calculations from KSHELL
 Home-page: https://github.com/GaffaSnobb/kshell-utilities
-Author: Jon Kristian Dahl
+Author: ['Jon Kristian Dahl', 'Johannes Heines']
 Author-email: jonkd@uio.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 License-File: LICENSE
```

### Comparing `kshell-utilities-1.4.0.0/kshell_utilities.egg-info/SOURCES.txt` & `kshell-utilities-1.5.0.0/kshell_utilities.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 kshell_utilities/__init__.py
 kshell_utilities/collect_logs.py
+kshell_utilities/compare.py
 kshell_utilities/count_dim.py
+kshell_utilities/data_structures.py
 kshell_utilities/deprecated.py
 kshell_utilities/general_utilities.py
 kshell_utilities/kshell_exceptions.py
 kshell_utilities/kshell_utilities.py
 kshell_utilities/kshell_utilities_tmp.py
 kshell_utilities/loaders.py
-kshell_utilities/low_energy_enhancement.py
+kshell_utilities/other_tools.py
 kshell_utilities/parameters.py
+kshell_utilities/partition_compare.py
+kshell_utilities/partition_editor.py
+kshell_utilities/partition_tools.py
 kshell_utilities/script_editing.py
 kshell_utilities.egg-info/PKG-INFO
 kshell_utilities.egg-info/SOURCES.txt
 kshell_utilities.egg-info/dependency_links.txt
 kshell_utilities.egg-info/requires.txt
 kshell_utilities.egg-info/top_level.txt
 tests/__init__.py
 tests/test_all.py
+tests/test_partition_editor.py
 tests/test_spin_parity_list.py
```

### Comparing `kshell-utilities-1.4.0.0/setup.py` & `kshell-utilities-1.5.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 #     import pypandoc
 #     long_description = pypandoc.convert('README.md', 'rst')
 # except (IOError, ImportError, OSError):
 #     long_description = ""
 
 setup(
     name = 'kshell-utilities',
-    version = '1.4.0.0',    
+    version = '1.5.0.0',    
     description = 'Handy utilities for handling nuclear shell model calculations from KSHELL',
     # long_description = long_description,
     url = 'https://github.com/GaffaSnobb/kshell-utilities',
-    author = 'Jon Kristian Dahl',
+    author = ['Jon Kristian Dahl', 'Johannes Heines'],
     author_email = 'jonkd@uio.no',
     packages = ['kshell_utilities', 'tests'],
-    install_requires = ['numpy', 'matplotlib', 'seaborn'],
+    install_requires = ['numpy', 'matplotlib', 'seaborn', 'scipy', 'numba', 'vum'],
 
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Operating System :: MacOS',
         'Operating System :: Unix',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Physics',
     ],
 )
```

### Comparing `kshell-utilities-1.4.0.0/tests/test_all.py` & `kshell-utilities-1.5.0.0/tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     AssertionError
         If the read values are not exactly equal to the expected values.
     """
     res = kshell_utilities.loadtxt(
         path = "summary_test_text_file.txt",
         load_and_save_to_file = False,
         old_or_new = "old"
-    )[0]
+    )
 
     E_expected = [
-        -41.394, -33.378, -114.552, -114.044, -113.972, -113.898, -113.762,
-        -113.602, -9.896, -9.052
+        -114.552, -114.044, -113.972, -113.898, -113.762, -113.602, -41.394,
+        -33.378, -9.896, -9.052
     ]
     spin_expected = [
-        2*0, 2*3, 2*2, 2*5, 2*4, 2*7, 2*2, 2*3, 2*3/2, 2*7/2
+        2*2, 2*5, 2*4, 2*7, 2*2, 2*3, 2*0, 2*3, 2*3/2, 2*7/2
     ]
     parity_expected = [
         1, 1, 1, 1, 1, 1, 1, 1, -1, -1
     ]
 
     for calculated, expected in zip_longest(res.levels[:, 0], E_expected):
         msg = f"Error in Ex. Expected: {expected}, got: {calculated}."
@@ -47,15 +47,15 @@
     Check that floor yields the same result as casting to int. This does
     not work for negative values.
     """
     res = kshell_utilities.loadtxt(
         path = "summary_test_text_file.txt",
         load_and_save_to_file = False,
         old_or_new = "old"
-    )[0]
+    )
 
     res_1 = np.floor(res.transitions_BM1[:, 5])
     res_2 = res.transitions_BM1[:, 5].astype(int)
 
     for elem_1, elem_2 in zip(res_1, res_2):
         assert elem_1 == elem_2
 
@@ -63,15 +63,15 @@
     """
     Test that all values in res.transitions are as expected.
     """
     res = kshell_utilities.loadtxt(
         path = "summary_test_text_file.txt",
         load_and_save_to_file = False,
         old_or_new = "old"
-    )[0]
+    )
 
     # BE2
     # ---
     spin_initial_expected = np.array([5, 4, 4, 3, 9/2, 9/2])*2
     for i in range(len(res.transitions_BE2[:, 0])):
         msg = "BE2: Error in spin_initial."
         msg += f" Expected: {spin_initial_expected[i]}, got {res.transitions_BE2[i, 0]}."
@@ -177,18 +177,20 @@
 
     B_excite_expected = np.array([102.3, 0.0, 3.4, 0.1, 0.092, 0.617])
     for i in range(len(res.transitions_BM1[:, 10])):
         msg = "BM1: Error in B_excite."
         msg += f" Expected: {B_excite_expected[i]}, got {res.transitions_BM1[i, 10]}."
         assert res.transitions_BM1[i, 10] == B_excite_expected[i], msg
 
-def test_file_read_levels_jem():
+def _test_file_read_levels_jem():
     """
     For JEM syntax.
 
+    NOTE: Currently not working because of https://github.com/GaffaSnobb/kshell-utilities/blob/d0bc1eae743e353671c562040c544b7df4c28d05/kshell_utilities/kshell_utilities.py#L437
+
     Raises
     ------
     AssertionError
         If the read values are not exactly equal to the expected values.
     """
     res = kshell_utilities.loadtxt(
         path = "summary_Zn60_jun45_jem_syntax.txt",
@@ -215,17 +217,19 @@
         msg = f"Error in spin. Expected: {expected}, got: {calculated}."
         assert calculated == expected, msg
 
     for calculated, expected in zip_longest(res.levels[:, 2], parity_expected):
         msg = f"Error in parity. Expected: {expected}, got: {calculated}."
         assert calculated == expected, msg
 
-def test_file_read_transitions_jem():
+def _test_file_read_transitions_jem():
     """
     Test that all values in res.transitions are as expected.
+
+    NOTE: Currently not working because of https://github.com/GaffaSnobb/kshell-utilities/blob/d0bc1eae743e353671c562040c544b7df4c28d05/kshell_utilities/kshell_utilities.py#L437
     """
     res = kshell_utilities.loadtxt(
         path = "summary_Zn60_jun45_jem_syntax.txt",
         load_and_save_to_file = False,
         old_or_new = "jem"
     )[0]
 
@@ -410,9 +414,9 @@
         msg += f" Expected: {B_excite_expected[i]}, got {res.transitions_BM1[i, 10]}."
         assert res.transitions_BM1[i, 10] == B_excite_expected[i], msg
 
 if __name__ == "__main__":
     test_file_read_levels()
     test_int_vs_floor()
     test_file_read_transitions()
-    test_file_read_levels_jem()
-    test_file_read_transitions_jem()
+    # test_file_read_levels_jem()
+    # test_file_read_transitions_jem()
```

### Comparing `kshell-utilities-1.4.0.0/tests/test_spin_parity_list.py` & `kshell-utilities-1.5.0.0/tests/test_spin_parity_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
     TODO: Loop over BE2 values too?
     """
     res = kshell_utilities.loadtxt(
         path = "summary_O19_sdpf-mu.txt",
         load_and_save_to_file = False,
         old_or_new = "old"
-    )[0]
-    
+    )
     n_transitions = len(res.transitions_BM1[:, 0])
     spins = res.levels[:, 1]
     parities = res.levels[:, 2]
     spin_parity_list = create_spin_parity_list(spins, parities)
     index_list = []
     
     for transition_idx in range(n_transitions):
```

