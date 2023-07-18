# Comparing `tmp/siman-1.3.7.tar.gz` & `tmp/siman-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.7.tar", last modified: Sun Jul 16 18:08:18 2023, max compression
+gzip compressed data, was "dist/siman-1.3.8.tar", last modified: Tue Jul 18 16:00:07 2023, max compression
```

## Comparing `siman-1.3.7.tar` & `siman-1.3.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.7/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.7/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-16 18:08:18.454508 siman-1.3.7/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.7/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-16 18:08:18.454508 siman-1.3.7/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-16 18:08:14.000000 siman-1.3.7/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.7/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.7/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.7/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.7/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.7/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.7/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.7/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.7/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.7/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.7/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.453508 siman-1.3.7/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.7/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.453508 siman-1.3.7/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.7/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.7/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-14 10:44:19.000000 siman-1.3.7/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.7/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.7/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.7/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.7/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.7/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.7/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16289 2023-07-16 18:04:57.000000 siman-1.3.7/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.7/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.7/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    87557 2023-07-16 18:04:57.000000 siman-1.3.7/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.7/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.7/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.7/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.7/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.7/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.7/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.7/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50657 2023-07-16 18:04:57.000000 siman-1.3.7/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.7/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.7/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.7/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.7/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.7/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.7/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.7/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.7/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.7/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.7/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.8/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.8/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-18 16:00:07.185332 siman-1.3.8/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.8/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-18 16:00:07.185332 siman-1.3.8/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-18 16:00:05.000000 siman-1.3.8/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.8/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.8/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.8/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.8/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.8/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.8/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.8/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.8/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.8/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.8/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.184332 siman-1.3.8/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.8/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.8/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.184332 siman-1.3.8/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.8/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.8/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.8/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.8/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.8/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20407 2023-07-18 15:59:51.000000 siman-1.3.8/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.8/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.8/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.8/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.8/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.8/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.8/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16435 2023-07-18 15:59:51.000000 siman-1.3.8/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.8/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.8/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    87557 2023-07-16 18:04:57.000000 siman-1.3.8/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.8/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.185332 siman-1.3.8/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.8/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.8/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.8/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.8/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.8/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.8/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.8/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50595 2023-07-18 15:59:51.000000 siman-1.3.8/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.8/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.8/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.8/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.8/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.8/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.8/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.8/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.8/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.8/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.8/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.8/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.8/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-18 16:00:07.183332 siman-1.3.8/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-18 16:00:07.000000 siman-1.3.8/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.7/LICENSE` & `siman-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/PKG-INFO` & `siman-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.7
+Version: 1.3.8
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.7/setup.py` & `siman-1.3.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.7",
+    version="1.3.8",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.7/siman/3d_plot.py` & `siman-1.3.8/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/SSHTools.py` & `siman-1.3.8/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/analysis.py` & `siman-1.3.8/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/analysis_functions.py` & `siman-1.3.8/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/analyze/segregation.py` & `siman-1.3.8/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/approximation.py` & `siman-1.3.8/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/bands.py` & `siman-1.3.8/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calc_manage.py` & `siman-1.3.8/siman/calc_manage.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calcul.py` & `siman-1.3.8/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calculators/aims.py` & `siman-1.3.8/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calculators/gaussian.py` & `siman-1.3.8/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calculators/qe.py` & `siman-1.3.8/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calculators/vasp.py` & `siman-1.3.8/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/calculators/vasp_old.py` & `siman-1.3.8/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/chg/chg_func.py` & `siman-1.3.8/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.8/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/classes.py` & `siman-1.3.8/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/calculation.py` & `siman-1.3.8/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/calculation_old.py` & `siman-1.3.8/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/cluster_batch_script.py` & `siman-1.3.8/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/cluster_run_script.py` & `siman-1.3.8/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/molecule.py` & `siman-1.3.8/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/core/structure.py` & `siman-1.3.8/siman/core/structure.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/database.py` & `siman-1.3.8/siman/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         conv   - dict, convergence sequences
         varset - dict, parameter sets of the project
         size_on_start, int - not used now
     """
 
     # databasefile = 'calc.s' #was used with python2
     # databasefile = 'calc.gdbm'
-    databasefile3 = 'calc.gdbm3'
+    # databasefile3 = 'calc.gdbm3'
+    databasefile3 = header.PATH2SHELVE_DBSUP
     # if header.RAMDISK:
     #     databasefile3 = header.RAMDISK+databasefile3
 
     # sys.exit()
 
 
     # if scratch == True: databasefile =   '/scratch/aksenov/calc.s'
@@ -113,32 +114,33 @@
     RETURN:
         None    
 
     """
     #size_on_finish = sys.getsizeof(dbase)
     #if size_on_finish != size_on_start:
     # runBash("cp calc.s calc_copy.s") #create copy before writing
