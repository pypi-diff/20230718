# Comparing `tmp/o2sclpy-0.927.post1.tar.gz` & `tmp/o2sclpy-0.928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "o2sclpy-0.927.post1.tar", last modified: Sun Jul 24 18:26:44 2022, max compression
+gzip compressed data, was "o2sclpy-0.928.tar", last modified: Tue Jul 18 05:21:58 2023, max compression
```

## Comparing `o2sclpy-0.927.post1.tar` & `o2sclpy-0.928.tar`

### file list

```diff
@@ -1,96 +1,36 @@
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.437860 o2sclpy-0.927.post1/
--rw-r--r--   0 awsteiner   (501) staff       (20)      145 2022-05-11 21:45:38.000000 o2sclpy-0.927.post1/.gitignore
--rw-r--r--   0 awsteiner   (501) staff       (20)     1073 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/.travis.yml
--rw-r--r--   0 awsteiner   (501) staff       (20)     2613 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/.travis.yml.old
--rw-r--r--   0 awsteiner   (501) staff       (20)    35141 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/LICENSE
--rw-r--r--   0 awsteiner   (501) staff       (20)       16 2022-07-24 16:59:08.000000 o2sclpy-0.927.post1/MANIFEST.in
--rw-r--r--   0 awsteiner   (501) staff       (20)      620 2022-07-24 18:26:44.437501 o2sclpy-0.927.post1/PKG-INFO
--rw-r--r--   0 awsteiner   (501) staff       (20)      113 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/README.md
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.403547 o2sclpy-0.927.post1/bin/
--rwxr-xr-x   0 awsteiner   (501) staff       (20)     1234 2022-04-13 14:28:43.000000 o2sclpy-0.927.post1/bin/o2graph
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.415448 o2sclpy-0.927.post1/doc/
--rw-r--r--   0 awsteiner   (501) staff       (20)        6 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/.gitignore
--rw-r--r--   0 awsteiner   (501) staff       (20)     1725 2022-07-22 22:12:57.000000 o2sclpy-0.927.post1/doc/Makefile
--rw-r--r--   0 awsteiner   (501) staff       (20)    17103 2022-07-22 22:02:03.000000 o2sclpy-0.927.post1/doc/base.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)       97 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/class_cap_cout.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      114 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/class_o2graph_plotter.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)       96 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/class_plot_base.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)       94 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/class_plotter.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      105 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/class_yt_plot_base.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     5326 2022-07-24 18:22:17.000000 o2sclpy-0.927.post1/doc/conf.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     5131 2022-07-22 22:02:05.000000 o2sclpy-0.927.post1/doc/eos.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      386 2022-06-28 17:41:20.000000 o2sclpy-0.927.post1/doc/ex_nucmass.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      396 2022-06-28 17:41:33.000000 o2sclpy-0.927.post1/doc/ex_sfho.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      476 2022-06-28 17:41:54.000000 o2sclpy-0.927.post1/doc/ex_skyrme.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      466 2022-06-28 17:42:04.000000 o2sclpy-0.927.post1/doc/ex_table.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      350 2022-07-22 19:45:27.000000 o2sclpy-0.927.post1/doc/examples.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     3198 2022-07-22 22:02:03.000000 o2sclpy-0.927.post1/doc/hdf.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      652 2022-07-24 18:22:17.000000 o2sclpy-0.927.post1/doc/index.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     1380 2022-07-21 20:28:40.000000 o2sclpy-0.927.post1/doc/install.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      321 2022-07-21 20:31:27.000000 o2sclpy-0.927.post1/doc/licensing.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     4883 2022-07-22 19:45:12.000000 o2sclpy-0.927.post1/doc/link_cpp.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     5037 2022-07-22 22:02:04.000000 o2sclpy-0.927.post1/doc/nuclei.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     4030 2022-07-21 20:30:20.000000 o2sclpy-0.927.post1/doc/o2graph.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     2318 2022-07-21 20:31:08.000000 o2sclpy-0.927.post1/doc/other.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      681 2022-07-21 20:30:57.000000 o2sclpy-0.927.post1/doc/other_objs.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     4711 2022-07-22 22:02:04.000000 o2sclpy-0.927.post1/doc/part.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     1597 2022-06-28 18:24:26.000000 o2sclpy-0.927.post1/doc/plot_ref.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      176 2021-10-15 20:55:47.000000 o2sclpy-0.927.post1/doc/ref_cpp.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      259 2022-07-21 20:34:06.000000 o2sclpy-0.927.post1/doc/ref_python.rst
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.416331 o2sclpy-0.927.post1/doc/static/
--rw-r--r--   0 awsteiner   (501) staff       (20)       17 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/.gitignore
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.419413 o2sclpy-0.927.post1/doc/static/figures/
--rw-r--r--   0 awsteiner   (501) staff       (20)       17 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/figures/.gitignore
--rw-r--r--   0 awsteiner   (501) staff       (20)    25224 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/figures/table_plotm_a.o2
--rw-r--r--   0 awsteiner   (501) staff       (20)    25224 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/figures/table_plotm_b.o2
--rw-r--r--   0 awsteiner   (501) staff       (20)    25224 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/figures/table_plotm_c.o2
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.420915 o2sclpy-0.927.post1/doc/static/licenses/
--rw-r--r--   0 awsteiner   (501) staff       (20)    20407 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/licenses/fdl_license.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)    35147 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/static/licenses/gpl_license.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)     4651 2022-07-24 04:50:06.000000 o2sclpy-0.927.post1/doc/static/o2graph.help.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)       59 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/doc/todos.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     2027 2022-06-28 18:24:30.000000 o2sclpy-0.927.post1/doc/yt.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     2289 2022-07-22 22:10:01.000000 o2sclpy-0.927.post1/makefile
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.430125 o2sclpy-0.927.post1/o2sclpy/
--rw-r--r--   0 awsteiner   (501) staff       (20)     4382 2022-06-09 01:15:52.000000 o2sclpy-0.927.post1/o2sclpy/__init__.py
--rw-r--r--   0 awsteiner   (501) staff       (20)   264011 2022-07-22 22:02:03.000000 o2sclpy-0.927.post1/o2sclpy/base.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     2562 2022-04-11 20:45:58.000000 o2sclpy-0.927.post1/o2sclpy/cap_cout.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    41806 2022-07-24 18:22:56.000000 o2sclpy-0.927.post1/o2sclpy/doc_data.py
--rw-r--r--   0 awsteiner   (501) staff       (20)   130067 2022-07-22 22:02:05.000000 o2sclpy-0.927.post1/o2sclpy/eos.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    50169 2022-07-22 22:02:03.000000 o2sclpy-0.927.post1/o2sclpy/hdf.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     7022 2022-06-09 01:15:19.000000 o2sclpy-0.927.post1/o2sclpy/hdf_add.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    13264 2022-04-11 20:48:26.000000 o2sclpy-0.927.post1/o2sclpy/link_o2scl.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    61750 2022-07-22 22:02:04.000000 o2sclpy-0.927.post1/o2sclpy/nuclei.py
--rw-r--r--   0 awsteiner   (501) staff       (20)   227957 2022-07-08 03:44:21.000000 o2sclpy-0.927.post1/o2sclpy/o2graph_plotter.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    34387 2022-04-10 04:15:06.000000 o2sclpy-0.927.post1/o2sclpy/other.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    76919 2022-07-22 22:02:04.000000 o2sclpy-0.927.post1/o2sclpy/part.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    61483 2022-05-03 19:42:19.000000 o2sclpy-0.927.post1/o2sclpy/plot_base.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    21081 2022-04-23 10:12:43.000000 o2sclpy-0.927.post1/o2sclpy/plot_info.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    15632 2022-04-11 21:01:58.000000 o2sclpy-0.927.post1/o2sclpy/plotter.py
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.435514 o2sclpy-0.927.post1/o2sclpy/test/
--rw-r--r--   0 awsteiner   (501) staff       (20)       19 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/o2sclpy/test/.gitignore
--rw-r--r--   0 awsteiner   (501) staff       (20)     4901 2021-10-17 03:01:22.000000 o2sclpy-0.927.post1/o2sclpy/test/test_cpp_class.py
--rw-r--r--   0 awsteiner   (501) staff       (20)      496 2022-03-17 04:44:43.000000 o2sclpy-0.927.post1/o2sclpy/test/test_lib_settings.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     3268 2022-04-18 12:55:32.000000 o2sclpy-0.927.post1/o2sclpy/test/test_table.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     1572 2022-04-17 00:38:15.000000 o2sclpy-0.927.post1/o2sclpy/test/test_table3d.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     1875 2021-10-18 02:30:20.000000 o2sclpy-0.927.post1/o2sclpy/test/test_table_units.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     3455 2022-04-10 04:42:05.000000 o2sclpy-0.927.post1/o2sclpy/test/test_tensor.py
--rw-r--r--   0 awsteiner   (501) staff       (20)     1135 2021-10-18 02:31:40.000000 o2sclpy-0.927.post1/o2sclpy/test/test_ug.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    32914 2022-05-06 19:40:02.000000 o2sclpy-0.927.post1/o2sclpy/utils.py
--rw-r--r--   0 awsteiner   (501) staff       (20)    34026 2022-05-03 21:34:49.000000 o2sclpy-0.927.post1/o2sclpy/yt_plot_base.py
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.432580 o2sclpy-0.927.post1/o2sclpy.egg-info/
--rw-r--r--   0 awsteiner   (501) staff       (20)      620 2022-07-24 18:26:44.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/PKG-INFO
--rw-r--r--   0 awsteiner   (501) staff       (20)     1680 2022-07-24 18:26:44.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/SOURCES.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)        1 2022-07-24 18:26:44.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/dependency_links.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)        1 2021-08-22 03:57:10.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/not-zip-safe
--rw-r--r--   0 awsteiner   (501) staff       (20)       36 2022-07-24 18:26:44.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/requires.txt
--rw-r--r--   0 awsteiner   (501) staff       (20)        8 2022-07-24 18:26:44.000000 o2sclpy-0.927.post1/o2sclpy.egg-info/top_level.txt
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.436554 o2sclpy-0.927.post1/old/
--rw-r--r--   0 awsteiner   (501) staff       (20)      723 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/old/class.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)      149 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/old/internal.rst
--rw-r--r--   0 awsteiner   (501) staff       (20)     2800 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/old/slack.py
--rw-r--r--   0 awsteiner   (501) staff       (20)       38 2022-07-24 18:26:44.437981 o2sclpy-0.927.post1/setup.cfg
--rw-r--r--   0 awsteiner   (501) staff       (20)     1092 2022-07-24 18:26:23.000000 o2sclpy-0.927.post1/setup.py
-drwxr-xr-x   0 awsteiner   (501) staff       (20)        0 2022-07-24 18:26:44.437023 o2sclpy-0.927.post1/snap/
--rw-r--r--   0 awsteiner   (501) staff       (20)      870 2022-07-24 18:22:17.000000 o2sclpy-0.927.post1/snap/snapcraft.yaml
--rw-r--r--   0 awsteiner   (501) staff       (20)       69 2021-08-15 03:56:54.000000 o2sclpy-0.927.post1/tox.ini
+drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.762675 o2sclpy-0.928/
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    35141 2023-05-23 14:43:12.000000 o2sclpy-0.928/LICENSE
+-rw-r--r--   0 awsteiner2   (502) staff       (20)       16 2023-05-23 14:43:12.000000 o2sclpy-0.928/MANIFEST.in
+-rw-r--r--   0 awsteiner2   (502) staff       (20)      618 2023-07-18 05:21:58.762190 o2sclpy-0.928/PKG-INFO
+-rw-r--r--   0 awsteiner2   (502) staff       (20)      113 2023-05-23 14:43:12.000000 o2sclpy-0.928/README.md
+drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.726865 o2sclpy-0.928/bin/
+-rwxr-xr-x   0 awsteiner2   (502) staff       (20)     1244 2023-07-09 04:54:59.000000 o2sclpy-0.928/bin/o2graph
+drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.757562 o2sclpy-0.928/o2sclpy/
+-rw-r--r--   0 awsteiner2   (502) staff       (20)     4434 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/__init__.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)   280045 2023-07-14 04:26:24.000000 o2sclpy-0.928/o2sclpy/base.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)     2562 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/cap_cout.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)     2054 2023-07-17 04:23:20.000000 o2sclpy-0.928/o2sclpy/doc_data.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)   132582 2023-07-14 04:26:27.000000 o2sclpy-0.928/o2sclpy/eos.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    21774 2023-07-09 05:04:03.000000 o2sclpy-0.928/o2sclpy/gmm.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    68275 2023-07-14 04:26:25.000000 o2sclpy-0.928/o2sclpy/hdf.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)     7022 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/hdf_add.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    16357 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/interpm.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    11217 2023-07-09 04:58:47.000000 o2sclpy-0.928/o2sclpy/kde.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    13264 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/link_o2scl.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    61878 2023-07-14 04:26:26.000000 o2sclpy-0.928/o2sclpy/nuclei.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)   230878 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/o2graph_plotter.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    78526 2023-07-14 04:26:25.000000 o2sclpy-0.928/o2sclpy/other.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    76508 2023-07-14 04:26:26.000000 o2sclpy-0.928/o2sclpy/part.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    95211 2023-07-10 18:55:03.000000 o2sclpy-0.928/o2sclpy/plot_base.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    21777 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/plot_info.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    30657 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/utils.py
+-rw-r--r--   0 awsteiner2   (502) staff       (20)    33623 2023-07-09 04:54:59.000000 o2sclpy-0.928/o2sclpy/yt_plot_base.py
+drwxr-xr-x   0 awsteiner2   (502) staff       (20)        0 2023-07-18 05:21:58.761493 o2sclpy-0.928/o2sclpy.egg-info/
+-rw-r--r--   0 awsteiner2   (502) staff       (20)      618 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/PKG-INFO
+-rw-r--r--   0 awsteiner2   (502) staff       (20)      591 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/SOURCES.txt
+-rw-r--r--   0 awsteiner2   (502) staff       (20)        1 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/dependency_links.txt
+-rw-r--r--   0 awsteiner2   (502) staff       (20)        1 2023-06-06 03:54:51.000000 o2sclpy-0.928/o2sclpy.egg-info/not-zip-safe
+-rw-r--r--   0 awsteiner2   (502) staff       (20)       36 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/requires.txt
+-rw-r--r--   0 awsteiner2   (502) staff       (20)        8 2023-07-18 05:21:58.000000 o2sclpy-0.928/o2sclpy.egg-info/top_level.txt
+-rw-r--r--   0 awsteiner2   (502) staff       (20)       38 2023-07-18 05:21:58.762861 o2sclpy-0.928/setup.cfg
+-rw-r--r--   0 awsteiner2   (502) staff       (20)     1090 2023-07-17 04:23:20.000000 o2sclpy-0.928/setup.py
```

### Comparing `o2sclpy-0.927.post1/LICENSE` & `o2sclpy-0.928/LICENSE`

 * *Files identical despite different names*

### Comparing `o2sclpy-0.927.post1/bin/o2graph` & `o2sclpy-0.928/bin/o2graph`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2020, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -19,14 +19,15 @@
 #  You should have received a copy of the GNU General Public License
 #  along with O2sclpy. If not, see <http://www.gnu.org/licenses/>.
 #  
 #  -------------------------------------------------------------------
 
 # For sys.argv
 import sys
+import os
 
 from o2sclpy.link_o2scl import linker
 
 l=linker()
 backend=l.get_library_settings(sys.argv)
 l.link_o2scl()
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/__init__.py` & `o2sclpy-0.928/o2sclpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -26,25 +26,27 @@
 #
 
 from o2sclpy.doc_data import *
 from o2sclpy.link_o2scl import *
 from o2sclpy.utils import *
 from o2sclpy.plot_base import *
 from o2sclpy.yt_plot_base import *
-from o2sclpy.plotter import *
 from o2sclpy.o2graph_plotter import *
 from o2sclpy.plot_info import *
 from o2sclpy.base import *
 from o2sclpy.part import *
 from o2sclpy.nuclei import *
 from o2sclpy.eos import *
 from o2sclpy.hdf import *
 from o2sclpy.hdf_add import *
 from o2sclpy.other import *
 from o2sclpy.cap_cout import *
+from o2sclpy.interpm import *
+from o2sclpy.gmm import *
+from o2sclpy.kde import *
 
 """
 The version number string
 """
 
 class todo_list:
     """
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/base.py` & `o2sclpy-0.928/o2sclpy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2022, Andrew W. Steiner
+  Copyright (C) 2020-2023, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -14,15 +14,15 @@
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with O2scl. If not, see <http://www.gnu.org/licenses/>.
 
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 """
 
 import ctypes
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 import numpy
 
@@ -33,15 +33,16 @@
 itp_akima_peri=5
 itp_monotonic=6
 itp_steffen=7
 itp_nearest_neigh=8
 
 class std_string:
     """
-    Python interface for C++ class ``std::string``.
+    Note that std_string objects are not "immutable" like Python
+    strings.
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -78,20 +79,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_string
         
-        Returns: a std_string object
+        Returns: std_string object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_string
+        
+        Returns: new copy of the std_string object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_string
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def length(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_std_string_length
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
@@ -109,15 +123,15 @@
         ret=func(self._ptr,n)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: char
+        | *value*: ``char``
         """
         func=self._link.o2scl.o2scl_std_string_setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_char]
         func(self._ptr,i,value)
         return
 
     def resize(self,n):
@@ -139,15 +153,15 @@
         return self.length()
      
     def init_bytes(self,s):
         """
         Initialize the string from a Python bytes object
     
         | Parameters:
-        | *s* a Python bytes string
+        | *s*: a Python bytes string
         """
         self.resize(len(s))
         for i in range(0,len(s)):
             self.__setitem__(i,s[i])
         return
     
     def to_bytes(self):
@@ -204,20 +218,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_vector
         
-        Returns: a std_vector object
+        Returns: std_vector object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_vector
+        
+        Returns: new copy of the std_vector object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_double_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_double__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -245,15 +272,15 @@
         ret=func(self._ptr,n)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: double
+        | *value*: ``double``
         """
         func=self._link.o2scl.o2scl_std_vector_double__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_double]
         func(self._ptr,i,value)
         return
 
     def __len__(self):
@@ -270,14 +297,37 @@
     
         Returns: a one-dimensional ``numpy`` array
         """
         ret=numpy.zeros((self.size()))
         for i in range(0,self.size()):
             ret[i]=self.__getitem__(i)
         return ret
+    
+    def from_list(self,lst):
+        """
+        Set the vector with a python list
+        """
+        self.resize(len(lst))
+        for i in range(0,len(lst)):
+            self[i]=lst[i]
+        return
+                 
+    def erase(self,index):
+        """
+        Erase item at specified index
+        """
+        n=self.size()
+        v2=self.deepcopy()
+        self.resize(n-1)
+        for i in range(0,n-1):
+            if i<index:
+                self[i]=v2[i]
+            else:
+                self[i]=v2[i+1]
+        return
 
 class std_vector_int:
     """
     Python interface for C++ class ``std::vector<int>``.
     """
 
     _ptr=0
@@ -318,20 +368,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_vector_int
         
-        Returns: a std_vector_int object
+        Returns: std_vector_int object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_vector_int
+        
+        Returns: new copy of the std_vector_int object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_int_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_int__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -359,15 +422,15 @@
         ret=func(self._ptr,n)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: int
+        | *value*: ``int``
         """
         func=self._link.o2scl.o2scl_std_vector_int__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_int]
         func(self._ptr,i,value)
         return
 
     def __len__(self):
@@ -432,20 +495,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_vector_size_t
         
-        Returns: a std_vector_size_t object
+        Returns: std_vector_size_t object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_vector_size_t
+        
+        Returns: new copy of the std_vector_size_t object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_size_t_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_size_t__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -473,15 +549,15 @@
         ret=func(self._ptr,n)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: size_t
+        | *value*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_size_t__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
         func(self._ptr,i,value)
         return
 
     def __len__(self):
@@ -568,20 +644,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_vector_string
         
-        Returns: a std_vector_string object
+        Returns: std_vector_string object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_vector_string
+        
+        Returns: new copy of the std_vector_string object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_std_string_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_std_string__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -598,42 +687,62 @@
         ret=func(self._ptr)
         return ret
 
     def __getitem__(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
-        | Returns: std_string object
+        | Returns: Python bytes object
         """
         func=self._link.o2scl.o2scl_std_vector_std_string__getitem
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         ret=func(self._ptr,n)
         strt=std_string(self._link,ret)
         strt._owner=True
         return strt.to_bytes()
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: Python bytes string
+        | *value*: Python bytes object
         """
         func=self._link.o2scl.o2scl_std_vector_std_string__setitem
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_char_p]
-        func(self._ptr,i,value)
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
+        s=std_string(self._link)
+        s.init_bytes(value)
+        func(self._ptr,i,s._ptr)
         return
 
     def __len__(self):
         """
         Return the length of the vector
     
         Returns: a Python int
         """
         return self.size()
+    
+    def set_list(self,ls):
+        """
+        Set the object from a python list
+        """
+        self.resize(len(ls))
+        for i in range(0,len(ls)):
+            self[i]=force_bytes(ls[i])
+        return
+    
+    def to_list(self):
+        """
+        Set the object from a python list
+        """
+        ret=[]
+        for i in range(0,self.size()):
+            ret.append(self[i])
+        return ret
 
 class ublas_vector:
     """
     Python interface for C++ class ``boost::numeric::ublas::vector<double>``.
     """
 
     _ptr=0
@@ -674,20 +783,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ublas_vector
         
-        Returns: a ublas_vector object
+        Returns: ublas_vector object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class ublas_vector
+        
+        Returns: new copy of the ublas_vector object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_boost_numeric_ublas_vector_double_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def size(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_vector_double__size
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
@@ -715,15 +837,15 @@
         ret=func(self._ptr,i)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: double
+        | *value*: ``double``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_vector_double__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_double]
         func(self._ptr,i,value)
         return
 
     def __len__(self):
@@ -788,20 +910,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ublas_vector_int
         
-        Returns: a ublas_vector_int object
+        Returns: ublas_vector_int object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class ublas_vector_int
+        
+        Returns: new copy of the ublas_vector_int object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_boost_numeric_ublas_vector_int_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def size(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_vector_int__size
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
@@ -829,15 +964,15 @@
         ret=func(self._ptr,i)
         return ret
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
-        | *value*: int
+        | *value*: ``int``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_vector_int__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_int]
         func(self._ptr,i,value)
         return
 
     def __len__(self):
@@ -902,20 +1037,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ublas_matrix
         
-        Returns: a ublas_matrix object
+        Returns: ublas_matrix object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class ublas_matrix
+        
+        Returns: new copy of the ublas_matrix object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_boost_numeric_ublas_matrix_double_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def size1(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_double__size1
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
@@ -939,29 +1087,29 @@
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_double__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
         func(self._ptr,m,n)
         return
 
-    def __getitem__(self,tup):
+    def __getitem__(self,matrix_tuple):
         """
         | Parameters:
         | *m*: ``size_t``
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_double__getitem
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
-        m,n=tup
+        m,n=matrix_tuple
         ret=func(self._ptr,m,n)
         return ret
 
-    def __setitem__(self,tup,value):
-        m,n=tup
+    def __setitem__(self,matrix_tuple,value):
+        m,n=matrix_tuple
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_double__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_double]
         func(self._ptr,m,n,value)
         return
 
     def to_numpy(self):
         """
@@ -1019,20 +1167,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ublas_matrix_int
         
-        Returns: a ublas_matrix_int object
+        Returns: ublas_matrix_int object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class ublas_matrix_int
+        
+        Returns: new copy of the ublas_matrix_int object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_boost_numeric_ublas_matrix_int_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def size1(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_int__size1
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
@@ -1056,29 +1217,29 @@
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_int__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
         func(self._ptr,m,n)
         return
 
-    def __getitem__(self,tup):
+    def __getitem__(self,matrix_tuple):
         """
         | Parameters:
         | *m*: ``size_t``
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_int__getitem
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
-        m,n=tup
+        m,n=matrix_tuple
         ret=func(self._ptr,m,n)
         return ret
 
-    def __setitem__(self,tup,value):
-        m,n=tup
+    def __setitem__(self,matrix_tuple,value):
+        m,n=matrix_tuple
         func=self._link.o2scl.o2scl_boost_numeric_ublas_matrix_int__setitem
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_int]
         func(self._ptr,m,n,value)
         return
 
     def to_numpy(self):
         """
@@ -1136,20 +1297,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_vector_vector
         
-        Returns: a std_vector_vector object
+        Returns: std_vector_vector object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class std_vector_vector
+        
+        Returns: new copy of the std_vector_vector object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_std_vector_double_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_std_vector_double__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -1247,20 +1421,33 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class vec_vec_string
         
-        Returns: a vec_vec_string object
+        Returns: vec_vec_string object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
+    def __deepcopy__(self,memo):
+        """
+        Deep copy function for class vec_vec_string
+        
+        Returns: new copy of the vec_vec_string object
+        """
+
+        new_obj=type(self)(self._link)
+        f2=self._link.o2scl.o2scl_copy_std_vector_std_vector_std_string_
+        f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        f2(self._ptr,new_obj._ptr)
+        return new_obj
+
     def resize(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
         """
         func=self._link.o2scl.o2scl_std_vector_std_vector_std_string__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
@@ -1277,21 +1464,22 @@
         ret=func(self._ptr)
         return ret
 
     def __getitem__(self,n):
         """
         | Parameters:
         | *n*: ``size_t``
-        | Returns: vec_vec_string object
+        | Returns: std_vector_string object
         """
         func=self._link.o2scl.o2scl_std_vector_std_vector_std_string__getitem
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         ret=func(self._ptr,n)
-        return ret
+        vstrt=std_vector_string(self._link,ret)
+        return vstrt
 
     def __setitem__(self,i,value):
         """
         | Parameters:
         | *i*: ``size_t``
         | *value*: std_vector_string object
         """
@@ -1306,22 +1494,18 @@
     
         Returns: a Python int
         """
         return self.size()
 
 class std_complex:
     """
-    Python interface for O\ :sub:`2`\ scl class ``std::complex<double>``,
-    see
-    https://neutronstars.utk.edu/code/o2scl/html/class/std::complex<double>.html .
-    
     Note that python complex numbers are immutable, but this class is
     not, so the real and imaginary parts can be changed with real_set()
     and imag_set(). 
-                                 
+        
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1358,15 +1542,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class std_complex
         
-        Returns: a std_complex object
+        Returns: std_complex object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def real(self):
         """
@@ -1429,22 +1613,18 @@
         Returns: a python complex number
         """
         ret=self.real()+self.imag()*1j
         return ret
 
 class lib_settings_class:
     """
-    Python interface for O\ :sub:`2`\ scl class ``lib_settings_class``,
+    Python interface for O₂scl class ``lib_settings_class``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/lib_settings_class.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1481,15 +1661,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class lib_settings_class
         
-        Returns: a lib_settings_class object
+        Returns: lib_settings_class object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_data_dir(self):
         """
@@ -1744,25 +1924,25 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class table
         
-        Returns: a table object
+        Returns: table object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
         Deep copy function for class table
         
-        Returns: a new copy of the table object
+        Returns: new copy of the table object
         """
 
         new_obj=type(self)(self._link)
         f2=self._link.o2scl.o2scl_copy_table_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
@@ -2077,14 +2257,25 @@
         """
         func_=ctypes.c_char_p(force_bytes(func))
         func=self._link.o2scl.o2scl_table__delete_rows_func
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p]
         func(self._ptr,func_)
         return
 
+    def delete_rows_ends(self,row_start,row_end):
+        """
+        | Parameters:
+        | *row_start*: ``size_t``
+        | *row_end*: ``size_t``
+        """
+        func=self._link.o2scl.o2scl_table__delete_rows_ends
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
+        func(self._ptr,row_start,row_end)
+        return
+
     def line_of_names(self,names):
         """
         | Parameters:
         | *names*: string
         """
         names_=ctypes.c_char_p(force_bytes(names))
         func=self._link.o2scl.o2scl_table__line_of_names
@@ -2098,14 +2289,26 @@
         | *data*: :class:`std_vector` object
         """
         func=self._link.o2scl.o2scl_table__line_of_data
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,data._ptr)
         return
 
+    def insert_row(self,nv,data,row):
+        """
+        | Parameters:
+        | *nv*: ``size_t``
+        | *data*: :class:`std_vector` object
+        | *row*: ``size_t``
+        """
+        func=self._link.o2scl.o2scl_table__insert_row
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_size_t]
+        func(self._ptr,nv,data._ptr,row)
+        return
+
     def ordered_lookup(self,scol,val):
         """
         | Parameters:
         | *scol*: string
         | *val*: ``double``
         | Returns: a Python int
         """
@@ -2519,14 +2722,24 @@
         # Create a std_vector object and copy the data over
         vec=std_vector(self._link)
         vec.resize(len(v))
         for i in range(0,len(v)):
             vec[i]=v[i]
         self.line_of_data_vector(vec)
         return
+                                 
+    def row_to_dict(self,row):
+        """
+        Convert the specified row to a python dictionary
+        """
+        dct={}
+        for i in range(0,self.get_ncolumns()):
+            dct[self.get_column_name(i)]=self.get(self.get_column_name(i),
+                                                  row)
+        return dct
 
 class table_units(table):
     """
     Python interface for O\ :sub:`2`\ scl class ``table_units``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/table_units.html .
     """
@@ -2565,25 +2778,25 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class table_units
         
-        Returns: a table_units object
+        Returns: table_units object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
         Deep copy function for class table_units
         
-        Returns: a new copy of the table_units object
+        Returns: new copy of the table_units object
         """
 
         new_obj=type(self)(self._link)
         f2=self._link.o2scl.o2scl_copy_table_units_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
@@ -2700,15 +2913,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid
         
-        Returns: a uniform_grid object
+        Returns: uniform_grid object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_nbins(self):
         """
@@ -2787,14 +3000,26 @@
         | *v*: :class:`std_vector` object
         """
         func=self._link.o2scl.o2scl_uniform_grid__vector
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,v._ptr)
         return
 
+    def to_numpy(self):
+        """
+        Copy the ``uniform_grid`` object to a numpy array
+    
+        Returns: a one-dimensional ``numpy`` array
+        """
+        v=std_vector(self._link)
+        self.vector(v)
+        ret=numpy.zeros((self.get_npoints()))
+        for i in range(0,self.get_npoints()):
+            ret[i]=v[i]
+        return ret
 
 class uniform_grid_end(uniform_grid):
     """
     Python interface for O\ :sub:`2`\ scl class ``uniform_grid_end``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/uniform_grid_end.html .
     """
@@ -2833,15 +3058,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_end
         
-        Returns: a uniform_grid_end object
+        Returns: uniform_grid_end object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,end,n_bins):
@@ -2899,15 +3124,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_width
         
-        Returns: a uniform_grid_width object
+        Returns: uniform_grid_width object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,width,n_bins):
@@ -2965,15 +3190,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_end_width
         
-        Returns: a uniform_grid_end_width object
+        Returns: uniform_grid_end_width object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,end,width):
@@ -3031,15 +3256,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_log_end
         
-        Returns: a uniform_grid_log_end object
+        Returns: uniform_grid_log_end object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,end,n_bins):
@@ -3097,15 +3322,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_log_width
         
-        Returns: a uniform_grid_log_width object
+        Returns: uniform_grid_log_width object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,width,n_bins):
@@ -3163,15 +3388,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class uniform_grid_log_end_width
         
-        Returns: a uniform_grid_log_end_width object
+        Returns: uniform_grid_log_end_width object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,start,end,width):
@@ -3186,22 +3411,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_double,ctypes.c_double,ctypes.c_double]
         return cls(link,f(start,end,width))
 
 
 class table3d:
     """
-    Python interface for O\ :sub:`2`\ scl class ``table3d``,
+    Python interface for O₂scl class ``table3d``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/table3d.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3238,25 +3459,25 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class table3d
         
-        Returns: a table3d object
+        Returns: table3d object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
         Deep copy function for class table3d
         
-        Returns: a new copy of the table3d object
+        Returns: new copy of the table3d object
         """
 
         new_obj=type(self)(self._link)
         f2=self._link.o2scl.o2scl_copy_table3d
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
@@ -3826,22 +4047,18 @@
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
 
 class index_spec:
     """
-    Python interface for O\ :sub:`2`\ scl class ``index_spec``,
+    Python interface for O₂scl class ``index_spec``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/index_spec.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3878,15 +4095,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class index_spec
         
-        Returns: a index_spec object
+        Returns: index_spec object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def type(self):
@@ -4027,22 +4244,18 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class ix_index:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_index``,
+    Python interface for O₂scl class ``ix_index``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_index.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4080,15 +4293,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_index
         
-        Returns: a ix_index object
+        Returns: ix_index object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix):
@@ -4103,22 +4316,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t]
         return cls(link,f(ix))
 
 
 class ix_fixed:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_fixed``,
+    Python interface for O₂scl class ``ix_fixed``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_fixed.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4156,15 +4365,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_fixed
         
-        Returns: a ix_fixed object
+        Returns: ix_fixed object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,ix2):
@@ -4179,22 +4388,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_size_t]
         return cls(link,f(ix,ix2))
 
 
 class ix_sum:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_sum``,
+    Python interface for O₂scl class ``ix_sum``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_sum.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4232,15 +4437,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_sum
         
-        Returns: a ix_sum object
+        Returns: ix_sum object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix):
@@ -4255,22 +4460,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t]
         return cls(link,f(ix))
 
 
 class ix_trace:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_trace``,
+    Python interface for O₂scl class ``ix_trace``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_trace.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4308,15 +4509,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_trace
         
-        Returns: a ix_trace object
+        Returns: ix_trace object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,ix2):
@@ -4331,22 +4532,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_size_t]
         return cls(link,f(ix,ix2))
 
 
 class ix_reverse:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_reverse``,
+    Python interface for O₂scl class ``ix_reverse``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_reverse.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4384,15 +4581,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_reverse
         
-        Returns: a ix_reverse object
+        Returns: ix_reverse object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix):
@@ -4407,22 +4604,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t]
         return cls(link,f(ix))
 
 
 class ix_range:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_range``,
+    Python interface for O₂scl class ``ix_range``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_range.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4460,15 +4653,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_range
         
-        Returns: a ix_range object
+        Returns: ix_range object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,start,end):
@@ -4483,22 +4676,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_size_t,ctypes.c_size_t]
         return cls(link,f(ix,start,end))
 
 
 class ix_interp:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_interp``,
+    Python interface for O₂scl class ``ix_interp``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_interp.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4536,15 +4725,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_interp
         
-        Returns: a ix_interp object
+        Returns: ix_interp object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,v):
@@ -4559,22 +4748,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_double]
         return cls(link,f(ix,v))
 
 
 class ix_grid:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_grid``,
+    Python interface for O₂scl class ``ix_grid``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_grid.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4612,15 +4797,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_grid
         
-        Returns: a ix_grid object
+        Returns: ix_grid object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,start,end,n_bins,log):
@@ -4635,22 +4820,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_double,ctypes.c_double,ctypes.c_size_t,ctypes.c_bool]
         return cls(link,f(ix,start,end,n_bins,log))
 
 
 class ix_gridw:
     """
-    Python interface for O\ :sub:`2`\ scl class ``ix_gridw``,
+    Python interface for O₂scl class ``ix_gridw``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/ix_gridw.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -4688,15 +4869,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class ix_gridw
         
-        Returns: a ix_gridw object
+        Returns: ix_gridw object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @classmethod
     def init(cls,link,ix,start,end,width,log):
@@ -4758,25 +4939,25 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class tensor
         
-        Returns: a tensor object
+        Returns: tensor object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
         Deep copy function for class tensor
         
-        Returns: a new copy of the tensor object
+        Returns: new copy of the tensor object
         """
 
         new_obj=type(self)(self._link)
         f2=self._link.o2scl.o2scl_copy_tensor_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
@@ -5036,30 +5217,49 @@
         """
         func=self._link.o2scl.o2scl_tensor__total_sum
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
-    def rearrange_and_copy(self,spec,verbose=0,err_on_fail=True):
+    def copy_table3d_sum(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
         """
         | Parameters:
-        | *spec*: string
-        | *verbose* =0: ``int``
-        | *err_on_fail* =true: ``bool``
-        | Returns: :class:`tensor` object
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
         """
-        spec_=ctypes.c_char_p(force_bytes(spec))
-        func=self._link.o2scl.o2scl_tensor__rearrange_and_copy
-        func.restype=ctypes.c_void_p
-        func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
-        ret2=func(self._ptr,spec_,verbose,err_on_fail)
-        ret=tensor(self._link,ret2)
-        ret.owner=True
-        return ret
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor__copy_table3d_sum
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
+        return
+
+    def copy_table3d(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
+        """
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
+        """
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor__copy_table3d
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
+        return
 
     @classmethod
     def create_size(cls,link,rank,sizes):
         """
         Constructor-like class method for tensor<> .
 
         | Parameters:
@@ -5109,534 +5309,739 @@
         and resize
         """
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
         self.resize_vector(len(svst),svst)
         return
 
-class tensor_grid:
+class tensor_int:
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor_grid``,
+    Python interface for O\ :sub:`2`\ scl class ``tensor``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor_grid.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
         """
-        Init function for class tensor_grid
+        Init function for class tensor_int
 
         | Parameters:
         | *link* :class:`linker` object
         | *pointer* ``ctypes.c_void_p`` pointer
 
         """
 
         if pointer==0:
-            f=link.o2scl.o2scl_create_tensor_grid_
+            f=link.o2scl.o2scl_create_tensor_int_std_vector_int_
             f.restype=ctypes.c_void_p
             f.argtypes=[]
             self._ptr=f()
         else:
             self._ptr=pointer
             self._owner=False
         self._link=link
         return
 
     def __del__(self):
         """
-        Delete function for class tensor_grid
+        Delete function for class tensor_int
         """
 
         if self._owner==True:
-            f=self._link.o2scl.o2scl_free_tensor_grid_
+            f=self._link.o2scl.o2scl_free_tensor_int_std_vector_int_
             f.argtypes=[ctypes.c_void_p]
             f(self._ptr)
             self._owner=False
             self._ptr=0
         return
 
     def __copy__(self):
         """
-        Shallow copy function for class tensor_grid
+        Shallow copy function for class tensor_int
         
-        Returns: a tensor_grid object
+        Returns: tensor_int object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
-        Deep copy function for class tensor_grid
+        Deep copy function for class tensor_int
         
-        Returns: a new copy of the tensor_grid object
+        Returns: new copy of the tensor_int object
         """
 
         new_obj=type(self)(self._link)
-        f2=self._link.o2scl.o2scl_copy_tensor_grid_
+        f2=self._link.o2scl.o2scl_copy_tensor_int_std_vector_int_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
 
     def is_valid(self):
         """
         """
-        func=self._link.o2scl.o2scl_tensor_grid__is_valid
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__is_valid
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
-    def set_val_vector(self,grid_point,val):
+    def clear(self):
+        """
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__clear
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
+        return
+
+    def set_vector(self,index,val):
         """
         | Parameters:
-        | *grid_point*: :class:`vector<double>` object
-        | *val*: ``double``
+        | *index*: :class:`vector<size_t>` object
+        | *val*: ``int``
         """
-        func=self._link.o2scl.o2scl_tensor_grid__set_val
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,grid_point._ptr,val)
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__set
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_int]
+        func(self._ptr,index._ptr,val)
         return
 
-    def get_val_vector(self,grid_point):
+    def set_all(self,x):
         """
         | Parameters:
-        | *grid_point*: :class:`vector<double>` object
-        | Returns: a Python float
+        | *x*: ``int``
         """
-        func=self._link.o2scl.o2scl_tensor_grid__get_val
-        func.restype=ctypes.c_double
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__set_all
+        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
+        func(self._ptr,x)
+        return
+
+    def get_vector(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`vector<size_t>` object
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get
+        func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,grid_point._ptr)
+        ret=func(self._ptr,index._ptr)
         return ret
 
-    def resize(self,rank,dim):
+    def resize_vector(self,n,index):
         """
         | Parameters:
-        | *rank*: ``size_t``
-        | *dim*: :class:`vector<size_t>` object
+        | *n*: ``size_t``
+        | *index*: :class:`vector<size_t>` object
         """
-        func=self._link.o2scl.o2scl_tensor_grid__resize
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
-        func(self._ptr,rank,dim._ptr)
+        func(self._ptr,n,index._ptr)
         return
 
-    def is_grid_set(self):
+    def get_rank(self):
         """
-        | Returns: a Python boolean
+        | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__is_grid_set
-        func.restype=ctypes.c_bool
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_rank
+        func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
-    def set_grid_packed(self,grid):
+    def get_size(self,i):
         """
         | Parameters:
-        | *grid*: :class:`vector<double>` object
+        | *i*: ``size_t``
+        | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__set_grid_packed
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,grid._ptr)
-        return
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_size
+        func.restype=ctypes.c_size_t
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
+        ret=func(self._ptr,i)
+        return ret
 
-    def set_grid_vec_vec(self,grid_vecs):
+    def get_data(self):
+        """
+        | Returns: :class:`std_vector_int` object
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_data
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        ret2=std_vector_int(self._link,ret)
+        return ret2
+
+    def total_size(self):
+        """
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__total_size
+        func.restype=ctypes.c_size_t
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def pack_indices(self,index):
         """
         | Parameters:
-        | *grid_vecs*: :class:`vector<vector<double>>` object
+        | *index*: :class:`std_vector_size_t` object
+        | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__set_grid_vec_vec
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__pack_indices
+        func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        func(self._ptr,grid_vecs._ptr)
+        ret=func(self._ptr,index._ptr)
+        return ret
+
+    def unpack_index(self,ix,index):
+        """
+        | Parameters:
+        | *ix*: ``size_t``
+        | *index*: :class:`std_vector_size_t` object
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__unpack_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
+        func(self._ptr,ix,index._ptr)
         return
 
-    def default_grid(self):
+    def min_value(self):
         """
+        | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__default_grid
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__min_value
+        func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
-        func(self._ptr)
-        return
+        ret=func(self._ptr)
+        return ret
 
-    def set_grid_i_vec(self,i,grid):
+    def min_index(self,index):
         """
         | Parameters:
-        | *i*: ``size_t``
-        | *grid*: :class:`vector<double>` object
+        | *index*: :class:`std_vector_size_t` object
         """
-        func=self._link.o2scl.o2scl_tensor_grid__set_grid_i_vec
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
-        func(self._ptr,i,grid._ptr)
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__min_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index._ptr)
         return
 
-    def set_grid_i_func(self,ix,func):
+    def min(self,index):
         """
         | Parameters:
-        | *ix*: ``size_t``
-        | *func*: string
+        | *index*: :class:`std_vector_size_t` object
+        | Returns: , a Python int
         """
-        func_=ctypes.c_char_p(force_bytes(func))
-        func=self._link.o2scl.o2scl_tensor_grid__set_grid_i_func
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_char_p]
-        func(self._ptr,ix,func_)
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__min
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_int)]
+        val_conv=ctypes.c_int(0)
+        func(self._ptr,index._ptr,ctypes.byref(val_conv))
+        return val_conv.value
+
+    def max_value(self):
+        """
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__max_value
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def max_index(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`std_vector_size_t` object
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__max_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index._ptr)
         return
 
-    def get_grid(self,i,j):
+    def max(self,index):
         """
         | Parameters:
-        | *i*: ``size_t``
-        | *j*: ``size_t``
-        | Returns: a Python float
+        | *index*: :class:`std_vector_size_t` object
+        | Returns: , a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__get_grid
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
-        ret=func(self._ptr,i,j)
-        return ret
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__max
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_int)]
+        val_conv=ctypes.c_int(0)
+        func(self._ptr,index._ptr,ctypes.byref(val_conv))
+        return val_conv.value
 
-    def get_grid_packed(self):
+    def minmax_value(self):
         """
-        | Returns: ``numpy`` array
+        | Parameters:
+        | Returns: , a Python int, a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__get_grid_packed
-        n_=ctypes.c_int(0)
-        ptr_=ctypes.POINTER(ctypes.c_double)()
-        func.argtypes=[ctypes.c_void_p,ctypes.POINTER(ctypes.POINTER(ctypes.c_double)),ctypes.POINTER(ctypes.c_int)]
-        func(self._ptr,ctypes.byref(ptr_),ctypes.byref(n_))
-        ret=numpy.ctypeslib.as_array(ptr_,shape=(n_.value,))
-        return ret
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__minmax_value
+        func.argtypes=[ctypes.c_void_p,ctypes.POINTER(ctypes.c_int),ctypes.POINTER(ctypes.c_int)]
+        min_conv=ctypes.c_int(0)
+        max_conv=ctypes.c_int(0)
+        func(self._ptr,ctypes.byref(min_conv),ctypes.byref(max_conv))
+        return min_conv.value,max_conv.value
 
-    def set_grid(self,i,j,val):
+    def minmax_index(self,index_min,index_max):
         """
         | Parameters:
-        | *i*: ``size_t``
-        | *j*: ``size_t``
-        | *val*: ``double``
+        | *index_min*: :class:`std_vector_size_t` object
+        | *index_max*: :class:`std_vector_size_t` object
         """
-        func=self._link.o2scl.o2scl_tensor_grid__set_grid
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_double]
-        func(self._ptr,i,j,val)
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__minmax_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index_min._ptr,index_max._ptr)
         return
 
-    def lookup_grid(self,i,val):
+    def minmax(self,index_min,index_max):
         """
         | Parameters:
-        | *i*: ``size_t``
-        | *val*: ``double``
+        | *index_min*: :class:`std_vector_size_t` object
+        | *index_max*: :class:`std_vector_size_t` object
+        | Returns: , a Python int, a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__minmax
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_int),ctypes.c_void_p,ctypes.POINTER(ctypes.c_int)]
+        min_conv=ctypes.c_int(0)
+        max_conv=ctypes.c_int(0)
+        func(self._ptr,index_min._ptr,ctypes.byref(min_conv),index_max._ptr,ctypes.byref(max_conv))
+        return min_conv.value,max_conv.value
+
+    def total_sum(self):
+        """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_grid__lookup_grid
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_double]
-        ret=func(self._ptr,i,val)
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__total_sum
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
         return ret
 
-    def copy_table3d_align(self,ix_x,ix_y,index,tab,z_name="z"):
+    def copy_table3d_sum(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
         """
         | Parameters:
         | *ix_x*: ``size_t``
         | *ix_y*: ``size_t``
-        | *index*: :class:`vector<size_t>` object
         | *tab*: :class:`table3d` object
-        | *z_name* ="z": string
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
         """
-        z_name_=ctypes.c_char_p(force_bytes(z_name))
-        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_align
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
-        func(self._ptr,ix_x,ix_y,index._ptr,tab._ptr,z_name_)
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__copy_table3d_sum
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
         return
 
-    def copy_table3d_align_setxy(self,ix_x,ix_y,index,tab,x_name="x",y_name="y",z_name="z"):
+    def copy_table3d(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
         """
         | Parameters:
         | *ix_x*: ``size_t``
         | *ix_y*: ``size_t``
-        | *index*: :class:`vector<size_t>` object
         | *tab*: :class:`table3d` object
         | *x_name* ="x": string
         | *y_name* ="y": string
-        | *z_name* ="z": string
+        | *slice_name* ="z": string
         """
         x_name_=ctypes.c_char_p(force_bytes(x_name))
         y_name_=ctypes.c_char_p(force_bytes(y_name))
-        z_name_=ctypes.c_char_p(force_bytes(z_name))
-        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_align_setxy
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
-        func(self._ptr,ix_x,ix_y,index._ptr,tab._ptr,x_name_,y_name_,z_name_)
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__copy_table3d
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
         return
 
-    def clear(self):
-        """
+    @classmethod
+    def create_size(cls,link,rank,sizes):
         """
-        func=self._link.o2scl.o2scl_tensor_grid__clear
-        func.argtypes=[ctypes.c_void_p]
-        func(self._ptr)
-        return
+        Constructor-like class method for tensor<int,std::vector<int>> .
 
-    def interp_linear(self,v):
-        """
         | Parameters:
-        | *v*: :class:`vector<double>` object
-        | Returns: a Python float
+
         """
-        func=self._link.o2scl.o2scl_tensor_grid__interp_linear
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,v._ptr)
-        return ret
 
-    def from_table3d_fermi(self,t3d,slice,n_points,low=0.0,high=0.0,width=0.0):
+        f=link.o2scl.o2scl_tensor_int_std_vector_int__create_size
+        f.restype=ctypes.c_void_p
+        f.argtypes=[ctypes.c_size_t,ctypes.c_void_p]
+        return cls(link,f(rank,sizes._ptr))
+
+    def create_size(self,v):
         """
-        | Parameters:
-        | *t3d*: :class:`table3d` object
-        | *slice*: string
-        | *n_points*: ``size_t``
-        | *low* =0.0: ``double``
-        | *high* =0.0: ``double``
-        | *width* =0.0: ``double``
+        Copy ``v`` to an :class:`std_vector_size_t` object and add the line of
+        data to the table
         """
-        slice_=ctypes.c_char_p(force_bytes(slice))
-        func=self._link.o2scl.o2scl_tensor_grid__from_table3d_fermi
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_size_t,ctypes.c_double,ctypes.c_double,ctypes.c_double]
-        func(self._ptr,t3d._ptr,slice_,n_points,low,high,width)
+        # Create a std_vector object and copy the data over
+        vec=std_vector_size_t(self._link)
+        vec.resize(len(v))
+        for i in range(0,len(v)):
+            vec[i]=v[i]
+        self.create_size_vector(vec)
         return
-
-    def rearrange_and_copy(self,spec,verbose=0,err_on_fail=True):
+     
+    def set(self,index,val):
         """
-        | Parameters:
-        | *spec*: string
-        | *verbose* =0: ``int``
-        | *err_on_fail* =true: ``bool``
-        | Returns: :class:`tensor_grid` object
+        Copy ``index`` to an :class:`std_vector_size_t` object and add the 
+        data to the table
         """
-        spec_=ctypes.c_char_p(force_bytes(spec))
-        func=self._link.o2scl.o2scl_tensor_grid__rearrange_and_copy
-        func.restype=ctypes.c_void_p
-        func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
-        ret2=func(self._ptr,spec_,verbose,err_on_fail)
-        ret=tensor_grid(self._link,ret2)
-        ret.owner=True
-        return ret
-
+        svst=std_vector_size_t(self._link)
+        svst.init_py(index)
+        self.set_vector(svst,val)
+        return
+     
+    def get(self,index):
+        """
+        Copy ``index`` to an :class:`std_vector_size_t` object and get the 
+        data from the table
+        """
+        svst=std_vector_size_t(self._link)
+        svst.init_py(index)
+        return self.get_vector(svst)
+    
+    def resize(self,index):
+        """
+        Copy ``index`` to an :class:`std_vector_size_t` object 
+        and resize
+        """
+        svst=std_vector_size_t(self._link)
+        svst.init_py(index)
+        self.resize_vector(svst)
+        return
 
-class tensor_int:
+class tensor_size_t:
     """
     Python interface for O\ :sub:`2`\ scl class ``tensor``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
         """
-        Init function for class tensor_int
+        Init function for class tensor_size_t
 
         | Parameters:
         | *link* :class:`linker` object
         | *pointer* ``ctypes.c_void_p`` pointer
 
         """
 
         if pointer==0:
-            f=link.o2scl.o2scl_create_tensor_int_std_vector_int_
+            f=link.o2scl.o2scl_create_tensor_size_t_std_vector_size_t_
             f.restype=ctypes.c_void_p
             f.argtypes=[]
             self._ptr=f()
         else:
             self._ptr=pointer
             self._owner=False
         self._link=link
         return
 
     def __del__(self):
         """
-        Delete function for class tensor_int
+        Delete function for class tensor_size_t
         """
 
         if self._owner==True:
-            f=self._link.o2scl.o2scl_free_tensor_int_std_vector_int_
+            f=self._link.o2scl.o2scl_free_tensor_size_t_std_vector_size_t_
             f.argtypes=[ctypes.c_void_p]
             f(self._ptr)
             self._owner=False
             self._ptr=0
         return
 
     def __copy__(self):
         """
-        Shallow copy function for class tensor_int
+        Shallow copy function for class tensor_size_t
         
-        Returns: a tensor_int object
+        Returns: tensor_size_t object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
-        Deep copy function for class tensor_int
+        Deep copy function for class tensor_size_t
         
-        Returns: a new copy of the tensor_int object
+        Returns: new copy of the tensor_size_t object
         """
 
         new_obj=type(self)(self._link)
-        f2=self._link.o2scl.o2scl_copy_tensor_int_std_vector_int_
+        f2=self._link.o2scl.o2scl_copy_tensor_size_t_std_vector_size_t_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
 
     def is_valid(self):
         """
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__is_valid
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__is_valid
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
     def clear(self):
         """
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__clear
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__clear
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
     def set_vector(self,index,val):
         """
         | Parameters:
         | *index*: :class:`vector<size_t>` object
-        | *val*: ``int``
+        | *val*: ``size_t``
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__set
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_int]
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__set
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_size_t]
         func(self._ptr,index._ptr,val)
         return
 
     def set_all(self,x):
         """
         | Parameters:
-        | *x*: ``int``
+        | *x*: ``size_t``
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__set_all
-        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__set_all
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         func(self._ptr,x)
         return
 
     def get_vector(self,index):
         """
         | Parameters:
         | *index*: :class:`vector<size_t>` object
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         ret=func(self._ptr,index._ptr)
         return ret
 
     def resize_vector(self,n,index):
         """
         | Parameters:
         | *n*: ``size_t``
         | *index*: :class:`vector<size_t>` object
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__resize
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__resize
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
         func(self._ptr,n,index._ptr)
         return
 
     def get_rank(self):
         """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_rank
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_rank
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
     def get_size(self,i):
         """
         | Parameters:
         | *i*: ``size_t``
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_size
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_size
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         ret=func(self._ptr,i)
         return ret
 
     def get_data(self):
         """
-        | Returns: :class:`std_vector_int` object
+        | Returns: :class:`std_vector_size_t` object
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__get_data
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_data
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
-        ret2=std_vector_int(self._link,ret)
+        ret2=std_vector_size_t(self._link,ret)
         return ret2
 
     def total_size(self):
         """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__total_size
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__total_size
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
     def min_value(self):
         """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__min_value
-        func.restype=ctypes.c_int
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__min_value
+        func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
+    def min_index(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`std_vector_size_t` object
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__min_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index._ptr)
+        return
+
+    def min(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`std_vector_size_t` object
+        | Returns: , a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__min
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_size_t)]
+        val_conv=ctypes.c_size_t(0)
+        func(self._ptr,index._ptr,ctypes.byref(val_conv))
+        return val_conv.value
+
     def max_value(self):
         """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__max_value
-        func.restype=ctypes.c_int
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__max_value
+        func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
+    def max_index(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`std_vector_size_t` object
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__max_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index._ptr)
+        return
+
+    def max(self,index):
+        """
+        | Parameters:
+        | *index*: :class:`std_vector_size_t` object
+        | Returns: , a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__max
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_size_t)]
+        val_conv=ctypes.c_size_t(0)
+        func(self._ptr,index._ptr,ctypes.byref(val_conv))
+        return val_conv.value
+
+    def minmax_value(self):
+        """
+        | Parameters:
+        | Returns: , a Python int, a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__minmax_value
+        func.argtypes=[ctypes.c_void_p,ctypes.POINTER(ctypes.c_size_t),ctypes.POINTER(ctypes.c_size_t)]
+        min_conv=ctypes.c_size_t(0)
+        max_conv=ctypes.c_size_t(0)
+        func(self._ptr,ctypes.byref(min_conv),ctypes.byref(max_conv))
+        return min_conv.value,max_conv.value
+
+    def minmax_index(self,index_min,index_max):
+        """
+        | Parameters:
+        | *index_min*: :class:`std_vector_size_t` object
+        | *index_max*: :class:`std_vector_size_t` object
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__minmax_index
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,index_min._ptr,index_max._ptr)
+        return
+
+    def minmax(self,index_min,index_max):
+        """
+        | Parameters:
+        | *index_min*: :class:`std_vector_size_t` object
+        | *index_max*: :class:`std_vector_size_t` object
+        | Returns: , a Python int, a Python int
+        """
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__minmax
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_size_t),ctypes.c_void_p,ctypes.POINTER(ctypes.c_size_t)]
+        min_conv=ctypes.c_size_t(0)
+        max_conv=ctypes.c_size_t(0)
+        func(self._ptr,index_min._ptr,ctypes.byref(min_conv),index_max._ptr,ctypes.byref(max_conv))
+        return min_conv.value,max_conv.value
+
     def total_sum(self):
         """
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_int_std_vector_int__total_sum
-        func.restype=ctypes.c_int
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__total_sum
+        func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
+    def copy_table3d_sum(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
+        """
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
+        """
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__copy_table3d_sum
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
+        return
+
+    def copy_table3d(self,ix_x,ix_y,tab,x_name="x",y_name="y",slice_name="z"):
+        """
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
+        """
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__copy_table3d
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,tab._ptr,x_name_,y_name_,slice_name_)
+        return
+
     @classmethod
     def create_size(cls,link,rank,sizes):
         """
-        Constructor-like class method for tensor<int,std::vector<int>> .
+        Constructor-like class method for tensor<size_t,std::vector<size_t>> .
 
         | Parameters:
 
         """
 
-        f=link.o2scl.o2scl_tensor_int_std_vector_int__create_size
+        f=link.o2scl.o2scl_tensor_size_t_std_vector_size_t__create_size
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_size_t,ctypes.c_void_p]
         return cls(link,f(rank,sizes._ptr))
 
     def create_size(self,v):
         """
         Copy ``v`` to an :class:`std_vector_size_t` object and add the line of
@@ -5645,15 +6050,15 @@
         # Create a std_vector object and copy the data over
         vec=std_vector_size_t(self._link)
         vec.resize(len(v))
         for i in range(0,len(v)):
             vec[i]=v[i]
         self.create_size_vector(vec)
         return
-     
+      
     def set(self,index,val):
         """
         Copy ``index`` to an :class:`std_vector_size_t` object and add the 
         data to the table
         """
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
@@ -5675,281 +6080,406 @@
         and resize
         """
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
         self.resize_vector(svst)
         return
 
-class tensor_size_t:
+class tensor_grid(tensor):
     """
-    Python interface for O\ :sub:`2`\ scl class ``tensor``,
+    Python interface for O\ :sub:`2`\ scl class ``tensor_grid``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/tensor.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/tensor_grid.html .
     """
 
-    _ptr=0
-    _link=0
-    _owner=True
-
     def __init__(self,link,pointer=0):
         """
-        Init function for class tensor_size_t
+        Init function for class tensor_grid
 
         | Parameters:
         | *link* :class:`linker` object
         | *pointer* ``ctypes.c_void_p`` pointer
 
         """
 
         if pointer==0:
-            f=link.o2scl.o2scl_create_tensor_size_t_std_vector_size_t_
+            f=link.o2scl.o2scl_create_tensor_grid_
             f.restype=ctypes.c_void_p
             f.argtypes=[]
             self._ptr=f()
         else:
             self._ptr=pointer
             self._owner=False
         self._link=link
         return
 
     def __del__(self):
         """
-        Delete function for class tensor_size_t
+        Delete function for class tensor_grid
         """
 
         if self._owner==True:
-            f=self._link.o2scl.o2scl_free_tensor_size_t_std_vector_size_t_
+            f=self._link.o2scl.o2scl_free_tensor_grid_
             f.argtypes=[ctypes.c_void_p]
             f(self._ptr)
             self._owner=False
             self._ptr=0
         return
 
     def __copy__(self):
         """
-        Shallow copy function for class tensor_size_t
+        Shallow copy function for class tensor_grid
         
-        Returns: a tensor_size_t object
+        Returns: tensor_grid object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def __deepcopy__(self,memo):
         """
-        Deep copy function for class tensor_size_t
+        Deep copy function for class tensor_grid
         
-        Returns: a new copy of the tensor_size_t object
+        Returns: new copy of the tensor_grid object
         """
 
         new_obj=type(self)(self._link)
-        f2=self._link.o2scl.o2scl_copy_tensor_size_t_std_vector_size_t_
+        f2=self._link.o2scl.o2scl_copy_tensor_grid_
         f2.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         f2(self._ptr,new_obj._ptr)
         return new_obj
 
     def is_valid(self):
         """
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__is_valid
+        func=self._link.o2scl.o2scl_tensor_grid__is_valid
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
-    def clear(self):
+    def set_val_vector(self,grid_point,val):
         """
+        | Parameters:
+        | *grid_point*: :class:`vector<double>` object
+        | *val*: ``double``
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__clear
-        func.argtypes=[ctypes.c_void_p]
-        func(self._ptr)
+        func=self._link.o2scl.o2scl_tensor_grid__set_val
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
+        func(self._ptr,grid_point._ptr,val)
         return
 
-    def set_vector(self,index,val):
+    def get_val_vector(self,grid_point):
         """
         | Parameters:
-        | *index*: :class:`vector<size_t>` object
-        | *val*: ``size_t``
+        | *grid_point*: :class:`vector<double>` object
+        | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__set
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_size_t]
-        func(self._ptr,index._ptr,val)
-        return
+        func=self._link.o2scl.o2scl_tensor_grid__get_val
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        ret=func(self._ptr,grid_point._ptr)
+        return ret
 
-    def set_all(self,x):
+    def resize_vector(self,rank,dim):
         """
         | Parameters:
-        | *x*: ``size_t``
+        | *rank*: ``size_t``
+        | *dim*: :class:`vector<size_t>` object
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__set_all
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
-        func(self._ptr,x)
+        func=self._link.o2scl.o2scl_tensor_grid__resize
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
+        func(self._ptr,rank,dim._ptr)
         return
 
-    def get_vector(self,index):
+    def is_grid_set(self):
+        """
+        | Returns: a Python boolean
+        """
+        func=self._link.o2scl.o2scl_tensor_grid__is_grid_set
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def set_grid_packed(self,grid):
         """
         | Parameters:
-        | *index*: :class:`vector<size_t>` object
-        | Returns: a Python int
+        | *grid*: :class:`vector<double>` object
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get
-        func.restype=ctypes.c_int
+        func=self._link.o2scl.o2scl_tensor_grid__set_grid_packed
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,index._ptr)
-        return ret
+        func(self._ptr,grid._ptr)
+        return
 
-    def resize_vector(self,n,index):
+    def set_grid_vec_vec(self,grid_vecs):
         """
         | Parameters:
-        | *n*: ``size_t``
-        | *index*: :class:`vector<size_t>` object
+        | *grid_vecs*: :class:`vector<vector<double>>` object
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__resize
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
-        func(self._ptr,n,index._ptr)
+        func=self._link.o2scl.o2scl_tensor_grid__set_grid_vec_vec
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,grid_vecs._ptr)
         return
 
-    def get_rank(self):
+    def default_grid(self):
         """
-        | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_rank
-        func.restype=ctypes.c_size_t
+        func=self._link.o2scl.o2scl_tensor_grid__default_grid
         func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
-        return ret
+        func(self._ptr)
+        return
 
-    def get_size(self,i):
+    def set_grid_i_vec(self,i,grid):
         """
         | Parameters:
         | *i*: ``size_t``
-        | Returns: a Python int
+        | *grid*: :class:`vector<double>` object
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_size
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
-        ret=func(self._ptr,i)
-        return ret
+        func=self._link.o2scl.o2scl_tensor_grid__set_grid_i_vec
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p]
+        func(self._ptr,i,grid._ptr)
+        return
 
-    def get_data(self):
+    def set_grid_i_func(self,ix,func):
         """
-        | Returns: :class:`std_vector_size_t` object
+        | Parameters:
+        | *ix*: ``size_t``
+        | *func*: string
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__get_data
-        func.restype=ctypes.c_void_p
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
-        ret2=std_vector_size_t(self._link,ret)
-        return ret2
+        func_=ctypes.c_char_p(force_bytes(func))
+        func=self._link.o2scl.o2scl_tensor_grid__set_grid_i_func
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_char_p]
+        func(self._ptr,ix,func_)
+        return
 
-    def total_size(self):
+    def get_grid(self,i,j):
         """
-        | Returns: a Python int
+        | Parameters:
+        | *i*: ``size_t``
+        | *j*: ``size_t``
+        | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__total_size
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
+        func=self._link.o2scl.o2scl_tensor_grid__get_grid
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t]
+        ret=func(self._ptr,i,j)
         return ret
 
-    def min_value(self):
+    def get_grid_packed(self):
         """
-        | Returns: a Python int
+        | Returns: ``numpy`` array
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__min_value
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
+        func=self._link.o2scl.o2scl_tensor_grid__get_grid_packed
+        n_=ctypes.c_int(0)
+        ptr_=ctypes.POINTER(ctypes.c_double)()
+        func.argtypes=[ctypes.c_void_p,ctypes.POINTER(ctypes.POINTER(ctypes.c_double)),ctypes.POINTER(ctypes.c_int)]
+        func(self._ptr,ctypes.byref(ptr_),ctypes.byref(n_))
+        ret=numpy.ctypeslib.as_array(ptr_,shape=(n_.value,))
         return ret
 
-    def max_value(self):
+    def set_grid(self,i,j,val):
         """
+        | Parameters:
+        | *i*: ``size_t``
+        | *j*: ``size_t``
+        | *val*: ``double``
+        """
+        func=self._link.o2scl.o2scl_tensor_grid__set_grid
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_double]
+        func(self._ptr,i,j,val)
+        return
+
+    def lookup_grid(self,i,val):
+        """
+        | Parameters:
+        | *i*: ``size_t``
+        | *val*: ``double``
         | Returns: a Python int
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__max_value
+        func=self._link.o2scl.o2scl_tensor_grid__lookup_grid
         func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_double]
+        ret=func(self._ptr,i,val)
         return ret
 
-    def total_sum(self):
+    def copy_slice_interp(self,ifix,vals):
         """
-        | Returns: a Python int
+        | Parameters:
+        | *ifix*: :class:`std_vector_size_t` object
+        | *vals*: :class:`std_vector` object
+        | Returns: :class:`tensor_grid` object
         """
-        func=self._link.o2scl.o2scl_tensor_size_t_std_vector_size_t__total_sum
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p]
-        ret=func(self._ptr)
+        func=self._link.o2scl.o2scl_tensor_grid__copy_slice_interp
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+        ret2=func(self._ptr,ifix._ptr,vals._ptr)
+        ret=tensor_grid(self._link,ret2)
+        ret.owner=True
         return ret
 
-    @classmethod
-    def create_size(cls,link,rank,sizes):
+    def copy_table3d_align(self,ix_x,ix_y,index,tab,z_name="z"):
         """
-        Constructor-like class method for tensor<size_t,std::vector<size_t>> .
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *index*: :class:`vector<size_t>` object
+        | *tab*: :class:`table3d` object
+        | *z_name* ="z": string
+        """
+        z_name_=ctypes.c_char_p(force_bytes(z_name))
+        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_align
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,index._ptr,tab._ptr,z_name_)
+        return
 
+    def copy_table3d_align_setxy(self,ix_x,ix_y,index,tab,x_name="x",y_name="y",z_name="z"):
+        """
         | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *index*: :class:`vector<size_t>` object
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *z_name* ="z": string
+        """
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        z_name_=ctypes.c_char_p(force_bytes(z_name))
+        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_align_setxy
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,index._ptr,tab._ptr,x_name_,y_name_,z_name_)
+        return
 
+    def copy_table3d_interp(self,ix_x,ix_y,index,tab,slice_name="z"):
+        """
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *index*: :class:`std_vector_size_t` object
+        | *tab*: :class:`table3d` object
+        | *slice_name* ="z": string
         """
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_interp
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,index._ptr,tab._ptr,slice_name_)
+        return
 
-        f=link.o2scl.o2scl_tensor_size_t_std_vector_size_t__create_size
-        f.restype=ctypes.c_void_p
-        f.argtypes=[ctypes.c_size_t,ctypes.c_void_p]
-        return cls(link,f(rank,sizes._ptr))
+    def copy_table3d_interp_values(self,ix_x,ix_y,values,tab,slice_name="z",verbose=0):
+        """
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *values*: :class:`std_vector` object
+        | *tab*: :class:`table3d` object
+        | *slice_name* ="z": string
+        | *verbose* =0: ``int``
+        """
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_interp_values
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int]
+        func(self._ptr,ix_x,ix_y,values._ptr,tab._ptr,slice_name_,verbose)
+        return
 
-    def create_size(self,v):
+    def copy_table3d_interp_values_setxy(self,ix_x,ix_y,values,tab,x_name="x",y_name="y",slice_name="z"):
         """
-        Copy ``v`` to an :class:`std_vector_size_t` object and add the line of
-        data to the table
+        | Parameters:
+        | *ix_x*: ``size_t``
+        | *ix_y*: ``size_t``
+        | *values*: :class:`std_vector` object
+        | *tab*: :class:`table3d` object
+        | *x_name* ="x": string
+        | *y_name* ="y": string
+        | *slice_name* ="z": string
         """
-        # Create a std_vector object and copy the data over
-        vec=std_vector_size_t(self._link)
-        vec.resize(len(v))
-        for i in range(0,len(v)):
-            vec[i]=v[i]
-        self.create_size_vector(vec)
+        x_name_=ctypes.c_char_p(force_bytes(x_name))
+        y_name_=ctypes.c_char_p(force_bytes(y_name))
+        slice_name_=ctypes.c_char_p(force_bytes(slice_name))
+        func=self._link.o2scl.o2scl_tensor_grid__copy_table3d_interp_values_setxy
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
+        func(self._ptr,ix_x,ix_y,values._ptr,tab._ptr,x_name_,y_name_,slice_name_)
         return
-      
-    def set(self,index,val):
+
+    def clear(self):
         """
-        Copy ``index`` to an :class:`std_vector_size_t` object and add the 
-        data to the table
         """
-        svst=std_vector_size_t(self._link)
-        svst.init_py(index)
-        self.set_vector(svst,val)
+        func=self._link.o2scl.o2scl_tensor_grid__clear
+        func.argtypes=[ctypes.c_void_p]
+        func(self._ptr)
         return
-     
-    def get(self,index):
+
+    def set_interp_type(self,interp_type):
         """
-        Copy ``index`` to an :class:`std_vector_size_t` object and get the 
-        data from the table
+        | Parameters:
+        | *interp_type*: ``size_t``
         """
-        svst=std_vector_size_t(self._link)
-        svst.init_py(index)
-        return self.get_vector(svst)
-    
+        func=self._link.o2scl.o2scl_tensor_grid__set_interp_type
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
+        func(self._ptr,interp_type)
+        return
+
+    def interp_linear_partial(self,ix_to_interp,ix,val):
+        """
+        | Parameters:
+        | *ix_to_interp*: :class:`std_vector_size_t` object
+        | *ix*: :class:`std_vector_size_t` object
+        | *val*: :class:`std_vector` object
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_tensor_grid__interp_linear_partial
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+        ret=func(self._ptr,ix_to_interp._ptr,ix._ptr,val._ptr)
+        return ret
+
+    def interp_linear(self,v):
+        """
+        | Parameters:
+        | *v*: :class:`vector<double>` object
+        | Returns: a Python float
+        """
+        func=self._link.o2scl.o2scl_tensor_grid__interp_linear
+        func.restype=ctypes.c_double
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        ret=func(self._ptr,v._ptr)
+        return ret
+
+    def from_table3d_fermi(self,t3d,slice,n_points,low=0.0,high=0.0,width=0.0):
+        """
+        | Parameters:
+        | *t3d*: :class:`table3d` object
+        | *slice*: string
+        | *n_points*: ``size_t``
+        | *low* =0.0: ``double``
+        | *high* =0.0: ``double``
+        | *width* =0.0: ``double``
+        """
+        slice_=ctypes.c_char_p(force_bytes(slice))
+        func=self._link.o2scl.o2scl_tensor_grid__from_table3d_fermi
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_size_t,ctypes.c_double,ctypes.c_double,ctypes.c_double]
+        func(self._ptr,t3d._ptr,slice_,n_points,low,high,width)
+        return
+
     def resize(self,index):
         """
         Copy ``index`` to an :class:`std_vector_size_t` object 
         and resize
         """
         svst=std_vector_size_t(self._link)
         svst.init_py(index)
-        self.resize_vector(svst)
+        self.resize_vector(len(svst),svst)
         return
 
 class find_constants_const_entry:
     """
-    Python interface for O\ :sub:`2`\ scl class ``find_constants<>::const_entry``,
+    Python interface for O₂scl class ``find_constants<>::const_entry``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/find_constants<>::const_entry.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -5986,15 +6516,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class find_constants_const_entry
         
-        Returns: a find_constants_const_entry object
+        Returns: find_constants_const_entry object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_names(self):
         """
@@ -6235,22 +6765,18 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_int]
         func(self._ptr,value)
         return
 
 
 class find_constants:
     """
-    Python interface for O\ :sub:`2`\ scl class ``find_constants<>``,
+    Python interface for O₂scl class ``find_constants<>``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/find_constants<>.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -6287,15 +6813,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class find_constants
         
-        Returns: a find_constants object
+        Returns: find_constants object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def output_list_cout(self):
         """
@@ -6327,22 +6853,18 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_int]
         func(self._ptr,name._ptr,verbose)
         return
 
 
 class convert_units_der_unit:
     """
-    Python interface for O\ :sub:`2`\ scl class ``convert_units<>::der_unit``,
+    Python interface for O₂scl class ``convert_units<>::der_unit``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/convert_units<>::der_unit.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -6379,15 +6901,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class convert_units_der_unit
         
-        Returns: a convert_units_der_unit object
+        Returns: convert_units_der_unit object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_label(self):
         """
@@ -6588,15 +7110,15 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
     def set(self,label,val,name='',m=0,k=0,s=0,K=0,A=0,mol=0,cd=0):
         """
         Set the properties of a derived unit
-        FIXME: beter docs here
+        FIXME: better docs here
         """
         label2=std_string(self._link)
         label2.init_bytes(force_bytes(label))
         self.set_label(label2)
         self.val=val
         name2=std_string(self._link)
         name2.init_bytes(force_bytes(name))
@@ -6655,15 +7177,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class convert_units
         
-        Returns: a convert_units object
+        Returns: convert_units object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def verbose(self):
@@ -6891,22 +7413,18 @@
         du=convert_units_der_unit(self._link)
         du.set(label,val,name,m,k,s,K,A,mol,cd)
         self.add_unit_internal(du)
         return
 
 class columnify:
     """
-    Python interface for O\ :sub:`2`\ scl class ``columnify``,
+    Python interface for O₂scl class ``columnify``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/columnify.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -6943,15 +7461,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class columnify
         
-        Returns: a columnify object
+        Returns: columnify object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def align_left(self):
@@ -6959,81 +7477,71 @@
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_left
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def align_right(self):
         """
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_right
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def align_lmid(self):
         """
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_lmid
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def align_rmid(self):
         """
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_rmid
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def align_dp(self):
         """
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_dp
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def align_lnum(self):
         """
         Property of type ``ctypes.c_int``
         """
         func=self._link.o2scl.o2scl_columnify_get_align_lnum
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
 
-
 class format_float:
     """
-    Python interface for O\ :sub:`2`\ scl class ``format_float``,
+    Python interface for O₂scl class ``format_float``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/format_float.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -7070,15 +7578,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class format_float
         
-        Returns: a format_float object
+        Returns: format_float object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def set_sig_figs(self,sig_figs):
         """
@@ -7168,156 +7676,20 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_bool]
         ret=func(self._ptr,x,debug)
         strt=std_string(self._link,ret)
         strt._owner=True
         return strt.to_bytes()
 
 
-class interp:
-    """
-    Python interface for O\ :sub:`2`\ scl class ``interp<std::vector<double>>``,
-    see
-    https://neutronstars.utk.edu/code/o2scl/html/class/interp<std::vector<double>>.html .
-    
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
-    """
-
-    _ptr=0
-    _link=0
-    _owner=True
-
-    def __init__(self,link,pointer=0):
-        """
-        Init function for class interp
-
-        | Parameters:
-        | *link* :class:`linker` object
-        | *pointer* ``ctypes.c_void_p`` pointer
-
-        """
-
-        if pointer==0:
-            f=link.o2scl.o2scl_create_interp_std_vector_double_
-            f.restype=ctypes.c_void_p
-            f.argtypes=[]
-            self._ptr=f()
-        else:
-            self._ptr=pointer
-            self._owner=False
-        self._link=link
-        return
-
-    def __del__(self):
-        """
-        Delete function for class interp
-        """
-
-        if self._owner==True:
-            f=self._link.o2scl.o2scl_free_interp_std_vector_double_
-            f.argtypes=[ctypes.c_void_p]
-            f(self._ptr)
-            self._owner=False
-            self._ptr=0
-        return
-
-    def __copy__(self):
-        """
-        Shallow copy function for class interp
-        
-        Returns: a interp object
-        """
-
-        new_obj=type(self)(self._link,self._ptr)
-        return new_obj
-
-    def eval(self,x0,n,x,y):
-        """
-        | Parameters:
-        | *x0*: ``double``
-        | *n*: ``size_t``
-        | *x*: :class:`std_vector` object
-        | *y*: :class:`std_vector` object
-        | Returns: a Python float
-        """
-        func=self._link.o2scl.o2scl_interp_std_vector_double__eval
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,x0,n,x._ptr,y._ptr)
-        return ret
-
-    def deriv(self,x0,n,x,y):
-        """
-        | Parameters:
-        | *x0*: ``double``
-        | *n*: ``size_t``
-        | *x*: :class:`std_vector` object
-        | *y*: :class:`std_vector` object
-        | Returns: a Python float
-        """
-        func=self._link.o2scl.o2scl_interp_std_vector_double__deriv
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,x0,n,x._ptr,y._ptr)
-        return ret
-
-    def deriv2(self,x0,n,x,y):
-        """
-        | Parameters:
-        | *x0*: ``double``
-        | *n*: ``size_t``
-        | *x*: :class:`std_vector` object
-        | *y*: :class:`std_vector` object
-        | Returns: a Python float
-        """
-        func=self._link.o2scl.o2scl_interp_std_vector_double__deriv2
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,x0,n,x._ptr,y._ptr)
-        return ret
-
-    def integ(self,x1,x2,n,x,y):
-        """
-        | Parameters:
-        | *x1*: ``double``
-        | *x2*: ``double``
-        | *n*: ``size_t``
-        | *x*: :class:`std_vector` object
-        | *y*: :class:`std_vector` object
-        | Returns: a Python float
-        """
-        func=self._link.o2scl.o2scl_interp_std_vector_double__integ
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p]
-        ret=func(self._ptr,x1,x2,n,x._ptr,y._ptr)
-        return ret
-
-    def set_type(self,interp_type):
-        """
-        | Parameters:
-        | *interp_type*: ``int``
-        """
-        func=self._link.o2scl.o2scl_interp_std_vector_double__set_type
-        func.argtypes=[ctypes.c_void_p,ctypes.c_int]
-        func(self._ptr,interp_type)
-        return
-
-
 class interp_vec:
     """
-    Python interface for O\ :sub:`2`\ scl class ``interp_vec<std::vector<double>>``,
+    Python interface for O₂scl class ``interp_vec<std::vector<double>>``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/interp_vec<std::vector<double>>.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -7354,15 +7726,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class interp_vec
         
-        Returns: a interp_vec object
+        Returns: interp_vec object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def set(self,n,x,y,interp_type):
         """
@@ -7431,289 +7803,230 @@
         func=self._link.o2scl.o2scl_interp_vec_std_vector_double__integ
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,x1,x2)
         return ret
 
 
-class interp_krige_optim:
+class interp_krige_optim_rbf_noise:
     """
-    Python interface for O\ :sub:`2`\ scl class ``interp_krige_optim<std::vector<double>>``,
+    Python interface for O₂scl class ``interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>``,
     see
-    https://neutronstars.utk.edu/code/o2scl/html/class/interp_krige_optim<std::vector<double>>.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
         """
-        Init function for class interp_krige_optim
+        Init function for class interp_krige_optim_rbf_noise
 
         | Parameters:
         | *link* :class:`linker` object
         | *pointer* ``ctypes.c_void_p`` pointer
 
         """
 
         if pointer==0:
-            f=link.o2scl.o2scl_create_interp_krige_optim_std_vector_double_
+            f=link.o2scl.o2scl_create_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise_
             f.restype=ctypes.c_void_p
             f.argtypes=[]
             self._ptr=f()
         else:
             self._ptr=pointer
             self._owner=False
         self._link=link
         return
 
     def __del__(self):
         """
-        Delete function for class interp_krige_optim
+        Delete function for class interp_krige_optim_rbf_noise
         """
 
         if self._owner==True:
-            f=self._link.o2scl.o2scl_free_interp_krige_optim_std_vector_double_
+            f=self._link.o2scl.o2scl_free_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise_
             f.argtypes=[ctypes.c_void_p]
             f(self._ptr)
             self._owner=False
             self._ptr=0
         return
 
     def __copy__(self):
         """
-        Shallow copy function for class interp_krige_optim
+        Shallow copy function for class interp_krige_optim_rbf_noise
         
-        Returns: a interp_krige_optim object
+        Returns: interp_krige_optim_rbf_noise object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def mode_loo_cv(self):
         """
         Property of type ``ctypes.c_size_t``
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_mode_loo_cv
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__get_mode_loo_cv
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
+    @property
+    def mode_loo_cv_bf(self):
+        """
+        Property of type ``ctypes.c_size_t``
+        """
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__get_mode_loo_cv_bf
+        func.restype=ctypes.c_size_t
+        func.argtypes=[ctypes.c_void_p]
+        return func(self._ptr)
 
     @property
     def mode_max_lml(self):
         """
         Property of type ``ctypes.c_size_t``
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_mode_max_lml
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__get_mode_max_lml
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
-
     @property
     def verbose(self):
         """
         Property of type ``ctypes.c_int``
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_verbose
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__get_verbose
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
     @verbose.setter
     def verbose(self,value):
         """
-        Setter function for interp_krige_optim<std::vector<double>>::verbose .
+        Setter function for interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>::verbose .
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set_verbose
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__set_verbose
         func.argtypes=[ctypes.c_void_p,ctypes.c_int]
         func(self._ptr,value)
         return
 
     @property
     def mode(self):
         """
         Property of type ``ctypes.c_size_t``
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_mode
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__get_mode
         func.restype=ctypes.c_size_t
         func.argtypes=[ctypes.c_void_p]
         return func(self._ptr)
 
     @mode.setter
     def mode(self,value):
         """
-        Setter function for interp_krige_optim<std::vector<double>>::mode .
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set_mode
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
-        func(self._ptr,value)
-        return
-
-    @property
-    def nlen(self):
-        """
-        Property of type ``ctypes.c_size_t``
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_nlen
-        func.restype=ctypes.c_size_t
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @nlen.setter
-    def nlen(self,value):
+        Setter function for interp_krige_optim<std::vector<double>,std::vector<double>,covar_funct_rbf_noise>::mode .
         """
-        Setter function for interp_krige_optim<std::vector<double>>::nlen .
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set_nlen
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__set_mode
         func.argtypes=[ctypes.c_void_p,ctypes.c_size_t]
         func(self._ptr,value)
         return
 
-    @property
-    def full_min(self):
-        """
-        Property of type ``ctypes.c_bool``
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__get_full_min
-        func.restype=ctypes.c_bool
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @full_min.setter
-    def full_min(self,value):
-        """
-        Setter function for interp_krige_optim<std::vector<double>>::full_min .
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set_full_min
-        func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
-        func(self._ptr,value)
-        return
-
-    def set_noise(self,size,x,y,noise_var,rescale=False,err_on_fail=True):
-        """
-        | Parameters:
-        | *size*: ``size_t``
-        | *x*: :class:`std_vector` object
-        | *y*: :class:`std_vector` object
-        | *noise_var*: ``double``
-        | *rescale* =false: ``bool``
-        | *err_on_fail* =true: ``bool``
-        | Returns: a Python int
-        """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set_noise
-        func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double,ctypes.c_bool,ctypes.c_bool]
-        ret=func(self._ptr,size,x._ptr,y._ptr,noise_var,rescale,err_on_fail)
-        return ret
-
-    def set(self,size,x,y,rescale,err_on_fail=True):
+    def set(self,size,x,y):
         """
         | Parameters:
         | *size*: ``size_t``
         | *x*: :class:`std_vector` object
         | *y*: :class:`std_vector` object
-        | *rescale*: ``bool``
-        | *err_on_fail* =true: ``bool``
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__set
-        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_bool,ctypes.c_bool]
-        func(self._ptr,size,x._ptr,y._ptr,rescale,err_on_fail)
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__set
+        func.argtypes=[ctypes.c_void_p,ctypes.c_size_t,ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,size,x._ptr,y._ptr)
         return
 
     def eval(self,x0):
         """
         | Parameters:
         | *x0*: ``double``
         | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__eval
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__eval
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,x0)
         return ret
 
     def deriv(self,x0):
         """
         | Parameters:
         | *x0*: ``double``
         | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__deriv
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__deriv
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,x0)
         return ret
 
     def deriv2(self,x0):
         """
         | Parameters:
         | *x0*: ``double``
         | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__deriv2
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__deriv2
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,x0)
         return ret
 
     def sigma(self,x0):
         """
         | Parameters:
         | *x0*: ``double``
         | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__sigma
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__sigma
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,x0)
         return ret
 
     def sample(self,x0):
         """
         | Parameters:
         | *x0*: ``double``
         | Returns: a Python float
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__sample
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__sample
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         ret=func(self._ptr,x0)
         return ret
 
     def sample_vec(self,x,y):
         """
         | Parameters:
         | *x*: :class:`std_vector` object
         | *y*: :class:`std_vector` object
         """
-        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double__sample_vec
+        func=self._link.o2scl.o2scl_interp_krige_optim_std_vector_double_std_vector_double_covar_funct_rbf_noise__sample_vec
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,x._ptr,y._ptr)
         return
 
 
 class terminal:
     """
-    Python interface for O\ :sub:`2`\ scl class ``terminal``,
+    Python interface for O₂scl class ``terminal``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/terminal.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -7750,15 +8063,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class terminal
         
-        Returns: a terminal object
+        Returns: terminal object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def is_redirected(self):
         """
@@ -7937,19 +8250,19 @@
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         strt=std_string(self._link,ret)
         strt._owner=True
         return strt.to_bytes()
 
-    def default_fg(self):
+    def default_fgbg(self):
         """
         | Returns: Python bytes object
         """
-        func=self._link.o2scl.o2scl_terminal_default_fg
+        func=self._link.o2scl.o2scl_terminal_default_fgbg
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         strt=std_string(self._link,ret)
         strt._owner=True
         return strt.to_bytes()
 
@@ -8086,22 +8399,18 @@
         strt=std_string(self._link,ret)
         strt._owner=True
         return strt.to_bytes()
 
 
 class gen_test_number:
     """
-    Python interface for O\ :sub:`2`\ scl class ``gen_test_number<double>``,
+    Python interface for O₂scl class ``gen_test_number<double>``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/gen_test_number<double>.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -8138,15 +8447,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class gen_test_number
         
-        Returns: a gen_test_number object
+        Returns: gen_test_number object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def reset(self):
         """
@@ -8175,22 +8484,18 @@
         func.argtypes=[ctypes.c_void_p]
         ret=func(self._ptr)
         return ret
 
 
 class funct_string:
     """
-    Python interface for O\ :sub:`2`\ scl class ``funct_string``,
+    Python interface for O₂scl class ``funct_string``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/funct_string.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -8228,15 +8533,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class funct_string
         
-        Returns: a funct_string object
+        Returns: funct_string object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def set_parm(self,name,val):
         """
@@ -8248,23 +8553,22 @@
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_funct_string_set_parm
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_double]
         ret=func(self._ptr,name_,val)
         return ret
 
-    def __getitem__(self,tup):
+    def __getitem__(self,x):
         """
         | Parameters:
         | *x*: ``double``
         """
         func=self._link.o2scl.o2scl_funct_string_getitem
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        m,n=tup
         ret=func(self._ptr,x)
         return ret
 
     @classmethod
     def init(cls,link,expr,var):
         """
         Constructor-like class method for funct_string .
@@ -8277,22 +8581,18 @@
         f.restype=ctypes.c_void_p
         f.argtypes=[ctypes.c_char_p,ctypes.c_char_p]
         return cls(link,f(expr_,var_))
 
 
 class comm_option_s:
     """
-    Python interface for O\ :sub:`2`\ scl class ``comm_option_s``,
+    Python interface for O₂scl class ``comm_option_s``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/comm_option_s.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -8329,15 +8629,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class comm_option_s
         
-        Returns: a comm_option_s object
+        Returns: comm_option_s object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def shrt(self):
@@ -8498,22 +8798,18 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_int]
         func(self._ptr,value)
         return
 
 
 class cmd_line_arg:
     """
-    Python interface for O\ :sub:`2`\ scl class ``cmd_line_arg``,
+    Python interface for O₂scl class ``cmd_line_arg``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/cmd_line_arg.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -8550,15 +8846,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class cmd_line_arg
         
-        Returns: a cmd_line_arg object
+        Returns: cmd_line_arg object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_arg(self):
         """
@@ -8639,22 +8935,18 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
 
 class cli:
     """
-    Python interface for O\ :sub:`2`\ scl class ``cli``,
+    Python interface for O₂scl class ``cli``,
     see
     https://neutronstars.utk.edu/code/o2scl/html/class/cli.html .
     
-    Note that python complex numbers are immutable, but this class is
-    not, so the real and imaginary parts can be changed with real_set()
-    and imag_set(). 
-                                 
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -8691,15 +8983,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class cli
         
-        Returns: a cli object
+        Returns: cli object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def sync_verbose(self):
@@ -8829,25 +9121,26 @@
         """
         func=self._link.o2scl.o2scl_cli_set_verbose
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_int]
         ret=func(self._ptr,v)
         return ret
 
-    def parse_for_aliases(self,sv,allow_undashed):
+    def parse_for_aliases(self,sv,allow_undashed,debug=False):
         """
         | Parameters:
         | *sv*: :class:`std_vector_string` object
         | *allow_undashed*: ``bool``
+        | *debug* =false: ``bool``
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_cli_parse_for_aliases
         func.restype=ctypes.c_int
-        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_bool]
-        ret=func(self._ptr,sv._ptr,allow_undashed)
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_bool,ctypes.c_bool]
+        ret=func(self._ptr,sv._ptr,allow_undashed,debug)
         return ret
 
     def apply_aliases(self,sv,istart,debug=False):
         """
         | Parameters:
         | *sv*: :class:`std_vector_string` object
         | *istart*: ``size_t``
@@ -8856,14 +9149,25 @@
         """
         func=self._link.o2scl.o2scl_cli_apply_aliases
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_size_t,ctypes.c_bool]
         ret=func(self._ptr,sv._ptr,istart,debug)
         return ret
 
+    def get_option_list(self):
+        """
+        | Returns: :class:`std_vector_string` object
+        """
+        func=self._link.o2scl.o2scl_cli_get_option_list
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        vstrt=std_vector_string(self._link,ret)
+        return vstrt
+
     def parameter_desc(self,name):
         """
         | Parameters:
         | *name*: string
         | Returns: Python bytes object
         """
         name_=ctypes.c_char_p(force_bytes(name))
@@ -8926,14 +9230,90 @@
         """
 
         f=self._link.o2scl.o2scl_free_shared_ptr_table_units_
         f.argtypes=[ctypes.c_void_p]
         f(self._s_ptr)
         return
 
+def rearrange_and_copy(link,t,spec,verbose=0,err_on_fail=True):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *t*: :class:`tensor<>` object
+        | *spec*: string
+        | *verbose*: ``int``
+        | *err_on_fail*: ``bool``
+        | Returns: ``tensor`` object
+    """
+    spec_=ctypes.c_char_p(force_bytes(spec))
+    func=link.o2scl.o2scl_rearrange_and_copy_tensor_double__wrapper
+    func.restype=ctypes.c_void_p
+    func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
+    ret=func(t._ptr,spec_,verbose,err_on_fail)
+    ten=tensor(link,ret)
+    ten._owner=True
+    return ten
+
+def rearrange_and_copy_int(link,t,spec,verbose=0,err_on_fail=True):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *t*: :class:`tensor<int>` object
+        | *spec*: string
+        | *verbose*: ``int``
+        | *err_on_fail*: ``bool``
+        | Returns: ``tensor_int`` object
+    """
+    spec_=ctypes.c_char_p(force_bytes(spec))
+    func=link.o2scl.o2scl_rearrange_and_copy_tensor_int_int__wrapper
+    func.restype=ctypes.c_void_p
+    func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
+    ret=func(t._ptr,spec_,verbose,err_on_fail)
+    ten=tensor(link,ret)
+    ten._owner=True
+    return ten
+
+def rearrange_and_copy_size_t(link,t,spec,verbose=0,err_on_fail=True):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *t*: :class:`tensor<size_t>` object
+        | *spec*: string
+        | *verbose*: ``int``
+        | *err_on_fail*: ``bool``
+        | Returns: ``tensor_size_t`` object
+    """
+    spec_=ctypes.c_char_p(force_bytes(spec))
+    func=link.o2scl.o2scl_rearrange_and_copy_tensor_size_t_size_t__wrapper
+    func.restype=ctypes.c_void_p
+    func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
+    ret=func(t._ptr,spec_,verbose,err_on_fail)
+    ten=tensor(link,ret)
+    ten._owner=True
+    return ten
+
+def grid_rearrange_and_copy(link,t,spec,verbose=0,err_on_fail=True):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *t*: :class:`tensor_grid<>` object
+        | *spec*: string
+        | *verbose*: ``int``
+        | *err_on_fail*: ``bool``
+        | Returns: ``tensor_grid`` object
+    """
+    spec_=ctypes.c_char_p(force_bytes(spec))
+    func=link.o2scl.o2scl_grid_rearrange_and_copy_tensor_grid_double__wrapper
+    func.restype=ctypes.c_void_p
+    func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_int,ctypes.c_bool]
+    ret=func(t._ptr,spec_,verbose,err_on_fail)
+    ten=tensor_grid(link,ret)
+    ten._owner=True
+    return ten
+
 def fermi_function(link,E,mu,T,limit=40.0):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *E*: ``double``
         | *mu*: ``double``
         | *T*: ``double``
@@ -9060,19 +9440,17 @@
 
 def wordexp_single_file(link,fname):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *fname*: :class:`std::string` object
     """
-    fname.__del__()
-    fname._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_wordexp_single_file_wrapper
-    func.argtypes=[ctypes.POINTER(ctypes.c_void_p)]
-    func(ctypes.byref(fname._ptr))
+    func.argtypes=[ctypes.c_void_p]
+    func(fname._ptr)
     fname._owner=True
     return
 
 def wordexp_wrapper(link,word,matches):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -9081,31 +9459,92 @@
     """
     word_=ctypes.c_char_p(force_bytes(word))
     func=link.o2scl.o2scl_wordexp_wrapper_wrapper
     func.argtypes=[ctypes.c_char_p,ctypes.c_void_p]
     func(word_,matches._ptr)
     return
 
+def function_to_double(link,s,verbose=0):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *s*: string
+        | *verbose*: ``int``
+        | Returns: ``ctypes.c_double`` object
+    """
+    s_=ctypes.c_char_p(force_bytes(s))
+    func=link.o2scl.o2scl_function_to_double_wrapper
+    func.restype=ctypes.c_double
+    func.argtypes=[ctypes.c_char_p,ctypes.c_int]
+    ret=func(s_,verbose)
+    return ret
+
+def function_to_double_nothrow(link,s,result,verbose=0):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *s*: string
+        | *result*: ``double``
+        | *verbose*: ``int``
+        | Returns: ``ctypes.c_int`` object
+    """
+    s_=ctypes.c_char_p(force_bytes(s))
+    func=link.o2scl.o2scl_function_to_double_nothrow_wrapper
+    func.restype=ctypes.c_int
+    func.argtypes=[ctypes.c_char_p,ctypes.c_void_p,ctypes.c_int]
+    ret=func(s_,result._ptr,verbose)
+    return ret
+
+def find_constant(link,name,unit):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *name*: string
+        | *unit*: string
+        | Returns: ``ctypes.c_double`` object
+    """
+    name_=ctypes.c_char_p(force_bytes(name))
+    unit_=ctypes.c_char_p(force_bytes(unit))
+    func=link.o2scl.o2scl_find_constant_wrapper
+    func.restype=ctypes.c_double
+    func.argtypes=[ctypes.c_char_p,ctypes.c_char_p]
+    ret=func(name_,unit_)
+    return ret
+
 def string_to_uint_list(link,x,list):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *x*: :class:`std::string` object
         | *list*: :class:`vector<size_t>` object
         | Returns: ``ctypes.c_int`` object
     """
-    x.__del__()
-    x._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_string_to_uint_list_vector_size_t__wrapper
     func.restype=ctypes.c_int
-    func.argtypes=[ctypes.POINTER(ctypes.c_void_p),ctypes.c_void_p]
-    ret=func(ctypes.byref(x._ptr),list._ptr)
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+    ret=func(x._ptr,list._ptr)
     x._owner=True
     return ret
 
+def rewrap_keep_endlines(link,str,sv,ncol=79,verbose=0,ignore_vt100=True):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *str*: string
+        | *sv*: :class:`std::vector<std::string>` object
+        | *ncol*: ``size_t``
+        | *verbose*: ``int``
+        | *ignore_vt100*: ``bool``
+    """
+    str_=ctypes.c_char_p(force_bytes(str))
+    func=link.o2scl.o2scl_rewrap_keep_endlines_wrapper
+    func.argtypes=[ctypes.c_char_p,ctypes.c_void_p,ctypes.c_size_t,ctypes.c_int,ctypes.c_bool]
+    func(str_,sv._ptr,ncol,verbose,ignore_vt100)
+    return
+
 def vector_level_count(link,level,n,x,y):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *level*: ``double``
         | *n*: ``size_t``
         | *x*: :class:`std::vector<double>` object
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/cap_cout.py` & `o2sclpy-0.928/o2sclpy/cap_cout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/eos.py` & `o2sclpy-0.928/o2sclpy/eos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2022, Andrew W. Steiner
+  Copyright (C) 2020-2023, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -14,29 +14,29 @@
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with O2scl. If not, see <http://www.gnu.org/licenses/>.
 
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 """
 
 import ctypes
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 
 from o2sclpy.base import *
 from o2sclpy.part import *
 
 class eos_base:
     """
-    Python interface for O\ :sub:`2`\ scl class eos_base.
+    Python interface for O2scl class eos_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_base.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -73,15 +73,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_base
         
-        Returns: a eos_base object
+        Returns: eos_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_def_thermo(self):
         """
@@ -102,17 +102,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
 
 class eos_had_base(eos_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_base.
+    Python interface for O2scl class eos_had_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_base
 
@@ -146,15 +146,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_base
         
-        Returns: a eos_had_base object
+        Returns: eos_had_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def eoa(self):
@@ -767,17 +767,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,nb,delta)
         return ret
 
 
 class eos_had_eden_base(eos_had_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_eden_base.
+    Python interface for O2scl class eos_had_eden_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_eden_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_eden_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_eden_base
 
@@ -811,26 +811,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_eden_base
         
-        Returns: a eos_had_eden_base object
+        Returns: eos_had_eden_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_pres_base(eos_had_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_pres_base.
+    Python interface for O2scl class eos_had_pres_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_pres_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_pres_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_pres_base
 
@@ -864,26 +864,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_pres_base
         
-        Returns: a eos_had_pres_base object
+        Returns: eos_had_pres_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_temp_base(eos_had_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_temp_base.
+    Python interface for O2scl class eos_had_temp_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_temp_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_base
 
@@ -917,15 +917,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_temp_base
         
-        Returns: a eos_had_temp_base object
+        Returns: eos_had_temp_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_temp_e(self,n,p,T,th):
         """
@@ -956,17 +956,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double,ctypes.c_void_p]
         ret=func(self._ptr,n._ptr,p._ptr,T,th._ptr)
         return ret
 
 
 class eos_had_temp_eden_base(eos_had_temp_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_temp_eden_base.
+    Python interface for O2scl class eos_had_temp_eden_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_temp_eden_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_eden_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_eden_base
 
@@ -1000,26 +1000,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_temp_eden_base
         
-        Returns: a eos_had_temp_eden_base object
+        Returns: eos_had_temp_eden_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_temp_pres_base(eos_had_temp_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_temp_pres_base.
+    Python interface for O2scl class eos_had_temp_pres_base.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_temp_pres_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_temp_pres_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_temp_pres_base
 
@@ -1053,26 +1053,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_temp_pres_base
         
-        Returns: a eos_had_temp_pres_base object
+        Returns: eos_had_temp_pres_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_had_skyrme(eos_had_temp_eden_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_skyrme.
+    Python interface for O2scl class eos_had_skyrme.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_skyrme.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_skyrme.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_skyrme
 
         | Parameters:
@@ -1105,15 +1105,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_skyrme
         
-        Returns: a eos_had_skyrme object
+        Returns: eos_had_skyrme object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def t0(self):
@@ -1454,17 +1454,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
 
 class eos_had_apr(eos_had_temp_eden_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_apr.
+    Python interface for O2scl class eos_had_apr.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_apr.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_apr.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_apr
 
         | Parameters:
@@ -1497,15 +1497,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_apr
         
-        Returns: a eos_had_apr object
+        Returns: eos_had_apr object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def pion(self):
@@ -1546,17 +1546,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
         func(self._ptr,value)
         return
 
 
 class eos_had_rmf(eos_had_temp_pres_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_had_rmf.
+    Python interface for O2scl class eos_had_rmf.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_had_rmf.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_had_rmf.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_had_rmf
 
         | Parameters:
@@ -1589,15 +1589,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_had_rmf
         
-        Returns: a eos_had_rmf object
+        Returns: eos_had_rmf object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def calc_e_steps(self):
@@ -2109,17 +2109,17 @@
         rho_conv=ctypes.c_double(rho)
         ret=func(self._ptr,ctypes.byref(sig_conv),ctypes.byref(ome_conv),ctypes.byref(rho_conv))
         return ret,sig_conv.value,ome_conv.value,rho_conv.value
 
 
 class eos_quark(eos_base):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_quark.
+    Python interface for O2scl class eos_quark.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_quark.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark
 
         | Parameters:
@@ -2152,26 +2152,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_quark
         
-        Returns: a eos_quark object
+        Returns: eos_quark object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class eos_quark_bag(eos_quark):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_quark_bag.
+    Python interface for O2scl class eos_quark_bag.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_quark_bag.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark_bag.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark_bag
 
         | Parameters:
@@ -2204,15 +2204,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_quark_bag
         
-        Returns: a eos_quark_bag object
+        Returns: eos_quark_bag object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def bag_constant(self):
@@ -2233,17 +2233,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class eos_quark_njl(eos_quark):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_quark_njl.
+    Python interface for O2scl class eos_quark_njl.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_quark_njl.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_quark_njl.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_quark_njl
 
         | Parameters:
@@ -2276,15 +2276,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_quark_njl
         
-        Returns: a eos_quark_njl object
+        Returns: eos_quark_njl object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def B0(self):
@@ -2405,17 +2405,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
         func(self._ptr,value)
         return
 
 
 class eos_tov:
     """
-    Python interface for O\ :sub:`2`\ scl class eos_tov.
+    Python interface for O2scl class eos_tov.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_tov.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -2453,15 +2453,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_tov
         
-        Returns: a eos_tov object
+        Returns: eos_tov object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def verbose(self):
@@ -2577,17 +2577,17 @@
         nb_conv=ctypes.c_double(0)
         func(self._ptr,pr,ctypes.byref(ed_conv),ctypes.byref(nb_conv))
         return ed_conv.value,nb_conv.value
 
 
 class eos_tov_buchdahl(eos_tov):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_tov_buchdahl.
+    Python interface for O2scl class eos_tov_buchdahl.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_tov_buchdahl.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_buchdahl.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_buchdahl
 
         | Parameters:
@@ -2620,15 +2620,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_tov_buchdahl
         
-        Returns: a eos_tov_buchdahl object
+        Returns: eos_tov_buchdahl object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def Pstar(self):
@@ -2744,17 +2744,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,r,beta)
         return ret
 
 
 class eos_tov_polytrope(eos_tov):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_tov_polytrope.
+    Python interface for O2scl class eos_tov_polytrope.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_tov_polytrope.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_polytrope.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_polytrope
 
         | Parameters:
@@ -2787,15 +2787,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_tov_polytrope
         
-        Returns: a eos_tov_polytrope object
+        Returns: eos_tov_polytrope object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def set_coeff_index(self,coeff,index):
         """
@@ -2807,17 +2807,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         func(self._ptr,coeff,index)
         return
 
 
 class eos_tov_linear(eos_tov):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_tov_linear.
+    Python interface for O2scl class eos_tov_linear.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_tov_linear.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_linear.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_linear
 
         | Parameters:
@@ -2850,15 +2850,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_tov_linear
         
-        Returns: a eos_tov_linear object
+        Returns: eos_tov_linear object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def set_cs2_eps0(self,cs2,eps0):
         """
@@ -2870,17 +2870,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         func(self._ptr,cs2,eps0)
         return
 
 
 class eos_tov_interp(eos_tov):
     """
-    Python interface for O\ :sub:`2`\ scl class eos_tov_interp.
+    Python interface for O2scl class eos_tov_interp.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/eos_tov_interp.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/eos_tov_interp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class eos_tov_interp
 
         | Parameters:
@@ -2913,15 +2913,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class eos_tov_interp
         
-        Returns: a eos_tov_interp object
+        Returns: eos_tov_interp object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def err_nonconv(self):
@@ -2939,14 +2939,74 @@
         Setter function for eos_tov_interp::err_nonconv .
         """
         func=self._link.o2scl.o2scl_eos_tov_interp_set_err_nonconv
         func.argtypes=[ctypes.c_void_p,ctypes.c_bool]
         func(self._ptr,value)
         return
 
+    def get_full_vece(self):
+        """
+        Get object of type :class:`std::vector<double>`
+        """
+        func1=self._link.o2scl.o2scl_eos_tov_interp_get_full_vece
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector(self._link,ptr)
+        return obj
+
+    def set_full_vece(self,value):
+        """
+        Set object of type :class:`std::vector<double>`
+        """
+        func=self._link.o2scl.o2scl_eos_tov_interp_set_full_vece
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_full_vecp(self):
+        """
+        Get object of type :class:`std::vector<double>`
+        """
+        func1=self._link.o2scl.o2scl_eos_tov_interp_get_full_vecp
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector(self._link,ptr)
+        return obj
+
+    def set_full_vecp(self,value):
+        """
+        Set object of type :class:`std::vector<double>`
+        """
+        func=self._link.o2scl.o2scl_eos_tov_interp_set_full_vecp
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_full_vecnb(self):
+        """
+        Get object of type :class:`std::vector<double>`
+        """
+        func1=self._link.o2scl.o2scl_eos_tov_interp_get_full_vecnb
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector(self._link,ptr)
+        return obj
+
+    def set_full_vecnb(self,value):
+        """
+        Set object of type :class:`std::vector<double>`
+        """
+        func=self._link.o2scl.o2scl_eos_tov_interp_set_full_vecnb
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
     def read_table(self,eos,s_cole,s_colp,s_colnb=""):
         """
         | Parameters:
         | *eos*: :class:`table_units<>` object
         | *s_cole*: string
         | *s_colp*: string
         | *s_colnb* ="": string
@@ -3033,17 +3093,17 @@
         func.argtypes=[ctypes.c_void_p]
         func(self._ptr)
         return
 
 
 class tov_solve:
     """
-    Python interface for O\ :sub:`2`\ scl class tov_solve.
+    Python interface for O2scl class tov_solve.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/tov_solve.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/tov_solve.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3080,15 +3140,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class tov_solve
         
-        Returns: a tov_solve object
+        Returns: tov_solve object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def buffer_size(self):
@@ -3699,14 +3759,27 @@
         """
         func=self._link.o2scl.o2scl_tov_solve_fixed
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
         ret=func(self._ptr,mass,pmax)
         return ret
 
+    def fixed_pr(self,pcent,pmax=1.0e20):
+        """
+        | Parameters:
+        | *pcent*: ``double``
+        | *pmax* =1.0e20: ``double``
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_tov_solve_fixed_pr
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p,ctypes.c_double,ctypes.c_double]
+        ret=func(self._ptr,pcent,pmax)
+        return ret
+
     def max(self):
         """
         | Returns: a Python int
         """
         func=self._link.o2scl.o2scl_tov_solve_max
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p]
@@ -3722,17 +3795,17 @@
         func.argtypes=[ctypes.c_void_p]
         sp=shared_ptr_table_units(self._link,func(self._ptr))
         return sp
 
 
 class tov_love:
     """
-    Python interface for O\ :sub:`2`\ scl class tov_love.
+    Python interface for O2scl class tov_love.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/tov_love.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/tov_love.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -3769,15 +3842,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class tov_love
         
-        Returns: a tov_love object
+        Returns: tov_love object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def show_ode(self):
@@ -3968,17 +4041,17 @@
         lambda_cgs_conv=ctypes.c_double(0)
         ret=func(self._ptr,ctypes.byref(yR_conv),ctypes.byref(beta_conv),ctypes.byref(k2_conv),ctypes.byref(lambda_km5_conv),ctypes.byref(lambda_cgs_conv))
         return ret,yR_conv.value,beta_conv.value,k2_conv.value,lambda_km5_conv.value,lambda_cgs_conv.value
 
 
 class nstar_cold:
     """
-    Python interface for O\ :sub:`2`\ scl class nstar_cold.
+    Python interface for O2scl class nstar_cold.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/nstar_cold.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nstar_cold.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -4015,15 +4088,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nstar_cold
         
-        Returns: a nstar_cold object
+        Returns: nstar_cold object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def pressure_dec_nb(self):
@@ -4141,14 +4214,25 @@
         Setter function for nstar_cold::acausal_pr .
         """
         func=self._link.o2scl.o2scl_nstar_cold_set_acausal_pr
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
+    def get_def_tov(self):
+        """
+        Get object of type :class:`tov_solve`
+        """
+        func1=self._link.o2scl.o2scl_nstar_cold_get_def_tov
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=tov_solve(self._link,ptr)
+        return obj
+
     @property
     def eos_neg(self):
         """
         Property of type ``ctypes.c_bool``
         """
         func=self._link.o2scl.o2scl_nstar_cold_get_eos_neg
         func.restype=ctypes.c_bool
@@ -4388,17 +4472,17 @@
         func.argtypes=[ctypes.c_void_p]
         sp=shared_ptr_table_units(self._link,func(self._ptr))
         return sp
 
 
 class nucleus_rmf:
     """
-    Python interface for O\ :sub:`2`\ scl class nucleus_rmf.
+    Python interface for O2scl class nucleus_rmf.
     See
-    https://neutronstars.utk.edu/code/o2scl/eos/html/class/nucleus_rmf.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucleus_rmf.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -4435,15 +4519,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucleus_rmf
         
-        Returns: a nucleus_rmf object
+        Returns: nucleus_rmf object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def stens(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/hdf.py` & `o2sclpy-0.928/o2sclpy/hdf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2022, Andrew W. Steiner
+  Copyright (C) 2020-2023, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -14,26 +14,27 @@
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with O2scl. If not, see <http://www.gnu.org/licenses/>.
 
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 """
 
 import ctypes
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 
 from o2sclpy.base import *
+from o2sclpy.other import *
 
 class hdf_file:
     """
-    Python interface for O\ :sub:`2`\ scl class ``hdf_file``,
+    Python interface for O2scl class ``hdf_file``,
     See
     https://neutronstars.utk.edu/code/o2scl/html/class/hdf_file.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
@@ -72,15 +73,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class hdf_file
         
-        Returns: a hdf_file object
+        Returns: hdf_file object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def compr_type(self):
@@ -394,23 +395,23 @@
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_get_szt_vec
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,v._ptr)
         return ret
 
-    def gets_vec(self,name,s):
+    def gets_vec_copy(self,name,s):
         """
         | Parameters:
         | *name*: string
         | *s*: :class:`std_vector_string` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
-        func=self._link.o2scl.o2scl_hdf_hdf_file_gets_vec
+        func=self._link.o2scl.o2scl_hdf_hdf_file_gets_vec_copy
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,s._ptr)
         return ret
 
     def setd_vec(self,name,v):
         """
@@ -450,23 +451,23 @@
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_set_szt_vec
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,v._ptr)
         return ret
 
-    def sets_vec(self,name,s):
+    def sets_vec_copy(self,name,s):
         """
         | Parameters:
         | *name*: string
         | *s*: :class:`std_vector_string` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
-        func=self._link.o2scl.o2scl_hdf_hdf_file_sets_vec
+        func=self._link.o2scl.o2scl_hdf_hdf_file_sets_vec_copy
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,s._ptr)
         return ret
 
     def getd_mat_copy(self,name,m):
         """
@@ -538,29 +539,29 @@
         ret=func(self._ptr,name_,t._ptr)
         return ret
 
     def geti_ten(self,name,t):
         """
         | Parameters:
         | *name*: string
-        | *t*: :class:`tensor<int>` object
+        | *t*: :class:`tensor_int` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_geti_ten
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,t._ptr)
         return ret
 
     def get_szt_ten(self,name,t):
         """
         | Parameters:
         | *name*: string
-        | *t*: :class:`tensor<size_t>` object
+        | *t*: :class:`tensor_size_t` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_get_szt_ten
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,t._ptr)
@@ -580,29 +581,29 @@
         ret=func(self._ptr,name_,t._ptr)
         return ret
 
     def seti_ten(self,name,t):
         """
         | Parameters:
         | *name*: string
-        | *t*: :class:`tensor<int>` object
+        | *t*: :class:`tensor_int` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_seti_ten
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,t._ptr)
         return ret
 
     def set_szt_ten(self,name,t):
         """
         | Parameters:
         | *name*: string
-        | *t*: :class:`tensor<size_t>` object
+        | *t*: :class:`tensor_size_t` object
         | Returns: a Python int
         """
         name_=ctypes.c_char_p(force_bytes(name))
         func=self._link.o2scl.o2scl_hdf_hdf_file_set_szt_ten
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_void_p]
         ret=func(self._ptr,name_,t._ptr)
@@ -756,15 +757,15 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_int,ctypes.c_void_p]
         func(self._ptr,verbose,hf2._ptr)
         return
 
 
 class acol_manager:
     """
-    Python interface for O\ :sub:`2`\ scl class ``acol_manager``,
+    Python interface for O2scl class ``acol_manager``,
     See
     https://neutronstars.utk.edu/code/o2scl/html/class/acol_manager.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
@@ -803,15 +804,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class acol_manager
         
-        Returns: a acol_manager object
+        Returns: acol_manager object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def get_env_var_name(self):
         """
@@ -869,14 +870,34 @@
         Setter function for acol_manager::verbose .
         """
         func=self._link.o2scl.o2scl_hdf_acol_manager_set_verbose
         func.argtypes=[ctypes.c_void_p,ctypes.c_int]
         func(self._ptr,value)
         return
 
+    def get_def_args(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_def_args
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_def_args(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_def_args
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
     def get_type(self):
         """
         Get object of type :class:`std::string`
         """
         func=self._link.o2scl.o2scl_hdf_acol_manager_get_type
         func.restype=ctypes.c_void_p
         func.argtypes=[ctypes.c_void_p]
@@ -1069,18 +1090,525 @@
         Set object of type :class:`std::string`
         """
         func=self._link.o2scl.o2scl_hdf_acol_manager_set_string_obj
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
         func(self._ptr,value._ptr)
         return
 
+    def get_cont_obj(self):
+        """
+        Get object of type :class:`std::vector<contour_line>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_cont_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=vector_contour_line(self._link,ptr)
+        return obj
+
+    def set_cont_obj(self,value):
+        """
+        Set object of type :class:`std::vector<contour_line>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_cont_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_ug_obj(self):
+        """
+        Get object of type :class:`uniform_grid<double>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_ug_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=uniform_grid<double>(self._link,ptr)
+        return obj
+
+    def set_ug_obj(self,value):
+        """
+        Set object of type :class:`uniform_grid<double>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_ug_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_intv_obj(self):
+        """
+        Get object of type :class:`std::vector<int>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_intv_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector_int(self._link,ptr)
+        return obj
+
+    def set_intv_obj(self,value):
+        """
+        Set object of type :class:`std::vector<int>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_intv_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_doublev_obj(self):
+        """
+        Get object of type :class:`std::vector<double>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_doublev_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector(self._link,ptr)
+        return obj
+
+    def set_doublev_obj(self,value):
+        """
+        Set object of type :class:`std::vector<double>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_doublev_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_size_tv_obj(self):
+        """
+        Get object of type :class:`std::vector<size_t>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_size_tv_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector_size_t(self._link,ptr)
+        return obj
+
+    def set_size_tv_obj(self,value):
+        """
+        Set object of type :class:`std::vector<size_t>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_size_tv_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_stringv_obj(self):
+        """
+        Get object of type :class:`std::vector<std::string>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_stringv_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector_string(self._link,ptr)
+        return obj
+
+    def set_stringv_obj(self,value):
+        """
+        Set object of type :class:`std::vector<std::string>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_stringv_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_vvstring_obj(self):
+        """
+        Get object of type :class:`std::vector<std::vector<std::string>>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_vvstring_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=vec_vec_string(self._link,ptr)
+        return obj
+
+    def set_vvstring_obj(self,value):
+        """
+        Set object of type :class:`std::vector<std::vector<std::string>>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_vvstring_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_vvdouble_obj(self):
+        """
+        Get object of type :class:`std::vector<std::vector<double>>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_vvdouble_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=std_vector_vector(self._link,ptr)
+        return obj
+
+    def set_vvdouble_obj(self,value):
+        """
+        Set object of type :class:`std::vector<std::vector<double>>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_vvdouble_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_tensor_obj(self):
+        """
+        Get object of type :class:`tensor<>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_tensor_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=tensor(self._link,ptr)
+        return obj
+
+    def set_tensor_obj(self,value):
+        """
+        Set object of type :class:`tensor<>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_tensor_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_tensor_int_obj(self):
+        """
+        Get object of type :class:`tensor<int>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_tensor_int_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=tensor_int(self._link,ptr)
+        return obj
+
+    def set_tensor_int_obj(self,value):
+        """
+        Set object of type :class:`tensor<int>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_tensor_int_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_tensor_size_t_obj(self):
+        """
+        Get object of type :class:`tensor<size_t>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_tensor_size_t_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=tensor_size_t(self._link,ptr)
+        return obj
+
+    def set_tensor_size_t_obj(self,value):
+        """
+        Set object of type :class:`tensor<size_t>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_tensor_size_t_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_tensor_grid_obj(self):
+        """
+        Get object of type :class:`tensor_grid<>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_tensor_grid_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=tensor_grid(self._link,ptr)
+        return obj
+
+    def set_tensor_grid_obj(self,value):
+        """
+        Set object of type :class:`tensor_grid<>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_tensor_grid_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_pdma_obj(self):
+        """
+        Get object of type :class:`prob_dens_mdim_amr<>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_pdma_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=prob_dens_mdim_amr(self._link,ptr)
+        return obj
+
+    def set_pdma_obj(self,value):
+        """
+        Set object of type :class:`prob_dens_mdim_amr<>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_pdma_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_pdmg_obj(self):
+        """
+        Get object of type :class:`prob_dens_mdim_gaussian<>`
+        """
+        func1=self._link.o2scl.o2scl_hdf_acol_manager_get_pdmg_obj
+        func1.restype=ctypes.c_void_p
+        func1.argtypes=[ctypes.c_void_p]
+        ptr=func1(self._ptr)
+        obj=prob_dens_mdim_gaussian(self._link,ptr)
+        return obj
+
+    def set_pdmg_obj(self,value):
+        """
+        Set object of type :class:`prob_dens_mdim_gaussian<>`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_pdmg_obj
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_command_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_command_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_command_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_command_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_type_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_type_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_type_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_type_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_param_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_param_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_param_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_param_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_help_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_help_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_help_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_help_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_exec_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_exec_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_exec_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_exec_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_url_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_url_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_url_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_url_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_default_color(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_default_color
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_default_color(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_default_color
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def get_color_spec(self):
+        """
+        Get object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_get_color_spec
+        func.restype=ctypes.c_void_p
+        func.argtypes=[ctypes.c_void_p]
+        s=std_string(self._link)
+        s._ptr=func(self._ptr)
+        return s.to_bytes()
+
+    def set_color_spec(self,value):
+        """
+        Set object of type :class:`std::string`
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_set_color_spec
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,value._ptr)
+        return
+
+    def help_found(self,arg1,arg2):
+        """
+        | Parameters:
+        | *arg1*: string
+        | *arg2*: string
+        | Returns: a Python boolean
+        """
+        arg1_=ctypes.c_char_p(force_bytes(arg1))
+        arg2_=ctypes.c_char_p(force_bytes(arg2))
+        func=self._link.o2scl.o2scl_hdf_acol_manager_help_found
+        func.restype=ctypes.c_bool
+        func.argtypes=[ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p]
+        ret=func(self._ptr,arg1_,arg2_)
+        return ret
+
+    def run_empty(self):
+        """
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_run_empty
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def validate_interp_type(self):
+        """
+        | Returns: a Python int
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_validate_interp_type
+        func.restype=ctypes.c_int
+        func.argtypes=[ctypes.c_void_p]
+        ret=func(self._ptr)
+        return ret
+
+    def parse_vec_string(self,args):
+        """
+        | Parameters:
+        | *args*: :class:`std_vector_string` object
+        """
+        func=self._link.o2scl.o2scl_hdf_acol_manager_parse_vec_string
+        func.argtypes=[ctypes.c_void_p,ctypes.c_void_p]
+        func(self._ptr,args._ptr)
+        return
+
+    def command_add(self,new_type):
+        """
+        | Parameters:
+        | *new_type*: string
+        """
+        new_type_=ctypes.c_char_p(force_bytes(new_type))
+        func=self._link.o2scl.o2scl_hdf_acol_manager_command_add
+        func.argtypes=[ctypes.c_void_p,ctypes.c_char_p]
+        func(self._ptr,new_type_)
+        return
+
+    def command_del(self,ltype):
+        """
+        | Parameters:
+        | *ltype*: string
+        """
+        ltype_=ctypes.c_char_p(force_bytes(ltype))
+        func=self._link.o2scl.o2scl_hdf_acol_manager_command_del
+        func.argtypes=[ctypes.c_void_p,ctypes.c_char_p]
+        func(self._ptr,ltype_)
+        return
+
 
 class cloud_file:
     """
-    Python interface for O\ :sub:`2`\ scl class ``cloud_file``,
+    Python interface for O2scl class ``cloud_file``,
     See
     https://neutronstars.utk.edu/code/o2scl/html/class/cloud_file.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
@@ -1119,15 +1647,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class cloud_file
         
-        Returns: a cloud_file object
+        Returns: cloud_file object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def hash_type(self):
@@ -1300,15 +1828,15 @@
         func=self._link.o2scl.o2scl_hdf_cloud_file_hdf5_open_hash
         func.restype=ctypes.c_int
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p,ctypes.c_char_p]
         ret=func(self._ptr,hf._ptr,file_,url_,hash_,dir_)
         return ret
 
 
-def hdf_input_table(link,hf,t,name):
+def hdf_input_table(link,hf,t,name=""):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table<>` object
         | *name*: string
     """
@@ -1322,19 +1850,17 @@
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table<>` object
         | *name*: :class:`std::string` object
     """
-    name.__del__()
-    name._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_hdf_hdf_input_n_table_wrapper
-    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_void_p)]
-    func(hf._ptr,t._ptr,ctypes.byref(name._ptr))
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,t._ptr,name._ptr)
     name._owner=True
     return
 
 def hdf_output_table(link,hf,t,name):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -1344,15 +1870,15 @@
     """
     name_=ctypes.c_char_p(force_bytes(name))
     func=link.o2scl.o2scl_hdf_hdf_output_table_wrapper
     func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
     func(hf._ptr,t._ptr,name_)
     return
 
-def hdf_input_table_units(link,hf,t,name):
+def hdf_input_table_units(link,hf,t,name=""):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table_units<>` object
         | *name*: string
     """
@@ -1366,19 +1892,17 @@
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table_units<>` object
         | *name*: :class:`std::string` object
     """
-    name.__del__()
-    name._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_hdf_hdf_input_n_table_units_wrapper
-    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_void_p)]
-    func(hf._ptr,t._ptr,ctypes.byref(name._ptr))
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,t._ptr,name._ptr)
     name._owner=True
     return
 
 def hdf_output_table_units(link,hf,t,name):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -1388,15 +1912,15 @@
     """
     name_=ctypes.c_char_p(force_bytes(name))
     func=link.o2scl.o2scl_hdf_hdf_output_table_units_wrapper
     func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
     func(hf._ptr,t._ptr,name_)
     return
 
-def hdf_input_table3d(link,hf,t,name):
+def hdf_input_table3d(link,hf,t,name=""):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table3d` object
         | *name*: string
     """
@@ -1410,19 +1934,17 @@
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`table3d` object
         | *name*: :class:`std::string` object
     """
-    name.__del__()
-    name._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_hdf_hdf_input_n_table3d_wrapper
-    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_void_p)]
-    func(hf._ptr,t._ptr,ctypes.byref(name._ptr))
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,t._ptr,name._ptr)
     name._owner=True
     return
 
 def hdf_output_table3d(link,hf,t,name):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -1432,15 +1954,15 @@
     """
     name_=ctypes.c_char_p(force_bytes(name))
     func=link.o2scl.o2scl_hdf_hdf_output_table3d_wrapper
     func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
     func(hf._ptr,t._ptr,name_)
     return
 
-def hdf_input_uniform_grid(link,hf,t,name):
+def hdf_input_uniform_grid(link,hf,t,name=""):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`uniform_grid<>` object
         | *name*: string
     """
@@ -1454,19 +1976,17 @@
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`uniform_grid<>` object
         | *name*: :class:`std::string` object
     """
-    name.__del__()
-    name._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_hdf_hdf_input_n_uniform_grid_wrapper
-    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_void_p)]
-    func(hf._ptr,t._ptr,ctypes.byref(name._ptr))
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,t._ptr,name._ptr)
     name._owner=True
     return
 
 def hdf_output_uniform_grid(link,hf,t,name):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -1476,15 +1996,15 @@
     """
     name_=ctypes.c_char_p(force_bytes(name))
     func=link.o2scl.o2scl_hdf_hdf_output_uniform_grid_wrapper
     func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
     func(hf._ptr,t._ptr,name_)
     return
 
-def hdf_input_tensor_grid(link,hf,t,name):
+def hdf_input_tensor_grid(link,hf,t,name=""):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`tensor_grid<>` object
         | *name*: string
     """
@@ -1498,19 +2018,17 @@
     """
         | Parameters:
         | *link* :class:`linker` object
         | *hf*: :class:`hdf_file` object
         | *t*: :class:`tensor_grid<>` object
         | *name*: :class:`std::string` object
     """
-    name.__del__()
-    name._ptr=ctypes.c_void_p()
     func=link.o2scl.o2scl_hdf_hdf_input_n_tensor_grid_wrapper
-    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.POINTER(ctypes.c_void_p)]
-    func(hf._ptr,t._ptr,ctypes.byref(name._ptr))
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,t._ptr,name._ptr)
     name._owner=True
     return
 
 def hdf_output_tensor_grid(link,hf,t,name):
     """
         | Parameters:
         | *link* :class:`linker` object
@@ -1520,14 +2038,56 @@
     """
     name_=ctypes.c_char_p(force_bytes(name))
     func=link.o2scl.o2scl_hdf_hdf_output_tensor_grid_wrapper
     func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
     func(hf._ptr,t._ptr,name_)
     return
 
+def hdf_input_vector_contour_line(link,hf,v,name=""):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *hf*: :class:`hdf_file` object
+        | *v*: :class:`std::vector<contour_line>` object
+        | *name*: string
+    """
+    name_=ctypes.c_char_p(force_bytes(name))
+    func=link.o2scl.o2scl_hdf_hdf_input_vector_contour_line_wrapper
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
+    func(hf._ptr,v._ptr,name_)
+    return
+
+def hdf_input_n_vector_contour_line(link,hf,v,name):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *hf*: :class:`hdf_file` object
+        | *v*: :class:`std::vector<contour_line>` object
+        | *name*: :class:`std::string` object
+    """
+    func=link.o2scl.o2scl_hdf_hdf_input_n_vector_contour_line_wrapper
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_void_p]
+    func(hf._ptr,v._ptr,name._ptr)
+    name._owner=True
+    return
+
+def hdf_output_vector_contour_line(link,hf,v,name):
+    """
+        | Parameters:
+        | *link* :class:`linker` object
+        | *hf*: :class:`hdf_file` object
+        | *v*: :class:`std::vector<contour_line>` object
+        | *name*: string
+    """
+    name_=ctypes.c_char_p(force_bytes(name))
+    func=link.o2scl.o2scl_hdf_hdf_output_vector_contour_line_wrapper
+    func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_char_p]
+    func(hf._ptr,v._ptr,name_)
+    return
+
 def value_spec(link,spec,d,verbose=0,err_on_fail=True):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *spec*: string
         | *d*: ``double``
         | *verbose*: ``int``
@@ -1585,24 +2145,25 @@
     spec_=ctypes.c_char_p(force_bytes(spec))
     func=link.o2scl.o2scl_hdf_vector_spec_wrapper
     func.restype=std_vector
     func.argtypes=[ctypes.c_char_p]
     ret=func(spec_)
     return ret
 
-def mult_vector_spec(link,spec,v,verbose=0,err_on_fail=True):
+def mult_vector_spec(link,spec,v,use_regex=False,verbose=0,err_on_fail=True):
     """
         | Parameters:
         | *link* :class:`linker` object
         | *spec*: string
         | *v*: :class:`std::vector<std::vector<double>>` object
+        | *use_regex*: ``bool``
         | *verbose*: ``int``
         | *err_on_fail*: ``bool``
         | Returns: ``ctypes.c_int`` object
     """
     spec_=ctypes.c_char_p(force_bytes(spec))
     func=link.o2scl.o2scl_hdf_mult_vector_spec_std_vector_double__wrapper
     func.restype=ctypes.c_int
-    func.argtypes=[ctypes.c_char_p,ctypes.c_void_p,ctypes.c_int,ctypes.c_bool]
-    ret=func(spec_,v._ptr,verbose,err_on_fail)
+    func.argtypes=[ctypes.c_char_p,ctypes.c_void_p,ctypes.c_bool,ctypes.c_int,ctypes.c_bool]
+    ret=func(spec_,v._ptr,use_regex,verbose,err_on_fail)
     return ret
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/hdf_add.py` & `o2sclpy-0.928/o2sclpy/hdf_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/link_o2scl.py` & `o2sclpy-0.928/o2sclpy/link_o2scl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/nuclei.py` & `o2sclpy-0.928/o2sclpy/nuclei.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2022, Andrew W. Steiner
+  Copyright (C) 2020-2023, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -14,28 +14,28 @@
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with O2scl. If not, see <http://www.gnu.org/licenses/>.
 
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 """
 
 import ctypes
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 
 from o2sclpy.part import *
 
 class nucleus(part):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucleus``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucleus.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucleus.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucleus
 
         | Parameters:
@@ -68,15 +68,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucleus
         
-        Returns: a nucleus object
+        Returns: nucleus object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def Z(self):
@@ -179,15 +179,15 @@
         return
 
 
 class nucmass_info:
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_info``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_info.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_info.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -224,15 +224,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_info
         
-        Returns: a nucmass_info object
+        Returns: nucmass_info object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def parse_elstring(self,ela):
         """
@@ -334,15 +334,15 @@
         return ret
 
 
 class nucmass:
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     @abstractmethod
@@ -380,15 +380,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass
         
-        Returns: a nucmass object
+        Returns: nucmass object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def m_prot(self):
@@ -666,15 +666,15 @@
         return ret
 
 
 class nucmass_table(nucmass):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_table``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_table.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_table.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_table
 
@@ -708,15 +708,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_table
         
-        Returns: a nucmass_table object
+        Returns: nucmass_table object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def n(self):
@@ -779,15 +779,15 @@
         return ret
 
 
 class nucmass_fit_base(nucmass):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_fit_base``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_fit_base.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_fit_base.html .
     """
 
     @abstractmethod
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_fit_base
 
@@ -821,15 +821,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_fit_base
         
-        Returns: a nucmass_fit_base object
+        Returns: nucmass_fit_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def nfit(self):
@@ -852,15 +852,15 @@
         return
 
 
 class nucmass_semi_empirical(nucmass_fit_base):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_semi_empirical``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_semi_empirical.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_semi_empirical.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_semi_empirical
 
         | Parameters:
@@ -893,15 +893,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_semi_empirical
         
-        Returns: a nucmass_semi_empirical object
+        Returns: nucmass_semi_empirical object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def B(self):
@@ -1030,15 +1030,15 @@
         return ret
 
 
 class nucmass_ame(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_ame``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_ame.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_ame.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_ame
 
         | Parameters:
@@ -1071,26 +1071,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_ame
         
-        Returns: a nucmass_ame object
+        Returns: nucmass_ame object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_table(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_table``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_dz_table.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_table.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_table
 
         | Parameters:
@@ -1123,26 +1123,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_dz_table
         
-        Returns: a nucmass_dz_table object
+        Returns: nucmass_dz_table object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_fit(nucmass_fit_base):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_fit``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_dz_fit.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_fit.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_fit
 
         | Parameters:
@@ -1175,26 +1175,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_dz_fit
         
-        Returns: a nucmass_dz_fit object
+        Returns: nucmass_dz_fit object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dz_fit_33(nucmass_fit_base):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_dz_fit_33``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_dz_fit_33.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dz_fit_33.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dz_fit_33
 
         | Parameters:
@@ -1227,26 +1227,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_dz_fit_33
         
-        Returns: a nucmass_dz_fit_33 object
+        Returns: nucmass_dz_fit_33 object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_frdm(nucmass_fit_base):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_frdm``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_frdm.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_frdm.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_frdm
 
         | Parameters:
@@ -1279,15 +1279,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_frdm
         
-        Returns: a nucmass_frdm object
+        Returns: nucmass_frdm object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def a1(self):
@@ -1810,15 +1810,15 @@
         return
 
 
 class nucmass_mnmsk(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_mnmsk``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_mnmsk.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_mnmsk.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_mnmsk
 
         | Parameters:
@@ -1851,26 +1851,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_mnmsk
         
-        Returns: a nucmass_mnmsk object
+        Returns: nucmass_mnmsk object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_mnmsk_exp(nucmass_mnmsk):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_mnmsk_exp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_mnmsk_exp.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_mnmsk_exp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_mnmsk_exp
 
         | Parameters:
@@ -1903,26 +1903,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_mnmsk_exp
         
-        Returns: a nucmass_mnmsk_exp object
+        Returns: nucmass_mnmsk_exp object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_gen(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_gen``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_gen.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_gen.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_gen
 
         | Parameters:
@@ -1955,26 +1955,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_gen
         
-        Returns: a nucmass_gen object
+        Returns: nucmass_gen object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_dglg(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_dglg``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_dglg.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_dglg.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_dglg
 
         | Parameters:
@@ -2007,26 +2007,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_dglg
         
-        Returns: a nucmass_dglg object
+        Returns: nucmass_dglg object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_hfb(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_hfb``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_hfb.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_hfb.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_hfb
 
         | Parameters:
@@ -2059,26 +2059,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_hfb
         
-        Returns: a nucmass_hfb object
+        Returns: nucmass_hfb object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_hfb_sp(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_hfb_sp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_hfb_sp.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_hfb_sp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_hfb_sp
 
         | Parameters:
@@ -2111,26 +2111,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_hfb_sp
         
-        Returns: a nucmass_hfb_sp object
+        Returns: nucmass_hfb_sp object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_ktuy(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_ktuy``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_ktuy.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_ktuy.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_ktuy
 
         | Parameters:
@@ -2163,26 +2163,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_ktuy
         
-        Returns: a nucmass_ktuy object
+        Returns: nucmass_ktuy object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_sdnp(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_sdnp``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_sdnp.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_sdnp.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_sdnp
 
         | Parameters:
@@ -2215,26 +2215,26 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_sdnp
         
-        Returns: a nucmass_sdnp object
+        Returns: nucmass_sdnp object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class nucmass_wlw(nucmass_table):
     """
     Python interface for O\ :sub:`2`\ scl class ``nucmass_wlw``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/nucmass_wlw.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/nucmass_wlw.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class nucmass_wlw
 
         | Parameters:
@@ -2267,15 +2267,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class nucmass_wlw
         
-        Returns: a nucmass_wlw object
+        Returns: nucmass_wlw object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 def ame_load(link,ame,name,exp_only):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/o2graph_plotter.py` & `o2sclpy-0.928/o2sclpy/o2graph_plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -28,35 +28,565 @@
 
 # For wrapping help text
 import textwrap
 
 # For code.interact() in 'python' command
 import code 
 
-# For rectangles
-import matplotlib.patches as patches
-
-from o2sclpy.doc_data import cmaps, new_cmaps, base_list
-from o2sclpy.doc_data import extra_types, extra_list, param_list
-from o2sclpy.doc_data import yt_param_list, acol_help_topics
+from o2sclpy.doc_data import cmaps, new_cmaps, extra_types
+from o2sclpy.doc_data import acol_help_topics
 from o2sclpy.doc_data import o2graph_help_topics, acol_types
 from o2sclpy.utils import parse_arguments, string_to_dict, terminal_py
-from o2sclpy.utils import force_bytes, default_plot, get_str_array
-from o2sclpy.utils import is_number, table_get_column, o2scl_get_type
+from o2sclpy.utils import force_bytes, default_plot
+from o2sclpy.utils import is_number
 from o2sclpy.utils import length_without_colors, wrap_line, screenify_py
-from o2sclpy.utils import get_ic_ptrs_to_list, string_equal_dash
-from o2sclpy.utils import reformat_python_docs, force_string
+from o2sclpy.utils import string_equal_dash
+from o2sclpy.utils import force_string, remove_spaces
 from o2sclpy.plot_base import plot_base
 from o2sclpy.yt_plot_base import yt_plot_base
 from o2sclpy.plot_info import marker_list, markers_plot, colors_near
 from o2sclpy.plot_info import cmap_list_func, cmaps_plot, xkcd_colors_list
 from o2sclpy.plot_info import colors_plot, color_list
 from o2sclpy.doc_data import version
 from o2sclpy.hdf import *
 from o2sclpy.base import *
+from o2sclpy.kde import *
+
+base_list=[
+    ["addcbar",plot_base.addcbar.__doc__],
+    ["arrow",plot_base.arrow.__doc__],
+    ["backend",
+     ("Documentation for backend\n\n"+
+      "Select the matplotlib backend to use.\n\n"+
+      "<backend>\n\n"+
+      "This commend selects the matplotlib backend. "+
+      "Typical values are 'Agg', 'TkAgg', 'WX', 'QTAgg', "+
+      "and 'QT4Agg'. Use backend Agg to save the plot to a "+
+      "file without opening a window. The backend can only "+
+      "be changed once, i.e. if the backend command is "+
+      "invoked more than once, then only the last invocation "+
+      "will have any effect.")],
+    ["canvas",plot_base.canvas.__doc__],
+    ["clf","Documentation for clf\n\n"+
+     "Clear the current figure.\n\n"+
+     "(No arguments.)\n\n"+
+     "Clear the current figure."],
+    ["cmap",plot_base.cmap.__doc__],
+    ["colors",plot_base.colors.__doc__],
+    ["ellipse",plot_base.ellipse.__doc__],
+    ["error-point",plot_base.error_point.__doc__],
+    ["eval","Documentation for eval\n\n"+
+     "Run the python eval() function.\n\n"+
+     "<python code>\n\n"+
+     "Take the python code given and execute it using eval(). "+
+     "For example, 'o2graph -eval \"print(numpy.pi)\"'."],
+    ["exec","Documentation for exec\n\n"+
+     "Run the python code specified in a file.\n\n"+
+     "<filename>\n\n"+
+     "Take the python code given and execute it using execfile()."],
+    ["image","Documentation for image\n\n"+
+     "Plot a png file in a matplotlib window.\n\n"+
+     "<png file>\n\n"+
+     "This command reads a png file, fills a plotting canvas "+
+     "and then calls matplotlib.pyplot.show()."],
+    ["inset",plot_base.inset.__doc__],
+    ["kde-plot",0],
+    ["kde-2d-plot",0],
+    ["line",plot_base.line.__doc__],
+    ["modax",plot_base.modax.__doc__],
+    ["mp4",0],
+    ["o2scl-addl-libs",
+     "Specify a list of list of additional libraries to load."],
+    ["o2scl-cpp-lib",
+     "Specify the location of the standard C++ library."],
+    ["o2scl-lib-dir",
+     "Specify the directory for the libo2scl shared library."],
+    ["plotv",0],
+    ["point",plot_base.point.__doc__],
+    ["python","Begin an interactive python session."],
+    ["rect",plot_base.rect.__doc__],
+    ["save",
+     "Documentation for save\n\n"+
+     "Save the current plot in a file.\n\n"+
+     "<filename>\n\n",
+     "Save the current plot in a file similar "+
+     "to plot.savefig(). The action of this command depends on "+
+     "which backend was selected. File type depends on the "+
+     "extension, typically either .png, .pdf, .eps, .jpg, .raw, "+
+     ".svg, and .tif."],
+    ["selax",plot_base.selax.__doc__],
+    ["show",plot_base.show.__doc__],
+    ["subadj","Documentation for subadj\n\n"+
+     "Adjust spacing of subplots\n\n"+
+     "<kwargs>\n\n"+
+     "Adjust the spacing for subplots after using the 'subplots' "+
+     "command. All arguments are keyword arguments. The kwargs "+
+     "for 'subadj' are left, right, bottom, top, "+
+     "wspace, and hspace. This just a wrapper to the "+
+     "pyplot.subplots_adjust() function. Note that, unlike the "+
+     "margin settings for the fig_dict parameter, the values "+
+     "'right' and 'top' are defined relative to the lower-left "+
+     "corner, so a small right margin is 'right=0.99'. The "+
+     "subplots_adjust() function requires right>left and "+
+     "top>bottom."],
+    ["subplots",plot_base.subplots.__doc__],
+    ["text",plot_base.text.__doc__],
+    ["textbox",plot_base.textbox.__doc__],
+    ["ttext",plot_base.ttext.__doc__],
+    ["xlimits",plot_base.xlimits.__doc__],
+    ["xtitle",plot_base.xtitle.__doc__],
+    ["ylimits",plot_base.ylimits.__doc__],
+    ["ytitle",plot_base.ytitle.__doc__],
+    ["yt-ann",0],
+    ["yt-arrow",yt_plot_base.yt_arrow.__doc__],
+    ["yt-axis",yt_plot_base.yt_plot_axis.__doc__],
+    ["yt-box",yt_plot_base.yt_box.__doc__],
+    ["yt-line",yt_plot_base.yt_line.__doc__],
+    ["yt-path",0],
+    ["yt-render",0],
+    ["yt-source-list","List yt sources"],
+    ["yt-text",0],
+    ["yt-tf",0],
+    ["yt-xtitle",yt_plot_base.yt_xtitle.__doc__],
+    ["yt-ytitle",yt_plot_base.yt_ytitle.__doc__],
+    ["yt-ztitle",yt_plot_base.yt_ztitle.__doc__],
+    ["zlimits",plot_base.zlimits.__doc__]
+]
+
+extra_list=[
+    ["double[]","plot1",0],
+    ["hist","hist-plot",0],
+    ["hist","plot",0],
+    ["hist_2d","den-plot",0],
+    ["int[]","plot1",0],
+    ["prob_dens_mdim_amr","plot",0],
+    ["size_t[]","plot1",0],
+    ["table","errorbar",0],
+    ["table","hist-plot",0],
+    ["table","hist2d-plot",0],
+    ["table","plot",0],
+    ["table","to-kde",0],
+    ["table","plot1",0],
+    ["table","plot-color",0],
+    ["table","rplot",0],
+    ["table","scatter",0],
+    ["table","yt-scatter",0],
+    ["table","yt-vertex-list",0],
+    ["table3d","den-plot",0],
+    ["table3d","den-plot-rgb",0],
+    ["table3d","make-png",0],
+    ["tensor","den-plot",0],
+    ["tensor<int>","den-plot",0],
+    ["tensor<size_t>","den-plot",0],
+    ["tensor_grid","den-plot",0],
+    ["tensor_grid","den-plot-anim",0],
+    ["tensor_grid","yt-add-vol",0],
+    ["vector<contour_line>","plot",0],
+]
+
+param_list=[
+    ["colbar","If true, den-plot adds a color legend (default False)."],
+    ["editor","If true, open the plot editor."],
+    ["fig_dict",("Dictionary for figure properties. The default value is "+
+                 "blank and implies ('fig_size_x=6.0, fig_size_y=6.0, "+
+                 "ticks_in=False, "+
+                 "rt_ticks=False, left_margin=0.14, right_margin=0.04, "+
+                 "bottom_margin=0.12, top_margin=0.04, fontsize=16'). "+
+                 "The x and y sizes of the figure object are in "+
+                 "fig_size_x and fig_size_y. The value ticks_in refers "+
+                 "to whether or not the ticks are inside or outside the "+
+                 "plot. The value of rt_ticks refers to whether or not "+
+                 "tick marks are plotted on the right and top sides of "+
+                 "the plot. If the font size is unspecified, then "+
+                 "the 'font' setting is used. "+
+                 "The font size parameter is multiplied by 0.8 "+
+                 "and then used for the axis labels. Note that this "+
+                 "value must be set before the plotting canvas is"+
+                 "created (which is done by 'subplots' or automatically "+
+                 "when the first object is added to the plot) in order "+
+                 "to have any effect.")],
+    ["font","Font scaling for text objects (default 16)."],
+    ["logx","If true, use a logarithmic x-axis (default False)."],
+    ["logy","If true, use a logarithmic y-axis (default False)."],
+    ["logz","If true, use a logarithmic z-axis (default False)."],
+    ["usetex","If true, use LaTeX for text rendering (default True)."],
+    ["verbose","Verbosity parameter (default 1)."],
+    ["xhi","Upper limit for x-axis (function if starts with '(')."],
+    ["xlo","Lower limit for x-axis (function if starts with '(')."],
+    ["xset","If true, x-axis limits have been set (default False)."],
+    ["yhi","Upper limit for y-axis (function if starts with '(')."],
+    ["ylo","Lower limit for y-axis (function if starts with '(')."],
+    ["yset","If true, y-axis limits have been set (default False)."],
+    ["zlo","Lower limit for z-axis (function if starts with '(')."],
+    ["zhi","Upper limit for z-axis (function if starts with '(')."],
+    ["zset","If true, z-axis limits have been set (default False)."]
+]
+"""
+List of o2sclpy parameters
+
+A list of 2-element entries, name and description
+"""
+
+yt_param_list=[
+    ["yt_filter",("Filter for yt-generated images (default '')"+
+                  "\n\nIf non-empty, must contain the "+
+                  "strings '%i' for input file and '%o' for "+
+                  "output file. A typical example is something like\n\n"+
+                  "convert -contrast-stretch 0 %i %o\n\n"+
+                  "which uses imagemagick to adjust the color curve.")],
+    ["yt_focus",("The yt camera focus as a string. "+
+                 "The string 'default' is equivalent "+
+                 "to '[0.5,0.5,0.5] internal'. This string can be "+
+                 "either in the "+
+                 "'internal' or 'user' unit system.")],
+    ["yt_path",("The yt animation path (default []), as list of "+
+                "lists. The list contains instructions such as\n\n"+
+                "['yaw',100,0.01]\n['zoom',100,2.0]\n...\n\n"+
+                "where the first entry in each sublist is always a type "+
+                "move, and the second entry in each sublist is always the "+
+                "number of frames over which to complete the move.\n\n"+
+                "Note that this variable is not set using -set or -get but "+
+                "by the 'yt-path' command.")],
+    ["yt_position",("The yt camera position as a string "+
+                    "The string 'default' is equivalent "+
+                    "to '[1.5,0.6,0.7] internal'. This string can be "+
+                    "either in the 'internal' or 'user' unit system.")],
+    ["yt_north",("The yt camera north vector string. "+
+                 "The string 'default' is equivalent to "
+                 "'[1.0,0.0,0.0]'. Always in the internal "+
+                 "unit system.")],
+    ["yt_width",("The yt camera width relative to the domain volume "+
+                 "as a string. The string 'default' is equivalent to "+
+                 "'[1.5,1.5,1.5]'. Always in the internal unit system.")],
+    ["yt_resolution","The rendering resolution (default (512,512))."],
+    ["yt_sigma_clip","Sigma clipping parameter (default 4.0)."]
+]
+"""
+List of yt parameters for o2sclpy
+
+A list of 2-element entries, name and description
+"""
+
+def doc_replacements(s,ter,amp,link,script=False):
+    """
+    Make some replacements from RST formatting to the terminal screen.
+
+    This function is in ``o2graph_plotter.py``.
+    """
+
+    amt=acol_manager(link,amp)
+
+    if script:
+        s=(force_string(amt.get_exec_color())+s+
+           force_string(amt.get_default_color()))
+        return s
+    
+    # Replace commands in base_list
+    for i in range(0,len(base_list)):
+        s=s.replace('``'+base_list[i][0]+'``',
+                    force_string(amt.get_command_color())+
+                    base_list[i][0]+
+                    force_string(amt.get_default_color()))
+        
+    # Replace commands in extra_list
+    for i in range(0,len(extra_list)):
+        s=s.replace('``'+extra_list[i][1]+'``',
+                    force_string(amt.get_command_color())+
+                    extra_list[i][1]+
+                    force_string(amt.get_default_color()))
+        
+    s=s.replace('o2graph',
+                (force_string(amt.get_exec_color())+'o2graph'+
+                 force_string(amt.get_default_color())))
+    s=s.replace('O2scl',
+                (force_string(amt.get_exec_color())+'O₂scl'+
+                 force_string(amt.get_default_color())))
+        
+    # Replace parameters in param_list
+    for i in range(0,len(param_list)):
+        s=s.replace('``'+param_list[i][0]+'``',
+                    force_string(amt.get_param_color())+
+                    param_list[i][0]+
+                    force_string(amt.get_default_color()))
+
+    # Replace yt_parameters in yt_param_list
+    for i in range(0,len(yt_param_list)):
+        s=s.replace('``'+yt_param_list[i][0]+'``',
+                    force_string(amt.get_param_color())+
+                    yt_param_list[i][0]+
+                    force_string(amt.get_default_color()))
+
+    # Replace yt_parameters in acol_types
+    for i in range(0,len(acol_types)):
+        s=s.replace('``'+acol_types[i]+'``',
+                    force_string(amt.get_type_color())+
+                    acol_types[i]+
+                    force_string(amt.get_default_color()))
+
+    # Decorate URLs
+    if s.find('https://')!=-1:
+        ix=s.find('https://')
+        found=False
+        j=ix
+        while j!=len(s) and found==False:
+            if s[j]==' ':
+                found=True
+            else:
+                j=j+1
+        if j==len(s):
+            s=(s[0:ix]+force_string(amt.get_url_color())+
+               s[ix:len(s)]+force_string(amt.get_default_color()))
+        else:
+            s=(s[0:ix]+force_string(amt.get_url_color())+
+               s[ix:j]+force_string(amt.get_default_color())+
+               s[j:len(s)])
+
+    # For ``code`` formatting
+    s=s.replace(' ``',' ')
+    s=s.replace('`` ',' ')
+    s=s.replace('``, ',', ')
+    s=s.replace('``. ','. ')
+
+    # Combine two spaces to one
+    s=s.replace('  ',' ')
+
+    # For :math:`` equations
+    s=s.replace(' :math:`',' ')
+    s=s.replace('` ',' ')
+    s=s.replace('`.','.')
+    s=s.replace('`',',')
+                    
+    return s
+
+def o2scl_get_type(o2scl,amp,link):
+    """
+    Get the type of the current object stored in the acol_manager
+    pointer
+    """
+
+    amt=acol_manager(link,amp)
+    return amt.get_type()
+
+def reformat_python_docs(cmd,doc_str,amp,link,
+                         return_short=False,verbose=0):
+    """
+    Reformat a python documentation string
+    """
+    
+    amt=acol_manager(link,amp)
+    
+    reflist=doc_str.split('\n')
+    
+    for i in range(0,len(reflist)):
+        reflist[i]=remove_spaces(reflist[i])
+        if verbose>1:
+            print(i,'x',reflist[i],'x')
+
+    if len(reflist)<1:
+        return
+
+    if reflist[0]=='':
+        if len(reflist)<2:
+            return
+        doc_str2=reflist[1]
+        for i in range(2,len(reflist)):
+            doc_str2=doc_str2+'\n'+reflist[i]
+    else:
+        doc_str2=reflist[0]
+        for i in range(1,len(reflist)):
+            doc_str2=doc_str2+'\n'+reflist[i]
+
+    reflist2=doc_str2.split('\n\n')
+
+    if False:
+        for i in range(0,len(reflist2)):
+            print(i,'x',reflist2[i],'x')
+    
+    ter=terminal_py()
+    try:
+        ncols=os.get_terminal_size().columns
+    except:
+        ncols=80
+
+    short=''
+    parm_desc=''
+    long_help=''
+
+    # The short description
+    if len(reflist2)==1:
+        short=reflist2[0].split('\n')[0]
+    elif len(reflist2)>=2:
+        short=reflist2[1]
+
+    if return_short:
+        return short
+
+    # The parameter description
+    if len(reflist2)>=3:
+        parm_desc=reflist2[2].replace('\n',' ')
+
+        parm_desc=parm_desc.replace('  ',' ')
+        sx='Command-line arguments: ``'
+        if parm_desc[0:len(sx)]==sx:
+            parm_desc=parm_desc[len(sx):]
+        if parm_desc[-2:]=='``':
+            parm_desc=parm_desc[0:-2]
+            
+    print('Usage: '+force_string(amt.get_command_color())+cmd+
+          force_string(amt.get_default_color())+' '+parm_desc)
+    
+    print('Short description:',short)
+
+    if len(reflist2)>=4:
+        print('')
+        print('Long description:')
+        last_pgh_colons=False
+        for j in range(3,len(reflist2)):
+            if len(reflist2[j])>0:
+                if last_pgh_colons:
+                    long_help=doc_replacements(reflist2[j].replace('\n',' '),
+                                               ter,amp,link,script=True)
+                    tmplist=long_help.split(' \ ')
+                else:
+                    long_help=doc_replacements(reflist2[j].replace('\n',' '),
+                                               ter,amp,link)
+                    tmplist=wrap_line(long_help,ncols-1)
+                if j!=3:
+                    print('')
+                for k in range(0,len(tmplist)):
+                    if last_pgh_colons:
+                        if k!=len(tmplist)-1:
+                            print(' ',tmplist[k],'\\')
+                        else:
+                            print(' ',tmplist[k])
+                    else:
+                        print(tmplist[k])
+                if long_help[-2:]=='::':
+                    last_pgh_colons=True
+                else:
+                    last_pgh_colons=False
+                    
+    return
+
+def reformat_python_docs_type(curr_type,cmd,doc_str,amp,link,
+                              return_short=False,verbose=0):
+    """
+    Reformat a python documentation string
+    """
+    
+    amt=acol_manager(link,amp)
+
+    reflist=doc_str.split('\n')
+    
+    for i in range(0,len(reflist)):
+        reflist[i]=remove_spaces(reflist[i])
+        if verbose>1:
+            print(i,'x',reflist[i],'x')
+
+    if len(reflist)<1:
+        return
+
+    if reflist[0]=='':
+        if len(reflist)<2:
+            return
+        doc_str2=reflist[1]
+        for i in range(2,len(reflist)):
+            doc_str2=doc_str2+'\n'+reflist[i]
+    else:
+        doc_str2=reflist[0]
+        for i in range(1,len(reflist)):
+            doc_str2=doc_str2+'\n'+reflist[i]
+
+    reflist2=doc_str2.split('\n\n')
+
+    sect_found=False
+    jfound=0
+    for j in range(0,len(reflist2)):
+        if reflist2[j]==("For objects of type ``"+
+                         force_string(curr_type)+"``:"):
+            sect_found=True
+            jfound=j+1
+
+    if sect_found==False:
+        print('Could not find documentation for type',curr_type,
+              'and command',cmd)
+        return
+
+    strt="For objects of type"
+    reflist3=[]
+    jlast=len(reflist2)
+    loop_done=False
+    for j in range(jfound,jlast):
+        if reflist2[j][0:len(strt)]==strt:
+            jlast=j
+            loop_done=True
+        elif loop_done==False:
+            reflist3.append(reflist2[j])
+
+    if False:
+        for j in range(0,len(reflist3)):
+            print(j,'y',reflist3[j],'y')
+            
+    ter=terminal_py()
+    ncols=os.get_terminal_size().columns
+
+    short=''
+    parm_desc=''
+    long_help=''
+
+    if len(reflist3)>0:
+        short=reflist3[0]
+
+    if return_short:
+        return short
+
+    if len(reflist3)>1:
+        parm_desc=reflist3[1].replace('\n',' ')
+
+        parm_desc=parm_desc.replace('  ',' ')
+        sx='Command-line arguments: ``'
+        if parm_desc[0:len(sx)]==sx:
+            parm_desc=parm_desc[len(sx):]
+        if parm_desc[-2:]=='``':
+            parm_desc=parm_desc[0:-2]
+            
+    print('Usage for type '+
+          force_string(amt.get_type_color())+curr_type+
+          force_string(amt.get_default_color())+': '+
+          force_string(amt.get_command_color())+cmd+
+          force_string(amt.get_default_color())+' '+parm_desc)
+    
+    print('Short description:',short)
+
+    if len(reflist3)>2:
+        print('')
+        print('Long description:')
+        for j in range(2,len(reflist3)):
+            if len(reflist3[j])>0:
+                long_help=doc_replacements(reflist3[j].replace('\n',' '),
+                                           ter,amp,link)
+                tmplist=wrap_line(long_help,ncols-1)
+                if j!=3:
+                    print('')
+                for k in range(0,len(tmplist)):
+                    print(tmplist[k])
+                    
+    return
+
+def table_get_column(o2scl,amp,link,name,return_pointer=False):
+    """
+    Return a column from the current table object stored
+    in the acol_manager object 'amp'
+    """
+
+    amt=acol_manager(link,amp)
+    tab=amt.get_table_obj()
+    col=tab[force_bytes(name)]
+
+    return col
 
 class o2graph_plotter(yt_plot_base):
     """
     A plotting class for the o2graph script. This class is a child of the
     :py:class:`o2sclpy.plot_base` class.
 
     This class is not necessarily intended to be instantiated by the 
@@ -65,15 +595,80 @@
     The function parameter `o2scl` must always be a ctypes DLL 
     object which points to the libo2scl shared library (.so on
     linux and .dylib on OSX). The function parameter `amp` must
     always be a pointer to the 
     :ref:`o2scl_acol::acol_manager<o2scl:acol_manager>` object.
     """
 
-    def set_wrapper(self,o2scl,amp,args):
+    cbar=0
+    """ 
+    Colorbar object
+    """
+
+    def __init__(self):
+        """
+        Desc
+        """
+        for line in base_list:
+            if line[0]=="plotv":
+                line[1]=o2graph_plotter.plotv.__doc__
+            elif line[0]=="yt-ann":
+                line[1]=o2graph_plotter.yt_ann_func.__doc__
+            elif line[0]=="yt-path":
+                line[1]=o2graph_plotter.yt_path_func.__doc__
+            elif line[0]=="yt-render":
+                line[1]=o2graph_plotter.yt_render.__doc__
+            elif line[0]=="yt-text":
+                line[1]=o2graph_plotter.yt_text.__doc__
+            elif line[0]=="mp4":
+                line[1]=o2graph_plotter.mp4.__doc__
+            elif line[0]=="kde-plot":
+                line[1]=o2graph_plotter.kde_plot.__doc__
+            elif line[0]=="kde-2d-plot":
+                line[1]=o2graph_plotter.kde_2d_plot.__doc__
+            elif line[0]=="yt-tf":
+                line[1]=o2graph_plotter.yt_tf_func.__doc__
+        for line in extra_list:
+            if line[1]=="to-kde":
+                line[2]=o2graph_plotter.to_kde.__doc__
+            if line[1]=="den-plot":
+                line[2]=o2graph_plotter.den_plot_o2graph.__doc__
+            if line[1]=="den-plot-rgb":
+                line[2]=o2graph_plotter.den_plot_rgb_o2graph.__doc__
+            if line[1]=="den-plot-anim":
+                line[2]=o2graph_plotter.den_plot_anim.__doc__
+            if line[1]=="errorbar":
+                line[2]=o2graph_plotter.errorbar.__doc__
+            elif line[1]=="hist-plot":
+                line[2]=o2graph_plotter.hist_plot.__doc__
+            elif line[1]=="hist2d-plot":
+                line[2]=o2graph_plotter.hist2d_plot.__doc__
+            elif line[1]=="plot":
+                line[2]=o2graph_plotter.plot_o2graph.__doc__
+            elif line[1]=="plot1":
+                line[2]=o2graph_plotter.plot1.__doc__
+            elif line[1]=="plot-color":
+                line[2]=o2graph_plotter.plot_color.__doc__
+            elif line[1]=="rplot":
+                line[2]=o2graph_plotter.rplot.__doc__
+            elif line[1]=="scatter":
+                line[2]=o2graph_plotter.scatter.__doc__
+            elif line[1]=="yt-add-vol":
+                line[2]=o2graph_plotter.yt_add_vol.__doc__
+            elif line[1]=="yt-anim":
+                line[2]=o2graph_plotter.yt_anim.__doc__
+            elif line[1]=="yt-scatter":
+                line[2]=o2graph_plotter.yt_scatter.__doc__
+            elif line[1]=="yt-vertex-list":
+                line[2]=o2graph_plotter.yt_vertex_list.__doc__
+
+        super().__init__()
+        return
+
+    def set_wrapper(self,o2scl,amp,link,args):
         """
         Wrapper around :py:func:`o2sclpy.plot_base.set` which sets
         plot-related parameters and sends other parameters to
         ``acol_manager``.
         """
 
         # First determine if it's an o2graph or yt parameter
@@ -99,31 +694,26 @@
         # both the o2graph and the acol version match. Otherwise, if
         # it's only an o2graph or yt parameter, then just return.
         if (match==True and 
             force_bytes(args[0])!=b'verbose'):
             return
 
         # Call the acol 'set' function
-        str_args='-set'
-        size_type=ctypes.c_int * (len(args)+1)
-        sizes=size_type()
-        sizes[0]=len('set')+1
-            
+        vs=std_vector_string(self.link2)
+        vs.resize(len(args)+1)
+        vs[0]=b'-set'
         for i in range(0,len(args)):
-            str_args=str_args+args[i]
-            sizes[i+1]=len(args[i])
-        ccp=ctypes.c_char_p(force_bytes(str_args))
-    
-        parse_fn=o2scl.o2scl_acol_parse
-        parse_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                           size_type,ctypes.c_char_p]
+            vs[i+1]=force_bytes(args[i])
+
+        amt=acol_manager(self.link2,amp)
             
         if self.verbose>2:
-            print('Calling acol set function for parameter',args[0],'.')
-        parse_fn(amp,len(args)+1,sizes,ccp)
+            print('Calling acol set function for parameter '+args[0]+'.')
+            
+        amt.parse_vec_string(vs)
 
         # End of function o2graph_plotter::set_wrapper()
         return
 
     def get_wrapper(self,o2scl,amp,args):
         """
         Wrapper around :py:func:`o2sclpy.plot_base.get` which
@@ -140,948 +730,819 @@
                 match=True
                 
         if match==True:
             
             self.get(args[0])
                             
         else:
-                        
-            str_args='-get'
-            size_type=ctypes.c_int * (len(args)+1)
-            sizes=size_type()
-            sizes[0]=len('get')+1
-        
+
+            vs=std_vector_string(self.link2)
+            vs.resize(len(args)+1)
+            vs[0]=b'-get'
             for i in range(0,len(args)):
-                str_args=str_args+args[i]
-                sizes[i+1]=len(args[i])
-            ccp=ctypes.c_char_p(force_bytes(str_args))
-        
-            parse_fn=o2scl.o2scl_acol_parse
-            parse_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                              size_type,ctypes.c_char_p]
-        
-            parse_fn(amp,len(args)+1,sizes,ccp)
+                vs[i+1]=force_bytes(args[i])
+
+            amt=acol_manager(self.link2,amp)
+
+            if self.verbose>2:
+                print('Calling acol get function for parameter '+
+                      args[0]+'.')
+
+            amt.parse_vec_string(vs)
 
         # End of function o2graph_plotter::get_wrapper()
         return
             
-    def gen_acol(self,o2scl,amp,cmd_name,args):
+    def ell_max(self,amp,link,args):
+        """
+        Desc
+        """
+        
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+
+        # Handle tensor and table3d types
+        if curr_type!=b'prob_dens_mdim_gaussian':
+            print("Command 'ell-max' not supported for type",
+                  curr_type,".")
+            return
+
+        amt=acol_manager(self.link2,amp)
+        pdmg=amt.get_pdmg_obj()
+        
+        if self.canvas_flag==False:
+            self.canvas()
+            
+        fx=float(eval(x))
+        fy=float(eval(y))
+        fw=float(eval(w))
+        fh=float(eval(h))
+        fangle=float(eval(angle))
+        if self.canvas_flag==False:
+            self.canvas()
+        r=patches.Ellipse((fx,fy),fw,fh,fangle,**kwargs)
+        self.axes.add_patch(r)
+        # End of function plot_base::ellipse()
+        
+        return
+        
+    def gen_acol(self,o2scl,amp,link,cmd_name,args):
         """
         Run a general ``acol`` command named ``cmd_name`` with arguments
-        stored in ``args``. This function uses the O\ :sub:`2`\ scl function
+        stored in ``args``. This function uses the O2scl function
         ``o2scl_acol_parse()``.
         """
 
-        str_args='-'+cmd_name
-        size_type=ctypes.c_int * (len(args)+1)
-        sizes=size_type()
-        sizes[0]=len(cmd_name)+1
+        vs=std_vector_string(self.link2)
+        vs.resize(len(args)+1)
         
+        vs[0]=b'-'+force_bytes(cmd_name)
         for i in range(0,len(args)):
-            str_args=str_args+args[i]
-            sizes[i+1]=len(args[i])
-        ccp=ctypes.c_char_p(force_bytes(str_args))
-
-        parse_fn=o2scl.o2scl_acol_parse
-        parse_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                           size_type,ctypes.c_char_p]
+            vs[i+1]=force_bytes(args[i])
+            
+        amt=acol_manager(self.link2,amp)
+        amt.parse_vec_string(vs)
         
-        parse_fn(amp,len(args)+1,sizes,ccp)
-
         # End of function o2graph_plotter::gen_acol()
         return
 
-    def den_plot(self,o2scl,amp,args):
+    def to_kde(self,o2scl,amp,link,args):
+        """Documentation for o2graph command ``to-kde``:
+
+        For objects of type ``table``:
+
+        Convert columns in a table to a KDE
+
+        Command-line arguments: ``<options or 'none'> 
+        <column 1> [column 2] ...``
+
+        Desc.
         """
-        Density plot from a ``table3d``, ``hist_2d``, ``tensor_grid``,
-        ``tensor``, ``tensor<int>``, or ``tensor<size_t>`` object.
+        
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+        amt=acol_manager(self.link2,amp)
+        print('here')
+        quit()
+        #if curr_type==b'table':
+        #else:
+
+    def mp4(self,args):
         """
+        Documentation for o2graph command ``mp4``:
 
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
+        Create an mp4 file from a series of images.
 
-        curr_type=o2scl_get_type(o2scl,amp)
+        Command-line arguments: ``<pattern> <output>``
 
-        # Handle tensor and table3d types
-        if (curr_type==b'tensor' or curr_type==b'tensor<size_t>' or
-            curr_type==b'tensor_grid' or curr_type==b'tensor<int>' or
-            curr_type==b'table3d'):
+        Typical patterns are "prefix%02dsuffix" and outputs
+        are "out.mp4"
+        """
+        if len(args)<2:
+            print('Command mpg needs more arguments.')
+            return
+        pattern=args[0]
+        output=args[1]
+        if output[-4:]!='.mp4':
+            output=output+'.mp4'
+        cmd=('ffmpeg -y -r 10 -f image2 -i '+pattern+
+             ' -vcodec libx264 '+
+             '-crf 25 -pix_fmt yuv420p '+output)
+        print('Executing ',cmd)
+        os.system(cmd)
+        
+        return
+        
+    def den_plot_o2graph(self,o2scl,amp,link,args):
+        """Documentation for o2graph command ``den-plot``:
 
-            kwstring=''
-            
-            # If the object is a tensor, convert to a table3d
-            # object before plotting
-            if curr_type!=b'table3d':
-                index1=0
-                index2=1
-                if len(args)==1:
-                    kwstring=args[0]
-                if len(args)>=2:
-                    index1=int(args[0])
-                    index2=int(args[1])
-                if len(args)>=3:
-                    kwstring=args[2]
-                if index1+index2!=1 and index1*index2!=0:
-                    print('Indices must be "0 1" or "1 0" in',
-                          'in den-plot.')
-                    return
-                    
-                conv_fn=o2scl.o2scl_acol_tensor_to_table3d
-                conv_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,ctypes.c_int]
-                conv_fn.restype=ctypes.c_int
-                
-                conv_ret=conv_fn(amp,index1,index2)
-                if conv_ret!=0:
-                    print('Automatic conversion to table3d failed.')
-                    return
-                slice_name="tensor"
-            else:
-                slice_name=args[0]
-                if len(args)>=2:
-                    kwstring=args[1]
-
-            # Now that we are guaranteed to have a table3d
-            # object to use, use that to create the density
-            # plot
-            get_fn=o2scl.o2scl_acol_get_slice
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr,
-                             int_ptr,double_ptr_ptr,double_ptr_ptr]
-
-            slice=ctypes.c_char_p(force_bytes(slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs=double_ptr()
-            get_fn(amp,slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs))
-
-            xgrid=[ptrx[i] for i in range(0,nx.value)]
-            ygrid=[ptry[i] for i in range(0,ny.value)]
-            stemp=[ptrs[i] for i in range(0,nx.value*ny.value)]
-            stemp2=numpy.array(stemp)
-            sl=stemp2.reshape(nx.value,ny.value)
-            sl=sl.transpose()
-
-            # If logz was specified, then manually apply the
-            # log to the data. Alternatively, we should consider
-            # using 'LogNorm' here, as suggested in
-            
-            #https://stackoverflow.com/questions/2546475/
-            #how-can-i-draw-a-log-normalized-imshow-plot-
-            #with-a-colorbar-representing-the-raw
-
-            if self.logz==True:
-                fail_found=False
-                for i in range(0,ny.value):
-                    for j in range(0,nx.value):
-                        if sl[i][j]>0.0:
-                            sl[i][j]=math.log10(sl[i][j])
-                        else:
-                            if fail_found==False:
-                                print('Failed to take log of',sl[i][j],
-                                      'at (i,j)=(',j,',',i,') or (',
-                                      xgrid[j],',',ygrid[i],
-                                      '). Setting point to zero and',
-                                      'suppressing future warnings.')
-                            fail_found=True
-                            sl[i][j]=0.0
-                                
-            # If the z range was specified, truncate all values
-            # outside that range (this truncation is done after
-            # the application of the log above)
-            if self.zset==True:
-                for i in range(0,ny.value):
-                    for j in range(0,nx.value):
-                        if sl[i][j]>self.zhi:
-                            sl[i][j]=self.zhi
-                        elif sl[i][j]<self.zlo:
-                            sl[i][j]=self.zlo
+        For objects of type ``table3d``:
 
-            if self.canvas_flag==False:
-                self.canvas()
+        Create a density plot from a slice of a table3d
 
-            dctt=string_to_dict(kwstring)
-            if dctt.pop('pcm',None)==True:
-                
-                print('Creating density plot using pcolormesh()')
-                if self.logx==True:
-                    self.axes.set_xscale('log')
-                if self.logy==True:
-                    self.axes.set_yscale('log')
-                self.last_image=self.axes.pcolormesh(xgrid,ygrid,sl,**dctt)
-                
-            else:
+        Command-line arguments: ``<slice> [kwargs]``
 
-                # The imshow() function doesn't work with a log axis, so we
-                # set the scales back to linear and manually take the log
-                self.axes.set_xscale('linear')
-                self.axes.set_yscale('linear')
-            
-                if self.logx==True:
-                    xgrid=[math.log(ptrx[i],10) for i in
-                           range(0,nx.value)]
-                if self.logy==True:
-                    ygrid=[math.log(ptry[i],10) for i in
-                           range(0,ny.value)]
+        Creates a density plot from the specified slice. A z-axis
+        density legend is displayed on the RHS if ``colbar`` is set to
+        True before plotting. If z-axis limits are specified, then
+        values larger than the upper limit are set equal to the upper
+        limit and values smaller than the lower limit are set equal to
+        the lower limit before plotting. 
+
+        The python function imshow() is used, unless 'pcm=True' is
+        specified, in which case the pcolormesh() function is used
+        instead. When 'pcm=False', logarithmic scales are handled by
+        taking the base 10 log of the x- or y-grids specified in the
+        table3d object before plotting. When 'pcm=True', logarithmic
+        axes can be handled automatically. The imshow() function
+        presumes a uniform linear or logarithmic x- and y-axis grid,
+        and the den-plot function will output a warning if this is not
+        the case. The pcolormesh() function can handle arbitrary x and
+        y-axis grids. If ``logz`` is set to true, then the base 10
+        logarithm is taken of the data before the density plot is
+        constructed. 
+
+        Some useful kwargs are cmap, interpolation (for
+        imshow), alpha, vmin, and vmax. 
+
+        See 
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
+        and
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pcolormesh.html
+        for more information and keyword arguments.
 
-                diffs_x=[xgrid[i+1]-xgrid[i] for i in range(0,len(xgrid)-1)]
-                mean_x=numpy.mean(diffs_x)
-                std_x=numpy.std(diffs_x)
-                diffs_y=[ygrid[i+1]-ygrid[i] for i in range(0,len(ygrid)-1)]
-                mean_y=numpy.mean(diffs_y)
-                std_y=numpy.std(diffs_y)
+        For objects of type ``hist_2d``:
+
+        Create a density plot from a hist_2d object
+
+        Command-line arguments: ``[kwargs]``
+
+        Creates a density plot from the current two-dimensional
+        histogram. A z-axis density legend is displayed on the RHS if
+        ``colbar`` is set to True before plotting. If z-axis limits
+        are specified, then values larger than the upper limit are set
+        equal to the upper limit and values smaller than the lower
+        limit are set equal to the lower limit before plotting.
+
+        The python function imshow() is used, unless 'pcm=True' is
+        specified, in which case the pcolormesh() function is used
+        instead. When 'pcm=False', logarithmic scales are handled by
+        taking the base 10 log of the x- or y-grids specified in the
+        table3d object before plotting. When 'pcm=True', logarithmic
+        axes can be handled automatically. The imshow() function
+        presumes a uniform linear or logarithmic x- and y-axis grid,
+        and the den-plot function will output a warning if this is not
+        the case. The pcolormesh() function can handle arbitrary x and
+        y-axis grids. If ``logz`` is set to true, then the base 10
+        logarithm is taken of the data before the density plot is
+        constructed. 
+
+        Some useful kwargs are cmap, interpolation (for
+        imshow), alpha, vmin, and vmax.
+
+        See 
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
+        and
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.pcolormesh.html
+        for more information and keyword arguments.
+
+        For objects of type ``tensor``:
+
+        Create a density plot from a tensor object.
+
+        Command-line arguments: ``[index_1 index_2] [kwargs]``
+
+        If the tensor has rank 2 and the indices are not specified,
+        then plot the first index along the x-axis and the second
+        index along the y-axis. A z-axis density legend is print on
+        the RHS if ``colbar`` is set to 1 before plotting. If z-axis
+        limits are specified, then values larger than the upper limit
+        are set equal to the upper limit and values smaller than the
+        lower limit are set equal to the lower limit before plotting.
+
+        For objects of type ``tensor<int>``:
+
+        Create a density plot from a tensor<int> object.
+
+        Command-line arguments: ``[index_1 index_2] [kwargs]``
+
+        If the tensor has rank 2 and the indices are not specified,
+        then plot the first index along the x-axis and the second
+        index along the y-axis. A z-axis density legend is print on
+        the RHS if ``colbar`` is set to 1 before plotting. If z-axis
+        limits are specified, then values larger than the upper limit
+        are set equal to the upper limit and values smaller than the
+        lower limit are set equal to the lower limit before plotting.
+
+        For objects of type ``tensor<size_t>``:
+
+        Create a density plot from a tensor<size_t> object.
+
+        Command-line arguments: ``[index_1 index_2] [kwargs]``
+
+        If the tensor has rank 2 and the indices are not specified,
+        then plot the first index along the x-axis and the second
+        index along the y-axis. A z-axis density legend is print on
+        the RHS if ``colbar`` is set to 1 before plotting. If z-axis
+        limits are specified, then values larger than the upper limit
+        are set equal to the upper limit and values smaller than the
+        lower limit are set equal to the lower limit before plotting.
+
+        For objects of type ``tensor_grid``:
+
+        Create a density plot from a tensor_grid object.
+
+        Command-line arguments: ``[index_1 index_2] [kwargs]``
+
+        If the tensor has rank 2 and the indices are not specified,
+        then plot the first index along the x-axis and the second
+        index along the y-axis. A z-axis density legend is print on
+        the RHS if ``colbar`` is set to 1 before plotting. If z-axis
+        limits are specified, then values larger than the upper limit
+        are set equal to the upper limit and values smaller than the
+        lower limit are set equal to the lower limit before plotting.
+
+        """
+        
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+        amt=acol_manager(self.link2,amp)
+
+        kwstring=''
+        slice_name=''
+        if curr_type==b'tensor':
+            if len(args)>=2:
+                amt.get_tensor_obj().copy_table3d(args[0],args[1],
+                                                  amt.get_table3d_obj())
+            else:
+                amt.get_tensor_obj().copy_table3d(0,1,amt.get_table3d_obj())
+            slice_name='z'
+            if len(args)>=3:
+                kwstring=args[2]
+            elif len(args)==1:
+                kwstring=args[0]
+        elif curr_type==b'tensor<size_t>':
+            if len(args)>=2:
+                amt.get_tensor_size_t_obj().copy_table3d(args[0],args[1],
+                                                         amt.get_table3d_obj())
+            else:
+                amt.get_tensor_size_t_obj().copy_table3d(0,1,
+                                                         amt.get_table3d_obj())
+            slice_name='z'
+            if len(args)>=3:
+                kwstring=args[2]
+            elif len(args)==1:
+                kwstring=args[0]
+        elif curr_type==b'tensor<int>':
+            if len(args)>=2:
+                amt.get_tensor_int_obj().copy_table3d(args[0],args[1],
+                                                      amt.get_table3d_obj())
+            else:
+                amt.get_tensor_int_obj().copy_table3d(0,1,
+                                                      amt.get_table3d_obj())
+            slice_name='z'
+            if len(args)>=3:
+                kwstring=args[2]
+            elif len(args)==1:
+                kwstring=args[0]
+        elif curr_type==b'tensor_grid':
+            svst=std_vector_size_t(self.link2)
+            tg=amt.get_tensor_grid_obj()
+            svst.resize(tg.get_rank())
+            func=tg.copy_table3d_align_setxy
+            t3d=amt.get_table3d_obj()
+            if len(args)>=2:
+                func(args[0],args[1],svst,t3d)
+            else:
+                func(0,1,svst,t3d)
+            slice_name='z'
+            if len(args)>=3:
+                kwstring=args[2]
+            elif len(args)==1:
+                kwstring=args[0]
+        elif curr_type==b'hist_2d':
             
-                if std_x/mean_x>1.0e-4 or std_x/mean_x>1.0e-4:
-                    print('Warning in o2graph::o2graph_plotter::den_plot():')
-                    print('  Nonlinearity of x or y grid is greater than '+
-                          '10^{-4}.')
-                    print('  Value of std(diff_x)/mean(diff_x): %7.6e .' %
-                          (std_x/mean_x))
-                    print('  Value of std(diff_y)/mean(diff_y): %7.6e .' %
-                          (std_y/mean_y))
-                    print('  The density plot may not be properly scaled.')
+            if len(args)>=1:
+                kwstring=args[0]
                 
-                extent1=xgrid[0]-(xgrid[1]-xgrid[0])/2
-                extent2=xgrid[nx.value-1]+(xgrid[nx.value-1]-
-                                           xgrid[nx.value-2])/2
-                extent3=ygrid[0]-(ygrid[1]-ygrid[0])/2
-                extent4=ygrid[ny.value-1]+(ygrid[ny.value-1]-
-                                           ygrid[ny.value-2])/2
-
-                f=self.axes.imshow
-                if len(kwstring)==0:
-                    self.last_image=f(sl,interpolation='nearest',
-                                      origin='lower',extent=[extent1,extent2,
-                                                             extent3,extent4],
-                                      aspect='auto')
-                else:
-                    self.last_image=f(sl,interpolation='nearest',
-                                      origin='lower',extent=[extent1,extent2,
-                                                             extent3,extent4],
-                                      aspect='auto',
-                                      **string_to_dict(kwstring))
-
-                # AWS 7/1/2020: I'm not sure why imshow() is now
-                # apparently mangling the minor tick settings. This
-                # restores them. 
-                self.axes.minorticks_on()
-                self.axes.tick_params('both',length=12,width=1,which='major')
-                self.axes.tick_params('both',length=5,width=1,which='minor')
-                self.axes.tick_params(labelsize=self.font*0.8)
+            dctt=string_to_dict(kwstring)
+            self.den_plot([amt.get_hist_2d_obj(),self.link2],**dctt)
+            return
+        
+        elif curr_type==b'table3d':
+            slice_name=args[0]
+            if len(args)>=2:
+                kwstring=args[1]
+        else:
+            print("Command 'den-plot' not supported for type",
+                  curr_type,".")
+            return
 
-            # The color bar is added later below...
+        dctt=string_to_dict(kwstring)
+        self.den_plot([amt.get_table3d_obj(),slice_name],**dctt)
 
-            # End of section for tensor types and table3d
-        elif curr_type==b'hist_2d':
+        return
 
-            get_fn=o2scl.o2scl_acol_get_hist_2d
-            get_fn.argtypes=[ctypes.c_void_p,int_ptr,double_ptr_ptr,
-                             int_ptr,double_ptr_ptr,double_ptr_ptr]
-
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs=double_ptr()
-            get_fn(amp,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs))
-
-            xgrid=[ptrx[i] for i in range(0,nx.value)]
-            ygrid=[ptry[i] for i in range(0,ny.value)]
-            stemp=[ptrs[i] for i in range(0,nx.value*ny.value)]
-            stemp2=numpy.array(stemp)
-            sl=stemp2.reshape(nx.value,ny.value)
-            sl=sl.transpose()
+    def den_plot_rgb_o2graph(self,o2scl,amp,link,args):
+        """
+        Documentation for o2graph command ``den-plot-rgb``:
 
-            if self.logx==True:
-                xgrid=[math.log(ptrx[i],10) for i in
-                       range(0,nx.value)]
-            if self.logy==True:
-                ygrid=[math.log(ptry[i],10) for i in
-                       range(0,ny.value)]
+        For objects of type ``table3d``:
 
-            if self.zset==True:
-                for i in range(0,ny.value):
-                    for j in range(0,nx.value):
-                        if sl[i][j]>self.zhi:
-                            sl[i][j]=self.zhi
-                        elif sl[i][j]<self.zlo:
-                            sl[i][j]=self.zlo
-                            
-            if self.logz==True:
-                for i in range(0,ny.value):
-                    for j in range(0,nx.value):
-                        sl[i][j]=math.log10(sl[i][j])
-                        
-            if self.canvas_flag==False:
-                self.canvas()
+        Create a density plot from a specified slice
 
-            extent1=xgrid[0]-(xgrid[1]-xgrid[0])/2
-            extent2=xgrid[nx.value-1]+(xgrid[nx.value-1]-
-                                       xgrid[nx.value-2])/2
-            extent3=ygrid[0]-(ygrid[1]-ygrid[0])/2
-            extent4=ygrid[ny.value-1]+(ygrid[ny.value-1]-
-                                       ygrid[ny.value-2])/2
-                        
-            if len(args)<1:
-                self.last_image=self.axes.imshow(sl,interpolation='nearest',
-                            origin='lower',extent=[extent1,extent2,
-                                                   extent3,extent4],
-                            aspect='auto')
-            else:
-                self.last_image=self.axes.imshow(sl,interpolation='nearest',
-                            origin='lower',extent=[extent1,extent2,
-                                                   extent3,extent4],
-                            aspect='auto',**string_to_dict(args[0]))
+        Command-line arguments: ``<slice r> <slice g> <slice b> [kwargs]``
 
-            # The color bar is added later below...
+        Create a density plot from the three specified slices. This
+        command uses imshow(). To directly create a .png file with no
+        axes, use make-png instead.
+        """
 
-            # End of section for type hist_2d
-        else:
-            print("Command 'den-plot' not supported for type",
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+        amt=acol_manager(self.link2,amp)
+
+        kwstring=''
+        if curr_type!=b'table3d':
+            print("Command 'den-plot-rgb' not supported for type",
                   curr_type,".")
             return
+            
+        slice_r=args[0]
+        slice_g=args[1]
+        slice_b=args[2]
+        if len(args)>=4:
+            kwstring=args[3]
 
-        if self.colbar==True:
-            cbar=self.fig.colorbar(self.last_image,ax=self.axes)
-            cbar.ax.tick_params('both',length=6,width=1,which='major')
-            cbar.ax.tick_params(labelsize=self.font*0.8)
+        dctt=string_to_dict(kwstring)
+        self.den_plot(amt.get_table3d_obj(),slice_r,slice_g,slice_b,
+                      **dctt)
 
-    def den_plot_rgb(self,o2scl,amp,args):
-        """
-        Density plot from a ``table3d`` object using three slices
-        to specify the red, green, and blue values.
+        return
+
+    def make_png_o2graph(self,o2scl,amp,link,args):
         """
+        Documentation for o2graph command ``make-png``:
+        
+        For objects of type ``table3d``:
 
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
+        Command-line arguments: ``<slice r> <slice g> <slice b> [kwargs]``
 
-        curr_type=o2scl_get_type(o2scl,amp)
+        Create a .png file from the three specified table3d slices.
+        This command requires pillow. To create a density-plot with
+        axes instead, use den-plot-rgb.
+        """
 
-        # Handle tensor and table3d types
-        if (curr_type==b'tensor' or curr_type==b'tensor<size_t>' or
-            curr_type==b'tensor_grid' or curr_type==b'tensor<int>' or
-            curr_type==b'table3d'):
-
-            # If the object is a tensor, convert to a table3d
-            # object before plotting
-            if curr_type!=b'table3d':
-                index1=0
-                index2=1
-                if len(args)==1:
-                    kwstring=args[0]
-                if len(args)>=2:
-                    index1=int(args[0])
-                    index2=int(args[1])
-                if len(args)>=3:
-                    kwstring=args[2]
-                if index1+index2!=1 and index1*index2!=0:
-                    print('Indices must be "0 1" or "1 0" in',
-                          'in den-plot.')
-                    return
-                    
-                conv_fn=o2scl.o2scl_acol_tensor_to_table3d
-                conv_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,ctypes.c_int]
-                conv_fn.restype=ctypes.c_int
-                
-                conv_ret=conv_fn(amp,index1,index2)
-                if conv_ret!=0:
-                    print('Automatic conversion to table3d failed.')
-                    return
-                slice_name="tensor"
-            else:
-                r_slice_name=args[0]
-                g_slice_name=args[1]
-                b_slice_name=args[2]
-                if len(args)>=4:
-                    kwstring=args[3]
-
-            # Now that we are guaranteed to have a table3d
-            # object to use, use that to create the density
-            # plot
-            get_fn=o2scl.o2scl_acol_get_slice
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr,
-                             int_ptr,double_ptr_ptr,double_ptr_ptr]
-
-            r_slice=ctypes.c_char_p(force_bytes(r_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_r=double_ptr()
-            get_fn(amp,r_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_r))
-
-            # Allocate the python storage
-            sl_all=numpy.zeros((ny.value,nx.value,3))
-            xgrid=numpy.zeros((nx.value))
-            ygrid=numpy.zeros((ny.value))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,0]=ptrs_r[ix]
-                    ix=ix+1
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+        amt=acol_manager(self.link2,amp)
 
-            # Copy the grid
-            for i in range(0,nx.value):
-                xgrid[i]=ptrx[i]
-            for j in range(0,ny.value):
-                ygrid[j]=ptry[j]
-            
-            g_slice=ctypes.c_char_p(force_bytes(g_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_g=double_ptr()
-            get_fn(amp,g_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_g))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,1]=ptrs_g[ix]
-                    ix=ix+1
+        kwstring=''
+        if curr_type!=b'table3d':
+            print("Command 'make-png' not supported for type",
+                  curr_type,".")
+            return
             
-            b_slice=ctypes.c_char_p(force_bytes(b_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_b=double_ptr()
-            get_fn(amp,b_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_b))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,2]=ptrs_b[ix]
-                    ix=ix+1
+        slice_r=args[0]
+        slice_g=args[1]
+        slice_b=args[2]
+        fname=args[3]
+        if len(args)>=5:
+            kwstring=args[4]
+
+        dctt=string_to_dict(kwstring)
+        renorm=dctt.pop('renorm',False)
 
+        try:
+            self.den_plot_rgb(amt.get_table3d_obj(),slice_r,slice_g,slice_b,
+                              make_png=fname,renorm=renorm,**dctt)
+        except Exception as e:
+            print('Exception in make_png_o2graph()',e)
+            raise
             
-            # If logz was specified, then manually apply the
-            # log to the data. Alternatively, we should consider
-            # using 'LogNorm' here, as suggested in
-            
-            # If the z range was specified, truncate all values
-            # outside that range (this truncation is done after
-            # the application of the log above)
-            
-            # if self.zset==True:
-            #     for i in range(0,ny.value):
-            #         for j in range(0,nx.value):
-            #             if sl_r[i][j]>self.zhi:
-            #                 sl_r[i][j]=self.zhi
-            #             elif sl_r[i][j]<self.zlo:
-            #                 sl_r[i][j]=self.zlo
-            #             if sl_g[i][j]>self.zhi:
-            #                 sl_g[i][j]=self.zhi
-            #             elif sl_g[i][j]<self.zlo:
-            #                 sl_g[i][j]=self.zlo
-            #             if sl_b[i][j]>self.zhi:
-            #                 sl_b[i][j]=self.zhi
-            #             elif sl_b[i][j]<self.zlo:
-            #                 sl_b[i][j]=self.zlo
+        return
 
-            if self.canvas_flag==False:
-                self.canvas()
+    def kde_plot(self,o2scl,amp,args,link):
+        """Documentation for o2graph command ``kde-plot``:
+
+        For objects of type ``table``:
+
+        Plot a KDE of one column
+
+        Command-line arguments: ``<column> [plot kwargs] [kde kwargs]``
+
+        Useful plot kwargs are all the usual plotting kwargs, plus
+        x_min=0, x_max=0, y_mult=1, and n_points=201.
 
-            # The imshow() function doesn't work with a log axis, so we
-            # set the scales back to linear and manually take the log
-            self.axes.set_xscale('linear')
-            self.axes.set_yscale('linear')
+        Useful KDE kwargs are kernel='gaussian', metric='euclidean',
+        transform='unit', and bandwidth='none'.
+        """
+        curr_type=o2scl_get_type(o2scl,amp,link)
+
+        if curr_type==b'table':
             
-            if self.logx==True:
-                xgrid=[math.log(ptrx[i],10) for i in
-                       range(0,nx.value)]
-            if self.logy==True:
-                ygrid=[math.log(ptry[i],10) for i in
-                       range(0,ny.value)]
+            amt=acol_manager(link,amp)
+            tab=amt.get_table_obj()
+
+            # Copy the table data to a 2D numpy array
+            x=numpy.zeros((tab.get_nlines(),1))
+            for i in range(0,tab.get_nlines()):
+                x[i,0]=tab.get(args[0],i)
+
+            # Set defaults
+            x_min=0
+            x_max=0
+            n_points=201
+            y_mult=1
+            
+            # Convert kwargs to string so we can extract
+            # n_points, x_min, and x_max
+            dct_plot={}
+            if len(args)>=2:
+                dct_plot=string_to_dict2(args[1],
+                                         list_of_ints=['n_points'],
+                                         list_of_floats=['x_min','x_max',
+                                                         'y_mult'])
+                x_min=dct_plot.pop('x_min',0)
+                x_max=dct_plot.pop('x_max',0)
+                y_mult=dct_plot.pop('y_mult',1)
+                n_points=dct_plot.pop('n_points',201)
+
+            # If x_min and x_max are not set, then determine them,
+            # either from the plot limits or from the minimum
+            # and maximum of the data
+            if x_min>=x_max:
+                if self.xset==False:
+                    # Determine min and max of data
+                    x_min=x[0,0]
+                    x_max=x[0,0]
+                    for i in range(1,tab.get_nlines()):
+                        if x[i,0]<x_min:
+                            x_min=x[i,0]
+                        if x[i,0]>x_max:
+                            x_max=x[i,0]
+                else:
+                    x_min=self.xlo
+                    x_max=self.xhi
+            print('x_min,x_max,n_points,y_mult:',x_min,x_max,n_points,y_mult)
+
+            # Use sklearn and a reasonable guess for the bandwidth,
+            # between 1.0e-2 and 1.0e+2. Note that the KDE is
+            # rescaled by default. 
+            k=kde_sklearn()
+            bw_array=[10**(float(i)/4.0-2.0) for i in range(0,17)]
 
-            diffs_x=[xgrid[i+1]-xgrid[i] for i in range(0,len(xgrid)-1)]
-            mean_x=numpy.mean(diffs_x)
-            std_x=numpy.std(diffs_x)
-            diffs_y=[ygrid[i+1]-ygrid[i] for i in range(0,len(ygrid)-1)]
-            mean_y=numpy.mean(diffs_y)
-            std_y=numpy.std(diffs_y)
-            
-            if std_x/mean_x>1.0e-4 or std_x/mean_x>1.0e-4:
-                print('Warning in o2graph::o2graph_plotter::den_plot():')
-                print('  Nonlinearity of x or y grid is greater than '+
-                      '10^{-4}.')
-                print('  Value of std(diff_x)/mean(diff_x): %7.6e .' %
-                      (std_x/mean_x))
-                print('  Value of std(diff_y)/mean(diff_y): %7.6e .' %
-                      (std_y/mean_y))
-                print('  The density plot may not be properly scaled.')
-                
-            extent1=xgrid[0]-(xgrid[1]-xgrid[0])/2
-            extent2=xgrid[nx.value-1]+(xgrid[nx.value-1]-
-                                       xgrid[nx.value-2])/2
-            extent3=ygrid[0]-(ygrid[1]-ygrid[0])/2
-            extent4=ygrid[ny.value-1]+(ygrid[ny.value-1]-
-                                       ygrid[ny.value-2])/2
-                        
-            f=self.axes.imshow
-            if len(kwstring)==0:
-                self.last_image=f(sl_all,
-                                  interpolation='nearest',
-                                  origin='lower',extent=[extent1,extent2,
-                                                         extent3,extent4],
-                                  aspect='auto')
+            # Set the KDE
+            if len(args)>=3:
+                k.set_data_str(x,bw_array,args[2])
             else:
-                self.last_image=f(sl_all,
-                                  interpolation='nearest',
-                                  origin='lower',extent=[extent1,extent2,
-                                                         extent3,extent4],
-                                  aspect='auto',
-                                  **string_to_dict(kwstring))
+                k.set_data_str(x,bw_array,'')
 
-            # The color bar is added later below...
+            # Use the new KDE to create x and y-arrays
+            xa=[]
+            ya=[]
+            xp=x_min
+            for i in range(0,n_points):
+                xa.append(xp)
+                ya.append(k.pdf([xp])*y_mult)
+                xp=xp+(x_max-x_min)/float(n_points-1)
 
-            # End of section for tensor types and table3d
+            # Plot
+            if len(args)<2:
+                self.plot([xa,ya])
+            else:
+                self.plot([xa,ya],**dct_plot)
+                
         else:
-            print("Command 'den-plot-rgb' not supported for type",
+            print("Command 'kde-plot' not supported for type",
                   curr_type,".")
             return
+        
+        # End of function o2graph_plotter::plot_o2graph()
+        return
 
-        if self.colbar==True:
-            cbar=self.fig.colorbar(self.last_image,ax=self.axes)
-            cbar.ax.tick_params('both',length=6,width=1,which='major')
-            cbar.ax.tick_params(labelsize=self.font*0.8)
+    def kde_2d_plot(self,o2scl,amp,args,link):
+        """Documentation for o2graph command ``kde-2d-plot``:
 
-    def make_png(self,o2scl,amp,args):
-        """
-        Create png from a ``table3d`` object using three slices
-        to specify the red, green, and blue values.
-        """
+        For objects of type ``table``:
 
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
+        Plot a KDE of two columns
 
-        curr_type=o2scl_get_type(o2scl,amp)
+        Command-line arguments: ``<column x> <column y> [options]``
 
-        # Handle tensor and table3d types
-        if (curr_type==b'tensor' or curr_type==b'tensor<size_t>' or
-            curr_type==b'tensor_grid' or curr_type==b'tensor<int>' or
-            curr_type==b'table3d'):
-
-            # If the object is a tensor, convert to a table3d
-            # object before plotting
-            if curr_type!=b'table3d':
-                index1=0
-                index2=1
-                if len(args)==1:
-                    kwstring=args[0]
-                if len(args)>=2:
-                    index1=int(args[0])
-                    index2=int(args[1])
-                if index1+index2!=1 and index1*index2!=0:
-                    print('Indices must be "0 1" or "1 0" in',
-                          'in den-plot.')
-                    return
-                    
-                conv_fn=o2scl.o2scl_acol_tensor_to_table3d
-                conv_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,ctypes.c_int]
-                conv_fn.restype=ctypes.c_int
-                
-                conv_ret=conv_fn(amp,index1,index2)
-                if conv_ret!=0:
-                    print('Automatic conversion to table3d failed.')
-                    return
-                slice_name="tensor"
-            else:
-                r_slice_name=args[0]
-                g_slice_name=args[1]
-                b_slice_name=args[2]
-
-            # Now that we are guaranteed to have a table3d
-            # object to use, use that to create the density
-            # plot
-            get_fn=o2scl.o2scl_acol_get_slice
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr,
-                             int_ptr,double_ptr_ptr,double_ptr_ptr]
-
-            r_slice=ctypes.c_char_p(force_bytes(r_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_r=double_ptr()
-            get_fn(amp,r_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_r))
-
-            # Allocate the python storage
-            sl_all=numpy.zeros((ny.value,nx.value,3))
-            xgrid=numpy.zeros((nx.value))
-            ygrid=numpy.zeros((ny.value))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,0]=ptrs_r[ix]
-                    ix=ix+1
+        Desc.
+        """
+        curr_type=o2scl_get_type(o2scl,amp,link)
 
-            # Copy the grid
-            for i in range(0,nx.value):
-                xgrid[i]=ptrx[i]
-            for j in range(0,ny.value):
-                ygrid[j]=ptry[j]
-            
-            g_slice=ctypes.c_char_p(force_bytes(g_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_g=double_ptr()
-            get_fn(amp,g_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_g))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,1]=ptrs_g[ix]
-                    ix=ix+1
+        if curr_type==b'table':
             
-            b_slice=ctypes.c_char_p(force_bytes(b_slice_name))
-            nx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ny=ctypes.c_int(0)
-            ptry=double_ptr()
-            ptrs_b=double_ptr()
-            get_fn(amp,b_slice,ctypes.byref(nx),ctypes.byref(ptrx),
-                   ctypes.byref(ny),ctypes.byref(ptry),
-                   ctypes.byref(ptrs_b))
-
-            # Copy from the C pointer to the python storage
-            ix=0
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    sl_all[j,i,2]=ptrs_b[ix]
-                    ix=ix+1
+            amt=acol_manager(link,amp)
+            tab=amt.get_table_obj()
 
-            
-            # If logz was specified, then manually apply the
-            # log to the data. Alternatively, we should consider
-            # using 'LogNorm' here, as suggested in
-            
-            # If the z range was specified, truncate all values
-            # outside that range (this truncation is done after
-            # the application of the log above)
-            
-            # if self.zset==True:
-            #     for i in range(0,ny.value):
-            #         for j in range(0,nx.value):
-            #             if sl_r[i][j]>self.zhi:
-            #                 sl_r[i][j]=self.zhi
-            #             elif sl_r[i][j]<self.zlo:
-            #                 sl_r[i][j]=self.zlo
-            #             if sl_g[i][j]>self.zhi:
-            #                 sl_g[i][j]=self.zhi
-            #             elif sl_g[i][j]<self.zlo:
-            #                 sl_g[i][j]=self.zlo
-            #             if sl_b[i][j]>self.zhi:
-            #                 sl_b[i][j]=self.zhi
-            #             elif sl_b[i][j]<self.zlo:
-            #                 sl_b[i][j]=self.zlo
-
-
-            from PIL import Image
-            im=Image.new(mode='RGB',size=(nx.value,ny.value))
-            pixels=im.load()
-            
-            min_val=sl_all[0,0,0]
-            max_val=sl_all[0,0,0]
-            
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    if sl_all[j,i,0]<min_val:
-                        min_val=sl_all[j,i,0]
-                    if sl_all[j,i,1]<min_val:
-                        min_val=sl_all[j,i,1]
-                    if sl_all[j,i,2]<min_val:
-                        min_val=sl_all[j,i,2]
-                    if sl_all[j,i,0]>max_val:
-                        max_val=sl_all[j,i,0]
-                    if sl_all[j,i,1]>max_val:
-                        max_val=sl_all[j,i,1]
-                    if sl_all[j,i,2]>max_val:
-                        max_val=sl_all[j,i,2]
-
-            print('o2graph::make-png(): Minimum is',
-                  min_val,'maximum is',max_val,'.')
-                        
-            for i in range(0,nx.value):
-                for j in range(0,ny.value):
-                    pixels[i,j]=(int(256*(sl_all[j,i,0]-min_val)/
-                                     (max_val-min_val)),
-                                 int(256*(sl_all[j,i,1]-min_val)/
-                                     (max_val-min_val)),
-                                 int(256*(sl_all[j,i,2]-min_val)/
-                                     (max_val-min_val)))
+            # Copy the table data to a numpy array
+            x=numpy.zeros((tab.get_nlines(),2))
+            for i in range(0,tab.get_nlines()):
+                x[i,0]=tab.get(args[0],i)
+                x[i,1]=tab.get(args[1],i)
+
+            x0_min=x[0,0]
+            x0_max=x[0,0]
+            x1_min=x[0,1]
+            x1_max=x[0,1]
+            for i in range(1,tab.get_nlines()):
+                if x[i,0]<x0_min:
+                    x0_min=x[i,0]
+                if x[i,0]>x0_max:
+                    x0_max=x[i,0]
+                if x[i,1]<x1_min:
+                    x1_min=x[i,1]
+                if x[i,1]>x1_max:
+                    x1_max=x[i,1]
+                
+            k=kde_sklearn()
+            bw_array=[10**(float(i)/4.0-2.0) for i in range(0,17)]
 
-            im.save(args[3])
-            
-            # End of section for tensor types and table3d
+            if len(args)>2:
+                k.set_data_str(x,bw_array,args[1])
+            else:
+                k.set_data_str(x,bw_array,'')
+
+            x0a=[]
+            x0p=x0_min
+            for i in range(0,201):
+                x0a.append(x0p)
+                x0p=x0p+(x0_max-x0_min)/200.0
+            x1a=[]
+            x1p=x1_min
+            for i in range(0,201):
+                x1a.append(x1p)
+                x1p=x1p+(x1_max-x1_min)/200.0
+            z=numpy.zeros((200,200))
+            for i in range(0,201):
+                for j in range(0,201):
+                    z[i,j]=k.pdf([x0a[i],x1a[j]])
+
+            if len(args)<3:
+                self.den_plot([x0a,x1a,z])
+            else:
+                self.den_plot([x0a,x1a,z],**string_to_dict(args[2]))
+                
         else:
-            print("Command 'make-png' not supported for type",
+            print("Command 'kde-2d-plot' not supported for type",
                   curr_type,".")
-            
+            return
+        
+        # End of function o2graph_plotter::plot_o2graph()
         return
 
-    def plot(self,o2scl,amp,args,link):
-        """
-        Plot a two-dimensional set of data
+    def plot_o2graph(self,o2scl,amp,args,link):
+        """Documentation for o2graph command ``plot``:
+
+        For objects of type ``table``:
+
+        Plot two columns.
+
+        Command-line arguments: ``<x> <y> [kwargs]``
+
+        Plot column <y> versus
+        column <x>. Some useful kwargs are color (c), dashes,
+        linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms). For example:
+        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
+        lw=0,marker='+' -show\". This command uses the matplotlib
+        plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``vec_vec_double``:
+
+        Plot one or two columns.
+
+        Command-line arguments: ``<x index> [y index or 'none'] [kwargs]``
+
+        Plot vector with index [index y] versus vector with index
+        <index x>. Alternatively, if the second argument is the
+        string 'none', plot the vector with index <index x>.
+        Some useful kwargs are color (c), dashes, linestyle
+        (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms). For example:
+        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
+        lw=0,marker='+' -show\". This command uses the matplotlib
+        plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``hist``:
+
+        Plot the histogram
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the histogram weights as a function of the bin
+        representative values. Some useful kwargs (which apply for all
+        three object types) are color (c), dashes, linestyle (ls),
+        linewidth (lw), marker, markeredgecolor (mec), markeredgewidth
+        (mew), markerfacecolor (mfc), markerfacecoloralt (mfcalt),
+        markersize (ms). For example: \"o2graph -create x 0 10 0.2
+        -function sin(x) y -plot x y lw=0,marker='+' -show\". This
+        command uses the matplotlib plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``vector<contour_line>``:
+
+        Plot the contour lines.
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the set of contour lines. Some useful kwargs (which apply
+        for all three object types) are color (c), dashes, linestyle
+        (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms). For example:
+        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
+        lw=0,marker='+' -show\". This command uses the matplotlib
+        plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``prob_dens_mdim_amr``:
+
+        Plot the probability distribution.
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the set of contour lines. Some useful kwargs (which apply
+        for all three object types) are color (c), dashes, linestyle
+        (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms). For example:
+        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
+        lw=0,marker='+' -show\". This command uses the matplotlib
+        plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
         """
 
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
-                            
-            failed=False
-
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            # colx=ctypes.c_char_p(force_bytes(args[0]))
-            # idx=ctypes.c_int(0)
-            # ptrx=double_ptr()
-            # get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
-            # if get_ret!=0:
-            #     print('Failed to get column named "'+args[0]+'".')
-            #     failed=True
-
-            amt=acol_manager(link,amp)
+            
+            amt=acol_manager(self.link2,amp)
             tab=amt.get_table_obj()
-            xv=tab[force_bytes(args[0])]
-
-            coly=ctypes.c_char_p(force_bytes(args[1]))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[1]+'".')
-                failed=True
+            
+            if len(args)<3:
+                self.plot([tab,args[0],args[1]])
+            else:
+                self.plot([tab,args[0],args[1]],**string_to_dict(args[2]))
 
-            if failed==False:
-                #xv=[ptrx[i] for i in range(0,idx.value)]
-                yv=[ptry[i] for i in range(0,idy.value)]
-        
-                if self.canvas_flag==False:
-                    self.canvas()
-                if self.logx==True:
-                    if self.logy==True:
-                        if len(args)<3:
-                            self.axes.loglog(xv,yv)
-                        else:
-                            self.axes.loglog(xv,yv,**string_to_dict(args[2]))
-                    else:
-                        if len(args)<3:
-                            self.axes.semilogx(xv,yv)
-                        else:
-                            self.axes.semilogx(xv,yv,**string_to_dict(args[2]))
-                else:
-                    if self.logy==True:
-                        if len(args)<3:
-                            self.axes.semilogy(xv,yv)
-                        else:
-                            self.axes.semilogy(xv,yv,**string_to_dict(args[2]))
-                    else:
-                        if len(args)<3:
-                            self.axes.plot(xv,yv)
-                        else:
-                            self.axes.plot(xv,yv,**string_to_dict(args[2]))
+            failed=False
 
             # End of section for 'table' type
-        elif curr_type==b'hist':
+            
+        elif curr_type==b'vec_vec_double':
+            
+            amt=acol_manager(self.link2,amp)
+            vvd=amt.get_vvdouble_obj()
+            
+            if len(args)<2 or args[1]=='none':
+                self.plot([vvd,int(args[0])])
+            elif len(args)<3:
+                self.plot([vvd,int(args[0]),int(args[1])])
+            else:
+                self.plot([vvd,int(args[0]),int(args[1])],
+                          **string_to_dict(args[2]))
 
-            get_reps_fn=o2scl.o2scl_acol_get_hist_reps
-            get_reps_fn.argtypes=[ctypes.c_void_p,
-                             int_ptr,double_ptr_ptr]
-                            
-            get_wgts_fn=o2scl.o2scl_acol_get_hist_wgts
-            get_wgts_fn.argtypes=[ctypes.c_void_p,
-                             int_ptr,double_ptr_ptr]
-                            
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_reps_fn(amp,ctypes.byref(idx),
-                        ctypes.byref(ptrx))
-
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_wgts_fn(amp,ctypes.byref(idy),
-                        ctypes.byref(ptry))
+            failed=False
 
-            xv=[ptrx[i] for i in range(0,idx.value)]
-            yv=[ptry[i] for i in range(0,idy.value)]
-    
-            if self.canvas_flag==False:
-                self.canvas()
-            if self.logx==True:
-                if self.logy==True:
-                    if len(args)<1:
-                        self.axes.loglog(xv,yv)
-                    else:
-                        self.axes.loglog(xv,yv,**string_to_dict(args[0]))
-                else:
-                    if len(args)<1:
-                        self.axes.semilogx(xv,yv)
-                    else:
-                        self.axes.semilogx(xv,yv,**string_to_dict(args[0]))
+            # End of section for 'vec_vec_double' type
+            
+        elif curr_type==b'hist':
+
+            amt=acol_manager(self.link2,amp)
+            hist=amt.get_hist_obj()
+            
+            if len(args)<3:
+                self.plot([hist,self.link2])
             else:
-                if self.logy==True:
-                    if len(args)<1:
-                        self.axes.semilogy(xv,yv)
-                    else:
-                        self.axes.semilogy(xv,yv,**string_to_dict(args[0]))
-                else:
-                    if len(args)<1:
-                        self.axes.plot(xv,yv)
-                    else:
-                        self.axes.plot(xv,yv,**string_to_dict(args[0]))
-                            
+                self.plot([hist,self.link2],**string_to_dict(args[0]))
+
+            failed=False
+            
             # End of section for 'hist' type
         elif curr_type==b'prob_dens_mdim_amr':
 
-            get_base_fn=o2scl.o2scl_acol_pdma_get_base
-            get_base_fn.argtypes=[ctypes.c_void_p,int_ptr,
-                                  int_ptr,double_ptr_ptr,double_ptr_ptr]
-                            
-            get_cube_fn=o2scl.o2scl_acol_pdma_get_cube
-            get_cube_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                                  double_ptr_ptr,double_ptr_ptr,
-                                  double_ptr,double_ptr]
-                            
-            ndimx=ctypes.c_int(0)
-            nx=ctypes.c_int(0)
-            lowx=double_ptr()
-            highx=double_ptr()
-            get_base_fn(amp,ctypes.byref(ndimx),ctypes.byref(nx),
-                        ctypes.byref(lowx),ctypes.byref(highx))
+            amt=acol_manager(self.link2,amp)
+            pdma=amt.get_pdma_obj()
+            ndimx=pdma.n_dim
+            mesh=pdma.get_mesh()
+            nx=mesh.size()
+            lowx=pdma.get_low()
+            highx=pdma.get_high()
 
+            if len(args)<2:
+                print('Not enough arguments to plot for an object',
+                      'of type prob_dens_mdim_amr.')
+            
             dimx=int(args[0])
             dimy=int(args[1])
 
             self.xlo=lowx[dimx]
             self.ylo=lowx[dimy]
             self.xset=True
             self.xhi=highx[dimx]
             self.yhi=highx[dimy]
             self.yset=True
+            print('%7.6e %7.6e %7.6e %7.6e' %
+                  (self.xlo,self.ylo,self.xhi,self.yhi))
 
             if self.canvas_flag==False:
                 self.canvas()
 
             # Need to figure out here how to convert fill function
             # to a value, keeping in mind it can depend on
             # fvy.value (fractional volume) or wy.value (weight)
                 
             fill_fn='None'
             if len(args)>=3:
                 fill_fn=args[2]
                 
             print('Fill function',fill_fn)
                 
-            for i in range(0,nx.value):
+            import matplotlib.patches as patches
 
-                iy=ctypes.c_int(i)
-                lowy=double_ptr()
-                highy=double_ptr()
-                fvy=ctypes.c_double(0.0)
-                wy=ctypes.c_double(0.0)
-                get_cube_fn(amp,iy,ctypes.byref(lowy),
-                            ctypes.byref(highy),
-                            ctypes.byref(fvy),
-                            ctypes.byref(wy))
-                
-                left=lowy[dimx]
-                lower=lowy[dimy]
-                right=highy[dimx]
-                upper=highy[dimy]
+            for i in range(0,nx):
+
+                m2=mesh[i]
+                low2=m2.get_low()
+                high2=m2.get_high()
+                left=low2[dimx]
+                lower=low2[dimy]
+                right=high2[dimx]
+                upper=high2[dimy]
+                fvy=m2.frac_vol
+                wy=m2.weight
                 w=right-left
                 h=upper-lower
+                print('%d %7.6e %7.6e %7.6e %7.6e %7.6e %7.6e' %
+                      (i,left,lower,w,h,fvy,wy))
 
                 if len(args)<4:
                     r=patches.Rectangle((left,lower),w,h,0.0,
-                                        alpha=fvy.value)
+                                        alpha=1,fill=None,lw=1)
                     self.axes.add_patch(r)
                 else:
                     strtemp='alpha='+str(fvy.value)+','+args[3]
                     r=patches.Rectangle((left,lower),w,h,0.0,
                                         **string_to_dict(strtemp))
                     self.axes.add_patch(r)
                             
             # End of section for 'prob_dens_mdim_amr' type
         elif curr_type==b'vector<contour_line>':
 
-            # Get the total number of contour lines
-            cont_n_fn=o2scl.o2scl_acol_contours_n
-            cont_n_fn.argtypes=[ctypes.c_void_p]
-            cont_n_fn.restype=ctypes.c_int
-            nconts=cont_n_fn(amp)
-
-            # Define types for extracting each contour line
-            cont_line_fn=o2scl.o2scl_acol_contours_line
-            cont_line_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                                   int_ptr,double_ptr_ptr,
-                                   double_ptr_ptr]
-            cont_line_fn.restype=ctypes.c_double
+            amt=acol_manager(self.link2,amp)
+            vcl=amt.get_cont_obj()
+            nconts=vcl.size()
 
             if self.canvas_flag==False:
                 self.canvas()
 
             # Loop over all contour lines
             for k in range(0,nconts):
-                idx=ctypes.c_int(0)
-                ptrx=double_ptr()
-                ptry=double_ptr()
-                lev=cont_line_fn(amp,k,ctypes.byref(idx),
-                                 ctypes.byref(ptrx),ctypes.byref(ptry))
-                xv=[ptrx[i] for i in range(0,idx.value)]
-                yv=[ptry[i] for i in range(0,idx.value)]
+
+                cl=vcl[k]
+                xv=cl.get_x().to_numpy()
+                yv=cl.get_y().to_numpy()
                 
                 if self.logx==True:
                     if self.logy==True:
-                        if len(args)<1:
+                        if len(args)<2:
                             self.axes.loglog(xv,yv)
                         else:
                             self.axes.loglog(xv,yv,**string_to_dict(args[0]))
                     else:
                         if len(args)<1:
                             self.axes.semilogx(xv,yv)
                         else:
@@ -1093,86 +1554,73 @@
                         else:
                             self.axes.semilogy(xv,yv,**string_to_dict(args[0]))
                     else:
                         if len(args)<1:
                             self.axes.plot(xv,yv)
                         else:
                             self.axes.plot(xv,yv,**string_to_dict(args[0]))
+                            
             # End of section for 'vector<contour_line>' type
         else:
             print("Command 'plot' not supported for type",
                   curr_type,".")
             return
-        
-        if self.xset==True:
-            self.axes.set_xlim(self.xlo,self.xhi)
-        if self.yset==True:
-            self.axes.set_ylim(self.ylo,self.yhi)
+
+        # AWS, Commented out on 5/3/23
+        #if self.xset==True:
+        #self.axes.set_xlim(self.xlo,self.xhi)
+        #if self.yset==True:
+        #    self.axes.set_ylim(self.ylo,self.yhi)
                                  
-        # End of function o2graph_plotter::plot()
+        # End of function o2graph_plotter::plot_o2graph()
         return
                                  
-    def plot_color(self,o2scl,amp,args):
-        """
-        Plot a set of line segments, coloring according to a third 
-        variable.
+    def plot_color(self,o2scl,amp,link,args):
         """
+        Documentation for o2graph command ``plot-color``:
 
+        For objects of type ``table``:
+
+        Plot three columns, using the third for the color
+
+        Command-line arguments: ``<x> <y> <c> <cmap> [kwargs]``
+
+        Plot column <y> versus
+        column <x> using column <c> to specify the line color.
+        Some useful kwargs are color (c), dashes,
+        linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms). For example:
+        \"o2graph -create x 0 10 0.2 -function sin(x) y -plot x y
+        lw=0,marker='+' -show\". This command uses the matplotlib
+        plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+        """
+        
         if len(args)<4:
             raise ValueError('Function plot_color() requires four values '+
                              'for the args list.')
         
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
                             
             failed=False
 
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            colx=ctypes.c_char_p(force_bytes(args[0]))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
-
-            coly=ctypes.c_char_p(force_bytes(args[1]))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[1]+'".')
-                failed=True
-
-            colz=ctypes.c_char_p(force_bytes(args[2]))
-            idz=ctypes.c_int(0)
-            ptrz=double_ptr()
-            get_ret=get_fn(amp,colz,ctypes.byref(idz),ctypes.byref(ptrz))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[2]+'".')
-                failed=True
-
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            xv=tab[force_bytes(args[0])]
+            yv=tab[force_bytes(args[1])]
+            zv=tab[force_bytes(args[2])]
+            
             cmap=args[3]
 
             if failed==False:
-                xv=[ptrx[i] for i in range(0,idx.value)]
-                yv=[ptry[i] for i in range(0,idy.value)]
-                zv=[ptrz[i] for i in range(0,idz.value)]
 
                 if self.logx:
                     for i in range(0,len(xv)):
                         xv[i]=math.log10(xv)
                 if self.logy:
                     for i in range(0,len(yv)):
                         yv[i]=math.log10(yv)
@@ -1201,16 +1649,15 @@
                     else:
                         self.axes.plot([xv[i],xv[i+1]],
                                        [yv[i],yv[i+1]],
                                        color=col,
                                        **string_to_dict(args[4]))
 
                 if self.colbar==True:
-                    cbar=self.fig.colorbar(mapper,
-                                           ax=self.axes)
+                    cbar=self.fig.colorbar(mapper,ax=self.axes)
                     cbar.ax.tick_params('both',length=6,width=1,which='major')
                     cbar.ax.tick_params(labelsize=self.font*0.8)
                     
             # End of section for 'table' type
         else:
             print("Command 'plot' not supported for type",
                   curr_type,".")
@@ -1220,183 +1667,130 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::plot_color()
         return
                                  
-    def rplot(self,o2scl,amp,args):
+    def rplot(self,o2scl,amp,link,args):
         """
-        Plot a region inside a curve or in between two curves
+        Documentation for o2graph command ``rplot``:
+
+        For objects of type ``table``:
+
+        Plot a region inside a column or in between two columns.
+
+        Command-line arguments: ``<x1> <y1> [x2 y2] [kwargs]``
+
+        If either 2 or 3 arguments are specified, this command plots
+        the region inside the curve defined by the specified set of x
+        and y values. The first point is copied at the end to ensure a
+        closed region. If 4 or 5 arguments are specified, then this
+        command plots the region in between two sets of x and y
+        values, again adding the first point from (x1,y1) to the end
+        to ensure a closed region.
         """
 
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
                             
             failed=False
 
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            colx1=ctypes.c_char_p(force_bytes(args[0]))
-            idx1=ctypes.c_int(0)
-            ptrx1=double_ptr()
-            get_ret=get_fn(amp,colx1,ctypes.byref(idx1),ctypes.byref(ptrx1))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
-
-            coly1=ctypes.c_char_p(force_bytes(args[1]))
-            idy1=ctypes.c_int(0)
-            ptry1=double_ptr()
-            get_ret=get_fn(amp,coly1,ctypes.byref(idy1),ctypes.byref(ptry1))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[1]+'".')
-                failed=True
-
-            if failed==False:
-                xv=[ptrx1[i] for i in range(0,idx1.value)]
-                yv=[ptry1[i] for i in range(0,idy1.value)]
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            xv=tab[force_bytes(args[0])]
+            yv=tab[force_bytes(args[1])]
                 
             if len(args)>3:
-                colx2=ctypes.c_char_p(force_bytes(args[2]))
-                idx2=ctypes.c_int(0)
-                ptrx2=double_ptr()
-                get_ret=get_fn(amp,colx2,ctypes.byref(idx2),ctypes.byref(ptrx2))
-                if get_ret!=0:
-                    print('Failed to get column named "'+args[2]+'".')
-                    failed=True
-
-                coly2=ctypes.c_char_p(force_bytes(args[3]))
-                idy2=ctypes.c_int(0)
-                ptry2=double_ptr()
-                get_ret=get_fn(amp,coly2,ctypes.byref(idy2),ctypes.byref(ptry2))
-                if get_ret!=0:
-                    print('Failed to get column named "'+args[3]+'".')
-                    failed=True
-
-                if failed==False:
-                    for i in range(0,idx2.value):
-                        xv.append(ptrx2[idx2.value-1-i])
-                        yv.append(ptry2[idy2.value-1-i])
+                zv=tab[force_bytes(args[2])]
+                wv=tab[force_bytes(args[3])]
+
+                for i in range(0,len(zv)):
+                    xv=numpy.append(xv,zv[len(zv)-1-i])
+                    yv=numpy.append(yv,wv[len(wv)-1-i])
 
-            if failed==False:
                 # Make sure the loop is closed
-                xv.append(ptrx1[0])
-                yv.append(ptry1[0])
+                xv=numpy.append(xv,zv[0])
+                yv=numpy.append(yv,wv[0])
         
-                if self.canvas_flag==False:
-                    self.canvas()
-                if len(args)==3:
-                    self.axes.fill(xv,yv,**string_to_dict(args[2]))
-                elif len(args)==5:
-                    self.axes.fill(xv,yv,**string_to_dict(args[4]))
-                else:
-                    self.axes.fill(xv,yv)
+            if self.canvas_flag==False:
+                self.canvas()
+            if len(args)==3:
+                self.axes.fill(xv,yv,**string_to_dict(args[2]))
+            elif len(args)==5:
+                self.axes.fill(xv,yv,**string_to_dict(args[4]))
+            else:
+                self.axes.fill(xv,yv)
 
-                if self.logx==True:
-                    self.axes.set_xscale('log')
-                if self.logy==True:
-                    self.axes.set_yscale('log')
+            if self.logx==True:
+                self.axes.set_xscale('log')
+            if self.logy==True:
+                self.axes.set_yscale('log')
                     
-                if self.xset==True:
-                    self.axes.set_xlim(self.xlo,self.xhi)
-                if self.yset==True:
-                    self.axes.set_ylim(self.ylo,self.yhi)
+            if self.xset==True:
+                self.axes.set_xlim(self.xlo,self.xhi)
+            if self.yset==True:
+                self.axes.set_ylim(self.ylo,self.yhi)
                                  
             # End of section for 'table' type
         else:
             print("Command 'rplot' not supported for type",
                   curr_type,".")
             return
         
         # End of function o2graph_plotter::rplot()
         return
                                  
-    def scatter(self,o2scl,amp,args):
+    def scatter(self,o2scl,amp,link,args):
         """
-        Generate a scatter plot.
+        Documentation for o2graph command ``scatter``:
+
+        For objects of type ``table``:
+
+        Create a scatter plot from 2-4 columns.
+
+        Command-line arguments: ``<x> <y> [s] [c] [kwargs]``
+
+        This command creates a scatter plot form columns <x> and <y>,
+        optionally using column [s] to choose the marker size and
+        optionally using column [c] to choose the marker color. To
+        vary the marker colors while choosing the default marker size
+        just specify 'None' as the argument for [s]. Or, to specify
+        keyword arguments while using the default size and color,
+        specify 'None' as the argument for both [s] and [c].
+
         """
 
-        import matplotlib.pyplot as plot
+        if self.verbose>1:
+            print('In o2graph_plotter::scatter().')
         
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
+        import matplotlib.pyplot as plot
         
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
                             
             failed=False
 
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            colx=ctypes.c_char_p(force_bytes(args[0]))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
-
-            coly=ctypes.c_char_p(force_bytes(args[1]))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[1]+'".')
-                failed=True
-
-            if failed==False:
-                xv=[ptrx[i] for i in range(0,idx.value)]
-                yv=[ptry[i] for i in range(0,idy.value)]
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            xv=tab[force_bytes(args[0])]
+            yv=tab[force_bytes(args[1])]
 
             sv=[]
             cv=[]
 
             if (len(args)>2 and force_bytes(args[2])!=b'None' and
                 force_bytes(args[2])!=b'none'):
-                cols=ctypes.c_char_p(force_bytes(args[2]))
-                ids=ctypes.c_int(0)
-                ptrs=double_ptr()
-                get_ret=get_fn(amp,cols,ctypes.byref(ids),ctypes.byref(ptrs))
-                if get_ret!=0:
-                    print('Failed to get column named "'+args[2]+'".')
-                    failed=True
-                else:
-                    sv=[ptrs[i] for i in range(0,ids.value)]
+                sv=tab[force_bytes(args[2])]
 
             if (len(args)>3 and force_bytes(args[3])!=b'None' and
                 force_bytes(args[3])!=b'none'):
-                colc=ctypes.c_char_p(force_bytes(args[3]))
-                idc=ctypes.c_int(0)
-                ptrc=double_ptr()
-                get_ret=get_fn(amp,colc,ctypes.byref(idc),ctypes.byref(ptrc))
-                if get_ret!=0:
-                    print('Failed to get column named "'+args[3]+'".')
-                    failed=True
-                else:
-                    cv=[ptrc[i] for i in range(0,idc.value)]
+                cv=tab[force_bytes(args[3])]
 
             if failed==False:
                 
                 if self.canvas_flag==False:
                     self.canvas()
                 ft=self.axes.scatter
                 if len(sv)>0:
@@ -1450,85 +1844,74 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::scatter()
         return
                                  
-    def hist_plot(self,o2scl,amp,args):
-        """
-        Plot a histogram.
+    def hist_plot(self,o2scl,amp,link,args):
         """
+        Documentation for o2graph command ``hist-plot``:
+
+        For objects of type ``table``:
+
+        Create a histogram plot from a column in a table
+
+        Command-line arguments: ``<col> [kwargs]``
 
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
+        For a table, create a histogram plot from the specified
+        column. This command uses matplotlib to construct the
+        histogram rather than using O2scl to create a histogram
+        object. This command uses the matplotlib hist() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html
+        for information and keyword arguments.
+
+        For objects of type ``hist``:
+
+        Create a histogram plot from the current histogram.
         
-        curr_type=o2scl_get_type(o2scl,amp)
+        Command-line arguments: ``[kwargs]``
+
+        Create a histogram plot from the current histogram. This
+        command uses the matplotlib hist() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html
+        for information and keyword arguments.
+        """
+
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
-                            
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            colx=ctypes.c_char_p(force_bytes(args[0]))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
+
             failed=False
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
+                
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            xv=tab[force_bytes(args[0])]
 
             if failed==False:
-                xv=[ptrx[i] for i in range(0,idx.value)]
         
                 if self.canvas_flag==False:
                     self.canvas()
                 if len(args)<2:
                     self.axes.hist(xv)
                 else:
                     self.axes.hist(xv,**string_to_dict(args[1]))
 
         elif curr_type==b'hist':
                     
-            get_reps_fn=o2scl.o2scl_acol_get_hist_reps
-            get_reps_fn.argtypes=[ctypes.c_void_p,
-                             int_ptr,double_ptr_ptr]
-                            
-            get_wgts_fn=o2scl.o2scl_acol_get_hist_wgts
-            get_wgts_fn.argtypes=[ctypes.c_void_p,
-                             int_ptr,double_ptr_ptr]
-                            
-            get_bins_fn=o2scl.o2scl_acol_get_hist_bins
-            get_bins_fn.argtypes=[ctypes.c_void_p,
-                             int_ptr,double_ptr_ptr]
-                            
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_reps_fn(amp,ctypes.byref(idx),
-                        ctypes.byref(ptrx))
-            xv=[ptrx[i] for i in range(0,idx.value)]
-
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_wgts_fn(amp,ctypes.byref(idy),
-                        ctypes.byref(ptry))
-            yv=[ptry[i] for i in range(0,idy.value)]
-
-            idz=ctypes.c_int(0)
-            ptrz=double_ptr()
-            get_bins_fn(amp,ctypes.byref(idz),
-                        ctypes.byref(ptrz))
-            zv=[ptrz[i] for i in range(0,idz.value)]
+            amt=acol_manager(self.link2,amp)
+            hist=amt.get_hist_obj()
+            wgts=hist.get_wgts()
+            reps=std_vector(self.link2)
+            hist.create_rep_vec(reps)
+            bins=hist.get_bins()
+
+            xv=reps.to_numpy()
+            yv=wgts.to_numpy()
+            zv=bins.to_numpy()
             
             if self.canvas_flag==False:
                 self.canvas()
             if len(args)<1:
                 self.axes.hist(xv,weights=yv,bins=zv)
             else:
                 self.axes.hist(xv,weights=yv,bins=zv,
@@ -1544,58 +1927,43 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::hist_plot()
         return
                                  
-    def hist2d_plot(self,o2scl,amp,args):
+    def hist2d_plot(self,o2scl,amp,link,args):
         """
-        Plot a two-dimensional histogram.
+        Documentation for o2graph command ``hist2d-plot``:
+
+        For objects of type ``table``:
+
+        Create a 2D histogram plot from two columns in a table
+
+        Command-line arguments: ``<col x> <col y> [kwargs]``
+
+        Create a 2D histogram plot from the specified columns. This
+        command uses matplotlib to construct the histogram rather than
+        using O2scl to create a hist object.
         """
 
         import matplotlib.pyplot as plot
         
-        # Useful pointer types
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
                             
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            xv=tab[force_bytes(args[0])]
+            yv=tab[force_bytes(args[1])]
 
             failed=False
 
-            colx=ctypes.c_char_p(force_bytes(args[0]))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
-            
-            coly=ctypes.c_char_p(force_bytes(args[1]))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+args[1]+'".')
-                failed=True
-
             if failed==False:
-                xv=[ptrx[i] for i in range(0,idx.value)]
-                yv=[ptry[i] for i in range(0,idy.value)]
         
                 if self.canvas_flag==False:
                     self.canvas()
                 if len(args)<3:
                     c,x,y,self.last_image=self.axes.hist2d(xv,yv)
                 else:
                     c,x,y,self.last_image=self.axes.hist2d(xv,yv,
@@ -1617,85 +1985,101 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::hist2d_plot()
         return
                                  
-    def errorbar(self,o2scl,amp,args):
-        """
-        Create a plot with error bars.
+    def errorbar(self,o2scl,amp,link,args):
+        """Documentation for o2graph command ``errorbar``:
+
+        For objects of type ``table``:
+
+        Plot the specified columns with errorbars.
+
+        Command-line arguments: ``<x> <y> <xerr> <yerr> [kwargs]``
+
+        Plot column <y> versus column <x> with symmetric error bars
+        given in column <xerr> and <yerr>. For no uncertainty in
+        either the x or y direction, just use 0 for <xerr> or <yerr>,
+        respectively.
+
+        Some useful kwargs for the errorbar command are:
+
+        ========== ================================= =============
+        keyword    description                       default value
+        ========== ================================= =============
+        ecolor     error bar color                   None
+        elinewidth error bar line width              None
+        capsize    cap size in points                None
+        barsabove  plot error bars on top of points  False
+        lolims     y value is lower limit            False
+        uplims     y value is upper limit            False
+        xlolims    x value is lower limit            False
+        xuplims    x value is upper limit            False
+        errorevery draw error bars on subset of data 1
+        capthick   thickness of error bar cap        None
+        ========== ================================= =============
+
+        For error points with no lines use, e.g. lw=0,elinewidth=1.
+        See also ``error-point`` for plotting a single point with
+        errorbars.
+
         """
 
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
                         
         if curr_type==b'table':
 
-            xv=table_get_column(o2scl,amp,args[0])
-            yv=table_get_column(o2scl,amp,args[1])
+            xv=table_get_column(o2scl,amp,self.link2,args[0])
+            yv=table_get_column(o2scl,amp,self.link2,args[1])
 
             if len(args)>=6 and args[2]=='None' or args[2]=='none':
                 if is_number(args[3]):
                     xerrv=float(args[3]);
                 else:
-                    xerrv=table_get_column(o2scl,amp,args[3])
+                    xerrv=table_get_column(o2scl,amp,self.link2,args[3])
             if len(args)>=6 and args[3]=='None' or args[3]=='none':
                 if is_number(args[2]):
                     xerrv=float(args[2]);
                 else:
-                    xerrv=table_get_column(o2scl,amp,args[2])
+                    xerrv=table_get_column(o2scl,amp,self.link2,args[2])
             elif len(args)>=6:
                 if is_number(args[2]):
                     if is_number(args[3]):
                         xerrv=[[float(args[2]),float(args[3])]
                                for i in range(0,idxerr.value)]
                     else:
-                        colxerr=ctypes.c_char_p(force_bytes(args[3]))
-                        idxerr=ctypes.c_int(0)
-                        ptrxerr=double_ptr()
-                        get_fn(amp,colxerr,ctypes.byref(idxerr),
-                               ctypes.byref(ptrxerr))
+                        ptrxerr=table_get_column(o2scl,amp,self.link2,args[3])
                         xerrv=[[float(args[2]),ptrxerr[i]] for i in
                                range(0,idxerr.value)]
                 else:
                     if is_number(args[3]):
-                        colxerr=ctypes.c_char_p(force_bytes(args[2]))
-                        idxerr=ctypes.c_int(0)
-                        ptrxerr=double_ptr()
-                        get_fn(amp,colxerr,ctypes.byref(idxerr),
-                               ctypes.byref(ptrxerr))
+                        ptrxerr=table_get_column(o2scl,amp,self.link2,args[2])
                         xerrv=[[ptrxerr[i],float(args[3])] for i in
                                range(0,idxerr.value)]
                     else:
-                        colxerr=ctypes.c_char_p(force_bytes(args[2]))
-                        idxerr=ctypes.c_int(0)
-                        ptrxerr=double_ptr()
-                        get_fn(amp,colxerr,ctypes.byref(idxerr),
-                               ctypes.byref(ptrxerr))
-                        colxerr2=ctypes.c_char_p(force_bytes(args[3]))
-                        idxerr2=ctypes.c_int(0)
-                        ptrxerr2=double_ptr()
-                        get_fn(amp,colxerr2,ctypes.byref(idxerr2),
-                               ctypes.byref(ptrxerr2))
+                        ptrxerr=table_get_column(o2scl,amp,self.link2,args[2])
+                        ptrxerr2=table_get_column(o2scl,amp,self.link2,args[3])
                         xerrv=[[ptrxerr[i],ptrxerr2[i]] for i in
                                range(0,idxerr.value)]
             else:
                 if args[2]=='None' or args[2]=='none':
                     xerrv=0.0
                 elif is_number(args[2]):
                     xerrv=float(args[2])
                 else:
-                    xerrv=table_get_column(o2scl,amp,args[2])
+                    xerrv=table_get_column(o2scl,amp,self.link2,args[2])
     
             if args[3]=='None' or args[3]=='none':
                 yerrv=0.0
             elif is_number(args[3]):
                 yerrv=float(args[3])
             else:
-                yerrv=table_get_column(o2scl,amp,args[3])
+                yerrv=table_get_column(o2scl,amp,self.link2,args[3])
 
             if self.canvas_flag==False:
                 self.canvas()
             if len(args)<5:
                 self.axes.errorbar(xv,yv,yerr=yerrv,xerr=xerrv)
             else:
                 self.axes.errorbar(xv,yv,yerr=yerrv,xerr=xerrv,
@@ -1711,90 +2095,111 @@
             self.axes.set_xlim(self.xlo,self.xhi)
         if self.yset==True:
             self.axes.set_ylim(self.ylo,self.yhi)
                                  
         # End of function o2graph_plotter::errorbar()
         return
                                  
-    def plot1(self,o2scl,amp,args):
-        """
-        Plot one array of data versus an integer x axis.
+    def plot1(self,o2scl,amp,link,args):
         """
-
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
+        Documentation for o2graph command ``plot1``:
         
-        curr_type=o2scl_get_type(o2scl,amp)
+        For objects of type ``table``:
+
+        Plot the specified column
+
+        Command-line arguments: ``<y> [kwargs]``
+
+        Plot column <y> versus row number. Some useful kwargs are
+        color (c), dashes, linestyle (ls), linewidth (lw), marker,
+        markeredgecolor (mec), markeredgewidth (mew), markerfacecolor
+        (mfc), markerfacecoloralt (mfcalt), markersize (ms). For
+        example: \"o2graph -create x 0 10 0.2 -function sin(x) y
+        -plot1 y ls='--',marker='o' -show\". This command uses the
+        matplotlib plot() function, see
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``double[]``:
+
+        Plot the array.
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the array. Some useful kwargs are color (c), dashes,
+        linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms).
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``int[]``:
+
+        Plot the array.
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the array. Some useful kwargs are color (c), dashes,
+        linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms).
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        For objects of type ``size_t[]``:
+
+        Plot the array.
+
+        Command-line arguments: ``[kwargs]``
+
+        Plot the array. Some useful kwargs are color (c), dashes,
+        linestyle (ls), linewidth (lw), marker, markeredgecolor (mec),
+        markeredgewidth (mew), markerfacecolor (mfc),
+        markerfacecoloralt (mfcalt), markersize (ms).
+        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
+        for information and keyword arguments. This command does not
+        yet support the matplotlib format parameter.
+
+        """
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+        amt=acol_manager(self.link2,amp)
                         
-        if curr_type==b'table':
+        failed=False
             
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            colx=ctypes.c_char_p(force_bytes(args[0]))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),ctypes.byref(ptrx))
-            failed=False
-            if get_ret!=0:
-                print('Failed to get column named "'+args[0]+'".')
-                failed=True
+        if curr_type==b'table':
 
-            if failed==False:
-                xv=[i for i in range(0,idx.value)]
-                yv=[ptrx[i] for i in range(0,idx.value)]
-        
-                if self.canvas_flag==False:
-                    self.canvas()
-                if self.logx==True:
-                    if self.logy==True:
-                        if len(args)<2:
-                            self.axes.loglog(xv,yv)
-                        else:
-                            self.axes.loglog(xv,yv,**string_to_dict(args[1]))
-                    else:
-                        if len(args)<2:
-                            self.axes.semilogx(xv,yv)
-                        else:
-                            self.axes.semilogx(xv,yv,**string_to_dict(args[1]))
-                else:
-                    if self.logy==True:
-                        if len(args)<2:
-                            self.axes.semilogy(xv,yv)
-                        else:
-                            self.axes.semilogy(xv,yv,**string_to_dict(args[1]))
-                    else:
-                        if len(args)<2:
-                            self.axes.plot(xv,yv)
-                        else:
-                            self.axes.plot(xv,yv,**string_to_dict(args[1]))
-                                
-                if self.xset==True:
-                    self.axes.set_xlim(self.xlo,self.xhi)
-                if self.yset==True:
-                    self.axes.set_ylim(self.ylo,self.yhi)
-                    
-        elif (curr_type==b'double[]' or curr_type==b'int[]' or
-              curr_type==b'size_t[]'):
+            tab=amt.get_table_obj()
+            yv=tab[force_bytes(args[0])][0:tab.get_nlines()]
+            args=args[1:]
 
-            get_fn=o2scl.o2scl_acol_get_double_arr
-            get_fn.argtypes=[ctypes.c_void_p,int_ptr,double_ptr_ptr]
-                            
-            id=ctypes.c_int(0)
-            ptr=double_ptr()
-            get_fn(amp,ctypes.byref(id),ctypes.byref(ptr))
+        elif curr_type==b'double[]':
+            
+            yv=amt.get_doublev_obj().to_numpy()
             
-            xv=[i for i in range(0,id.value)]
-            yv=[ptr[i] for i in range(0,id.value)]
+        elif curr_type==b'int[]':
 
+            yv=amt.get_intv_obj().to_numpy()
+            
+        elif curr_type==b'size_t[]':
+            
+            yv=amt.get_size_tv_obj().to_numpy()
+            
+        else:
+            
+            print("Command 'plot1' not supported for type",
+                  curr_type,".")
+            return
+            
+        if failed==False:
+            
+            xv=[i for i in range(0,len(yv))]
+        
             if self.canvas_flag==False:
                 self.canvas()
             if self.logx==True:
                 if self.logy==True:
                     if len(args)<1:
                         self.axes.loglog(xv,yv)
                     else:
@@ -1811,213 +2216,304 @@
                     else:
                         self.axes.semilogy(xv,yv,**string_to_dict(args[0]))
                 else:
                     if len(args)<1:
                         self.axes.plot(xv,yv)
                     else:
                         self.axes.plot(xv,yv,**string_to_dict(args[0]))
-                            
+                                
             if self.xset==True:
                 self.axes.set_xlim(self.xlo,self.xhi)
             if self.yset==True:
                 self.axes.set_ylim(self.ylo,self.yhi)
                     
         # End of function o2graph_plotter::plot1()
         return
             
-    def plotv(self,o2scl,amp,args):
-        """
-        Plot one or two multiple vector specifications
-        """
+    def plotv(self,o2scl,amp,link,args):
+        """Documentation for o2graph command ``plotv``:
 
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
-        
-        if curr_type==b'vector<contour_line>':
-             print('Store and clear the vector<contour_line> object '+
-                   'before using \'plotv\'.')
-             return 1
+        Plot several vector-like data sets.
+
+        Command-line arguments: ``[multiple vector spec. for x] 
+        <multiple vector spec. for y>``
+
+        The plotv command plots one or several pairs of vectors for x
+        and y. The total number of curves plotted will be the number
+        of vector data sets from the first argument times the number
+        of vector data sets from the second argument. If the x and y
+        vector lengths are not equal, then the longer vector is
+        truncated. Any kwargs are applied to all curves plotted. For
+        details on multiple vector specifications, use o2graph -help
+        mult-vector-spec.
+
+        There is an additional keyword argument ``filter``. The filter
+        is parsed through the python eval() function and all pairs of
+        points for which the function evaluates to False are omitted
+        from the plot. Local variables of interest are ``x`` and
+        ``y``, corresponding to the x and y value at each point, and
+        ``k``, the current array index.
+        """
+
+        amt=acol_manager(self.link2,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
+
+        filt=''
+        if len(args)>=3:
+            kwargs=string_to_dict(args[2])
+            filt=kwargs.pop('filter','')
         
-        conv_fn=o2scl.o2scl_acol_mult_vectors_to_conts
-        conv_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                          ctypes.c_char_p]
-        conv_fn.restype=ctypes.c_int
+        if self.canvas_flag==False:
+            self.canvas()
 
         if (len(args)>=2 and force_bytes(args[1])!=b'none' and
             force_bytes(args[1])!=b'None'):
-            if self.verbose>1:
+            
+            if self.verbose>1 or True:
                 print('Calling mult_vectors_to_conts() with',
                       args[0],'and',args[1])
-            mvs1=ctypes.c_char_p(force_bytes(args[0]))
-            mvs2=ctypes.c_char_p(force_bytes(args[1]))
-            conv_ret=conv_fn(amp,mvs1,mvs2)
-            if conv_ret!=0:
-                print('Failed to read "'+args[0]+'" and "'+args[1]+'".')
-                return 2
+                
+            vvdx=std_vector_vector(self.link2)
+            retx=mult_vector_spec(self.link2,args[0],vvdx,False,self.verbose,
+                                  False)
+            vvdy=std_vector_vector(self.link2)
+            rety=mult_vector_spec(self.link2,args[1],vvdy,False,self.verbose,
+                                  False)
+
+            for i in range(0,vvdx.size()):
+                for j in range(0,vvdy.size()):
+
+                    xarr=vvdx[i]
+                    yarr=vvdy[j]
+                    
+                    if len(xarr)!=len(yarr):
+                        print('o2graph command plotv warning: x vector',
+                              i,'and y vector',j,'dont have the same',
+                              'size.')
+                        print('  Length of x:',len(xarr),'y:',len(yarr))
+                    if len(filt)>0:
+                        xarr2=[]
+                        yarr2=[]
+                        for k in range(0,len(xarr)):
+                            if k<len(xarr):
+                                x=xarr[k]
+                                y=yarr[k]
+                                if eval(filt)==True:
+                                    xarr2.append(xarr[k])
+                                    yarr2.append(yarr[k])
+                    else:
+                        xarr2=xarr
+                        yarr2=yarr
+                    if self.logx==True:
+                        if self.logy==True:
+                            if len(args)>=3:
+                                self.axes.loglog(xarr2,yarr2,
+                                                 **kwargs)
+                            else:
+                                self.axes.loglog(xarr2,yarr2)
+                        else:
+                            if len(args)>=3:
+                                self.axes.semilogx(xarr2,yarr2,
+                                                 **kwargs)
+                            else:
+                                self.axes.semilogx(xarr2,yarr2)
+                    else:
+                        if self.logy==True:
+                            if len(args)>=3:
+                                self.axes.semilogy(xarr2,yarr2,
+                                                 **kwargs)
+                            else:
+                                self.axes.semilogy(xarr2,yarr2)
+                        else:
+                            if len(args)>=3:
+                                self.axes.plot(xarr2,yarr2,
+                                               **kwargs)
+                            else:
+                                self.axes.plot(xarr2,yarr2)
+            
         else:
+            
             if self.verbose>1:
                 print('Calling mult_vectors_to_conts() with',
                       args[0])
-            mvs1=ctypes.c_char_p(0)
-            mvs2=ctypes.c_char_p(force_bytes(args[0]))
-            conv_ret=conv_fn(amp,mvs1,mvs2)
-            if conv_ret!=0:
-                print('Failed to read "'+args[0])
-                return 2
-        
-        
-        # Get the total number of contour lines
-        cont_n_fn=o2scl.o2scl_acol_contours_n
-        cont_n_fn.argtypes=[ctypes.c_void_p]
-        cont_n_fn.restype=ctypes.c_int
-        nconts=cont_n_fn(amp)
-
-        # Define types for extracting each contour line
-        cont_line_fn=o2scl.o2scl_acol_contours_line
-        cont_line_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,
-                               int_ptr,double_ptr_ptr,
-                               double_ptr_ptr]
-        cont_line_fn.restype=ctypes.c_double
-
-        if self.canvas_flag==False:
-            self.canvas()
-
-        # Loop over all contour lines
-        for k in range(0,nconts):
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            ptry=double_ptr()
-            lev=cont_line_fn(amp,k,ctypes.byref(idx),
-                             ctypes.byref(ptrx),ctypes.byref(ptry))
-            xv=[ptrx[i] for i in range(0,idx.value)]
-            yv=[ptry[i] for i in range(0,idx.value)]
                 
-            if self.logx==True:
-                if self.logy==True:
-                    if len(args)<3:
-                        self.axes.loglog(xv,yv)
-                    else:
-                        self.axes.loglog(xv,yv,**string_to_dict(args[2]))
+            vvdy=std_vector_vector(self.link2)
+            mult_vector_spec(self.link2,args[0],vvdy,False,self.verbose,False)
+            
+            kwstring=''
+            if (len(args)>=3 and (force_bytes(args[1])==b'none' or
+                                  force_bytes(args[1])==b'None')):
+                kwstring=args[2]
+            elif len(args)>=2:
+                kwstring=args[1]
+            
+            for j in range(0,vvdy.size()):
+
+                yarr=vvdy[j]
+                xarr=[i for i in range(0,len(vvdy[j]))]
+
+                if len(filt)>0:
+                    xarr2=[]
+                    yarr2=[]
+                    for k in range(0,len(xarr)):
+                        if k<len(xarr):
+                            x=xarr[k]
+                            y=yarr[k]
+                            if eval(filt)==True:
+                                xarr2.append(xarr[k])
+                                yarr2.append(yarr[k])
                 else:
-                    if len(args)<3:
-                        self.axes.semilogx(xv,yv)
-                    else:
-                        self.axes.semilogx(xv,yv,**string_to_dict(args[2]))
-            else:
-                if self.logy==True:
-                    if len(args)<3:
-                        self.axes.semilogy(xv,yv)
+                    xarr2=xarr
+                    yarr2=yarr
+                
+                if self.logx==True:
+                    if self.logy==True:
+                        if kwstring!='':                            
+                            self.axes.loglog(xarr2,yarr2,
+                                             **string_to_dict(kwstring))
+                        else:
+                            self.axes.loglog(xarr2,yarr2)
                     else:
-                        self.axes.semilogy(xv,yv,**string_to_dict(args[2]))
+                        if kwstring!='':
+                            self.axes.semilogx(xarr2,yarr2,
+                                             **string_to_dict(kwstring))
+                        else:
+                            self.axes.semilogx(xarr2,yarr2)
                 else:
-                    if len(args)<3:
-                        self.axes.plot(xv,yv)
+                    if self.logy==True:
+                        if kwstring!='':
+                            self.axes.semilogy(xarr2,yarr2,
+                                             **string_to_dict(kwstring))
+                        else:
+                            self.axes.semilogy(xarr2,yarr2)
                     else:
-                        self.axes.plot(xv,yv,**string_to_dict(args[2]))
-                        
+                        if kwstring!='':
+                            self.axes.plot(xarr2,yarr2,
+                                             **string_to_dict(kwstring))
+                        else:
+                            self.axes.plot(xarr2,yarr2)
+                    
         # End of function o2graph_plotter::plotv()
         return
         
-    def print_param_docs(self):
+    def print_param_docs(self,amt):
         """
         Print parameter documentation.
 
         Called by help_func().
         """
 
         ter=terminal_py()
         str_line=ter.horiz_line()
         print('\n'+str_line)
         print('\nO2graph parameter list:')
         print(' ')
         for line in param_list:
             if line[0]!='verbose':
                 if line[0]=='colbar':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.colbar))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.colbar))
                 elif line[0]=='fig-dict':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.fig_dict))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.fig_dict))
                 elif line[0]=='font':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.font))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.font))
                 elif line[0]=='logx':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.logx))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.logx))
                 elif line[0]=='logy':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.logy))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.logy))
                 elif line[0]=='logz':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.logz))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.logz))
                 elif line[0]=='xhi':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.xhi))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.xhi))
                 elif line[0]=='xlo':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.xlo))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.xlo))
                 elif line[0]=='xset':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.xset))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.xset))
                 elif line[0]=='yhi':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.yhi))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.yhi))
                 elif line[0]=='ylo':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.ylo))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.ylo))
                 elif line[0]=='yset':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.yset))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.yset))
                 elif line[0]=='zhi':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.zhi))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.zhi))
                 elif line[0]=='zlo':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.zlo))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.zlo))
                 elif line[0]=='zset':
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg())+' '+str(self.zset))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color())+' '+
+                          str(self.zset))
                 else:
-                    print((ter.red_fg()+ter.bold()+line[0]+
-                           ter.default_fg()))
+                    print(force_string(amt.get_param_color())+line[0]+
+                          force_string(amt.get_default_color()))
                 print(' '+line[1])
                 print(' ')
         print(str_line)
         print('\nyt-related settings:')
         print(' ')
         for line in yt_param_list:
             if line[0]=='yt_filter':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+self.yt_filter)
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_filter))
             if line[0]=='yt_focus':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+self.yt_focus)
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_focus))
             if line[0]=='yt_position':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+self.yt_position)
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_position))
             if line[0]=='yt_width':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+self.yt_width)
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_width))
             if line[0]=='yt_north':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+self.yt_north)
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_north))
             if line[0]=='yt_path':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+str(self.yt_path))
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_path))
             if line[0]=='yt_resolution':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+str(self.yt_resolution))
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_resolution))
             if line[0]=='yt_sigma_clip':
-                print((ter.red_fg()+ter.bold()+line[0]+
-                       ter.default_fg())+' '+str(self.yt_sigma_clip))
+                print(force_string(amt.get_param_color())+line[0]+
+                      force_string(amt.get_default_color())+' '+
+                      str(self.yt_sigma_clip))
             print(' '+line[1])
             print(' ')
 
         # End of function o2graph_plotter::print_param_docs()
         return
             
     def parse_argv(self,argv,o2scl,link):
@@ -2027,183 +2523,134 @@
         This is the main function used by the :ref:`o2graph_script` .
         Once it has created a list of strings from argv, it calls
         parse_string_list() to call the proper functions. It 
         creates the pointer to the o2scl acol_manager object 
         called `amp`.
         """
 
+        # Set the o2scl library pointer in the plot_base parent
+        self.link2=link
+        
         # Create an acol_manager object and get the pointer
-        o2scl.o2scl_hdf_create_acol_manager.restype=ctypes.c_void_p
-        amp=o2scl.o2scl_hdf_create_acol_manager()
+        am=acol_manager(self.link2)
+        amp=am._ptr
 
-        names_fn=o2scl.o2scl_acol_set_names
-        names_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,ctypes.c_char_p,
-                           ctypes.c_int,ctypes.c_char_p,ctypes.c_int,
-                           ctypes.c_char_p]
+        s=std_string(self.link2)
+        s.init_bytes(b'O2GRAPH_DEFAULTS')
+        am.set_env_var_name(s)
+        
+        am.run_empty()
+        cl=am.get_cl()
 
         # Get current type
         ter=terminal_py()
-        cmd_name=b'o2graph'
         cmd_desc=(b'o2graph: A data viewing and '+
                   b'processing program for '+force_bytes(ter.bold())+
-                  b'O2scl'+force_bytes(ter.default_fg())+
+                  b'O2scl'+force_bytes(ter.default_fgbg())+
                   b'.\n  Version: '+force_bytes(version)+b'\n')
-        env_var=b'O2GRAPH_DEFAULTS'
-        names_fn(amp,len(cmd_name),ctypes.c_char_p(cmd_name),
-                 len(cmd_desc),ctypes.c_char_p(cmd_desc),
-                 len(env_var),ctypes.c_char_p(env_var))
-
-        # Apply aliases before parsing. We convert argv 
-        # to a set of integer and character arrays, then
-        # pass them to o2scl_acol_apply_aliases()
-        if True:
-
-            orig_len=len(argv)
-            
-            int_ptr=ctypes.POINTER(ctypes.c_int)
-            char_ptr=ctypes.POINTER(ctypes.c_char)
-            int_ptr_ptr=ctypes.POINTER(int_ptr)
-            char_ptr_ptr=ctypes.POINTER(char_ptr)
-
-            # Allocate space for arrays
-            tiarr=(ctypes.c_int*len(argv))()
-            ttot=0
-            for i in range(0,len(argv)):
-                ttot+=len(argv[i])
-            tcarr=(ctypes.c_char*ttot)()
-
-            # Fill arrays with data
-            tcnt=0
-            for i in range(0,len(argv)):
-                tiarr[i]=len(argv[i])
-                #print(i,tiarr[i])
-                for j in range(0,len(argv[i])):
-                    tcarr[tcnt]=bytes(argv[i][j],'utf8')
-                    #print(j,tcarr[tcnt])
-                    tcnt=tcnt+1
-
-            # Call the alias_counts() function to find out how big the
-            # destination arrays need to be. This two step-process
-            # allows python to handle the memory allocation.
-            count_fn=o2scl.o2scl_acol_alias_counts
-            count_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,int_ptr,
-                               ctypes.c_char_p,int_ptr,int_ptr]
-            n_new=ctypes.c_int(0)
-            s_new=ctypes.c_int(0)
-            count_fn(amp,len(argv),tiarr,tcarr,ctypes.byref(n_new),
-                     ctypes.byref(s_new))
-
-            # Allocate the new integer and string arrays
-            tiarr2=(ctypes.c_int*n_new.value)()
-            tcarr2=(ctypes.c_char*s_new.value)()
-
-            # Setup and call alias function
-            alias_fn=o2scl.o2scl_acol_apply_aliases
-            alias_fn.argtypes=[ctypes.c_void_p,ctypes.c_int,int_ptr,
-                               ctypes.c_char_p,int_ptr,ctypes.c_char_p]
-            alias_fn(amp,len(argv),tiarr,tcarr,tiarr2,tcarr2)
-
-            # Construct the new argv list. We skip alias
-            # definitions because they are already taken care of
-            argv=[]
-            icnt=0
-            cnt=0
-            iskip=0
-            if len(tiarr2)!=orig_len:
-                print('After applying alias,',orig_len,'->',len(tiarr2))
-            for i in range(0,n_new.value):
-                tstr=''
-                for j in range(0,tiarr2[i]):
-                    tstr=tstr+tcarr2[cnt].decode('utf-8')
-                    cnt=cnt+1
-                if tstr=='-alias':
-                    iskip=2
-                elif iskip==0:
-                    argv.append(tstr)
-                    if len(tiarr2)!=orig_len:
-                        print(icnt,argv[icnt])
-                    icnt=icnt+1
-                else:
-                    iskip=iskip-1
-            
+
+        s.init_bytes(b'o2graph')
+        cl.set_cmd_name(s)
+        
+        s.init_bytes(cmd_desc)
+        cl.set_desc(s)
+
+        # 12/9 The problem here is that o2graph appears to be
+        # using acol to process the aliases. I think everything
+        # may be fixed now with aliases.
+        
+        #if 'O2GRAPH_DEFAULTS' in os.environ:
+        #    am.def_args=os.environ['O2GRAPH_DEFAULTS']
+        #    vs_da=am.def_args.split()
+        #    print('parsing default args')
+        #    print('vs_da:',vs_da);
+        #    vs_da2=std_vector_string(link)
+        #    vs_da2.set_list(vs_da)
+        #    print('here, going to pfa')
+        #    cl.parse_for_aliases(vs_da2,True)
+        #    print('vs2:',vs_da);
+        #    self.parse_string_list(vs_da,o2scl,amp,link)
+        #    print('done.')
+        #else:
+        #    am.def_args=''
+
         if len(argv)<=1:
             done_flag=False
             readline.parse_and_bind('tab: complete')
             readline.parse_and_bind('set editing-mode emacs')
             while done_flag==False:
                 line=input('o2graph> ')
                 if line[0:4]=='quit' or line[0:4]=='exit':
                     done_flag=True
                 else:
                     strlist=line.split(' ')
                     strlist[0]='-'+strlist[0]
-                    self.parse_string_list(strlist,o2scl,amp,link)
+                    self.parse_string_list(strlist,o2scl,amp,self.link2)
         else:
-            strlist=[str(argv[i]) for i in range(1,len(argv))]
+            
+            vs=std_vector_string(self.link2)
+            vs.set_list(argv)
+            cl.apply_aliases(vs,0,True)
+            strlist=[]
+            for i in range(0,len(vs)):
+                strlist.append(force_string(vs[i]))
+            
             if self.verbose>2:
                 print('Number of arguments:',len(strlist),'arguments.')
                 print('Argument List:',strlist)
-            self.parse_string_list(strlist,o2scl,amp,link)
+            self.parse_string_list(strlist,o2scl,amp,self.link2)
 
         # End of function o2graph_plotter::parse_argv()
         return
 
-    def yt_add_vol(self,o2scl,amp,args,keyname='o2graph_vol'):
-        """
-        Add a volume source to a yt visualization from a
-        tensor_grid object.
+    def yt_add_vol(self,o2scl,amp,link,args,keyname='o2graph_vol'):
         """
+        Documentation for o2graph command ``yt-add-vol``:
+
+        For objects of type ``tensor_grid``:
 
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
+        Add a tensor_grid object as a yt volume source
 
-        curr_type=o2scl_get_type(o2scl,amp)
+        Command-line arguments: ``[kwargs]``
+
+        This command adds the volumetric data specified in the
+        ``tensor_grid`` object as a yt volume source. The transfer
+        function previously specified by ``yt-tf`` is used, or if
+        unspecified, then yt's transfer_function_helper is used to
+        create a 3 layer default transfer function.
+
+        """
+
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if curr_type==b'tensor_grid':
             
             self.yt_check_backend()
             import yt
             from yt.visualization.volume_rendering.api \
                 import create_volume_source
             from yt.visualization.volume_rendering.transfer_function_helper \
                 import TransferFunctionHelper
 
-            # Set up wrapper for get function
-            get_fn=o2scl.o2scl_acol_get_tensor_grid3
-            get_fn.argtypes=[ctypes.c_void_p,int_ptr,int_ptr,
-                             int_ptr,double_ptr_ptr,
-                             double_ptr_ptr,double_ptr_ptr,
-                             double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-             # Call get function
-            nx=ctypes.c_int(0)
-            ny=ctypes.c_int(0)
-            nz=ctypes.c_int(0)
-            ret=ctypes.c_int(0)
-            gridx=double_ptr()
-            gridy=double_ptr()
-            gridz=double_ptr()
-            data=double_ptr()
-            ret=get_fn(amp,ctypes.byref(nx),ctypes.byref(ny),
-                       ctypes.byref(nz),ctypes.byref(gridx),
-                       ctypes.byref(gridy),ctypes.byref(gridz),
-                       ctypes.byref(data))
-            if ret==2:
+            amt=acol_manager(self.link2,amp)
+            tg3=amt.get_tensor_grid_obj()
+            rk=tg3.get_rank()
+            if rk!=3:
                 print("Object of type 'tensor_grid' does not have rank 3.")
                 return
-            elif ret==1:
-                print("Object is not of type 'tensor_grid'.")
-                return
-
-            nx=nx.value
-            ny=ny.value
-            nz=nz.value
+            sza=tg3.get_size_arr()
+            nx=sza[0]
+            ny=sza[1]
+            nz=sza[2]
+            grid_packed=tg3.get_grid_packed()
+            gridx=[grid_packed[i] for i in range(0,nx)]
+            gridy=[grid_packed[i+nx] for i in range(0,ny)]
+            gridz=[grid_packed[i+nx+ny] for i in range(0,nz)]
+            
+            data=tg3.get_data()
             total_size=nx*ny*nz
 
             if self.xset==False:
                 self.xlo=gridx[0]
                 self.xhi=gridx[nx-1]
                 self.xset=True
             if self.yset==False:
@@ -2273,20 +2720,20 @@
             
             import yt
             from yt.visualization.volume_rendering.api \
                 import create_volume_source
             from yt.visualization.volume_rendering.transfer_function_helper \
                 import TransferFunctionHelper
 
-            tg=tensor_grid(link)
-            amt=acol_manager(link,amp)
+            tg=tensor_grid(self.link2)
+            amt=acol_manager(self.link2,amp)
             t3d=amt.get_table3d_obj()
             tg.from_table3d_fermi(args[0])
 
-            grid=std_vector(link)
+            grid=std_vector(self.link2)
             grid=tg.get_grid_packed()
             nx=tg.get_size(0)
             ny=tg.get_size(1)
             nz=tg.get_size(2)
             gridx=[grid[i] for i in range(0,nx)]
             gridy=[grid[i] for i in range(nx,nx+ny)]
             gridz=[grid[i] for i in range(nx+ny,nx+ny+nz)]
@@ -2355,80 +2802,61 @@
                             
             if self.yt_created_camera==False:
                 self.yt_create_camera(ds)
                 
         # End of function o2graph_plotter::yt_add_vol()
         return
         
-    def den_plot_anim(self,o2scl,amp,args):
+    def den_plot_anim(self,o2scl,amp,link,args):
         """Documentation for o2graph command ``den-plot-anim``:
 
         Create an animated density plot from a rank 3 tensor_grid
         object
 
         Command-line arguments: ``<x index> <y index> <z index [+'r']>
-        <mp4 filename>``
+        <mp4 filename> [kwargs for imshow()]``
 
-        Create an mp4 animation of a density plot from a tensor_grid3
-        object. The first argument specifies which tensor index is
-        along the x axis (either ``0``, ``1`` or ``2``), the second
-        argument is the tensor index is along the y axis (either
-        ``0``, ``1`` or ``2``), and the third argument is the tensor
-        index which will be animated. If the third argument has an
-        additional ``r`` suffix, then the animation will be reversed,
-        so that the first frame corresponds to the largest value of
-        the grid for the associated index.
+        Create an mp4 animation of a density plot from a
+        ``tensor_grid`` object with rank 3. The first argument
+        specifies which tensor index is along the x axis (either
+        ``0``, ``1`` or ``2``), the second argument is the tensor
+        index is along the y axis (either ``0``, ``1`` or ``2``), and
+        the third argument is the tensor index which will be animated.
+        If the third argument has an additional ``r`` suffix, then the
+        animation will be reversed, so that the first frame
+        corresponds to the largest value of the grid for the
+        associated index.
 
         Experimental.
 
         """
 
         import matplotlib.pyplot as plot
         
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-        
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if curr_type==b'tensor_grid':
 
             # Set up wrapper for get function
-            get_fn=o2scl.o2scl_acol_get_tensor_grid3
-            get_fn.argtypes=[ctypes.c_void_p,int_ptr,int_ptr,
-                             int_ptr,double_ptr_ptr,
-                             double_ptr_ptr,double_ptr_ptr,
-                             double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-            
-             # Call get function
-            nx=ctypes.c_int(0)
-            ny=ctypes.c_int(0)
-            nz=ctypes.c_int(0)
-            ret=ctypes.c_int(0)
-            gridx=double_ptr()
-            gridy=double_ptr()
-            gridz=double_ptr()
-            data=double_ptr()
-            ret=get_fn(amp,ctypes.byref(nx),ctypes.byref(ny),
-                       ctypes.byref(nz),ctypes.byref(gridx),
-                       ctypes.byref(gridy),ctypes.byref(gridz),
-                       ctypes.byref(data))
-            if ret==2:
+            amt=acol_manager(self.link2,amp)
+            tg3=amt.get_tensor_grid_obj()
+            rk=tg3.get_rank()
+            if rk!=3:
                 print("Object of type 'tensor_grid' does not have rank 3.")
                 return
-            elif ret==1:
-                print("Object is not of type 'tensor_grid'.")
-                return
-
-            nx=nx.value
-            ny=ny.value
-            nz=nz.value
+            sza=tg3.get_size_arr()
+            nx=sza[0]
+            ny=sza[1]
+            nz=sza[2]
+            grid_packed=tg3.get_grid_packed()
+            gridx=[grid_packed[i] for i in range(0,nx)]
+            gridy=[grid_packed[i+nx] for i in range(0,ny)]
+            gridz=[grid_packed[i+nx+ny] for i in range(0,nz)]
+            
+            data=tg3.get_data()
             total_size=nx*ny*nz
 
             if args[0]=='0':
                 xgrid=[gridx[i] for i in range(0,nx)]
                 nx2=nx
             elif args[0]=='1':
                 xgrid=[gridy[i] for i in range(0,ny)]
@@ -2456,42 +2884,49 @@
             elif args[2]=='1r':
                 n_frames=ny
             elif args[2]=='2':
                 n_frames=nz
             elif args[2]=='2r':
                 n_frames=nz
 
+            kwstring=''
+            if len(args)>=5:
+                kwstring=args[4]
+            dctt=string_to_dict(kwstring)
+                
             if n_frames>9999:
                 print('Large number of frames (',n_frames,') not',
                       'supported in den-plot-anim.')
                 return
-            
-            arr=numpy.ctypeslib.as_array(data,shape=(nx,ny,nz))
-            print(arr.shape)
+
+            arr=data.reshape((nx,ny,nz))
 
             if self.colbar==True:
                 # The animation of the colorbar messes up the
                 # automatic colorbar placement, so this is a hack to
                 # attempt make sure the colorbar is placed correctly
                 # in all frames.
                 dct=string_to_dict(self.fig_dict)
                 if ('right_margin' not in dct.keys() or
                     dct['right_margin']<0.1):
+                    print('xxx')
                     dct['right_margin']=0.15
-                if ('top_margin' not in dct.keys() or
-                    dct['top_margin']<0.06):
+                if 'top_margin' not in dct.keys():
                     dct['top_margin']=0.06
                 if 'left_margin' not in dct.keys():
                     dct['left_margin']=0.14
                 if 'bottom_margin' not in dct.keys():
                     dct['bottom_margin']=0.12
                 rm=dct['right_margin']
                 lm=dct['left_margin']
                 tm=dct['top_margin']
                 bm=dct['bottom_margin']
+                if self.verbose>1:
+                    print('o2graph_plotter.den_plot_anim(): margins',
+                          rm,lm,tm,bm)
                 if self.canvas_flag==False:
                     if 'fontsize' not in dct.keys():
                         dct['fontsize']=self.font
                     (self.fig,self.axes)=default_plot(**dct)
                     # Plot limits
                     if self.xset==True:
                         self.axes.set_xlim(self.xlo,self.xhi)
@@ -2512,15 +2947,15 @@
             if self.logx==True:
                 for i in range(0,len(xgrid)):
                     xgrid[i]=math.log(xgrid[i],10)
                     
             if self.logy==True:
                 for i in range(0,len(ygrid)):
                     ygrid[i]=math.log(ygrid[i],10)
-                        
+
             for k in range(0,n_frames):
                 if args[2]=='0':
                     sl=arr[k,:,:]
                 elif args[2]=='0r':
                     sl=arr[n_frames-1-k,:,:]
                 elif args[2]=='1':
                     sl=arr[:,k,:]
@@ -2592,15 +3027,15 @@
                     self.last_image.remove()
                     del self.last_image
                         
                 self.last_image=self.axes.imshow(sl,interpolation='nearest',
                                                  origin='lower',
                                                  extent=[tmp1,tmp2,
                                                          tmp3,tmp4],
-                                                 aspect='auto')
+                                                 aspect='auto',**dctt)
                 
                 if self.colbar==True:
                     dpa_cax2=self.fig.add_axes([1.0-rm*0.9,
                                                 bm,rm*0.3,
                                                 1.0-bm-tm])
                     self.cbar=self.fig.colorbar(self.last_image,
                                                 cax=dpa_cax2)
@@ -2660,132 +3095,79 @@
             os.system(cmd)
 
             # End of "if curr_type==b'tensor_grid':"
                 
         # End of function o2graph_plotter::den_plot_anim()
         return
         
-    def help_func(self,o2scl,amp,args):
+    def help_func(self,o2scl,amp,link,args):
         """
         Function to process the help command.
         """
 
-        base_list_new=[
-            ["addcbar",plot_base.addcbar.__doc__],
-            ["arrow",plot_base.arrow.__doc__],
-            ["backend",
-             ("Documentation for backend\n\n"+
-              "Select the matplotlib backend to use.\n\n"+
-              "<backend>\n\n"+
-              "This commend selects the matplotlib backend. "+
-              "Typical values are 'Agg', 'TkAgg', 'WX', 'QTAgg', "+
-              "and 'QT4Agg'. Use backend Agg to save the plot to a "+
-              "file without opening a window. The backend can only "+
-              "be changed once, i.e. if the backend command is "+
-              "invoked more than once, then only the last invocation "+
-              "will have any effect.")],
-            ["canvas",plot_base.canvas.__doc__],
-            ["cmap",plot_base.cmap.__doc__],
-            ["cmap2",plot_base.cmap2.__doc__],
-            ["den-plot-anim",o2graph_plotter.den_plot_anim.__doc__],
-            ["image","Documentation for image\n\n"+
-             "Plot a png file in a matplotlib window.\n\n"+
-             "<png file>\n\n"+
-             "This command reads a png file, fills a plotting canvas "+
-             "and then calls matplotlib.pyplot.show()."],
-            ["yt-axis",yt_plot_base.yt_plot_axis.__doc__],
-            ["yt-path",o2graph_plotter.yt_path_func.__doc__],
-            ["yt-text",o2graph_plotter.yt_text.__doc__],
-            ["yt-tf",o2graph_plotter.yt_tf_func.__doc__],
-            ["yt-xtitle",yt_plot_base.yt_xtitle.__doc__],
-            ["yt-ytitle",yt_plot_base.yt_ytitle.__doc__],
-            ["yt-ztitle",yt_plot_base.yt_ztitle.__doc__]
-        ]
-
+        amt=acol_manager(self.link2,amp)
+        cl=amt.get_cl()
+        
         # The command we're looking for help on (if specified)
         cmd=''
 
         # vt100 inits
         ter=terminal_py()
         str_line=ter.horiz_line()
 
         # Get current type
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if len(args)==1:
+            # If just a command is specified
+            
             cmd=args[0]
+            
         elif len(args)==2:
             # If both a type and command are specified
                         
             curr_type=args[0]
             cmd=args[1]
 
-        # See if we matched an o2graph command
+        # True if the user-specified arguments were matched
         match=False
 
-        for line in base_list_new:
+        # Handle the case of an o2graph command from the base list
+        for line in base_list:
             if cmd==line[0]:
                 match=True
-                reformat_python_docs(cmd,line[1],base_list_new)
+                reformat_python_docs(cmd,line[1],amp,self.link2)
         
         # Handle the case of an o2graph command from the
-        # base list
+        # extra list
         if match==False:
-            for line in base_list:
-                if cmd==line[0]:
+            for line in extra_list:
+                if ((curr_type==line[0] or
+                     curr_type==force_bytes(line[0])) and
+                    cmd==line[1]):
                     match=True
-                    print('Usage: '+ter.cyan_fg()+ter.bold()+cmd+
-                          ter.default_fg()+
-                          ' '+line[2]+'\n\n'+line[1]+'\n')
-                    tempx_arr=wrap_line(line[3])
-                    for i in range (0,len(tempx_arr)):
-                        print(tempx_arr[i])
-                                
-        # Handle the case of an o2graph command from the
-        # extra list
-        for line in extra_list:
-            if ((curr_type==line[0] or
-                 curr_type==force_bytes(line[0])) and
-                cmd==line[1]):
-                match=True
-                print('Usage: '+ter.cyan_fg()+ter.bold()+cmd+ter.default_fg()+
-                      ' '+line[3]+'\n\n'+line[2]+'\n')
-                tempx_arr=wrap_line(line[4])
-                for i in range (0,len(tempx_arr)):
-                    print(tempx_arr[i])
+                    reformat_python_docs_type(curr_type,cmd,line[2],amp,self.link2)
 
-        # If we haven't matched yet, then show commands for
-        # other types
+        # Handle the case of an o2graph command from the
+        # extra list without a matching type
         if match==False:
             for line in extra_list:
                 if cmd==line[1]:
                     match=True
-                    str_line=ter.horiz_line()
                     print('\n'+str_line)
-                    print('Type: '+ter.magenta_fg()+ter.bold()+line[0]+
-                          ter.default_fg()+':')
-                    print('Usage: '+cmd+' '+ter.cyan_fg()+ter.bold()+line[3]+
-                          ter.default_fg()+'\n\n'+line[2]+'\n')
+                    #print('here2')
+                    reformat_python_docs_type(line[0],cmd,line[2],amp,self.link2)
                     
-                    tempx_arr=line[4].split('\n')
-                    for j in range(0,len(tempx_arr)):
-                        if len(tempx_arr[j])<79:
-                            print(tempx_arr[j])
-                        else:
-                            str_list=textwrap.wrap(tempx_arr[j],79)
-                            for i in range (0,len(str_list)):
-                                print(str_list[i])
-
         # If we haven't matched yet, check for get/set parameters
         if match==False:
             for line in param_list:
                 if cmd==line[0]:
                     match=True
-                    print('O2graph parameter modified by get/set: '+
-                          line[0]+'\n')
+                    print('O2graph parameter modified by the get and set',
+                          'commands: '+line[0]+'\n')
                     
                     tempx_arr=line[1].split('\n')
                     for j in range(0,len(tempx_arr)):
                         if len(tempx_arr[j])<79:
                             print(tempx_arr[j])
                         else:
                             str_list=textwrap.wrap(tempx_arr[j],79)
@@ -2794,252 +3176,136 @@
 
         # If we haven't matched yet, check for get/set parameters
         # from yt
         if match==False:
             for line in yt_param_list:
                 if cmd==line[0]:
                     match=True
-                    print('yt parameter modified by get/set: '+line[0]+'\n')
+                    print('yt parameter modified by the get and',
+                          'set commands: '+line[0]+'\n')
                     
                     tempx_arr=line[1].split('\n')
                     for j in range(0,len(tempx_arr)):
                         if len(tempx_arr[j])<79:
                             print(tempx_arr[j])
                         else:
                             str_list=textwrap.wrap(tempx_arr[j],79)
                             for i in range (0,len(str_list)):
                                 print(str_list[i])
 
-        finished=False
-        
-        if cmd=='cmaps' and len(args)==1:
-            cmap_list_func()
-            finished=True
-
-        if (len(args)==1 or len(args)==2) and args[0]=='cmaps-plot':
-            if len(args)==2:
-                cmaps_plot(args[1])
-            else:
-                cmaps_plot()
-            finished=True
-            
-        if (len(args)==1 or len(args)==2) and args[0]=='colors-plot':
-            if len(args)==2:
-                colors_plot(args[1])
-            else:
-                colors_plot()
-            finished=True
-
-        if (len(args)<=3 and len(args)>=1 and args[0]=='colors-near'):
-            if len(args)==3:
-                colors_near(col=args[1],fname=args[2])
-            elif len(args)==2:
-                colors_near(col=args[1])
-            else:
-                colors_near()
-            finished=True
-                        
-        if (cmd=='colors') and len(args)==1:
-            color_list()
-            finished=True
-                        
-        if (cmd=='xkcd-colors') and len(args)==1:
-            xkcd_colors_list()
-            finished=True
-
+        # Handle o2graph topics
         if (cmd=='markers') and len(args)==1:
             marker_list()
-            finished=True
+            match=True
             
         if (len(args)==1 or len(args)==2) and args[0]=='markers-plot':
             if len(args)==2:
                 markers_plot(args[1])
             else:
                 markers_plot()
-            finished=True
+            match=True
 
         # Handle acol topics and types
-        if (len(args)==1 and (cmd=='strings-spec' or cmd=='functions' or
-                              cmd=='mult-vector-spec' or cmd=='types' or
-                              cmd=='value-spec' or cmd=='vector-spec' or
-                              cmd=='index-spec' or cmd=='char' or
-                              cmd=='double' or cmd=='double[]' or
-                              cmd=='hist' or cmd=='hist_2d' or
-                              cmd=='int' or cmd=='int[]' or
-                              cmd=='prob_dens_amr' or cmd=='size_t' or
-                              cmd=='size_t[]' or cmd=='string' or
-                              cmd=='string[]' or cmd=='table' or
-                              cmd=='table3d' or cmd=='tensor' or
-                              cmd=='tensor<int>' or cmd=='tensor<size_t>' or
-                              cmd=='tensor_grid' or
-                              cmd=='uniform_grid<double>' or
-                              cmd=='vector<contour_line>')):
-            self.gen_acol(o2scl,amp,'help',args)
-            finished=True
-            
-        if match==False and finished==False:
-
-            # Since we didn't match anything above, see if
-            # it is an acol command
-            
-            # C types
-            int_ptr=ctypes.POINTER(ctypes.c_int)
-            int_ptr_ptr=ctypes.POINTER(int_ptr)
-            char_ptr=ctypes.POINTER(ctypes.c_char)
-            char_ptr_ptr=ctypes.POINTER(char_ptr)
-
-            acol_match=False
-                
-            # If len(args)>=2, then the user gave a type,
-            # so check options based on that type
-            if len(args)>=2:
+        if match==False:
+            if len(args)==1:
+                if amt.help_found(args[0],'')==True:
+                    self.gen_acol(o2scl,amp,self.link2,'help',args)
+                    match=True
+            elif len(args)==2 and amt.help_found(args[0],args[1])==True:
+                self.gen_acol(o2scl,amp,self.link2,'help',args)
+                match=True
 
-                # Function interface
-                get_fn=o2scl.o2scl_acol_get_cli_options_type
-                get_fn.argtypes=[ctypes.c_void_p,char_ptr,int_ptr,int_ptr_ptr,
-                                 char_ptr_ptr]
-                get_fn.restype=ctypes.c_int
-
-                # Arguments
-                size=ctypes.c_int(0)
-                iptr=int_ptr()
-                cptr=char_ptr()
-                curr_type2=ctypes.c_char_p(force_bytes(curr_type))
-        
-                # Function call
-                get_ret=get_fn(amp,curr_type2,ctypes.byref(size),
-                               ctypes.byref(iptr),ctypes.byref(cptr))
-
-                # tlist is the list of acol commands
-                tlist=get_ic_ptrs_to_list(size,iptr,cptr)
-
-                # If specified, look up command in acol list
-                if len(args)>0:
-                    for j in range(0,len(tlist)):
-                        if string_equal_dash(tlist[j],cmd):
-                            acol_match=True
-
-            # If either len(args)<2 or the last section failed, then in
-            # either case we need to compute tlist 
-            if acol_match==False:
-
-                # Check acol options based on the current type
-                
-                # Function interface
-                get_fn=o2scl.o2scl_acol_get_cli_options
-                get_fn.argtypes=[ctypes.c_void_p,int_ptr,int_ptr_ptr,
-                                 char_ptr_ptr]
-                get_fn.restype=ctypes.c_int
-    
-                # Arguments
-                size=ctypes.c_int(0)
-                iptr=int_ptr()
-                cptr=char_ptr()
-            
-                # Function call
-                get_ret=get_fn(amp,ctypes.byref(size),
-                               ctypes.byref(iptr),ctypes.byref(cptr))
-    
-                # tlist is the list of acol commands
-                tlist=get_ic_ptrs_to_list(size,iptr,cptr)
+        # If there was no match, do a command list
+        if match==False:
+            
+            print('o2graph: A data viewing and '+
+                  'processing program for '+ter.bold()+
+                  'O2scl'+ter.default_fgbg()+
+                  '.\n  Version: '+version)
+            print(' ')
+            if curr_type==b'':
+                print('List of command-line options which',
+                      'do not require a current object:\n')
+            else:
+                # AWS removed decode on 10/27/2020
+                # and converted to force_string() on 5/6/22
+                print('List of command-line options',
+                      '(current object type is',
+                      force_string(amt.get_type_color())+
+                      force_string(curr_type)+
+                      force_string(amt.get_default_color())+'):\n')
+            full_list=[]
+
+            tlist=cl.get_option_list()
+            for j in range(0,len(tlist)):
+                desc=cl.option_short_desc(tlist[j])
+                full_list.append([tlist[j],desc])
+
+            for line2 in base_list:
+                short=reformat_python_docs(line2[0],line2[1],amp,
+                                           self.link2,True)
+                full_list.append([force_bytes(line2[0]),
+                                  force_bytes(short)])
 
-                if len(args)<2:
-                    # If specified, look up command in acol list
-                    acol_match=False
-                    if len(args)>0:
-                        for j in range(0,len(tlist)):
-                            if string_equal_dash(tlist[j],args[0]):
-                                acol_match=True
-
-            # If there was no match, do a command list
-            if acol_match==False:
-
-                desc_fn=o2scl.o2scl_acol_cli_option_desc
-                desc_fn.argtypes=[ctypes.c_void_p,char_ptr,int_ptr,
-                                  char_ptr_ptr]
-                desc_fn.restype=ctypes.c_int
-                
-                print('o2graph: A data viewing and '+
-                      'processing program for '+ter.bold()+
-                      'O2scl'+ter.default_fg()+
-                      '.\n  Version: '+version)
-                print(' ')
-                if curr_type==b'':
-                    print('List of command-line options which',
-                          'do not require a current object:\n')
+            if curr_type!='':
+                for line in extra_list:
+                    if force_bytes(line[0])==curr_type:
+                        #print('here3')
+                        short=reformat_python_docs_type(curr_type,line[1],
+                                                        line[2],amp,
+                                                        self.link2,True)
+                        full_list.append([force_bytes(line[1]),
+                                          force_bytes(short)])
+
+            full_list2=sorted(full_list,key=lambda x: x[0])
+            max_len=0
+            for k in range(0,len(full_list2)):
+                full_list2[k][0]=(force_string(amt.get_command_color())+
+                                  full_list2[k][0].decode('utf-8')+
+                                  force_string(amt.get_default_color()))
+                full_list2[k][1]=full_list2[k][1].decode('utf-8')
+                if length_without_colors(full_list2[k][0])>max_len:
+                    max_len=length_without_colors(full_list2[k][0])
+            for k in range(0,len(full_list2)):
+                strt='  '
+                extra=max_len-length_without_colors(full_list2[k][0])
+                strt+='-'+full_list2[k][0]
+                for ij in range(0,extra):
+                    strt+=' '
+                strt+=' '+full_list2[k][1]
+                print(strt)
+            print('\n'+str_line)
+            help_topics=sorted(acol_help_topics+o2graph_help_topics)
+                
+            strt='Additional help topics: '
+            for j in range(0,len(help_topics)):
+                if j<len(help_topics)-1:
+                    strt+=(force_string(amt.get_help_color())+
+                           help_topics[j]+
+                           force_string(amt.get_default_color())+', ')
                 else:
-                    # AWS removed decode on 10/27/2020
-                    # but Converted to force_string on 5/6/22
-                    print('List of command-line options',
-                          '(current object type is',
-                          force_string(curr_type)+'):\n')
-                full_list=[]
-
-                for j in range(0,len(tlist)):
-                    opt_name=ctypes.c_char_p(tlist[j])
-                    desc_ret=desc_fn(amp,opt_name,iptr,cptr)
-                    desc=b''
-                    for k in range(0,iptr[0]):
-                        desc=desc+cptr[k]
-                    full_list.append([tlist[j],desc])
-
-                for line in base_list:
-                    full_list.append([force_bytes(line[0]),
-                                      force_bytes(line[1])])
-
-                if curr_type!='':
-                    for line in extra_list:
-                        if force_bytes(line[0])==curr_type:
-                            full_list.append([force_bytes(line[1]),
-                                              force_bytes(line[2])])
-
-                full_list2=sorted(full_list,key=lambda x: x[0])
-                max_len=0
-                for k in range(0,len(full_list2)):
-                    full_list2[k][0]=(ter.cyan_fg()+ter.bold()+
-                                      full_list2[k][0].decode('utf-8')+
-                                      ter.default_fg())
-                    full_list2[k][1]=full_list2[k][1].decode('utf-8')
-                    if length_without_colors(full_list2[k][0])>max_len:
-                        max_len=length_without_colors(full_list2[k][0])
-                for k in range(0,len(full_list2)):
-                    strt='  '
-                    extra=max_len-length_without_colors(full_list2[k][0])
-                    strt+='-'+full_list2[k][0]
-                    for ij in range(0,extra):
-                        strt+=' '
-                    strt+=' '+full_list2[k][1]
-                    print(strt)
-                print('\n'+str_line)
-                help_topics=sorted(acol_help_topics+o2graph_help_topics)
-                strt='Additional help topics: '
-                for j in range(0,len(help_topics)):
-                    if j<len(help_topics)-1:
-                        strt+=(ter.green_fg()+ter.bold()+
-                               help_topics[j]+ter.default_fg()+', ')
-                    else:
-                        strt+=('and '+ter.green_fg()+ter.bold()+
-                               help_topics[j]+ter.default_fg()+'.')
-                tlist=wrap_line(strt)
-                for j in range(0,len(tlist)):
-                    print(tlist[j])
-            else:
-                # Otherwise, it's an acol command so
-                self.gen_acol(o2scl,amp,'help',args)
+                    strt+=('and '+force_string(amt.get_help_color())+
+                           help_topics[j]+
+                           force_string(amt.get_default_color())+'.')
+                        
+            tlist=wrap_line(strt)
+            for j in range(0,len(tlist)):
+                print(tlist[j])
             
         # If the user specified 'help set', then print
         # the o2graph parameter documentation
         if (cmd=='set' or cmd=='get') and len(args)==1:
-            self.print_param_docs()
+            self.print_param_docs(amt)
 
         # End of function o2graph_plotter::help_func()
         return
         
     def yt_tf_func(self,args):
-        """Documentation for o2graph command ``yt-tf``:
+        """
+        Documentation for o2graph command ``yt-tf``:
 
         Edit the yt transfer function.
 
         Command-line arguments: ``<mode> <args>``
 
         To create a new transfer function, use 'new' for <mode> and
         the remaining <args> are <min> <max> [nbins] .To add a
@@ -3153,36 +3419,68 @@
 
         self.yt_path.append(args)
         print('yt_path is',self.yt_path)
         
         return
 
     def yt_ann_func(self,o2scl,amp,args):
-        """
-        Add the o2graph commands specified in `args` to the 
-        list of yt annotations to be used in the next yt render.
+        """Documentation for o2graph command ``yt-ann``:
+
+        Annotate a yt rendering (experimental).
+
+        Command-line arguments: ``[args]``
+        
+        The ``yt-ann`` command adds a list of o2graph commands that
+        can be used to annotate a yt rendering. Annotations are normal
+        o2graph 2D plotting commands built upon a coordinate system
+        with (0,0) as the lower-left corner of the image and (1,1) as
+        the upper-right corner. Arguments for ``yt-ann`` may include
+        dashes but must end with the word 'end'.
+        
+        For example::
+
+          -yt-ann -text 0.1 0.95 \"Ann. example\" color=w,ha=left end
+        
         The list or arguments in `args` must end with 'end'. 
         If `args` contains only one entry ('end'), then the
         list of annotations is cleared.
+
         """
 
         if len(args)==1 and force_bytes(args[0])==b'end':
             print('Clearing all yt annotations.')
         else:
             for i in range(0,len(args)):
                 if force_bytes(args[i])!=b'end':
                     self.yt_ann.append(args[i])
             print('yt_ann is',self.yt_ann)
         
         return
 
-    def yt_scatter(self,o2scl,amp,args):
+    def yt_scatter(self,o2scl,amp,link,args):
         """
-        Create a 3D scatter plot with yt using data from an
-        O\ :sub:`2`\ scl table object
+        Documentation for o2graph command ``yt-scatter``:
+
+        For objects of type ``table``:
+
+        Add scattered points to a yt scene
+        
+        Command-line arguments: ``<x column> <y column> <z column> 
+        [size column] [red column] [green column] [blue column] 
+        [alpha column]``
+
+        Add a series of points to a yt scene. If a volume has not yet
+        been added, then a default volume is added. If the x, y-, or
+        z-axis limits have not yet been set, then they are set by the
+        limits of the data. If the size column is unspecified, 'none',
+        or 'None', then the default value of 3 is used. If the color
+        columns are unspecified, 'none' or 'None', then [1,1,1] is
+        used, and finally the default for the alpha column is 0.5. If
+        any of the values for the color columns are less than zero or
+        greater than 1, then that color column is rescaled to [0,1].
         """
 
         if len(args)<3:
             print('Function yt_scatter() requires three ',
                   'column arguments.')
             return
 
@@ -3201,64 +3499,31 @@
         if len(args)>=6:
             green_column=args[5]
         if len(args)>=7:
             blue_column=args[6]
         if len(args)>=8:
             alpha_column=args[7]
         
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-                    
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if curr_type==b'table':
             if self.yt_check_backend()==1:
                 return
 
             import yt
             from yt.visualization.volume_rendering.api \
                 import PointSource
-                        
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-                        
-            colx=ctypes.c_char_p(force_bytes(column_x))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),
-                           ctypes.byref(ptrx))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_x+'".')
-                failed=True
-                            
-            coly=ctypes.c_char_p(force_bytes(column_y))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),
-                           ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_y+'".')
-                failed=True
-
-            colz=ctypes.c_char_p(force_bytes(column_z))
-            idz=ctypes.c_int(0)
-            ptrz=double_ptr()
-            get_ret=get_fn(amp,colz,ctypes.byref(idz),
-                           ctypes.byref(ptrz))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_z+'".')
-                failed=True
+
+            failed=False
+            
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            ptrx=tab[force_bytes(column_x)]
+            ptry=tab[force_bytes(column_y)]
+            ptrz=tab[force_bytes(column_z)]
 
             if (force_bytes(size_column)==b'None' or
                 force_bytes(size_column)==b'none'):
                 size_column=''
             if (force_bytes(red_column)==b'None' or
                 force_bytes(red_column)==b'none'):
                 red_column=''
@@ -3272,123 +3537,103 @@
                 force_bytes(alpha_column)==b'none'):
                 alpha_column=''
 
             print('size,red,green,blue,alpha:',size_column,red_column,
                   green_column,blue_column,alpha_column)
             
             if size_column!='':
-                cols=ctypes.c_char_p(force_bytes(size_column))
-                ids=ctypes.c_int(0)
-                ptrs=double_ptr()
-                get_ret=get_fn(amp,cols,ctypes.byref(ids),
-                               ctypes.byref(ptrs))
+                ptrs=tab[force_bytes(size_column)]
                 
             if red_column!='':
-                colr=ctypes.c_char_p(force_bytes(red_column))
-                idr=ctypes.c_int(0)
-                ptrr=double_ptr()
-                get_ret=get_fn(amp,colr,ctypes.byref(idr),
-                               ctypes.byref(ptrr))
+                ptrr=tab[force_bytes(red_column)]
                 
             if green_column!='':
-                colg=ctypes.c_char_p(force_bytes(green_column))
-                idg=ctypes.c_int(0)
-                ptrg=double_ptr()
-                get_ret=get_fn(amp,colg,ctypes.byref(idg),
-                               ctypes.byref(ptrg))
+                ptrg=tab[force_bytes(green_column)]
                 
             if blue_column!='':
-                colb=ctypes.c_char_p(force_bytes(blue_column))
-                idb=ctypes.c_int(0)
-                ptrb=double_ptr()
-                get_ret=get_fn(amp,colb,ctypes.byref(idb),
-                               ctypes.byref(ptrb))
+                ptrb=tab[force_bytes(blue_column)]
                 
             if alpha_column!='':
-                cola=ctypes.c_char_p(force_bytes(alpha_column))
-                ida=ctypes.c_int(0)
-                ptra=double_ptr()
-                get_ret=get_fn(amp,cola,ctypes.byref(ida),
-                               ctypes.byref(ptra))
+                ptra=tab[force_bytes(alpha_column)]
 
             if red_column!='' and blue_column!='' and green_column!='':
                 rescale_r=False
                 rescale_g=False
                 rescale_b=False
-                for i in range(0,idr.value):
+                for i in range(0,len(ptrr)):
                     if ptrr[i]<0.0 or ptrr[i]>1.0:
                         rescale_r=True
                     if ptrg[i]<0.0 or ptrg[i]>1.0:
                         rescale_g=True
                     if ptrb[i]<0.0 or ptrb[i]>1.0:
                         rescale_b=True
                 if rescale_r:
                     min_r=ptrr[0]
                     max_r=ptrr[0]
-                    for i in range(0,idr.value):
+                    for i in range(0,len(ptrr)):
                         if ptrr[i]<min_r:
                             min_r=ptrr[i]
                         if ptrr[i]>max_r:
                             max_r=ptrr[i]
                 if rescale_g:
                     min_g=ptrg[0]
                     max_g=ptrg[0]
-                    for i in range(0,idr.value):
+                    for i in range(0,len(ptrg)):
                         if ptrg[i]<min_g:
                             min_g=ptrg[i]
                         if ptrg[i]>max_g:
                             max_g=ptrg[i]
                 if rescale_b:
                     min_b=ptrb[0]
                     max_b=ptrb[0]
-                    for i in range(0,idr.value):
+                    for i in range(0,len(ptrb)):
                         if ptrb[i]<min_b:
                             min_b=ptrb[i]
                         if ptrb[i]>max_b:
                             max_b=ptrb[i]
                 if rescale_r:
                     print('Rescaling red range   (%0.6e,%0.6e) to (0,1)' %
                           (min_r,max_r))
-                    for i in range(0,idr.value):
+                    for i in range(0,len(ptrr)):
                         ptrr[i]=(ptrr[i]-min_r)/(max_r-min_r)
                 if rescale_g:
                     print('Rescaling green range (%0.6e,%0.6e) to (0,1)' %
                           (min_g,max_g))
-                    for i in range(0,idg.value):
+                    for i in range(0,len(ptrg)):
                         ptrg[i]=(ptrg[i]-min_g)/(max_g-min_g)
                 if rescale_b:
                     print('Rescaling blue range  (%0.6e,%0.6e) to (0,1)' %
                           (min_b,max_b))
-                    for i in range(0,idb.value):
+                    for i in range(0,len(ptrb)):
                         ptrb[i]=(ptrb[i]-min_b)/(max_b-min_b)
                 
             if self.xset==False:
                 self.xlo=ptrx[0]
                 self.xhi=ptrx[0]
-                for i in range(0,idx.value):
+                for i in range(0,len(ptrx)):
                     if ptrx[i]<self.xlo:
                         self.xlo=ptrx[i]
                     if ptrx[i]>self.xhi:
                         self.xhi=ptrx[i]
                 print('Set xlimits to (%0.6e,%0.6e)' % (self.xlo,self.xhi))
                 self.xset=True
             if self.yset==False:
                 self.ylo=ptry[0]
                 self.yhi=ptry[0]
-                for i in range(0,idy.value):
+                for i in range(0,len(ptry)):
                     if ptry[i]<self.ylo:
                         self.ylo=ptry[i]
                     if ptry[i]>self.yhi:
                         self.yhi=ptry[i]
                 print('Set ylimits to (%0.6e,%0.6e)' % (self.ylo,self.yhi))
                 self.yset=True
             if self.zset==False:
                 self.zlo=ptrz[0]
                 self.zhi=ptrz[0]
-                for i in range(0,idz.value):
+                for i in range(0,len(ptrz)):
                     if ptrz[i]<self.zlo:
                         self.zlo=ptrz[i]
                     if ptrz[i]>self.zhi:
                         self.zhi=ptrz[i]
                 print('Set zlimits to (%0.6e,%0.6e)' % (self.zlo,self.zhi))
                 self.zset=True
             x_range=self.xhi-self.xlo
@@ -3402,15 +3647,15 @@
                     icnt=icnt+1
             if icnt==0:
                 self.yt_def_vol()
             
             pts=[]
             cols=[]
             sizes=[]
-            for i in range(0,idx.value):
+            for i in range(0,len(ptrx)):
                 pts.append([(ptrx[i]-self.xlo)/x_range,
                             (ptry[i]-self.ylo)/y_range,
                             (ptrz[i]-self.zlo)/z_range])
                 if red_column=='' or blue_column=='' or green_column=='':
                     cols.append([1.0,1.0,1.0,0.5])
                 else:
                     if alpha_column=='':
@@ -3450,20 +3695,28 @@
                   curr_type,'.')
             
         # End of function o2graph_plotter::yt_scatter()
         return
         
     def yt_vertex_list(self,o2scl,amp,link,args):
         """
-        This function can be accessed in o2graph by the
-        o2graph command ``yt-vertex-list``.
+        Documentation for o2graph command ``yt-vertex-list``:
         
-        Command-line arguments: ``[kwargs]``
-        Plot a series of line segments between a list of
-        vertices specified in an O\ :sub:`2`\ scl table.
+        For objects of type ``table``:
+
+        Draw a line from a series of vertices in a table.
+
+        Command-line arguments: ``<x column> <y column> <z column> 
+        [kwargs]``
+        
+        Create a series of yt LineSource objects in a visualization
+        using the three specified columns as vertices. One line segment
+        will be drawn from the values in the first row to the values in
+        the second row, one line segment from the second row to the
+        third row, and so on.
         """
 
         if len(args)<3:
             print('Function yt_vertex_list() requires three ',
                   'column arguments.')
             return
 
@@ -3477,67 +3730,31 @@
                 print('yt-source-list',icnt,key,type(value))
                 icnt=icnt+1
         # If there are no yt sources yet, then create a
         # default volume object
         if icnt==0:
             self.yt_def_vol()
 
-        #amt=acol_manager(link,amp)
-        #print('curr_type:',amt.get_type())
-            
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-        double_ptr=ctypes.POINTER(ctypes.c_double)
-        double_ptr_ptr=ctypes.POINTER(double_ptr)
-                    
-        curr_type=o2scl_get_type(o2scl,amp)
+        curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
         if curr_type==b'table':
             if self.yt_check_backend()==1:
                 return
 
             import yt
             from yt.visualization.volume_rendering.api \
                 import LineSource
-                        
-            get_fn=o2scl.o2scl_acol_get_column
-            get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                             int_ptr,double_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-                        
-            colx=ctypes.c_char_p(force_bytes(column_x))
-            idx=ctypes.c_int(0)
-            ptrx=double_ptr()
-            get_ret=get_fn(amp,colx,ctypes.byref(idx),
-                           ctypes.byref(ptrx))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_x+'".')
-                failed=True
-                            
-            coly=ctypes.c_char_p(force_bytes(column_y))
-            idy=ctypes.c_int(0)
-            ptry=double_ptr()
-            get_ret=get_fn(amp,coly,ctypes.byref(idy),
-                           ctypes.byref(ptry))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_y+'".')
-                failed=True
-
-            colz=ctypes.c_char_p(force_bytes(column_z))
-            idz=ctypes.c_int(0)
-            ptrz=double_ptr()
-            get_ret=get_fn(amp,colz,ctypes.byref(idz),
-                           ctypes.byref(ptrz))
-            if get_ret!=0:
-                print('Failed to get column named "'+
-                      column_z+'".')
-                failed=True
+
+            failed=False
+            
+            amt=acol_manager(self.link2,amp)
+            tab=amt.get_table_obj()
+            ptrx=tab[force_bytes(column_x)]
+            ptry=tab[force_bytes(column_y)]
+            ptrz=tab[force_bytes(column_z)]
 
             if self.xset==False:
                 self.xlo=ptrx[0]
                 self.xhi=ptrx[0]
                 for i in range(0,idx.value):
                     if ptrx[i]<self.xlo:
                         self.xlo=ptrx[i]
@@ -3600,26 +3817,26 @@
                   curr_type+'.')
             
         # End of function o2graph_plotter::yt_vertex_list()
         return
         
     def yt_mesh(self,o2scl,amp,link,args):
         """
-        Plot a mesh from vertices specified by a slice of O\ :sub:`2`\ scl
+        Plot a mesh from vertices specified by a slice of O2scl
         table3d object.
         """
 
         if len(args)<1:
             print('Function yt_mesh() requires a slice ',
                   'column arguments.')
             return
 
         slc=args[0]
 
-        amt=acol_manager(link,amp)
+        amt=acol_manager(self.link2,amp)
         curr_type=amt.get_type()
             
         if curr_type==b'table3d':
             if self.yt_check_backend()==1:
                 return
 
             import yt
@@ -3705,59 +3922,43 @@
         else:
             print('Command yt-mesh does not work with type',
                   curr_type+'.')
             
         # End of function o2graph_plotter::yt_mesh()
         return
         
-    def commands(self,o2scl,amp,args):
+    def commands(self,o2scl,amp,link,args):
         """
         Output the currently available commands.
         """
 
+        amt=acol_manager(self.link2,amp)
         ter=terminal_py()
+        cl=amt.get_cl()
         
-        # C types
-        int_ptr=ctypes.POINTER(ctypes.c_int)
-        int_ptr_ptr=ctypes.POINTER(int_ptr)
-        char_ptr=ctypes.POINTER(ctypes.c_char)
-        char_ptr_ptr=ctypes.POINTER(char_ptr)
-            
-        # Function arguments
-        this_type=ctypes.c_char_p(b'')
-        size=ctypes.c_int(0)
-        iptr=int_ptr()
-        cptr=char_ptr()
-            
-        # Function interfaces
-        get_fn=o2scl.o2scl_acol_get_cli_options
-        get_fn.argtypes=[ctypes.c_void_p,int_ptr,int_ptr_ptr,
-                         char_ptr_ptr]
-        get_fn.restype=ctypes.c_int
-
-        get_type_fn=o2scl.o2scl_acol_get_cli_options_type
-        get_type_fn.argtypes=[ctypes.c_void_p,char_ptr,int_ptr,
-                              int_ptr_ptr,char_ptr_ptr]
-        get_type_fn.restype=ctypes.c_int
-
         if len(args)>0 and args[0]=='all':
 
             print('Commands from acol which do not require a current',
                   'object:\n')
+
+            old_type=amt.get_type()
+            amt.command_del(old_type)
+            amt.command_add(b'')
+            list_temp=cl.get_option_list()
+            base_acol_comm_list=[]
+            for i in range(0,len(list_temp)):
+                base_acol_comm_list.append(list_temp[i])
+            amt.command_del(b'')
+            amt.command_add(old_type)
             
-            # Function call
-            get_ret=get_type_fn(amp,this_type,ctypes.byref(size),
-                                ctypes.byref(iptr),ctypes.byref(cptr))
-    
-            base_acol_comm_list=get_ic_ptrs_to_list(size,iptr,cptr)
             base_acol_comm_list=sorted(base_acol_comm_list)
             comm_list=[]
             for i in range(0,len(base_acol_comm_list)):
-                st=base_acol_comm_list[i].decode('utf-8')
-                comm_list.append(ter.cmd_str(st))
+                st=force_string(base_acol_comm_list[i])
+                comm_list.append(ter.cmd_str(st,amt))
             
             comm_rows=screenify_py(comm_list)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
 
             print(' ')
             
@@ -3765,58 +3966,51 @@
                   'object:\n')
 
             comm_list=[]
             for line in base_list:
                 comm_list.append(force_bytes(line[0]))
             comm_list_dec=sorted(comm_list)
             for i in range(0,len(comm_list_dec)):
-                comm_list_dec[i]=ter.cmd_str(comm_list_dec[i].decode('utf-8'))
+                comm_list_dec[i]=ter.cmd_str(comm_list_dec[i].decode('utf-8'),
+                                             amt)
             comm_rows=screenify_py(comm_list_dec)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
                 
             print(' ')
 
             for this_type in acol_types:
                 
                 print('Acol and o2graph commands for an object of type '+
-                      ter.type_str(str(this_type))+':\n')
+                      ter.type_str(force_string(this_type),amt)+':\n')
                 
-                # Function interface
-                get_fn=o2scl.o2scl_acol_get_cli_options_type
-                get_fn.argtypes=[ctypes.c_void_p,char_ptr,int_ptr,int_ptr_ptr,
-                                 char_ptr_ptr]
-                get_fn.restype=ctypes.c_int
-        
-                # Arguments
-                size=ctypes.c_int(0)
-                iptr=int_ptr()
-                cptr=char_ptr()
-                this_type2=ctypes.c_char_p(force_bytes(this_type))
-                
-                # Function call
-                get_ret=get_fn(amp,this_type2,ctypes.byref(size),
-                               ctypes.byref(iptr),ctypes.byref(cptr))
-        
-                # comm_list is the list of acol commands for this type
-                comm_list=get_ic_ptrs_to_list(size,iptr,cptr)
+                old_type=amt.get_type()
+                amt.command_del(old_type)
+                amt.command_add(force_bytes(this_type))
+                temp_list=cl.get_option_list()
+                comm_list=[]
+                for i in range(0,len(temp_list)):
+                    comm_list.append(temp_list[i])
+                amt.command_del(force_bytes(this_type))
+                amt.command_add(old_type)
                 
                 for line in extra_list:
                     if (this_type==line[0] or
                         this_type==force_bytes(line[0])):
                         comm_list.append(force_bytes(line[1]))
 
                 comm_list2=sorted(comm_list)
                 for comm_entry in base_acol_comm_list:
                     if comm_entry in comm_list:
                         comm_list2.remove(comm_entry)
 
                 if len(comm_list2)>0:
                     for i in range(0,len(comm_list2)):
-                        comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'))
+                        comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'),
+                                                  amt)
                     comm_rows=screenify_py(comm_list2)
                     for i in range(0,len(comm_rows)):
                         print(comm_rows[i])
                 else:
                     print('<none>')
                     
                 print(' ')
@@ -3828,132 +4022,95 @@
             if curr_type not in acol_types:
                 print("Command 'commands' cannot find type ",curr_type+'.')
                 print('List of valid types:')
                 print('')
                 print(acol_types)
                 return
 
-            # C types
-            int_ptr=ctypes.POINTER(ctypes.c_int)
-            int_ptr_ptr=ctypes.POINTER(int_ptr)
-            char_ptr=ctypes.POINTER(ctypes.c_char)
-            char_ptr_ptr=ctypes.POINTER(char_ptr)
-        
-            # Function interface
-            get_fn=o2scl.o2scl_acol_get_cli_options_type
-            get_fn.argtypes=[ctypes.c_void_p,char_ptr,int_ptr,int_ptr_ptr,
-                             char_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            # Arguments
-            size=ctypes.c_int(0)
-            iptr=int_ptr()
-            cptr=char_ptr()
-            curr_type2=ctypes.c_char_p(force_bytes(curr_type))
-        
-            # Function call
-            get_ret=get_fn(amp,curr_type2,ctypes.byref(size),
-                           ctypes.byref(iptr),ctypes.byref(cptr))
-
+            old_type=amt.get_type()
+            amt.command_del(old_type)
+            amt.command_add(force_bytes(curr_type))
+            temp_list=cl.get_option_list()
+            comm_list=[]
+            for i in range(0,len(temp_list)):
+                comm_list.append(temp_list[i])
+            amt.command_del(force_bytes(curr_type))
+            amt.command_add(old_type)
+                
             # comm_list is the list of acol commands for this type
             print('Commands from acol for objects of type',
-                  ter.type_str(curr_type)+':')
+                  ter.type_str(curr_type,amt)+':')
             print('')
-            comm_list=get_ic_ptrs_to_list(size,iptr,cptr)
             
             comm_list2=sorted(comm_list)
             for i in range(0,len(comm_list2)):
-                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'))
+                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'),
+                                          amt)
             comm_rows=screenify_py(comm_list2)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
             print('')
 
             print('Commands from o2graph which do not require a current',
                   'object.')
             print('')
             comm_list=[]
             for line in base_list:
                 comm_list.append(force_bytes(line[0]))
 
             comm_list2=sorted(comm_list)
             for i in range(0,len(comm_list2)):
-                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'))
+                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'),
+                                          amt)
             comm_rows=screenify_py(comm_list2)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
             print('')
                 
             print('Commands from o2graph for objects of type',
-                  ter.type_str(curr_type)+':')
+                  ter.type_str(curr_type,amt)+':')
             print('')
             comm_list=[]
             for line in extra_list:
                 if (curr_type==line[0] or
                     curr_type==force_bytes(line[0])):
                     comm_list.append(force_bytes(line[1]))
 
             comm_list2=sorted(comm_list)
             for i in range(0,len(comm_list2)):
-                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'))
+                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'),
+                                          amt)
             comm_rows=screenify_py(comm_list2)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
                         
         else:
 
-            int_ptr=ctypes.POINTER(ctypes.c_int)
-            double_ptr=ctypes.POINTER(ctypes.c_double)
-            char_ptr=ctypes.POINTER(ctypes.c_char)
-            double_ptr_ptr=ctypes.POINTER(double_ptr)
-            char_ptr_ptr=ctypes.POINTER(char_ptr)
-            
-            curr_type=o2scl_get_type(o2scl,amp)
+            curr_type=o2scl_get_type(o2scl,amp,self.link2)
 
             if curr_type==b'':
                 print('O2graph commands which do not require a '+
                       'current object.')
             else:
                 print('O2graph commands for an object of type '+
-                      ter.type_str(curr_type.decode('utf-8'))+':\n')
+                      ter.type_str(curr_type.decode('utf-8'),amt)+':\n')
             
-            # C types
-            int_ptr=ctypes.POINTER(ctypes.c_int)
-            int_ptr_ptr=ctypes.POINTER(int_ptr)
-            char_ptr=ctypes.POINTER(ctypes.c_char)
-            char_ptr_ptr=ctypes.POINTER(char_ptr)
-        
-            # Function interface
-            get_fn=o2scl.o2scl_acol_get_cli_options
-            get_fn.argtypes=[ctypes.c_void_p,int_ptr,int_ptr_ptr,
-                             char_ptr_ptr]
-            get_fn.restype=ctypes.c_int
-
-            # Arguments
-            size=ctypes.c_int(0)
-            iptr=int_ptr()
-            cptr=char_ptr()
-        
-            # Function call
-            get_ret=get_fn(amp,ctypes.byref(size),
-                           ctypes.byref(iptr),ctypes.byref(cptr))
-
-            # comm_list is the list of acol commands for this type
-            comm_list=get_ic_ptrs_to_list(size,iptr,cptr)
+            comm_list=cl.get_option_list().to_list()
             
             for line in base_list:
                 comm_list.append(force_bytes(line[0]))
             for line in extra_list:
                 if (curr_type==line[0] or
                     curr_type==force_bytes(line[0])):
                     comm_list.append(force_bytes(line[1]))
 
             comm_list2=sorted(comm_list)
             for i in range(0,len(comm_list2)):
-                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'))
+                comm_list2[i]=ter.cmd_str(comm_list2[i].decode('utf-8'),
+                                          amt)
             comm_rows=screenify_py(comm_list2)
             for i in range(0,len(comm_rows)):
                 print(comm_rows[i])
                         
         # End of function o2graph_plotter::commands()
         return
 
@@ -3984,15 +4141,15 @@
                    sigma_clip=self.yt_sigma_clip,dpi=100)
             self.yt_trans=self.yt_scene._render_figure.transFigure
             self.axes=axt.axes
             self.fig=self.yt_scene._render_figure
             self.canvas_flag=True
             if self.verbose>1:
                 print('Adding annotations:')
-            self.parse_string_list(self.yt_ann,o2scl,amp,link)
+            self.parse_string_list(self.yt_ann,o2scl,amp,self.link2)
             if self.verbose>1:
                 print('Done adding annotations:')
             #self.text(0.1,0.9,'x',color='w',fontsize=self.font*1.25,
                 #transform=tf)
             self.canvas_flag=False
             #axt.axes.text(0.1,0.9,'test',color='w',transform=tf,
             #fontsize=self.font*1.25)
@@ -4011,16 +4168,16 @@
         # After having saved the image, filter it
         self.filter_image(fname)
             
         return
 
     def _make_fname(self,prefix,suffix,i_frame,n_frames):
         """
-        Construct the animation filename from frame index and frame total,
-        padding with zeros when necessary.
+        Construct the animation filename from frame index and frame 
+        total, padding with zeros when necessary. 
         """
         if n_frames>=1000:
             if i_frame<10:
                 fname2=prefix+'000'+str(i_frame)+suffix
             elif i_frame<100:
                 fname2=prefix+'00'+str(i_frame)+suffix
             elif i_frame<1000:
@@ -4042,15 +4199,15 @@
         else:
             fname2=prefix+str(i_frame)+suffix
         return fname2
 
     def restore_position(self,pos):
         """
         Restore the value of self.yt_position from the array 'pos'
-        which is 
+        which is ...
         """
         
         if self.yt_position=='default':
             self.yt_position=str([pos[0]*(self.xhi-self.xlo)+
                                   self.xlo,
                                   pos[1]*(self.yhi-self.ylo)+
                                   self.ylo,
@@ -4199,31 +4356,44 @@
             print('Moving file back:',
                   'mv /tmp/yt_filtered.png '+fname)
             os.system('mv /tmp/yt_filtered.png '+fname)
         return
     
     def yt_render(self,o2scl,amp,link,fname,mov_fname='',loop=False):
         """
-        Complete the yt render and save the image to a file. If necessary,
-        compile the images into a movie and save into the specified
-        file name.
+        Documentation for o2graph command ``yt-render``:
+
+        Render the yt volume visualization.
+
+        Command-line arguments: ``<filename or pattern> [kwargs]``
+
+        Perform the volume rendering. If yt_path is empty, then the
+        first argument is the filename. If yt_path is not empty then
+        the first argument is a filename pattern containing * where
+        each frame will be stored. If yt_path is not empty and a movie
+        filename is given, then ffmpeg will be used to combine the
+        frames into an mp4 file.
+
+        The keyword argument ``mov_fname`` specifies the output
+        movie file (if an animation is specified with ``yt-path``).
+        If empty, the filename ``o2graph.mp4`` is used. 
         """
 
         if self.yt_scene==0:
             print('Cannot perform a yt render without a scene.')
             return
         
         # AWS 10/14/19 the call to save() below does
         # the render() so I don't think I need this
         #self.yt_scene.render()
 
         if len(self.yt_path)==0:
 
             # No path, so just call save and finish
-            self.yt_save_annotate(o2scl,amp,link,fname);
+            self.yt_save_annotate(o2scl,amp,self.link2,fname);
 
         else:
 
             # Setup destination filename
             if mov_fname=='':
                 print('No movie filename specified so using',
                       'o2graph.mp4')
@@ -4242,15 +4412,15 @@
             for ip in range(0,len(self.yt_path)):
                 n_frames=n_frames+int(self.yt_path[ip][1])
             print(n_frames,'total frames')
 
             # Render initial frame
             i_frame=0
             fname2=self._make_fname(prefix,suffix,i_frame,n_frames)
-            self.yt_save_annotate(o2scl,amp,link,fname2);
+            self.yt_save_annotate(o2scl,amp,self.link2,fname2);
 
             # Loop over all movements
             for ip in range(0,len(self.yt_path)):
 
                 # Number of frames for this movement
                 n_frames_move=int(self.yt_path[ip][1])
             
@@ -4312,15 +4482,15 @@
                             
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
-                        self.yt_save_annotate(o2scl,amp,link,fname2);
+                        self.yt_save_annotate(o2scl,amp,self.link2,fname2);
                     
                         # End of 'for ifr in range(0,n_frames_move)'
                     
                     # Restore position array
                     self.restore_position(pos)
                     
                     # End of loop 'if self.yt_path[ip][0]=='yaw''
@@ -4352,15 +4522,15 @@
                         
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
-                        self.yt_save_annotate(o2scl,amp,link,fname2);
+                        self.yt_save_annotate(o2scl,amp,self.link2,fname2);
                         
                         # End of 'for ifr in range(0,n_frames_move)'
 
                     # Width
                     self.restore_width(self.yt_camera.width)
                         
                     # End of loop 'if self.yt_path[ip][0]=='zoom''
@@ -4413,15 +4583,15 @@
 
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
-                        self.yt_save_annotate(o2scl,amp,link,fname2);
+                        self.yt_save_annotate(o2scl,amp,self.link2,fname2);
 
                         # End of 'for ifr in range(0,n_frames_move)'
                         
                     # Restore position array
                     self.restore_position(pos)
 
                     # End of loop 'if self.yt_path[ip][0]=='move''
@@ -4474,15 +4644,15 @@
 
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
-                        self.yt_save_annotate(o2scl,amp,link,fname2);
+                        self.yt_save_annotate(o2scl,amp,self.link2,fname2);
 
                         # End of 'for ifr in range(0,n_frames_move)'
                         
                 elif self.yt_path[ip][0]=='moveauto':
 
                     # Move the camera, automatically changing the
                     # focus to lie along the direction of motion
@@ -4562,15 +4732,15 @@
 
                         # Update text objects
                         self.yt_update_text()
 
                         # Save new frame
                         fname2=self._make_fname(prefix,suffix,
                                                 i_frame,n_frames)
-                        self.yt_save_annotate(o2scl,amp,link,fname2);
+                        self.yt_save_annotate(o2scl,amp,self.link2,fname2);
 
                         # End of 'for ifr in range(0,n_frames_move)'
                         
                 # End of 'for ip in range(0,len(self.yt_path)):'
 
             # -r is rate (in frames/sec), -f is format, -vcodec is
             # video codec (apparently 420p works well with quicktime),
@@ -4702,49 +4872,62 @@
                     if self.verbose>2:
                         print('Process set.')
                         print('args:',strlist[ix:ix_next])
                         
                     if ix_next-ix<3:
                         print('Not enough parameters for set option.')
                     else:
-                        self.set_wrapper(o2scl,amp,strlist[ix+1:ix_next])
+                        self.set_wrapper(o2scl,amp,self.link2,strlist[ix+1:ix_next])
                         
-                elif cmd_name=='cmap':
+                elif cmd_name=='ell-max':
 
                     if self.verbose>2:
-                        print('Process cmap.')
+                        print('Process ell-max.')
                         print('args:',strlist[ix:ix_next])
                         
-                    if ix_next-ix<3:
-                        print('Not enough parameters for set option.')
+                    if ix_next-ix<1:
+                        print('Not enough parameters for ell-max option.')
                     else:
-                        self.cmap(strlist[ix+1],strlist[ix+2:ix_next])
+                        self.ell_max(strlist[ix+1],strlist[ix+2:ix_next])
                         
-                elif cmd_name=='cmap2':
+                elif cmd_name=='colors':
 
                     if self.verbose>2:
-                        print('Process cmap2.')
+                        print('Process colors.')
                         print('args:',strlist[ix:ix_next])
                         
-                    if ix_next-ix<3:
-                        print('Not enough parameters for set option.')
+                    if ix_next-ix<1:
+                        print('Not enough parameters for ell-max option.')
                     else:
-                        self.cmap2(strlist[ix+1],strlist[ix+2:ix_next])
+                        self.colors(strlist[ix+1:ix_next])
+                        
+                elif cmd_name=='cmap':
+
+                    if self.verbose>2:
+                        print('Process cmap.')
+                        print('args:',strlist[ix:ix_next])
+                        
+                    if ix_next-ix<2:
+                        print('Not enough parameters for cmap option.')
+                    elif ix_next-ix<3:
+                        self.cmap(strlist[ix+1])
+                    else:
+                        self.cmap(strlist[ix+1],strlist[ix+2:ix_next])
                         
                 elif cmd_name=='make-png':
 
                     if self.verbose>2:
                         print('Process make-png.')
                         print('args:',strlist[ix:ix_next])
                         
                     if ix_next-ix<3:
-                        print('Not enough parameters for set option.')
+                        print('Not enough parameters for make-png option.')
                     else:
-                        self.make_png(o2scl,amp,
-                                      strlist[ix+1:ix_next])
+                        self.make_png_o2graph(o2scl,amp,self.link2,
+                                              strlist[ix+1:ix_next])
                         
                 elif cmd_name=='get':
                     
                     if self.verbose>2:
                         print('Process get.')
                         print('args:',strlist[ix:ix_next])
                         
@@ -4755,36 +4938,36 @@
 
                 elif cmd_name=='commands':
                     
                     if self.verbose>2:
                         print('Process commands.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.commands(o2scl,amp,
+                    self.commands(o2scl,amp,self.link2,
                                   strlist[ix+1:ix_next])
                     
                 elif cmd_name=='yt-add-vol':
 
                     if self.verbose>2:
                         print('Process yt-add-vol.')
                         print('args:',strlist[ix:ix_next])
                         
-                    self.yt_add_vol(o2scl,amp,
+                    self.yt_add_vol(o2scl,amp,self.link2,
                                     strlist[ix+1:ix_next])
                     
                 elif cmd_name=='yt-scatter':
 
                     if self.verbose>2:
                         print('Process yt-scatter.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<4:
                         print('Not enough parameters for yt-scatter.')
                     else:
-                        self.yt_scatter(o2scl,amp,strlist[ix+1:ix_next])
+                        self.yt_scatter(o2scl,amp,self.link2,strlist[ix+1:ix_next])
                                                     
                 elif cmd_name=='yt-path':
 
                     if self.verbose>2:
                         print('Process yt-path.')
                         print('args:',strlist[ix:ix_next])
 
@@ -4952,27 +5135,27 @@
                     if self.verbose>2:
                         print('Process yt-vertex-list.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<4:
                         print('Not enough parameters for yt-vertex-list.')
                     else:
-                        self.yt_vertex_list(o2scl,amp,link,
+                        self.yt_vertex_list(o2scl,amp,self.link2,
                                             strlist[ix+1:ix_next])
                                                     
                 elif cmd_name=='yt-mesh':
 
                     if self.verbose>2:
                         print('Process yt-mesh.')
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<2:
                         print('Not enough parameters for yt-mesh.')
                     else:
-                        self.yt_mesh(o2scl,amp,link,
+                        self.yt_mesh(o2scl,amp,self.link2,
                                      strlist[ix+1:ix_next])
                                                     
                 elif cmd_name=='yt-source-list':
 
                     if self.verbose>2:
                         print('Process yt-source-list.')
                         print('args:',strlist[ix:ix_next])
@@ -5006,17 +5189,17 @@
                     if self.verbose>2:
                         print('Process render.')
                         print('args:',strlist[ix:ix_next])
                         
                     if ix_next-ix<2:
                         print('Not enough parameters for yt-render.')
                     elif ix_next-ix<3:
-                        self.yt_render(o2scl,amp,link,strlist[ix+1])
+                        self.yt_render(o2scl,amp,self.link2,strlist[ix+1])
                     else:
-                        self.yt_render(o2scl,amp,link,strlist[ix+1],
+                        self.yt_render(o2scl,amp,self.link2,strlist[ix+1],
                                        **string_to_dict(strlist[ix+2]))
 
                 elif cmd_name=='yt-tf':
 
                     if self.verbose>2:
                         print('Process yt-tf.')
                         print('args:',strlist[ix:ix_next])
@@ -5025,114 +5208,153 @@
                     
                 elif cmd_name=='help' or cmd_name=='h':
                     
                     if self.verbose>2:
                         print('Process help.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.help_func(o2scl,amp,strlist[ix+1:ix_next])
+                    self.help_func(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='plot':
                     
                     if self.verbose>2:
                         print('Process plot.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.plot(o2scl,amp,strlist[ix+1:ix_next],link)
+                    self.plot_o2graph(o2scl,amp,strlist[ix+1:ix_next],self.link2)
 
                 elif cmd_name=='plot-color':
                     
                     if self.verbose>2:
                         print('Process plot-color.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.plot_color(o2scl,amp,strlist[ix+1:ix_next])
+                    self.plot_color(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='rplot':
                     
                     if self.verbose>2:
                         print('Process rplot.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.rplot(o2scl,amp,strlist[ix+1:ix_next])
+                    self.rplot(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='scatter':
                     
                     if self.verbose>2:
                         print('Process scatter.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.scatter(o2scl,amp,strlist[ix+1:ix_next])
+                    self.scatter(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='hist-plot':
                     
                     if self.verbose>2:
                         print('Process hist-plot.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.hist_plot(o2scl,amp,strlist[ix+1:ix_next])
+                    self.hist_plot(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='errorbar':
                     
                     if self.verbose>2:
                         print('Process errorbar.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.errorbar(o2scl,amp,strlist[ix+1:ix_next])
+                    self.errorbar(o2scl,amp,self.link2,strlist[ix+1:ix_next])
 
                 elif cmd_name=='hist2d-plot':
                     
                     if self.verbose>2:
                         print('Process hist2d-plot.')
                         print('args:',strlist[ix:ix_next])
                         
-                    self.hist2d_plot(o2scl,amp,strlist[ix+1:ix_next])
+                    self.hist2d_plot(o2scl,amp,self.link2,
+                                     strlist[ix+1:ix_next])
                             
                 elif cmd_name=='den-plot':
                     
                     if self.verbose>2:
                         print('Process den-plot.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.den_plot(o2scl,amp,strlist[ix+1:ix_next])
+                    self.den_plot_o2graph(o2scl,amp,self.link2,
+                                          strlist[ix+1:ix_next])
+                
+                elif cmd_name=='mp4':
+                    
+                    if self.verbose>2:
+                        print('Process mp4.')
+                        print('args:',strlist[ix:ix_next])
+
+                    self.mp4(strlist[ix+1:ix_next])
+                
+                elif cmd_name=='kde-plot':
+                    
+                    if self.verbose>2:
+                        print('Process kde-plot.')
+                        print('args:',strlist[ix:ix_next])
+
+                    self.kde_plot(o2scl,amp,strlist[ix+1:ix_next],
+                                  self.link2)
+                
+                elif cmd_name=='kde-2d-plot':
+                    
+                    if self.verbose>2:
+                        print('Process kde-2d-plot.')
+                        print('args:',strlist[ix:ix_next])
+
+                    self.kde_2d_plot(o2scl,amp,strlist[ix+1:ix_next],
+                                  self.link2)
+                
+                elif cmd_name=='to-kde':
+                    
+                    if self.verbose>2:
+                        print('Process to-kde.')
+                        print('args:',strlist[ix:ix_next])
+
+                    self.to_kde(o2scl,amp,self.link2,
+                                strlist[ix+1:ix_next])
                 
                 elif cmd_name=='den-plot-rgb':
                     
                     if self.verbose>2:
                         print('Process den-plot-rgb.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.den_plot_rgb(o2scl,amp,strlist[ix+1:ix_next])
+                    self.den_plot_rgb_o2graph(o2scl,amp,self.link2,
+                                              strlist[ix+1:ix_next])
                 
                 elif cmd_name=='den-plot-anim':
                     
                     if self.verbose>2:
                         print('Process den-plot-anim.')
                         print('args:',strlist[ix:ix_next])
 
-                    self.den_plot_anim(o2scl,amp,strlist[ix+1:ix_next])
+                    self.den_plot_anim(o2scl,amp,self.link2,
+                                       strlist[ix+1:ix_next])
                 
                 elif cmd_name=='plot1':
                     
                     if self.verbose>2:
                         print('Process plot1.')
                         print('args:',strlist[ix:ix_next])
                         
-                    self.plot1(o2scl,amp,strlist[ix+1:ix_next])
+                    self.plot1(o2scl,amp,self.link2,strlist[ix+1:ix_next])
                             
                 elif cmd_name=='plotv':
                     
                     if self.verbose>2:
                         print('Process plotv.')
                         print('args:',strlist[ix:ix_next])
                         
                     if ix_next-ix<2:
                         print('Not enough parameters for plotv option.')
                     else:
-                        self.plotv(o2scl,amp,strlist[ix+1:ix_next])
+                        self.plotv(o2scl,amp,self.link2,strlist[ix+1:ix_next])
                                                     
                 elif cmd_name=='text':
                     
                     if self.verbose>2:
                         print('Process text.')
                         print('args:',strlist[ix:ix_next])
                         
@@ -5291,15 +5513,15 @@
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<2:
                         print('Not enough parameters for xtitle option.')
                     elif ix_next-ix==2:
                         self.xtitle(strlist[ix+1])
                     elif ix_next-ix>2 and ix_next-ix<5:
-                        print('All three location parameters needed.')
+                        print('All three location parameters (xtitle).')
                     elif ix_next-ix==5:
                         self.xtitle(strlist[ix+1],
                                     loc=[float(eval(strlist[ix+2])),
                                          float(eval(strlist[ix+3])),
                                          float(eval(strlist[ix+4]))])
                         
                 elif cmd_name=='ytitle':
@@ -5309,15 +5531,15 @@
                         print('args:',strlist[ix:ix_next])
 
                     if ix_next-ix<2:
                         print('Not enough parameters for ytitle option.')
                     elif ix_next-ix==2:
                         self.ytitle(strlist[ix+1])
                     elif ix_next-ix>2 and ix_next-ix<5:
-                        print('All three location parameters needed.')
+                        print('All three location parameters needed (ytitle).')
                     elif ix_next-ix==5:
                         self.ytitle(strlist[ix+1],
                                     loc=[float(eval(strlist[ix+2])),
                                          float(eval(strlist[ix+3])),
                                          float(eval(strlist[ix+4]))])
                         
                 # elif cmd_name=='ztitle':
@@ -5575,28 +5797,33 @@
                     if self.verbose>2:
                         print('Process backend in __init__.py.')
                         print('args:',strlist[ix:ix_next])
                 else:
                     if self.verbose>2:
                         print('Process acol command '+cmd_name+'.')
                         print('args:',strlist[ix:ix_next])
-                    self.gen_acol(o2scl,amp,cmd_name,
+                    self.gen_acol(o2scl,amp,self.link2,cmd_name,
                                   strlist[ix+1:ix_next])
-                    if (cmd_name=='v' or cmd_name=='version'):
-                        try:
-                            import h5py
-                        except:
-                            print('\n(Import h5py failed.)')
-                        else:
-                            vv=h5py.h5.get_libversion()
-                            print('\nHDF5 version from h5py:',
-                                  vv[0],vv[1],vv[2])
+                    # AWS, 3/9/23: I had to take this out, I think
+                    # because it's not supported in the older version
+                    # of HDF5 which is used in Ubuntu, but at some
+                    # point I can put it back.
+                    #
+                    # if (cmd_name=='v' or cmd_name=='version'):
+                    #     try:
+                    #         import h5py
+                    #     except:
+                    #         print('\n(Import h5py failed.)')
+                    #     else:
+                    #         vv=h5py.h5.get_libversion()
+                    #         print('\nHDF5 version from h5py:',
+                    #               vv[0],vv[1],vv[2])
                     
                 # Increment to the next option
                 ix=ix_next
                 
             if self.verbose>2:
-                print('Going to next.')
+                print('Going to next argument in parse_string_list().')
                 
         # End of function o2graph_plotter::parse_string_list()
         return
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/part.py` & `o2sclpy-0.928/o2sclpy/part.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 
-  Copyright (C) 2020-2022, Andrew W. Steiner
+  Copyright (C) 2020-2023, Andrew W. Steiner
 
   This file is part of O2scl.
 
   O2scl is free software; you can redistribute it and/or modify
   it under the terms of the GNU General Public License as published by
   the Free Software Foundation; either version 3 of the License, or
   (at your option) any later version.
@@ -14,15 +14,15 @@
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU General Public License for more details.
 
   You should have received a copy of the GNU General Public License
   along with O2scl. If not, see <http://www.gnu.org/licenses/>.
 
-  -------------------------------------------------------------------
+  ───────────────────────────────────────────────────────────────────
 """
 
 import ctypes
 from abc import abstractmethod
 from o2sclpy.utils import force_bytes
 
 class thermo:
@@ -68,15 +68,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class thermo
         
-        Returns: a thermo object
+        Returns: thermo object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def ed(self):
@@ -182,15 +182,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class part
         
-        Returns: a part object
+        Returns: part object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def g(self):
@@ -476,15 +476,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion
         
-        Returns: a fermion object
+        Returns: fermion object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def kf(self):
@@ -525,17 +525,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class quark(fermion):
     """
-    Python interface for O\ :sub:`2`\ scl class ``quark``,
+    Python interface for O2scl class ``quark``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/quark.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/quark.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class quark
 
         | Parameters:
@@ -568,15 +568,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class quark
         
-        Returns: a quark object
+        Returns: quark object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def B(self):
@@ -662,15 +662,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_zerot
         
-        Returns: a fermion_zerot object
+        Returns: fermion_zerot object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def kf_from_density(self,f):
         """
@@ -763,15 +763,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_thermo
         
-        Returns: a fermion_thermo object
+        Returns: fermion_thermo object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_mu_deg(self,f,T,prec):
         """
@@ -886,15 +886,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_rel
         
-        Returns: a fermion_rel object
+        Returns: fermion_rel object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def err_nonconv(self):
@@ -953,34 +953,14 @@
         """
         func=self._link.o2scl.o2scl_fermion_rel_set_deg_limit
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
     @property
-    def exp_limit(self):
-        """
-        Property of type ``ctypes.c_double``
-        """
-        func=self._link.o2scl.o2scl_fermion_rel_get_exp_limit
-        func.restype=ctypes.c_double
-        func.argtypes=[ctypes.c_void_p]
-        return func(self._ptr)
-
-    @exp_limit.setter
-    def exp_limit(self,value):
-        """
-        Setter function for fermion_rel::exp_limit .
-        """
-        func=self._link.o2scl.o2scl_fermion_rel_set_exp_limit
-        func.argtypes=[ctypes.c_void_p,ctypes.c_double]
-        func(self._ptr,value)
-        return
-
-    @property
     def upper_limit_fac(self):
         """
         Property of type ``ctypes.c_double``
         """
         func=self._link.o2scl.o2scl_fermion_rel_get_upper_limit_fac
         func.restype=ctypes.c_double
         func.argtypes=[ctypes.c_void_p]
@@ -1237,15 +1217,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_nonrel
         
-        Returns: a fermion_nonrel object
+        Returns: fermion_nonrel object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_density(self,f,T):
         """
@@ -1281,17 +1261,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,f._ptr,T)
         return
 
 
 class boson(part):
     """
-    Python interface for O\ :sub:`2`\ scl class ``boson``,
+    Python interface for O2scl class ``boson``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/boson.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/boson.html .
     """
 
     def __init__(self,link,pointer=0):
         """
         Init function for class boson
 
         | Parameters:
@@ -1324,15 +1304,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class boson
         
-        Returns: a boson object
+        Returns: boson object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def co(self):
@@ -1353,17 +1333,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,value)
         return
 
 
 class boson_rel:
     """
-    Python interface for O\ :sub:`2`\ scl class ``boson_rel``,
+    Python interface for O2scl class ``boson_rel``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/boson_rel.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/boson_rel.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -1400,15 +1380,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class boson_rel
         
-        Returns: a boson_rel object
+        Returns: boson_rel object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_density(self,b,T):
         """
@@ -1509,15 +1489,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class classical_thermo
         
-        Returns: a classical_thermo object
+        Returns: classical_thermo object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_density(self,p,T):
         """
@@ -1585,15 +1565,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class thermo_np_deriv_press
         
-        Returns: a thermo_np_deriv_press object
+        Returns: thermo_np_deriv_press object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def dsdT(self):
@@ -1759,15 +1739,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class thermo_np_deriv_helm
         
-        Returns: a thermo_np_deriv_helm object
+        Returns: thermo_np_deriv_helm object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def dsdT(self):
@@ -1933,15 +1913,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class part_deriv_press
         
-        Returns: a part_deriv_press object
+        Returns: part_deriv_press object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def dndmu(self):
@@ -2056,15 +2036,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class part_deriv
         
-        Returns: a part_deriv object
+        Returns: part_deriv object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class fermion_deriv(fermion):
@@ -2106,15 +2086,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_deriv
         
-        Returns: a fermion_deriv object
+        Returns: fermion_deriv object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
 
 class deriv_thermo_base:
@@ -2160,15 +2140,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class deriv_thermo_base
         
-        Returns: a deriv_thermo_base object
+        Returns: deriv_thermo_base object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def heat_cap_ppart_const_vol(self,p,T):
         """
@@ -2292,15 +2272,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_deriv_rel
         
-        Returns: a fermion_deriv_rel object
+        Returns: fermion_deriv_rel object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def exp_limit(self):
@@ -2551,15 +2531,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_deriv_nr
         
-        Returns: a fermion_deriv_nr object
+        Returns: fermion_deriv_nr object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def flimit(self):
@@ -2704,15 +2684,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class classical_deriv_thermo
         
-        Returns: a classical_deriv_thermo object
+        Returns: classical_deriv_thermo object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     def calc_density(self,p,T):
         """
@@ -2735,17 +2715,17 @@
         func.argtypes=[ctypes.c_void_p,ctypes.c_void_p,ctypes.c_double]
         func(self._ptr,p._ptr,T)
         return
 
 
 class fermion_mag_zerot:
     """
-    Python interface for O\ :sub:`2`\ scl class ``fermion_mag_zerot``,
+    Python interface for O2scl class ``fermion_mag_zerot``,
     See
-    https://neutronstars.utk.edu/code/o2scl/part/html/class/fermion_mag_zerot.html .
+    https://neutronstars.utk.edu/code/o2scl/html/class/fermion_mag_zerot.html .
     """
 
     _ptr=0
     _link=0
     _owner=True
 
     def __init__(self,link,pointer=0):
@@ -2782,15 +2762,15 @@
             self._ptr=0
         return
 
     def __copy__(self):
         """
         Shallow copy function for class fermion_mag_zerot
         
-        Returns: a fermion_mag_zerot object
+        Returns: fermion_mag_zerot object
         """
 
         new_obj=type(self)(self._link,self._ptr)
         return new_obj
 
     @property
     def nmax_up(self):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/plot_info.py` & `o2sclpy-0.928/o2sclpy/plot_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -20,17 +20,14 @@
 #  -------------------------------------------------------------------
 #
 
 import sys
 import numpy
 import textwrap
 
-# For rectangles
-import matplotlib.patches as patches
-
 from o2sclpy.utils import default_plot, string_to_dict, terminal_py
 from o2sclpy.doc_data import cmaps, new_cmaps
 
 def marker_list():
     """ 
     Print a list of matplotlib markers which work in o2graph
     command-line arguments.
@@ -215,14 +212,15 @@
         from matplotlib.colors import to_rgba
         from matplotlib import colors as mc
 
         # Obtain a list of CSS4 and XKCD colors
         colors=dict(**mc.CSS4_COLORS,**mc.XKCD_COLORS)
 
         # Remove leading space
+        col_orig=col
         while col[0].isspace():
             col=col[1:]
 
         # Convert from string to [r,g,b] if necessary
         if col[0]=='(' or col[0]=='[':
             col=col.replace('(',' ')
             col=col.replace(')',' ')
@@ -231,15 +229,17 @@
             col=col.split(',')
             col=[float(col[0]),float(col[1]),float(col[2])]
         
         # Convert the specified color to [r,g,b,a] where
         # all four entries are between 0 and 1
         
         colt=to_rgba(col)
-        print('converted',col,'to',colt)
+        print('o2sclpy.plot_info.colors_near() converted',col_orig,
+              'to:\n  (%7.6e,%7.6e,%7.6e,%7.6e).' % (colt[0],colt[1],
+                                                     colt[2],colt[3]))
         ir=colt[0]
         ig=colt[1]
         ib=colt[2]
         
         selected=[]
         
         crange=0.100
@@ -261,48 +261,59 @@
                 return val[0]
             selected2=sorted(selected,key=lambda x: x[1])
             #print(selected2)
             #print('Found list with range ',crange)
 
         # If col was converted to (r,g,b), then convert back to a
         # string.
-        col_fixpound=str(col).replace('#','\\#')
-        title=(r'$ \mathrm{O}_2\mathrm{sc'+
-               'lpy~list~of~colors~near~'+col_fixpound+'}: $')
+
+        # AWS, 10/16/22: This replacement was necessary with
+        # usetex=True, but now usetex=False, so we remove it
+        #col_fixpound=str(col).replace('#','\\#')
+        
+        #title=(r'$ \mathrm{O}_2\mathrm{sc'+
+        #'lpy~list~of~colors~near~'+col+'}: $')
+        title=r'$ O_{2}sclpy~list~of~colors~near~'+str(col)+': $'
+               
         #print('title',title)
 
         if len(selected)>80:
             selected=selected[0:80]
     
         if len(selected)>0:
             #print('selected',selected)
             n=len(selected)
             header=1
             ncols=4
             nrows=n//ncols
             #print('ncols,nrows',ncols,nrows)
-            plot.rc('text',usetex=True)
+            plot.rc('text',usetex=False)
             plot.rc('font',family='serif')
             fig,axes=plot.subplots(figsize=(9.5,6.4))
             # Get height and width
-            X,Y=fig.get_dpi()*fig.get_size_inches()
+            X,Y=fig.get_size_inches()*100
             h=Y/(nrows+header+1)
             w=X/ncols
         
             for i in range(0,n):
                 row=i%nrows
                 column=i//nrows
                 y=Y-((row+header)*h)-h
                 xi_line=w*(column+0.05)
                 xf_line=w*(column+0.25)
-                xi_text=w*(column+0.3)
-                
-                axes.text(xi_text,y,selected[i][0],
-                          fontsize=(h*0.4),
-                          ha='left',va='center')
+                xi_text=w*(column+0.27)
+
+                if len(selected[i][0])>15:
+                    axes.text(xi_text,y,selected[i][0],
+                              fontsize=(h*0.3),
+                              ha='left',va='center')
+                else:
+                    axes.text(xi_text,y,selected[i][0],
+                              fontsize=(h*0.4),
+                              ha='left',va='center')
     
                 axes.hlines(y+h*0.1,xi_line,xf_line,
                             color=selected[i][0],
                             linewidth=(h*0.8))
 
             column=2.4
             row=-1.2
@@ -328,14 +339,17 @@
             if (matplotlib.get_backend()!='Agg' and 
                 matplotlib.get_backend()!='agg'):
                 if fname=='':
                     plot.show()
             elif fname=='':
                 print('Backend is Agg but no filename is specified',
                       'so no output was created.')
+
+            plot.rc('text',usetex=True)
+                
         else:
             print('Error. Not enough colors selected in colors_near().')
             
     return
 
 def cmap_list_func():
     """ 
@@ -360,25 +374,26 @@
         for i in range (0,len(str_list)):
             print(str_list[i])
         print(' ')
     print('Remember that colormaps can all be',
           'reversed by using a "_r" suffix.')
     print(' ')
     print("To create a plot of the colormaps, use",
-          "'o2graph -help cmaps-plot' or")
-    print("'o2graph -help cmaps-plot plot_file.png'")
+          "'o2graph -cmap plot' or")
+    print("'o2graph -cmap plot plot_file.png'")
     return
 
 def cmaps_plot(fname=''):
     """ 
     Create a plot of matplotlib and o2sclpy colormaps.
     """
     print('Generating colormap summary figure.')
                         
     import matplotlib.pyplot as plot
+    import matplotlib.patches as patches
     
     # An internal implementation of
     # https://matplotlib.org/3.1.0/gallery/
     # color/colormap_reference.html
                         
     #self.left_margin=0.01
     #self.right_margin=0.01
@@ -406,52 +421,50 @@
                                        ncols=ncols,
                                        figsize=(fig_x,
                                                 fig_y))
     fig.subplots_adjust(top=1.0-0.35/fig_y,
                              bottom=0.15/fig_y,
                              left=0.01,right=0.99,
                              wspace=0.01)
-    plot.rc('text',usetex=True)
+    plot.rc('text',usetex=False)
     plot.rc('font',family='serif')
 
     for i in range(0,nrows):
         for j in range(0,ncols):
             axes[i][j].set_axis_off()
                         
     row_ctr=0
     col_ctr=0
     for category, cmap_list in cmaps:
         for name in cmap_list:
-            name2=name.replace('_','\_')
             ax=axes[row_ctr][col_ctr]
             ax.imshow(gradient,aspect='auto',
                              cmap=plot.get_cmap(name))
             r=patches.Rectangle((0.32,0.1),0.36,0.8,0,
                                 fc=(1,1,1,0.7),lw=0,
                                 fill=True,
                                 transform=ax.transAxes)
             ax.add_patch(r)
-            ax.text(0.5,0.45,name2,
+            ax.text(0.5,0.45,name,
                                 va='center',ha='center',
-                                fontsize=8,color=(0,0,0),
+                                fontsize=10,color=(0,0,0),
                                 transform=ax.transAxes)
             row_ctr=row_ctr+1
             if row_ctr>=nrows:
                 row_ctr=0
                 col_ctr=col_ctr+1
     for category, cmap_list in new_cmaps:
         for name in cmap_list:
-            name2=name.replace('_','\_')
             ax=axes[row_ctr][col_ctr]
             ax.imshow(gradient,aspect='auto',
                       cmap=plot.get_cmap(name))
             r=patches.Rectangle((0.32,0.1),0.36,0.8,0,fc=(1,1,1,0.7),lw=0,
                                 fill=True,transform=ax.transAxes)
             ax.add_patch(r)
-            ax.text(0.5,0.45,name2,va='center',ha='center',
+            ax.text(0.5,0.45,name,va='center',ha='center',
                     fontsize=8,color=(0,0,0),transform=ax.transAxes)
             row_ctr=row_ctr+1
             if row_ctr>=nrows:
                 row_ctr=0
                 col_ctr=col_ctr+1
 
     ax=axes[0][0]
@@ -469,14 +482,16 @@
     if (matplotlib.get_backend()!='Agg' and 
         matplotlib.get_backend()!='agg'):
         if fname=='':
             plot.show()
     elif fname=='':
         print('Backend is Agg but no filename is specified',
               'so no output was created.')
+        
+    plot.rc('text',usetex=True)
     return
 
 def colors_plot(fname='',dpi=10):
     """
     Create a plot of the matplotlib CSS4 colors and, optionally,
     store the plot in file named 'fname'.
     """
@@ -484,58 +499,64 @@
     import matplotlib.pyplot as plot
 
     colors=dict(**mc.CSS4_COLORS)
     by_hsv=sorted((tuple(mc.rgb_to_hsv(mc.to_rgba(color)[:3])),name)
                     for name, color in colors.items())
     sorted_names=[name for hsv, name in by_hsv]
     n=len(sorted_names)
-    header=1
+    header=2
     ncols=4
     nrows=n//ncols
-    plot.rc('text',usetex=True)
+    plot.rc('text',usetex=False)
     plot.rc('font',family='serif')
-    fig,axes=plot.subplots(figsize=(8,6.6))
+    fig,axes=plot.subplots(figsize=(9.5,6.4))
+    #fig,axes=plot.subplots(figsize=(8,6.6))
+    #print('dpi',dpi)
     # Get height and width
-    fig.set_dpi(dpi)
+    #fig.set_dpi(dpi)
     X,Y=fig.get_dpi()*fig.get_size_inches()
     h=Y/(nrows+1+header)
     w=X/ncols
 
     for i, name in enumerate(sorted_names):
         row=i%nrows
         col=i//nrows
         y=Y-((row+header)*h)-h
         xi_line=w*(col+0.05)
         xf_line=w*(col+0.25)
         xi_text=w*(col+0.3)
-        axes.text(xi_text,y,name,fontsize=(h*0.6),
-                ha='left',va='center')
+        axes.text(xi_text,y+h*0.5,name,fontsize=(h*0.3),
+                  ha='left',va='center')
 
-        axes.hlines(y+h*0.1,xi_line,xf_line,
-                  color=colors[name],linewidth=(h*0.8))
+        axes.hlines(y+h*0.5,xi_line,xf_line,
+                    color=colors[name],linewidth=(h*0.31))
 
-        axes.set_xlim(0,X)
-        axes.set_ylim(0,Y+header)
-        axes.set_axis_off()
+    axes.set_xlim(0,X)
+    axes.set_ylim(0,Y+header)
+    axes.set_axis_off()
                             
     fig.subplots_adjust(left=0,right=1,top=1,bottom=0,
                         hspace=0,wspace=0)
-    axes.text(X*0.5,(Y+header)*0.965,r'$ \mathrm{O}_2\mathrm{sc'+
-              'lpy~colors~summary} $',fontsize=16,ha='center')
+    axes.text(X*0.5,(Y+header)*0.965,r'$ \mathrm{O}_{2}\mathrm{sclpy~colors~summary} $',
+              fontsize=16,ha='center')
+
     if fname!='':
         plot.savefig(fname)
         print('Created image file '+fname+'.')
     import matplotlib
     if (matplotlib.get_backend()!='Agg' and 
         matplotlib.get_backend()!='agg'):
         if fname=='':
             plot.show()
     elif fname=='':
         print('Backend is Agg but no filename is specified',
               'so no output was created.')
+        
+    plot.rc('text',usetex=True)
+        
     return
 
 def color_list():
     """
     List matplotlib base and CSS4 colors along with their
     values in #RRGGBB hexadecimal format.
     """
@@ -566,28 +587,28 @@
             outs=outs+(col+' '+str(css4_dict[col])).ljust(26)
             outs=outs+'\n'
         ctr=ctr+1
     print(outs)
     print(' ')
     outs=("o2sclpy also supports the (r,g,b) format, the [r,g,b,a] format, "+
           "the HTML format, the grayscale single-value format, "+
-          "and the XKCD colors (see '-help xkcd-colors' for a list). "+
+          "and the XKCD colors (see '-colors xkcd' for a list). "+
           "For (r,g,b) colors, parentheses must be used, and the r, g,"+
           " and b numbers should be from 0.0 to 1.0. For [r,g,b,a] "+
           "colors, square brackets must be used and the r, g, b, "+
           "and a numbers should be from 0.0 to 1.0. The HTML "+
           "format is #RRGGBB where RR, GG, and BB are two-digit "+
           "hexadecimal values.")
     str_list=textwrap.wrap(outs,79)
     for i in range (0,len(str_list)):
         print(str_list[i])
     print(' ')
     print("To create a plot of colors, use",
-          "'o2graph -help colors-plot' or")
-    print("'o2graph -help colors-plot plot_file.png'")
+          "'o2graph -colors plot' or")
+    print("'o2graph -colors plot plot_file.png'")
     return
 
 def xkcd_colors_list():
     """
     List all of the XKCD colors along with their 
     values in #RRGGBB hexadecimal format.
     """
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/utils.py` & `o2sclpy-0.928/o2sclpy/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -24,120 +24,43 @@
 # For os.getenv()
 import os
 
 # For numpy.bytes_
 import numpy
 
 # To test between Linux/OSX using system()
-import platform
+# AWS, 2/20/23, apparently no longer used
+#import platform
 
 # For CDLL loading
-import ctypes
-from ctypes.util import find_library
+# AWS, 2/20/23, apparently no longer used
+#import ctypes
+#from ctypes.util import find_library
+
+def cpp_test(x):
+    """
+    Desc
+    """
+    return x*numpy.pi
 
 def remove_spaces(string):
+    """
+    Remove spaces at the beginning specified string and return the 
+    result.
+
+    This function is in ``utils.py``.
+    """
     while len(string)>0 and string[0]==' ':
         string=string[1:]
     return string
 
-def doc_replacements(s,base_list_new,ter):
-
-    # Replace commands in base_list_new
-    for i in range(0,len(base_list_new)):
-        s=s.replace('``'+base_list_new[i][0]+'``',
-                    ter.cyan_fg()+ter.bold()+base_list_new[i][0]+
-                    ter.default_fg())
-
-    # For ``code`` formatting
-    s=s.replace(' ``',' ')
-    s=s.replace('`` ',' ')
-    s=s.replace('``, ',', ')
-    s=s.replace('``. ','. ')
-
-    # Combine two spaces to one
-    s=s.replace('  ',' ')
-
-    # For :math:`` equations
-    s=s.replace(' :math:`',' ')
-    s=s.replace('` ',' ')
-    s=s.replace('`.','.')
-    s=s.replace('`',',')
-                    
-    return s
-
-def reformat_python_docs(cmd,doc_str,base_list_new):
-
-    reflist=doc_str.split('\n')
-    
-    for i in range(0,len(reflist)):
-        reflist[i]=remove_spaces(reflist[i])
-        #print(i,'x',reflist[i],'x')
-
-    if len(reflist)<1:
-        return
-
-    if reflist[0]=='':
-        if len(reflist)<2:
-            return
-        doc_str2=reflist[1]
-        for i in range(2,len(reflist)):
-            doc_str2=doc_str2+'\n'+reflist[i]
-    else:
-        doc_str2=reflist[0]
-        for i in range(0,len(reflist)):
-            doc_str2=doc_str2+'\n'+reflist[i]
-
-    reflist2=doc_str2.split('\n\n')
-
-    if False:
-        for i in range(0,len(reflist2)):
-            print(i,'x',reflist2[i],'x')
-    
-    ter=terminal_py()
-    ncols=os.get_terminal_size().columns
-
-    short=''
-    parm_desc=''
-    long_help=''
-
-    # The short description
-    if len(reflist2)>=2:
-        short=reflist2[1]
-
-    # The parameter description
-    if len(reflist2)>=3:
-        parm_desc=reflist2[2].replace('\n',' ')
-
-        parm_desc=parm_desc.replace('  ',' ')
-        sx='Command-line arguments: ``'
-        if parm_desc[0:len(sx)]==sx:
-            parm_desc=parm_desc[len(sx):]
-        if parm_desc[-2:]=='``':
-            parm_desc=parm_desc[0:-2]
-            
-    print('Usage: '+ter.cyan_fg()+ter.bold()+cmd+
-          ter.default_fg()+' '+parm_desc)
-    print('Short description:',short)
-
-    if len(reflist2)>=4:
-        print('')
-        print('Long description:')
-        for j in range(3,len(reflist2)):
-            if len(reflist2[j])>0:
-                long_help=doc_replacements(reflist2[j].replace('\n',' '),
-                                           base_list_new,ter)
-                tmplist=wrap_line(long_help,ncols-1)
-                if j!=3:
-                    print('')
-                for k in range(0,len(tmplist)):
-                    print(tmplist[k])
-
 def string_to_color(str_in):
     """
-    Convert a string to a color
+    Convert a string to a color, either ``(r,g,b)`` to an RGB color
+    or ``[r,g,b,a]`` to an RGBA color.
     """
 
     if str_in[0]=='(':
         temps=str_in[1:len(str_in)-1]
         temp2=temps.split(',')
         return (float(temp2[0]),float(temp2[1]),float(temp2[2]))
     elif str_in[0]=='[':
@@ -145,105 +68,29 @@
         temp2=temps.split(',')
         return [float(temp2[0]),float(temp2[1]),float(temp2[2]),
                 float(temp2[3])]
     
     return str_in
 
 def if_yt_then_Agg(backend,argv):
-    # Determine if yt commands are present
+    """
+    Determine if yt commands are present, and if found, then automatically
+    convert to the Agg backend.
+    """
             
     yt_found=False
     for i in range(1,len(argv)):
         if argv[i][0:4]=='-yt-' and yt_found==False:
             if backend!='' and backend!='agg' and backend!='Agg':
-                print('Backend was not set to Agg but yt commands were found.')
+                print('Backend was not set to Agg but yt '+
+                      'commands were found.')
             yt_found=True
             backend='Agg'
     return backend
 
-def o2scl_get_type(o2scl,amp):
-    """
-    Get the type of the current object stored in the acol_manager
-    pointer
-    """
-    # pointer types
-    char_ptr=ctypes.POINTER(ctypes.c_char)
-    char_ptr_ptr=ctypes.POINTER(char_ptr)
-    int_ptr=ctypes.POINTER(ctypes.c_int)
-    
-    # Set up wrapper for type function
-    type_fn=o2scl.o2scl_acol_get_type
-    type_fn.argtypes=[ctypes.c_void_p,int_ptr,char_ptr_ptr]
-    
-    # Get current type
-    it=ctypes.c_int(0)
-    type_ptr=char_ptr()
-    type_fn(amp,ctypes.byref(it),ctypes.byref(type_ptr))
-
-    # Construct the type as a byte string
-    curr_type=b''
-    for i in range(0,it.value):
-        curr_type=curr_type+type_ptr[i]
-    return curr_type
-
-def table3d_get_slice(o2scl,amp,name):
-    """
-    Return a slice from the current table3d object stored
-    in the acol_manager object 'amp'
-    """
-    get_fn=o2scl.o2scl_acol_get_slice
-    get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                     int_ptr,double_ptr_ptr,
-                     int_ptr,double_ptr_ptr,double_ptr_ptr]
-    
-    slice=ctypes.c_char_p(force_bytes(slice_name))
-    nx=ctypes.c_int(0)
-    ptrx=double_ptr()
-    ny=ctypes.c_int(0)
-    ptry=double_ptr()
-    ptrs=double_ptr()
-    get_fn(amp,slice,ctypes.byref(nx),ctypes.byref(ptrx),
-           ctypes.byref(ny),ctypes.byref(ptry),
-           ctypes.byref(ptrs))
-    return (nx,ptrx,ny,ptry,ptrs)
-
-def table_get_column(o2scl,amp,name,return_pointer=False):
-    """
-    Return a column from the current table object stored
-    in the acol_manager object 'amp'
-    """
-
-    # C types
-    int_ptr=ctypes.POINTER(ctypes.c_int)
-    double_ptr=ctypes.POINTER(ctypes.c_double)
-    double_ptr_ptr=ctypes.POINTER(double_ptr)
-
-    # Function interface
-    get_fn=o2scl.o2scl_acol_get_column
-    get_fn.argtypes=[ctypes.c_void_p,ctypes.c_char_p,
-                     int_ptr,double_ptr_ptr]
-    get_fn.restype=ctypes.c_int
-
-    # Arguments
-    col=ctypes.c_char_p(force_bytes(name))
-    size=ctypes.c_int(0)
-    pointer=double_ptr()
-
-    # Function call
-    get_ret=get_fn(amp,col,ctypes.byref(size),ctypes.byref(pointer))
-    if get_ret!=0:
-        print('Failed to get column named "'+name+'".')
-        return None
-
-    if return_pointer:
-        return pointer
-        
-    col=[pointer[i] for i in range(0,size.value)]
-    return col
-
 def is_number(s):
     """
     Return true if 's' is likely a number
     """
     try:
         float(s)
         return True
@@ -264,40 +111,23 @@
     This function returns the bytes object corresponding to ``obj``
     in case it is a string using UTF-8. 
     """
     if isinstance(obj,numpy.bytes_)==True or isinstance(obj,bytes)==True:
         return obj.decode('utf-8')
     return obj
 
-# This function is probably best replaced by get_str_array() below
-#
-# def parse_col_names(dset):
-#     nc=dset['nc'].__getitem__(0)
-#     nw=dset['nw'].__getitem__(0)
-#     counter=dset['counter']
-#     data=dset['data']
-#     clist=[]
-#     k=0
-#     for i in range(0,nw):
-#         column=''
-#         for j in range(0,counter[i]):
-#             column=column+str(unichr(data[k]))
-#             k=k+1
-#         clist.append(column)
-#     return clist
-
 def default_plot(left_margin=0.14,bottom_margin=0.12,
                  right_margin=0.04,top_margin=0.04,fontsize=16,
                  fig_size_x=6.0,fig_size_y=6.0,ticks_in=False,
                  rt_ticks=False,editor=False):
     
     import matplotlib.pyplot as plot
 
     """
-    This function sets up the O\ :sub:`2`\ sclpy ``matplotlib``
+    This function sets up the O2sclpy ``matplotlib``
     defaults. It returns a pair of objects, the figure object and axes
     object. The fontsize argument times 0.8 is used 
     for the size of the font labels. Setting the ``ticks_in`` argument
     to ``True`` makes the ticks point inwards instead of outwards
     and setting ``rt_ticks`` to ``True`` puts ticks (but not labels)
     on the right and top edges of the plot. 
     
@@ -383,27 +213,14 @@
     # We're done with the characters, but there are some blank
     # strings left. Add the appropriate blanks at the end.
     while word_counter<nw:
         list.append('')
         word_counter=word_counter+1
     return list
 
-def get_ic_ptrs_to_list(size,lengths,chars):
-    """
-    """
-    tlist=[]
-    count=0
-    for i in range(0,size.value):
-        strt=b''
-        for j in range(0,lengths[i]):
-            strt=strt+chars[count]
-            count+=1
-        tlist.append(strt)
-    return tlist
-
 def parse_arguments(argv,verbose=0):
     """
     Old command-line parser (this is currently unused and
     it's not clear if it will be useful in the future).
 
     This function is in ``utils.py``.
     """
@@ -454,14 +271,58 @@
                               str(ix_next)+' to list for '+cmd_name)
                     list_one.append(argv[ix_next])
                     ix_next=ix_next+1
             list.append(list_one)
             ix=ix_next
     return (list,unproc_list)
 
+def string_to_dict2(s,list_of_ints=[],list_of_floats=[],list_of_bools=[]):
+    """
+    Convert a string to a dictionary, converting strings to 
+    values when necessary.
+    """
+        
+    # First split into keyword = value pairs
+    arr=s.split(',')
+    # Create empty dictionary
+    dct={}
+
+    if len(s)==0:
+        return dct
+        
+    for i in range(0,len(arr)):
+
+        # For each pair, split keyword and value.
+        arr2=arr[i].split('=')
+        
+        # Remove preceeding and trailing whitespace from the
+        # keywords (not for the values)
+        while arr2[0][0].isspace():
+            arr2[0]=arr2[0][1:]
+        while arr2[0][len(arr2[0])-1].isspace():
+            arr2[0]=arr2[0][:-1]
+
+        # Remove quotes if necessary
+        if len(arr2)>1 and len(arr2[1])>2:
+            if arr2[1][0]=='\'' and arr2[1][len(arr2[1])-1]=='\'':
+                arr2[1]=arr2[1][1:len(arr2[1])-1]
+            if arr2[1][0]=='"' and arr2[1][len(arr2[1])-1]=='"':
+                arr2[1]=arr2[1][1:len(arr2[1])-1]
+
+        if arr2[0] in list_of_ints:
+            arr2[1]=int(arr2[1])
+        if arr2[0] in list_of_floats:
+            arr2[1]=float(arr2[1])
+        if arr2[0] in list_of_bools:
+            arr2[1]=bool(arr2[1])
+                    
+        dct[arr2[0]]=arr2[1]
+
+    return dct
+
 def string_to_dict(s):
     """
     Convert a string to a dictionary, with extra processing for
     colors, subdictionaries, and matplotlib keyword arguments which
     are expected to have integer or floating point values.
 
     This function is in ``utils.py``.
@@ -593,14 +454,16 @@
                 arr2[1]=float(arr2[1])
             if arr2[0]=='pad':
                 arr2[1]=float(arr2[1])
             if arr2[0]=='capsize':
                 arr2[1]=float(arr2[1])
             if arr2[0]=='capthick':
                 arr2[1]=float(arr2[1])
+            if arr2[0]=='rotation':
+                arr2[1]=float(arr2[1])
 
             # Convert strings to bool values
             if arr2[0]=='sharex':
                 if arr2[1]=='True':
                     arr2[1]=True
                 else:
                     arr2[1]=False
@@ -825,15 +688,15 @@
         """
         strt=''
         if self.redirected:
             return strt
         strt=strt+chr(27)+'[1m'
         return strt
     
-    def default_fg(self):
+    def default_fgbg(self):
         """
         Set the foreground color to the default
         """
         strt=''
         if self.redirected:
             return strt
         strt=strt+chr(27)+'[m'
@@ -852,46 +715,76 @@
         else:
             str_line=str_line+chr(27)+'(0'
             for jj in range(0,78):
                 str_line+='q'
             str_line=str_line+chr(27)+'(B'
         return str_line
 
-    def type_str(self,strt):
-        return self.magenta_fg()+self.bold()+strt+self.default_fg()
-    
-    def cmd_str(self,strt):
-        return self.cyan_fg()+self.bold()+strt+self.default_fg()
-    
-    def topic_str(self,strt):
-        return self.green_fg()+self.bold()+strt+self.default_fg()
-    
-    def var_str(self,strt):
-        return self.red_fg()+self.bold()+strt+self.default_fg()
+    def type_str(self,strt,amt):
+        return (force_string(amt.get_type_color())+strt+
+                force_string(amt.get_default_color()))
+    
+    def cmd_str(self,strt,amt):
+        return (force_string(amt.get_command_color())+strt+
+                force_string(amt.get_default_color()))
+    
+    def topic_str(self,strt,amt):
+        return (force_string(amt.get_help_color())+strt+
+                force_string(amt.get_default_color()))
+    
+    def var_str(self,strt,amt):
+        return (force_string(amt.get_param_color())+strt+
+                force_string(amt.get_default_color()))
 
 def length_without_colors(strt):
     """
     Compute the length of strt, ignoring characters which correspond
     to VT100 formatting sequences
     """
     count=0
     index=0
     while index<len(strt):
         if strt[index]!=chr(27):
             count=count+1
         elif index+2<len(strt) and strt[index+1]=='[' and strt[index+2]=='m':
+            # default_fgbg case
             index=index+2
         elif index+3<len(strt) and strt[index+1]=='[' and strt[index+3]=='m':
+            # underline, lowint, bold case
             index=index+3
         elif index+4<len(strt) and strt[index+1]=='[' and strt[index+4]=='m':
+            # red_fg, blue_fg, etc. case
             index=index+4
         elif index+2<len(strt) and strt[index+1]=='(' and strt[index+2]=='0':
+            # alt font case
             index=index+2
         elif index+2<len(strt) and strt[index+1]=='(' and strt[index+2]=='B':
+            # normal font case
             index=index+2
+        elif (index+8<len(strt) and strt[index+1]=='[' and
+              (strt[index+2]=='3' or strt[index+2]=='4') and
+              strt[index+3]=='8' and strt[index+4]==';' and
+              strt[index+5]=='5' and strt[index+6]==';' and
+              strt[index+8]=='m'):
+            # eight bit fg/bg case with single digit color
+            index=index+8
+        elif (index+9<len(strt) and strt[index+1]=='[' and
+              (strt[index+2]=='3' or strt[index+2]=='4') and
+              strt[index+3]=='8' and strt[index+4]==';' and
+              strt[index+5]=='5' and strt[index+6]==';' and
+              strt[index+9]=='m'):
+            # eight bit fg/bg case with double digit color
+            index=index+9
+        elif (index+10<len(strt) and strt[index+1]=='[' and
+              (strt[index+2]=='3' or strt[index+2]=='4') and
+              strt[index+3]=='8' and strt[index+4]==';' and
+              strt[index+5]=='5' and strt[index+6]==';' and
+              strt[index+10]=='m'):
+            # eight bit fg/bg case with triple digit color
+            index=index+10
         index=index+1
     return count
             
 def wrap_line(line,ncols=79):
     """
     From a string 'line', create a list of strings which adds return
     characters in order to attempt to ensure each line is less than
```

### Comparing `o2sclpy-0.927.post1/o2sclpy/yt_plot_base.py` & `o2sclpy-0.928/o2sclpy/yt_plot_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  -------------------------------------------------------------------
 #  
-#  Copyright (C) 2006-2022, Andrew W. Steiner
+#  Copyright (C) 2006-2023, Andrew W. Steiner
 #  
 #  This file is part of O2sclpy.
 #  
 #  O2sclpy is free software; you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation; either version 3 of the License, or
 #  (at your option) any later version.
@@ -22,90 +22,60 @@
 import math
 import numpy
 import os
 
 # For system type detection
 import platform
 
-# To create new color maps
-from matplotlib.colors import LinearSegmentedColormap
-
-# For rectangles and ellipses
-import matplotlib.patches as patches
-
 from o2sclpy.utils import parse_arguments, string_to_dict
 from o2sclpy.utils import force_bytes, default_plot, get_str_array
 from o2sclpy.utils import string_to_color
 from o2sclpy.plot_base import plot_base
 
 class yt_plot_base(plot_base):
     """
     A base class with simplifications for plots generated in yt
     """
 
     # yt settings modifiable by get and set
 
     yt_filter=''
     """
-    Filter for yt images. If non-empty, must contain the 
-    strings '%i' for input file and '%o' for output file. A typical
-    example is something like
-
-    convert -contrast-stretch 0 %i %o 
-
-    which uses imagemagick to adjust the color curve.
+    Filter for yt images. 
     """
     yt_resolution=(512,512)
     """
     Resolution for yt rendering (default (512,512))
     """
     yt_focus='default'
     """
-    yt camera focus as a string. The string 'default' is equivalent
-    to '[0.5,0.5,0.5] internal'. Either in the 'internal' or 'user' 
-    unit system.
+    yt camera focus as a string. 
     """
     yt_position='default'
     """
-    yt camera position as a string. The string 'default' is equivalent
-    to '[1.5,0.6,0.7] internal'. Either in the 'internal' or 'user' 
-    unit system.
+    yt camera position as a string. 
     """
     yt_width='default'
     """
-    yt camera width as a string. The string 'default' is equivalent to 
-    '[1.5,1.5,1.5]'. Always in the internal unit system.
+    yt camera width as a string.
     """
     yt_north='default'
     """
-    yt camera north vector string. The string 'default' is equivalent to
-    '[1.0,0.0,0.0]'. Always in the internal unit system.
+    yt camera north vector string. 
     """
     yt_sigma_clip=4.0
     """
     The sigma_clip parameter for yt (default 4.0)
     """
 
     # Other yt settings
     
     yt_path=[]
     """
-    yt animation path (default []), as list of lists. The
-    list contains instructions such as
-
-    ['yaw',100,0.01]
-    ['zoom',100,2.0]
-    ...
-
-    where the first entry in each sublist is always a type
-    move, and the second entry in each sublist is always the 
-    number of frames over which to complete the move.
-
-    Note that this is not set using -set or -get but by the
-    'yt-path' command.
+    yt animation path (default []), as list of lists.
     """
     yt_ann=[]
     """
     Annotations for yt renders. This list is controlled by
     the 'yt-ann' command.
     """
     yt_trans=0
@@ -156,14 +126,21 @@
     The yt camera object
     """
     yt_created_camera=False
     """
     If true, then the yt camera object has been created
     """
 
+    def __init__(self):
+        """
+        Desc
+        """
+        super().__init__()
+        return
+        
     def yt_update_text(self):
         """
         Update the text objects during an animation by removing them from
         the scene and adding them back.
         """
 
         for i in range(0,len(self.yt_text_objects)):
@@ -555,25 +532,37 @@
                 reorient=False,scale=0.6,font=30,
                 keyname='o2sclpy_text',dpi=100,filename='',
                 coords=''):
         """Documentation for o2graph command ``yt-text``:
 
         Add text to the yt volume.
 
-        Command-line arguments: ``<x> <y> <z> <text> reorient=False``
+        Command-line arguments: ``<x> <y> <z> <text> [kwargs]``
 
-        Plot text given in ``textstr`` in a yt volume visualization at
-        location ``(tx,ty,tz)``. If reorient is ``True``, then 
-        the during an animation, the text will be redrawn so that
-        it is parallel to the camera. The ``scale`` and ``font``
-        parameters are passed on to the yt_text_to_scene() function.
+        Plot text given in ``<textstr>`` in a yt volume visualization at
+        location ``(tx,ty,tz)``. 
+
+        The keyword arguments and their defaults are
+        ``textcolor=(1,1,1,0.5)``, ``reorient=False``, ``scale=0.6``,
+        ``font=30``, ``keyname='o2sclpy_text'``, ``dpi=100``,
+        ``filename=''``, and ``coords=''``.
+
+        If ``coords`` is empty or ``user``, then the given coordinates
+        are assumed to be in the user coordinate system. If ``coords``
+        is ``internal``, then the coordinates are assumed to be in the
+        internal coordinate system from ``[0,0,0]`` to ``[1,1,1]``. If
+        reorient is ``True``, then the during an animation, the text
+        will be redrawn so that it is parallel to the camera. The
+        ``scale`` and ``font`` parameters are passed on to the
+        yt_text_to_scene() function. 
 
         In the future, the plan is to allow tx, ty, and tz to be
         functions of 'i', so the text can be moved. For now tx, ty,
         and tz are just floating point numbers.
+
         """
 
         if (self.xset==False or self.yset==False or
             self.zset==False):
             print('Cannot place text before limits set.')
             return
 
@@ -826,36 +815,38 @@
     def yt_plot_axis(self,xval=1.0,yval=1.0,zval=1.0,
                      color=[1.0,1.0,1.0,0.5],
                      coords='internal',keyname='o2sclpy_axis'):
         """Documentation for o2graph command ``yt-axis``:
 
         Add an axis to the yt volume.
 
-        Command-line arguments: ``xval=1.0,yval=1.0,zval=1.0,
-        color=[1.0,1.0,1.0,0.5],coords='internal',keyname='o2sclpy_axis'``
-        
-        This command plots an axis from the origin to the three points
-        ``[0,0,xval]``, ``[0,yval,0]``, and ``[0,0,zval]``. There are
-        two keyword arguments, the first is ``color=[1,1,1,0.5]``, the
-        color of the axis arrows. The other is a string for the
-        coordinate system, and keyname, the name for the yt object.
-        Use ``coords=user`` for the user-based coordinate system and
-        ``coords=internal`` for the internal coordinate system.
+        Command-line arguments: ``[kwargs]``
 
-        Note that it is often most convenient to create the 
-        first volume source to set the scaling of the user-based
+        This command plots an axis from the origin to the three points
+        ``[0,0,xval]``, ``[0,yval,0]``, and ``[0,0,zval]``. The values
+        ``xval``, ``yval``, and ``zval`` are keyword arguments which
+        default to 1.0. The keyword argument ``color=[1,1,1,0.5]``
+        specifies the color of the axis arrows. The keyword argument
+        ``coords`` specifies the coordinate system. Use
+        ``coords=user`` for the user-based coordinate system and
+        ``coords=internal`` (the default) for the internal coordinate
+        system. The final keyword argument ``keyname=o2sclpy_axis`` is
+        the name for the yt object.
+
+        Note that it is often most convenient to create the first
+        volume source (e.g. either with ``yt-add-vol``
+        or``yt-scatter``) to set the scaling of the user-based
         coordinate system before using the ``yt-axis`` command.
 
         This function creates a PointSource at the origin and then
         three arrows pointing from the origin along the x-, y-, and
         z-axes. The specified color is used for the origin and all
         three arrows. The arrows are constructed with one main
         LineSource and then several smaller LineSource objects in a
         conical shape to create the arrow heads.
-
         """
 
         if self.yt_scene==0:
             print('Cannot plot yt axis without a scene.')
             return
         
         print('plot_base:yt_plot_axis(): Adding axis.')
```

### Comparing `o2sclpy-0.927.post1/setup.py` & `o2sclpy-0.928/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md","r") as file_handle:
     long_description=file_handle.read()
 
 setuptools.setup(name='o2sclpy',
-                 version='0.927.post1',
+                 version='0.928',
                  author='Andrew W. Steiner',
-                 author_email='awsteiner@mykolab.com',
+                 author_email='awsteiner0@protonmail.com',
                  description='Python extensions for O2scl',
                  long_description=long_description,
                  long_description_content_type="text/markdown",                 
                  url='https://neutronstars.utk.edu/code/o2sclpy',
                  license='GPLv3',
                  packages=['o2sclpy'],
                  install_requires=['h5py','numpy','matplotlib>=3.1','requests'],
```