-    databasefile3 = 'calc.gdbm3'
-
+    # databasefile3 = 'calc.gdbm3'
+    databasefile3 = header.PATH2SHELVE_DBSUP
+    databasefile3_copy = databasefile3+'_copy'
     # if header.RAMDISK:
     #     databasefile3 = header.RAMDISK+databasefile3
     size = os.path.getsize
 
 
 
 
-    if os.path.isfile(databasefile3) and os.path.isfile('calc_copy.gdbm3'):
-        if size(databasefile3) < size('calc_copy.gdbm3') - 200000:
+    if os.path.isfile(databasefile3) and os.path.isfile(databasefile3_copy):
+        if size(databasefile3) < size(databasefile3_copy) - 200000:
 
-            print(size(databasefile3), size('calc_copy.gdbm3'))
+            print(size(databasefile3), size(databasefile3_copy))
             printlog('Error! actual database file is smaller than reserve copy, something is wrong! Check')
 
         else:
             ''
-            shutil.copyfile(databasefile3, 'calc_copy.gdbm3')
+            shutil.copyfile(databasefile3, databasefile3_copy)
     
 
 
     if 0:
         d = shelve.open('calc.s', protocol=1) #Write database of calculations
         d[calc_key]       = calc
         d[conv_key]       = conv
@@ -174,38 +176,38 @@
         d.close()   
 
         if header.reorganize: #please run me from time to time to reduce the size of the database file, calc
             with dbm.open(databasefile3, 'w') as d:
                 d.reorganize()
 
 
-        printlog('Opening ', header.calc_database, 'for writing')
+        printlog('Opening ', header.PATH2SHELVE_DB, 'for writing')
 
-        with shelve.Shelf(dbm.open(header.calc_database, 'c'), protocol = 3) as d:
+        with shelve.Shelf(dbm.open(header.PATH2SHELVE_DB, 'c'), protocol = 3) as d:
             for key in header.db:
                 printlog('saving key:', key, imp = '')
                 # print(key)
                 # print(key, header.calc[key].inh_id)
                 d[str(key)] = header.db[key]
         
         if header.reorganize: #please run me from time to time to reduce the size of the database file
-            with dbm.open(header.calc_database, 'w') as d:
+            with dbm.open(header.PATH2SHELVE_DB, 'w') as d:
                 d.reorganize()
 
 
     printlog("\nEnd of work at "+str(datetime.datetime.now())+'\n')
 
     try:
         header.log.close()
     except:
         pass
 
     #Update history file
-    with  open('history','w') as his:
-        #print history
+    with  open(header.PATH2HISTORYFILE,'w') as his:
+        printlog('Writing history file', header.PATH2HISTORYFILE)
         for i in header.history:
             #print i
             his.write(i+"\n")
     
     print("\nDatabase has been successfully updated\n")
     
     return
```

### Comparing `siman-1.3.7/siman/default_project_conf.py` & `siman-1.3.8/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/dev_functions.py` & `siman-1.3.8/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/dos_functions.py` & `siman-1.3.8/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/fit_hex.py` & `siman-1.3.8/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/functions.py` & `siman-1.3.8/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/geo.py` & `siman-1.3.8/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/header.py` & `siman-1.3.8/siman/header.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,17 @@
 reorganize = 0 # use this from time to time to optimize database file size
 verbose_log = 0 # in addition to normal log write verbose log in any case by openning the log_verbose each time
 cluster_address = ''
 override_cluster_address = 0 # 1 or 0, override read calculations to header.CLUSTERS[cluster]['address'], usefull when switching between proxy and back of the same cluster
 pymatgen_flag = None
 open_terminal = False #used in runBash
 siman_run = False #
-calc_database = 'only_calc.gdbm3' # name for calculation database, db dict
-
+PATH2SHELVE_DBSUP = 'calc.gdbm3' # supporting database
+PATH2SHELVE_DB = 'only_calc.gdbm3' # name for calculation database, db dict
+PATH2HISTORYFILE = 'history' 
 
 
 
 
 
 
 #1. Read default global settings for siman package
@@ -120,15 +121,15 @@
     spec.loader.exec_module(project_conf)
     # print(dir(project_conf))
     config_vars = ['CIF2CELL', 'DEFAULT_CLUSTER', 'EXCLUDE_NODES', 
     'NEW_BATCH', 'PATH2ARCHIVE', 'PATH2DATABASE', 'PATH2JMOL', 'PATH2NEBMAKE', 
     'PATH2PHONOPY', 'PATH2POTENTIALS', 'PATH2PROJECT', 'PBS_PROCS', 
     'RAMDISK', 'SIMAN_WEB', 'WALLTIME_LIMIT', 
     'geo_folder', 'path_to_images', 'path_to_paper', 
-    'path_to_wrapper', 'pmgkey', 'reorganize', 'CLUSTERS',]
+    'path_to_wrapper', 'pmgkey', 'reorganize', 'CLUSTERS', 'PATH2SHELVE_DBSUP', 'PATH2SHELVE_DB', 'PATH2HISTORYFILE']
 
     for var in config_vars:
         try: 
             value = getattr(project_conf, var)
             # print(type(value))
             setattr(header, var, value)
             # exec(var + " = " + str(value))
@@ -158,15 +159,15 @@
         # else:
 
         if dict.__contains__(self, key):
             # print('key', key, 'is  in self')
             val = dict.__getitem__(self, key)
         
         else:
-            with shelve.open(calc_database, protocol = 3) as d:
+            with shelve.open(PATH2SHELVE_DB, protocol = 3) as d:
                 try:
                     val = d[str(key)]
                     dict.__setitem__(self, key, val)
                     # print('reading ',str(key), 'from db')
                 except:
                     print('Problem with key',key,', return None')
                     val = None
@@ -182,24 +183,24 @@
 
     def __contains__(self, key):
 
         if dict.__contains__(self, key):
             return True
         
         else:
-            with shelve.open(calc_database, protocol = 3) as d:
+            with shelve.open(PATH2SHELVE_DB, protocol = 3) as d:
                 # print('checking if key',key, 'is in db:', str(key) in d)
                 # print(self)
                 return str(key) in d
 
     def items(self):
 
         keys = []
 
-        with shelve.open(calc_database, protocol = 3) as d:
+        with shelve.open(PATH2SHELVE_DB, protocol = 3) as d:
             for key in d:
                 key = key.replace("'", "").replace('(', '').replace(')', '') #remove unnessary symbols from string
                 l = key.split(',') # go back to tuple
 
                 if len(l) == 3 and l[2].strip().isdigit():
                     keyt = (l[0].strip(), l[1].strip(), int(l[2]))
                     keys.append(keyt)
```

### Comparing `siman-1.3.7/siman/impurity.py` & `siman-1.3.8/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/inout.py` & `siman-1.3.8/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/kpoints_functions.py` & `siman-1.3.8/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/mat_prop/mat_prop.py` & `siman-1.3.8/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/matproj_functions.py` & `siman-1.3.8/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/monte.py` & `siman-1.3.8/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/monte_functions.py` & `siman-1.3.8/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/neb.py` & `siman-1.3.8/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/pairs.py` & `siman-1.3.8/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/picture_functions.py` & `siman-1.3.8/siman/picture_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
 
         Aksyonov D.A.
 
 
     """
 
 
+
     if image_name == None:
         image_name  = filename
 
     # print(ver_lines)
     # sys.exit()
     # fontsize = 1
     # print(fontsize)
@@ -321,21 +322,21 @@
     if fontsize:
         # header.mpl.rcParams.update({'font.size': fontsize+4})
         # fontsize = 2
         SMALL_SIZE = fontsize
         MEDIUM_SIZE = fontsize
         BIGGER_SIZE = fontsize
 
-        header.mpl.rc('font', size=SMALL_SIZE)          # controls default text sizes
-        header.mpl.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
-        header.mpl.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
-        header.mpl.rc('xtick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
-        header.mpl.rc('ytick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
-        header.mpl.rc('legend', fontsize=SMALL_SIZE)    # legend fontsize
-        header.mpl.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
+        mpl.rc('font', size=SMALL_SIZE)          # controls default text sizes
+        mpl.rc('axes', titlesize=SMALL_SIZE)     # fontsize of the axes title
+        mpl.rc('axes', labelsize=MEDIUM_SIZE)    # fontsize of the x and y labels
+        mpl.rc('xtick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
+        mpl.rc('ytick', labelsize=SMALL_SIZE)    # fontsize of the tick labels
+        mpl.rc('legend', fontsize=SMALL_SIZE)    # legend fontsize
+        mpl.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
 
 
         # font = {'family' : 'normal',
         #         'weight' : 'bold',
         #         'size'   : fontsize}
 
         # header.mpl.rc('font', **font)
@@ -345,15 +346,15 @@
             legend_fontsize = fontsize
     
 
 
 
     if legend_fontsize:
         ''
-        header.mpl.rc('legend', fontsize= legend_fontsize) 
+        mpl.rc('legend', fontsize= legend_fontsize) 
 
     if corner_letter_pos is None:
         corner_letter_pos = [0.05,0.8]
     # print('fontsize', fontsize, legend_fontsize)
 
 
     if hasattr(header, 'first'):
@@ -397,15 +398,15 @@
     if params is None:
         params = {}
 
 
     if corner_letter:
         # print(corner_letter)
         ''
-        sz = header.mpl.rcParams['font.size']
+        sz = mpl.rcParams['font.size']
         ax.text(corner_letter_pos[0],corner_letter_pos[1], corner_letter, size = sz*1.5, transform=ax.transAxes) # transform = None - by default in data coordinates!
 
         # text(x, y, s, bbox=dict(facecolor='red', alpha=0.5))
 
 
     if convex:
         from scipy.spatial import ConvexHull
```

### Comparing `siman-1.3.7/siman/plot_functions.py` & `siman-1.3.8/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/polaron.py` & `siman-1.3.8/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/polaron_hop.py` & `siman-1.3.8/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/polaron_mod.py` & `siman-1.3.8/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/project_funcs.py` & `siman-1.3.8/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/properties_2d.py` & `siman-1.3.8/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/properties_energy.py` & `siman-1.3.8/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/properties_lattice.py` & `siman-1.3.8/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/set_functions.py` & `siman-1.3.8/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/simanrc.py` & `siman-1.3.8/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/small_functions.py` & `siman-1.3.8/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/structure_functions.py` & `siman-1.3.8/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/table_functions.py` & `siman-1.3.8/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/thermo.py` & `siman-1.3.8/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman/workflow_utilities.py` & `siman-1.3.8/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.7/siman.egg-info/PKG-INFO` & `siman-1.3.8/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.7
+Version: 1.3.8
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.7/siman.egg-info/SOURCES.txt` & `siman-1.3.8/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

